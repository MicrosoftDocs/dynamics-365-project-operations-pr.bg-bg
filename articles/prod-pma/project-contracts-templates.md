---
title: Синхронизирайте договори за проекти и проекти директно от Project Service Automation с Finance
description: Тази тема описва шаблона и основните задачи, които се използват за синхронизиране на прогнозни часове на договор на проект и проекти директно от Microsoft Dynamics 365 Project Service Automation в Dynamics 365 Finance.
author: Yowelle
manager: AnnBe
ms.date: 12/17/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-13
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 85722f61a672cc55cd2b511dc80ebfbe4807b957
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950386"
---
# <a name="synchronize-project-contracts-and-projects-directly-from-project-service-automation-to-finance"></a>Синхронизирайте договори за проекти и проекти директно от Project Service Automation с Finance 

[!include[banner](../includes/banner.md)]

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Тази тема описва шаблона и основните задачи, които се използват за синхронизиране на прогнозни часове на договор на проект и проекти директно от Dynamics 365 Project Service Automation в Dynamics 365 Finance.

> [!NOTE] 
> Ако използвате Enterprise Edition 7.3.0, трябва да инсталирате KB 4074835.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Поток от данни за Project Service Automation към Finance

> [!NOTE]
> Преди да можете да използвате решението за интегриране на Project Service Automation to Finance, трябва да сте запознати с функцията за интегриране на данни на Dynamics 365.

Решението за интеграция на Project Service Automation to Finance използва функцията за интегриране на данни, за да синхронизира данните между копията на Project Service Automation и Finance. Шаблони за интеграция, които се предлагат с функцията за интеграция на данни, позволяват потока относно договори на проект, проект,аспекти на договор на проект и прогнозни разходи за проекти от Project Service Automation към Finance.

Следващата илюстрация показва как данните се синхронизират между Project Service Automation и Finance.

[![Поток от данни за интеграция на Project Service Automation с Finance](./media/ProjectsAndContractsFlow_upd.JPG)](./media/ProjectsAndContractsFlow.JPG)

## <a name="templates-and-tasks"></a>Шаблони и задачи

За достъп до наличните шаблони, в администраторски център на Microsoft Power Apps, изберете **Проекти** и след това в горния десен ъгъл изберете **Нов проект**, за да изберете публични шаблони.

Следният шаблони и основните задачи се използват за синхронизиране на договорите по проект и проекти от Project Service Automation към Finance:

### <a name="integrating-with-dynamics-365-project-service-automation-v2x"></a>Интегриране с Dynamics 365 Project Service Automation v2.x
- **Име на шаблона в Интегриране на данни:** Проекти и договори (Project Service Automation към Finance)
- **Име на задачите в проекта:**

    - Договори за проект за Project Service Automation към Finance
    - Проекти за Project Service Automation към Finance
    - Аспекти на договор за проект за Project Service Automation към Finance
    - Контролни точи на аспекти на договор за проект за Project Service Automation към Finance
  
### <a name="integrating-with-dynamics-365-project-service-automation-v3x"></a>Интегриране с Dynamics 365 Project Service Automation v3.x
В Project Service Automation има промяна на схемата, която влияе върху шаблона за етапа на проектната линия на договора и е необходима употреба на версията v2 на шаблона за интегриране на Project Service Automation v3.x с Dynamics 365.

- **Име на шаблона в Интегриране на данни:** Проекти и договори (Project Service Automation 3.x към Finance) - v2
- **Име на задачите в проекта:**

    - Договори за проект за Project Service Automation към Finance
    - Проекти за Project Service Automation към Finance
    - Аспекти на договор за проект за Project Service Automation към Finance
    - Контролни точи на аспекти на договор за проект за Project Service Automation към Finance

Преди да може да се случи синхронизиране на договори за проекти и проекти, трябва да синхронизирате акаунти.

## <a name="entity-set"></a>Набор от обекти

| Project Service Automation       | Finance                                                |
|----------------------------------|--------------------------------------------------------|
| Поръчки                           | Интеграционен обект за договори за проект                |
| Проекти                         | Интеграционен обект за проект                         |
| Редове на поръчка                      | Интеграционен обект за реда на договор за проект           |
| Контролни точки по аспекти на договор по проект | Интеграционен обект за контролна точка на договор за проект |

## <a name="entity-flow"></a>Поток на обекта

Договорите по проект за часовете на проекта се управляват в Project Service Automation и се синхронизират с Finance като прогнози договори по проект. Като част от шаблона за интеграция можете да зададете източника на интеграция във Finance за договор за проект.

Времето и материалите и проектите с фиксирана цена се управляват в Project Service Automation и се синхронизират с финанси като проекти. Като част от интеграцията на шаблона можете да зададете източника на интеграция за проекта във Finance. Понастоящем се поддържат само проекти с време и материали и с фиксирана цена.


Аспектите на договор по проект за часовете на проекта се управляват в Project Service Automation и се синхронизират с Finance като правила за фактуриране на договори. Ако методът за фактуриране се различава от типа проект по подразбиране, синхронизацията актуализира типа на проекта за проекта по линия на договора и групата на проекта.

Контролните точки на аспекти на договор по проект за часовете на проекта се управляват в Project Service Automation и се синхронизират с Finance като правила за контролни точки на правила на договор по проект.

## <a name="project-service-automation-to-finance-integration-solution"></a>Project Service Automation за интеграция на решението Finance

Полето **ИД на договор за проект** е достъпно на страницата **Договори за проекти**. Това поле е превърнато в естествен и уникален ключ в подкрепа на интеграцията.

Когато се създава нов договор за проект, ако стойност **ИД на договор за проект** вече не съществува, тя се генерира автоматично чрез използване на числова последователност. Стойността се състои от **ORD**, последвано от нарастваща последователност от числа и след това суфикс от шест знака. Ето един пример: **ORD-01022-Z4M9Q0**.

Полето **Номер на договор** е достъпно на страницата **Проекти**. Това поле е превърнато в естествен и уникален ключ в подкрепа на интеграцията.

Когато се създава нов проект, ако стойност **Номер на проект** още не съществува, тя се генерира автоматично чрез използване на числова последователност. Стойността се състои от **PRJ**, последвано от нарастваща последователност от числа и след това суфикс от шест знака. Ето един пример: **PRJ-01049-CCNID0**.

Когато се прилага решението за интегриране на Project Service Automation to Finance, скриптът за надстройка задава **ИД на договор за проект** поле за съществуващи договори за проекти и **Номер на проекта** поле за съществуващи проекти в Project Service Automation.

## <a name="prerequisites-and-mapping-setup"></a>Предпоставки и настройка на картографиране

- Преди да може да се случи синхронизиране на договори за проекти и проекти, трябва да синхронизирате акаунти.
- Във вашия набор от връзки добавете поле за интегриране на поле за ключ за **msdyn\_organizationalunits** на **msdyn\_name \[Name\]**. Може първо да се наложи да добавите проект към набора от връзки. За повече информация вижте [Интегриране на данни в Common Data Service за приложения](/powerapps/administrator/data-integrator).
- Във вашия набор от връзки добавете поле за интегриране на поле за ключ за **msdyn\_projects** на **msdynce\_projectnumber \[Project Number\]**. Може първо да се наложи да добавите проект към набора от връзки. За повече информация вижте [Интегриране на данни в Common Data Service за приложения](/powerapps/administrator/data-integrator).
- **SourceDataID** за договорите за проекти и проектите могат да бъдат актуализирани до различна стойност или премахнати от картографирането. Стойността на шаблона по подразбиране е **Project Service Automation**.
- Картографирането **PaymentTerms** трябва да бъде актуализирано, така че да отразява валидни условия на плащане във финансите. Можете също да премахнете картографирането от проектната задача. Картата по подразбиране има стойности по подразбиране за демонстрационни данни. Следващата таблица показва стойностите в Project Service Automation.

    | Стойност | Описание   |
    |-------|---------------|
    | 1     | Нето 30        |
    | 2     | 2% 10, Нето 30 |
    | 3     | Нето 45        |
    | 4     | Нето 60        |

## <a name="power-query"></a>Power Query

Използвайте Microsoft Power Query за Excel, за да филтрирате данни, ако са изпълнени следните условия:

- Имате поръчки за продажба в Dynamics 365 Sales.
- Имате няколко организационни единици в Project Service Automation и тези организационни единици ще бъдат съпоставени с множество юридически лица във финансите.

Ако трябва да използвате Power Query, следвайте тези указания:

- Шаблонът Проекти и договори (PSA до Fin и Ops) има филтър по подразбиране, който включва само поръчки за продажба на **Работен елемент (msdyn\_ordertype = 192350001)** тип. Този филтър помага да се гарантира, че не се създават договори за проекти за поръчки за продажба във Finance. Ако създадете свой собствен шаблон, трябва да добавите този филтър.
- Създайте филтър Power Query, който включва само договорните организации, които трябва да бъдат синхронизирани с юридическото лице на набора за интеграционна връзка. Например проектни договори, които имате с организационната единица на договорите Contoso US трябва да бъдат синхронизирани с юридическото лице USSI, но договорите за проекти, които имате с организационната единица на договора на Contoso Global трябва да се синхронизира с юридическото лице на USMF. Ако не добавите този филтър към картографирането на вашата задача, всички договори за проекти ще бъдат синхронизирани с юридическото лице, което е дефинирано за набора от връзки, независимо от организационната единица на договора.

## <a name="template-mapping-in-data-integration"></a>Съпоставяне на шаблони при интеграция на данни

> [!NOTE] 
> Полетата **CustomerReference**, **AddressCity**, **AddressCountryRegionID**, **AddressDescription**, **AddressLine1**, **AddressLine2**, **AddressState** и **AddressZipCode** не са включени в картографирането по подразбиране за проектни договори. Можете да добавите съпоставянията, ако изисквате тези данни да бъдат синхронизирани за договори за проекти.
>
> Полетата **Описание**, **ParentID**, **ProjectGroup**, **ProjectManagerPersonnelNumber** и **ProjectType** не са включени в картографирането по подразбиране за проекти. Можете да добавите съпоставянията, ако изисквате тези данни да бъдат синхронизирани за проекти.

Следните илюстрации показват примери на нанасяне на задача за съпоставяне в интеграция на данни. Картографирането показва информация за полето, която ще бъде синхронизирана от Project Service Automation към Finance.

[![Съпоставяне на шаблон на договор за проект](./media/ProjectContractTemplateMapping.JPG)](./media/ProjectContractTemplateMapping.JPG)

[![Съпоставяне на шаблон на проект](./media/ProjectTemplateMapping.JPG)](./media/ProjectTemplateMapping.JPG)

[![Съпоставяне на шаблон на редове на договор за проект](./media/ProjectContractLinesMapping.JPG)](./media/ProjectContractLinesMapping.JPG)

[![Съпоставяне на шаблон на контролна точка на аспекти на договор за проект](./media/ProjectContractLineMilestonesMapping.JPG)](./media/ProjectContractLineMilestonesMapping.JPG)

#### <a name="project-contract-line-milestone-mapping-in-the-projects-and-contracts-psa-3x-to-dynamics---v2-template"></a>Съпоставяне на етапа на проектната линия на проекти в проекти и договори (PSA 3.x към Dynamics) - шаблон v2:

[![Съпоставяне на шаблон на контролна точка с шаблон на втора версия](./media/ProjectContractLineMilestoneMapping_v2.jpg)](./media/ProjectContractLineMilestoneMapping_v2.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]