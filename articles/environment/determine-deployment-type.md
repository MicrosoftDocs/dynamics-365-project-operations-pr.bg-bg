---
title: Определяне на типа на внедряването ви
description: Тази тема предоставя информация, която да ви помогне да определите правилния тип на внедряване за Project Operations за фирмата си.
author: stsporen
manager: Annbe
ms.date: 11/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: e9d3a5d8e6e1daafac72a3b4c0380b679d1869bd
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401205"
---
# <a name="determine-your-deployment-type"></a>Определяне на типа на внедряването ви

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

> [!IMPORTANT]
> След като закупите лиценза, започнете оттук, за да определите най-добрия модел за внедряване на Dynamics 365 Project Operations с помощта на [Направляван поток на инсталация](https://aka.ms/provisionprojectoperations).
> След като завършите ръководството за инсталиране, ще бъдете насочени към правилния портал за управление, за да завършите инсталацията си. Вижте подробностите за разполагане, за да завършите инсталацията.


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a>Съществуващите клиенти на Dynamics използват Dynamics 365 Project Service Automation
Project Operations включва възможностите, предоставени с Project Service Automation. Пътят за надстройка ще бъде издаден за тези клиенти в изданието от 2021 г., вълна 1.

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a>Съществуващи клиенти на Dynamics 365 Finance използват управление на проекти и счетоводство 

Съществуващите клиенти на Finance, които използват функционалността за управление на проекти и счетоводство, могат да продължат да я използват както е. Вижте [Project Operations за сценарии, базирани на наличност/поръчка за производство](#pma).


## <a name="deployment-types"></a>Типове внедряване
Project Operations поддържа множество опции за разполагане, за да отговарят на вашите изисквания. Независимо дали сте нов или съществуващ клиент на Dynamics 365, Project Operations може да поддържа вашите нужди.

Нашият [Въпросник за разполагане](https://aka.ms/provisionprojectoperations) ще ви помогне да определите правилното внедряване. Резултатите ще ви насочат към един от следните типове внедряване:

- [Леко внедряване – фактуриране на сделката към проформа](#lite)
- [Project Operations за сценарии, базирани на ресурси/неналичност](#integrated)
- [Project Operations за сценарии, базирани на наличност/поръчка за производство](#pma)

Project Operations поддържа сценарии за складирани / производствени поръчки и нескладирани / базирани на ресурси сценарии в същата среда чрез конфигурации на ниво юридическо лице. Например Contoso може да използва възможностите за складиране / производствени поръчки в своето производствено съоръжение в САЩ (юридическо лице = Contoso Manufacturing United States). Contoso може да използва нескладовите / базирани на ресурси възможности в тяхното съоръжение за обслужване на Contoso Robotics Arms в Обединеното кралство (юридическо лице = Contoso Robotics United Kingdom).

### <a name="lite-deployment---deal-to-proforma-invoicing"></a><a  name="lite"></a>Леко внедряване – фактуриране на сделката към проформа

Вграденото внедряване включва следните възможности:

- Процес на продажби за проекти, който разширява работата с приложенията на Dynamics 365 Sales
- Планиране на проекти с помощта на Microsoft Project за мрежата
- Многоизмерно ценообразуване
- Унифицирано управление на ресурси
- Проследяване на време
- Основен разход
- Проформа фактури и фактуриране за клиенти 

#### <a name="deployment-steps"></a>Стъпки на внедряването
Определете най-добрия модел за внедряване на Project Operations с помощта на [Въпросник за разполагане](https://aka.ms/provisionprojectoperations).

За това разполагане вижте [Регистрация за абонаменти за предварителен преглед](lite-preview-subscription-sign-up.md) и [Осигуряване на нова среда](lite-deployment.md). 


### <a name="project-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"></a>Project Operations за сценарии, базирани на ресурси/неналичност
Project Operations за сценарии с ресурси / не складирани включват следните възможности:
 
- Процес на продажби за проекти, който разширява приложенията на Dynamics 365 Sales
- Планиране на проекти с помощта на Microsoft Project за мрежата
- Многоизмерно ценообразуване
- Унифицирано управление на ресурси
- Проследяване на време
- Основен разход
- Пълен разход
- OCR на разписка
- Проформа фактури и фактуриране за клиенти 
- Признаване на приходи за проекти

#### <a name="deployment-steps"></a>Стъпки на внедряването
Определете най-добрия модел за внедряване на Project Operations с помощта на [Въпросник за разполагане](https://aka.ms/provisionprojectoperations).

За това разполагане вижте [Регистрация за абонаменти за предварителен преглед](resource-sign-up-preview-subscription.md) и [Осигуряване на нова среда](resource-provision-new-environment.md). 


### <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a>Project Operations за сценарии, базирани на наличност/поръчка за производство

- Планиране на проект с помощта на ССР
- Управление на ресурс
- Проследяване на време
- Пълен разход
- OCR на разписка
- Пълно фактуриране
- Признаване на приходите
- Производствени поръчки
- Поддръжка на материали

#### <a name="deployment-steps"></a>Стъпки на внедряването
Определете най-добрия модел за внедряване на Project Operations с помощта на [Въпросник за разполагане](https://aka.ms/provisionprojectoperations).

За това разполагане вижте [Регистрация за абонаменти за предварителен преглед](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) и [Осигуряване на нова среда](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json). 

