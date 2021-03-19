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
ms.openlocfilehash: 9c9e31dc6d4d5a8ad5cc568f2d7d673c8703936d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284840"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a><span data-ttu-id="93306-103">Добавяне на нови персонализирани формуляри на обекти (Project Service Automation 2.x)</span><span class="sxs-lookup"><span data-stu-id="93306-103">Add new custom entity forms (Project Service Automation 2.x)</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

## <a name="type-field"></a><span data-ttu-id="93306-104">Поле „Тип“</span><span class="sxs-lookup"><span data-stu-id="93306-104">Type field</span></span> 

<span data-ttu-id="93306-105">Dynamics 365 Project Service Automation разчита на полето **Тип** (**msdyn\_ordertype**) на обектите „Възможност“, „Оферта“, „Поръчка“ и „Фактура“, за да разграничи **базираните на работа** версии на тези обекти от **базираните на елементи** и **базираните на обслужване** версии.</span><span class="sxs-lookup"><span data-stu-id="93306-105">Dynamics 365 Project Service Automation relies on the **Type** (**msdyn\_ordertype**) field of the Opportunity, Quote, Order, and Invoice entities to distinguish **work-based** versions of these entities from **item-based** and **service-based** versions.</span></span> <span data-ttu-id="93306-106">Базираните на работа на тези обекти се обработват от PSA.</span><span class="sxs-lookup"><span data-stu-id="93306-106">Work-based versions of these entities are handled by PSA.</span></span> <span data-ttu-id="93306-107">Много бизнес логика от страна на клиента и сървъра на решението зависи от полето **Тип**.</span><span class="sxs-lookup"><span data-stu-id="93306-107">Lots of business logic on the client side and server side of the solution depends on the **Type** field.</span></span> <span data-ttu-id="93306-108">Затова е важно полето да се инициализира с правилна стойност, когато се създават обектите.</span><span class="sxs-lookup"><span data-stu-id="93306-108">Therefore, it's important that the field be initialized with a correct value when the entities are created.</span></span> <span data-ttu-id="93306-109">Неправилна стойност може да доведе до неправилни поведения и някои бизнес логики може да не работят правилно.</span><span class="sxs-lookup"><span data-stu-id="93306-109">An incorrect value can cause incorrect behaviors, and some business logic might not run correctly.</span></span>

## <a name="automatic-form-switching"></a><span data-ttu-id="93306-110">Автоматично превключване на формуляри</span><span class="sxs-lookup"><span data-stu-id="93306-110">Automatic form switching</span></span>

<span data-ttu-id="93306-111">За да избегне потенциални повреда на данни и неочаквани поведения, които са причинени от неправилна инициализация и редактиране на записи на обекти на продажби, PSA вече включва логика за автоматично превключване на формуляри в стандартни формуляри.</span><span class="sxs-lookup"><span data-stu-id="93306-111">To avoid potential data corruption and unexpected behaviors that are caused by incorrect initialization and editing of the sales entity records, PSA now includes logic for automatic form switching in out-of-box forms.</span></span> <span data-ttu-id="93306-112">Тази логика отвежда потребителите до правилния формуляр за работа с базираната на работа версия или друг тип обект „Възможност“, „Оферта“, „Поръчка“ или „Фактура“.</span><span class="sxs-lookup"><span data-stu-id="93306-112">This logic takes users to the correct form for working with the work-based version or any other type of Opportunity, Quote, Order, or Invoice entity.</span></span> <span data-ttu-id="93306-113">Когато даден потребител отвори базирана на работа версия на обект „Възможност“, „Оферта“, „Поръчка“ или „Фактура“, формулярът се превключва към **Информация за проекта**.</span><span class="sxs-lookup"><span data-stu-id="93306-113">When a user opens the work-based version of an Opportunity, Quote, Order, or Invoice entity, the form is switched to **Project Information**.</span></span>

<span data-ttu-id="93306-114">Логиката на автоматичното превключване на формуляри разчита на съпоставянето между стойността **formId** и полето **msdyn\_ordertype**.</span><span class="sxs-lookup"><span data-stu-id="93306-114">The automatic form switching logic relies on the mapping between the **formId** value and the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="93306-115">Всички стандартни формуляри са добавени към това съпоставяне.</span><span class="sxs-lookup"><span data-stu-id="93306-115">All out-of-box forms have been added to that mapping.</span></span> <span data-ttu-id="93306-116">Персонализираните формуляри обаче трябва да се добавят ръчно, за да се укаже коя версия на обекта е планирано да обработват.</span><span class="sxs-lookup"><span data-stu-id="93306-116">However, custom forms must be manually added to indicate which version of the entity they are intended to handle.</span></span> <span data-ttu-id="93306-117">Това е базирано на полето **msdyn\_ordertype**.</span><span class="sxs-lookup"><span data-stu-id="93306-117">This is based on the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="93306-118">Ако превключването на формуляри липсва от съпоставянето, логиката ще превключи към стандартния формуляр въз основа на стойността, записана в полето **msdyn\_ordertype** на обекта.</span><span class="sxs-lookup"><span data-stu-id="93306-118">If the form switching is missing from the mapping, logic will switch to the out-of-box form, based on the value that is saved in the **msdyn\_ordertype** field of the entity.</span></span>

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a><span data-ttu-id="93306-119">Добавяне на потребителски формуляри и включване на логиката за превключване на формуляра</span><span class="sxs-lookup"><span data-stu-id="93306-119">Add custom forms and turn on the form switching logic</span></span>

<span data-ttu-id="93306-120">Следващият пример показва как да добавите персонализиран формуляр, **Информация за моя проект**, така че да работи с базирани на работа възможности.</span><span class="sxs-lookup"><span data-stu-id="93306-120">The following example shows how to add a custom form, **My Project Information**, so that it works with work-based opportunities.</span></span> <span data-ttu-id="93306-121">Същият процес се използва за добавяне на персонализирани формуляри, така че да работят с оферти, поръчки и фактури.</span><span class="sxs-lookup"><span data-stu-id="93306-121">The same process is used to add custom forms so that they work with quotes, orders, and invoices.</span></span>

<span data-ttu-id="93306-122">Изпълнете следните стъпки, за да създадете персонализирана версия на формуляра **Информация за проекта**.</span><span class="sxs-lookup"><span data-stu-id="93306-122">Follow these steps to create a custom version of the **Project Information** form.</span></span>

1. <span data-ttu-id="93306-123">В обекта „Възможност“ отворете формуляра **Информация за проекта** и запишете копие под името **Информация за моя проект**.</span><span class="sxs-lookup"><span data-stu-id="93306-123">In the Opportunity entity, open the **Project Information** form, and save a copy under the name **My Project Information**.</span></span>
2. <span data-ttu-id="93306-124">Отворете новия формуляр и след това в свойствата се уверете, че скриптовете за инициализация на формуляра от формуляр **Информация за проекта** са налице.</span><span class="sxs-lookup"><span data-stu-id="93306-124">Open the new form, and then, in the properties, make sure that the form initialization scripts from the **Project Information** form are present.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="93306-125">Не премахвайте скриптовете.</span><span class="sxs-lookup"><span data-stu-id="93306-125">Don't remove the scripts.</span></span> <span data-ttu-id="93306-126">В противен случай някои данни може да се инициализират неправилно.</span><span class="sxs-lookup"><span data-stu-id="93306-126">Otherwise, some data might be initialized incorrectly.</span></span>

3. <span data-ttu-id="93306-127">Проверете дали полето **Тип** (**msdyn\_ordertype**) е налице във формуляра.</span><span class="sxs-lookup"><span data-stu-id="93306-127">Verify that the **Type** (**msdyn\_ordertype**) field is present in the form.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="93306-128">Не премахвайте това поле.</span><span class="sxs-lookup"><span data-stu-id="93306-128">Don't remove this field.</span></span> <span data-ttu-id="93306-129">В противен случай скриптовете за инициализиране ще се изпълнят неуспешно.</span><span class="sxs-lookup"><span data-stu-id="93306-129">Otherwise, the initialization scripts will fail.</span></span>

4. <span data-ttu-id="93306-130">Намерете стойността **formId** на новия формуляр.</span><span class="sxs-lookup"><span data-stu-id="93306-130">Find the **formId** value of the new form.</span></span> <span data-ttu-id="93306-131">Можете да изпълните стъпката по два начина:</span><span class="sxs-lookup"><span data-stu-id="93306-131">You can complete this step in two ways:</span></span>

    - <span data-ttu-id="93306-132">Експортирайте формуляра **Информация за моя проект информация** като част от незавършено решение и след това потърсете стойността на **formid** във файла customization.xml на експортираното решение.</span><span class="sxs-lookup"><span data-stu-id="93306-132">Export the **My Project Information** form as part of an unmanaged solution, and then look up the **formId** value in the customization.xml file of the exported solution.</span></span>
    - <span data-ttu-id="93306-133">Отворете формуляра **Информация за моя проект** в редактора на формуляри и след това потърсете глобален еднозначен идентификатор (GUID) до параметъра **fromid** в URL адреса, както е показано на илюстрацията по-долу.</span><span class="sxs-lookup"><span data-stu-id="93306-133">Open the **My Project Information** form in the form editor, and then look for the globally unique identifier (GUID) next to the **fromId** parameter in the URL, as shown in the following illustration.</span></span>

    ![Стойността formId на новия формуляр в URL адреса](media/how-to-add-custom-forms-in-v2.0.png)

5. <span data-ttu-id="93306-135">Създайте съпоставяне на **msdyn\_ordertype** за стойността **formId**, като редактирате уеб ресурса msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js.</span><span class="sxs-lookup"><span data-stu-id="93306-135">Create an **msdyn\_ordertype** mapping for the **formId** value by editing the msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js web resource.</span></span> <span data-ttu-id="93306-136">Премахнете кода от ресурса и го заменете със следния код.</span><span class="sxs-lookup"><span data-stu-id="93306-136">Remove the code from the resource, and replace it with the following code.</span></span>

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

6. <span data-ttu-id="93306-137">Запишете и след това публикувайте персонализациите.</span><span class="sxs-lookup"><span data-stu-id="93306-137">Save and then publish the customizations.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]