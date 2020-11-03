---
title: Промени в обектите, контролите и потребителския интерфейс (Project Service Automation 3.x)
description: Тази тема описва промените в решението за Microsoft Dynamics Project Service Automation 3.x.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 03/15/2019
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
ms.openlocfilehash: 2d93e5eaae7cff302be1cb2e96e3f45c24739b0c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4072015"
---
# <a name="entity-control-and-user-interface-changes-project-service-automation-3x"></a>Промени в обектите, контролите и потребителския интерфейс (Project Service Automation 3.x)
В изданието на Microsoft Dynamics Project Service Automation (PSA) 3.x са направени много промени в обектите, контролите, изгледите и потребителския интерфейс. Тази тема предоставя информация относно тези важни промени.

## <a name="parent-child-relationships-for-sales-document-sales-document-line-sales-document-line-detail-entities"></a>Родителски-дъщерни релации за обектите документ за продажба, ред на документ за продажба, подробности за ред на документ за продажба
Във версиите на Dynamics 365 Project Service Automation (PSA), публикувани преди версия 3.0, някои от релациите между обектите документи за продажби, редове на документи за продажби и подробности за ред на документ за продажби се изпълняваха чрез полета от низов тип, които съхраняваха представяне на низ на GUID на свързания обект. Това се дължи на ограничения на платформата, които изискваха значителен персонализиран код от страната на сървъра и на клиента на решението, за да могат тези релации да работят, подобно на типичните релации между обекти в Dynamics CRM, и полетата от низов тип да функционират като справочни полета.

PSA 3.0 е актуализирана, за да използва новите релации между обектите документ за продажба и ред на документ за продажба.

Тъй като справочните полета вече могат да се използват за посочване на препратки към обекти, полетата, които съдържат стойността на низа на GUID на свързания обект в предишните версии, вече не са необходими и поради това са отхвърлени. Персонализираният код от страна на клиента и сървъра, който обработва релациите, дефинирани от наследени полета от низов тип, също е отхвърлен.

### <a name="entity-schema-changes"></a>Промени в схемата на обектите
Следващата таблица предоставя индивидуален списък на отхвърлените полета от низов тип и новите справочни полета за обектите. 

 Обект |   Отхвърлено поле (низ) | Ново поле (справочно)
--- | --- | ---
Подробности за фактура (ред на фактура) |  msdyn_contractline |    msdyn_contractlineid
msdyn_actual (действителни) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_contractlineinvoiceschedule (график за фактуриране на редове на договор по проект) |    msdyn_contractline |    msdyn_contractlineid
msdyn_contractlinescheduleofvalue (контролна точка за ред на договор по проект) |   msdyn_contractline |    msdyn_contractlineid
msdyn_fact (фактически) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_invoicelinetransaction (подробности за ред на фактура) | msdyn_invoiceline <br> msdyn_salescontractline | msdyn_invoicelineid <br> msdyn_salescontractlineid
msdyn_journalline (счетоводен запис) |  msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlineresourcecategory (категория ресурс за ред на договор по проект) | msdyn_salescontractline |   msdyn_contractlineid
msdyn_orderlinetransaction (подробности за ред на договор по проект) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlinetransactioncategory (категория транзакции на ред на договор по проект) |   msdyn_contractline |    msdyn_contractlineid
msdyn_orderlinetransactionclassification (класификация на транзакции на ред на договор по проект) |   msdyn_contractline |    msdyn_contractlineid
msdyn_quotelineinvoiceschedule (график за фактуриране на ред на оферта) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelineresourcecategory (категория на ресурс за ред на оферта) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinescheduleofvalue (контролна точка за ред на оферта) | msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransaction (подробности за ред на оферта) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactioncategory (категория транзакции за ред на оферта) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactionclassification (класификация на транзакция за ред на оферта) |  msdyn_quoteline |   msdyn_quotelineid
SalesOrderDetail (ред на поръчка) | msdyn_quotelineid | msdyn_quoteline 

### <a name="deprecated-custom-views-and-controls"></a>Отхвърлени персонализирани изгледи и контроли
Следните персонализирани изгледи и контроли и свързаните с тях артефакти са отхвърлени.

- Изглед на платимост.
- Персонализирани контроли за мрежа за показване на подробности за реда на офертата на страницата **Информация за проекта** за реда на офертата.
- Персонализирани контроли за показване на подробности за реда на офертата по проекта на страницата **Информация за проекта** за реда на поръчката за продажби.

> [!NOTE]
> За пълния списък с отхвърлени ресурси вижте [Отхвърлени уеб ресурси в Project Service Automation v3.x.](../developer-guides/web-resources-deprecated-v3.x.md)

## <a name="unified-client-interface-app-module"></a>Модул на приложението на унифициран клиентски интерфейс
С въвеждането на модулите на приложението на унифицирания клиентски интерфейс (UCI) записите в картата на сайта в PSA са премахнати от системата.  
Функционалността, свързана с превключване на формуляри за „Възможност“, „Оферта“, „Поръчка“ и „Фактура“, е отхвърлена като ненужна вече, защото модулът на приложението включва само версии за PSA на формулярите.  

Следните уеб ресурси са отхвърлени:

- msdyn_\SalesDocument\SalesDocumentFormLoader.js
- msdyn_\SalesDocument\PSSalesDocumentCustomFormIds.js

> [!NOTE]
> За пълния списък с отхвърлени ресурси вижте [Отхвърлени уеб ресурси в Project Service Automation v3.x.](../developer-guides/web-resources-deprecated-v3.x.md).


