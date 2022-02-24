---
title: Добавяне на нови персонализирани формуляри на обекти (Project Service Automation 2.x)
description: Тази тема предоставя информация за това как да добавите персонализирани формуляри на обекти за възможности, оферти, поръчки или фактури в Dynamics 365 Project Service Automation 2.x.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 3/14/2019
ms.topic: article
ms.service: business-applications
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 31986efed81892cc5722cb8f5e292cde14d8843d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144580"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a>Добавяне на нови персонализирани формуляри на обекти (Project Service Automation 2.x)

[!include [banner](../../includes/psa-now-project-operations.md)]

## <a name="type-field"></a>Поле „Тип“ 

Dynamics 365 Project Service Automation разчита на полето **Тип** (**msdyn\_ordertype**) на обектите „Възможност“, „Оферта“, „Поръчка“ и „Фактура“, за да разграничи **базираните на работа** версии на тези обекти от **базираните на елементи** и **базираните на обслужване** версии. Базираните на работа на тези обекти се обработват от PSA. Много бизнес логика от страна на клиента и сървъра на решението зависи от полето **Тип**. Затова е важно полето да се инициализира с правилна стойност, когато се създават обектите. Неправилна стойност може да доведе до неправилни поведения и някои бизнес логики може да не работят правилно.

## <a name="automatic-form-switching"></a>Автоматично превключване на формуляри

За да избегне потенциални повреда на данни и неочаквани поведения, които са причинени от неправилна инициализация и редактиране на записи на обекти на продажби, PSA вече включва логика за автоматично превключване на формуляри в стандартни формуляри. Тази логика отвежда потребителите до правилния формуляр за работа с базираната на работа версия или друг тип обект „Възможност“, „Оферта“, „Поръчка“ или „Фактура“. Когато даден потребител отвори базирана на работа версия на обект „Възможност“, „Оферта“, „Поръчка“ или „Фактура“, формулярът се превключва към **Информация за проекта**.

Логиката на автоматичното превключване на формуляри разчита на съпоставянето между стойността **formId** и полето **msdyn\_ordertype**. Всички стандартни формуляри са добавени към това съпоставяне. Персонализираните формуляри обаче трябва да се добавят ръчно, за да се укаже коя версия на обекта е планирано да обработват. Това е базирано на полето **msdyn\_ordertype**. Ако превключването на формуляри липсва от съпоставянето, логиката ще превключи към стандартния формуляр въз основа на стойността, записана в полето **msdyn\_ordertype** на обекта.

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a>Добавяне на потребителски формуляри и включване на логиката за превключване на формуляра

Следващият пример показва как да добавите персонализиран формуляр, **Информация за моя проект**, така че да работи с базирани на работа възможности. Същият процес се използва за добавяне на персонализирани формуляри, така че да работят с оферти, поръчки и фактури.

Изпълнете следните стъпки, за да създадете персонализирана версия на формуляра **Информация за проекта**.

1. В обекта „Възможност“ отворете формуляра **Информация за проекта** и запишете копие под името **Информация за моя проект**.
2. Отворете новия формуляр и след това в свойствата се уверете, че скриптовете за инициализация на формуляра от формуляр **Информация за проекта** са налице. 

    > [!IMPORTANT]
    > Не премахвайте скриптовете. В противен случай някои данни може да се инициализират неправилно.

3. Проверете дали полето **Тип** (**msdyn\_ordertype**) е налице във формуляра. 

    > [!IMPORTANT]
    > Не премахвайте това поле. В противен случай скриптовете за инициализиране ще се изпълнят неуспешно.

4. Намерете стойността **formId** на новия формуляр. Можете да изпълните стъпката по два начина:

    - Експортирайте формуляра **Информация за моя проект информация** като част от незавършено решение и след това потърсете стойността на **formid** във файла customization.xml на експортираното решение.
    - Отворете формуляра **Информация за моя проект** в редактора на формуляри и след това потърсете глобален еднозначен идентификатор (GUID) до параметъра **fromid** в URL адреса, както е показано на илюстрацията по-долу.

    ![Стойността formId на новия формуляр в URL адреса](media/how-to-add-custom-forms-in-v2.0.png)

5. Създайте съпоставяне на **msdyn\_ordertype** за стойността **formId**, като редактирате уеб ресурса msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js. Премахнете кода от ресурса и го заменете със следния код.

    ```javascript
    define(["require", "exports"], function (require, exports) {
        "use strict";
        var SalesDocumentCustomFormIds = (function () {
            function SalesDocumentCustomFormIds() {
            }
            SalesDocumentCustomFormIds.overwriteFormIds = function (mappedFormIds) {
                /*
                ---- Notes ----
                mappedFormIds[SalesEntity][OrderType] => The array of forms IDs that support particular entity and order type
                Add or overwrite customized formId for the particular entity and order type by calling:
                    mappedFormIds[<EntityType>][<msdyn_ordertype>].push("<formId>");
                Allowed msdyn_ordertype values for reference:
                    ServiceBased: 690970002 (Field Service version of the entity)
                    WorkBased: 192350001 (PSA version of the entity)
                    ItemBased: 192350000 (Regular out of the box entity)
                Uncomment and update one of the following lines to register custom PSA form for required entity:
                */      
                //mappedFormIds[1][192350001].push("<formId>"); //Quote
                //mappedFormIds[5][192350001].push("<formId>"); //Quote Line
                //mappedFormIds[2][192350001].push("<formId>"); //Sales Order
                //mappedFormIds[6][192350001].push("<formId>"); //Sales Order Line
                // In this example we have added new form for Opportunity
                mappedFormIds[0][192350001].push("192EE537-DCC4-45D3-B7AF-EA694B9113D2"); //Opportunity
                //mappedFormIds[4][192350001].push("<formId>"); //Opportunity Line
            };
            return SalesDocumentCustomFormIds;
        }());
        exports.default = SalesDocumentCustomFormIds;
    });
    ```

6. Запишете и след това публикувайте персонализациите.
