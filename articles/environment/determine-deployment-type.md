---
title: Типове внедряване
description: Тази тема предоставя информация, която да ви помогне да определите правилния тип на внедряване за Project Operations за фирмата си.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: c3cf378caae4510482a8ee6771bf2e6decfe3b48
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948748"
---
# <a name="deployment-types"></a>Типове внедряване

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

> [!IMPORTANT]
> След като закупите лиценза, започнете оттук, за да определите най-добрия модел за внедряване на Dynamics 365 Project Operations с помощта на [Направляван поток на инсталация](https://aka.ms/provisionprojectoperations).
> След като завършите ръководството за инсталиране, ще бъдете насочени към правилния портал за управление, за да завършите инсталацията си. Вижте подробностите за разполагане по-долу, за да завършите инсталацията.


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a>Съществуващите клиенти на Dynamics използват Dynamics 365 Project Service Automation
Project Operations включва възможностите, предоставени с Project Service Automation. Пътека за надграждане ще бъде пусната за тези клиенти в бъдеще.

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a>Съществуващи клиенти на Dynamics 365 Finance използват управление на проекти и счетоводство 

Съществуващите клиенти на Finance, които използват функционалността за управление на проекта и счетоводството, могат да продължат да използват това, както е. Вижте [Project Operations за сценарии, базирани на наличност/поръчка за производство](#pma).

Project Operations поддържа множество опции за разполагане, за да отговарят на вашите изисквания. Независимо дали сте нов или съществуващ клиент на Dynamics 365, Project Operations може да поддържа вашите нужди.

Нашият [Въпросник за разполагане](https://aka.ms/provisionprojectoperations) ще ви помогне да определите правилното внедряване. Резултатите ще ви насочат към един от следните типове внедряване:

- [Леко внедряване – фактуриране на сделката към проформа](#lite)
- [Project Operations за сценарии, базирани на ресурси/неналичност](#integrated)
- [Project Operations за сценарии, базирани на наличност/поръчка за производство](#pma)

Project Operations поддържа сценарии за складирани / производствени поръчки и нескладирани / базирани на ресурси сценарии в същата среда чрез конфигурации на ниво юридическо лице. Например Contoso може да се възползва от възможностите за складиране / производствени поръчки в тяхното производствено съоръжение в САЩ (Юридическо лице = Contoso Manufacturing Съединени щати) и нескладови / базирани на ресурси възможности в сервиза си за обслужване Contoso Robotics Arms в Обединеното кралство (Юридическо лице = Contoso Robotics Обединено кралство).

## <a name="a-namelitelite-deployment---deal-to-proforma-invoicing"></a><a name="lite"><a/>Леко внедряване – фактуриране на сделката към проформа
Вграденото внедряване включва следните възможности:

- Планиране на проекти с помощта на Microsoft Project за мрежата
- Многоизмерно ценообразуване
- Унифицирано управление на ресурси
- Проследяване на време
- Основни разходи
- Предложение за фактура

### <a name="deployment-steps"></a>Стъпки на внедряването:
Определете най-добрия модел за внедряване на Project Operations с помощта на [Въпросник за разполагане](https://aka.ms/provisionprojectoperations).

За това разполагане вижте [Регистрация за абонаменти за предварителен преглед](lite-preview-subscription-sign-up.md) и [Осигуряване на нова среда](lite-deployment.md). 


## <a name="a-nameintegratedproject-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"><a/>Project Operations за сценарии, базирани на ресурси/неналичност
Project Operations за сценарии с ресурси / не складирани включват следните възможности:
  
- Планиране на проекти с помощта на Microsoft Project за мрежата
- Многоизмерно ценообразуване
- Унифицирано управление на ресурси
- Проследяване на време
- Основни разходи
- Пълен разход
- OCR на разписка
- Пълно фактуриране
- Признаване на приходите

### <a name="deployment-steps"></a>Стъпки на внедряването:
Определете най-добрия модел за внедряване на Project Operations с помощта на [Въпросник за разполагане](https://aka.ms/provisionprojectoperations).

За това разполагане вижте [Регистрация за абонаменти за предварителен преглед](resource-sign-up-preview-subscription.md) и [Осигуряване на нова среда](resource-provision-new-environment.md). 


## <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a>Project Operations за сценарии, базирани на наличност/поръчка за производство

- Планиране на проект с помощта на ССР
- Управление на ресурс
- Проследяване на време
- Пълен разход
- OCR на разписка
- Пълно фактуриране
- Признаване на приходите
- Производствени поръчки
- Поддръжка на материали

### <a name="deployment-steps"></a>Стъпки на внедряването:
Определете най-добрия модел за внедряване на Project Operations с помощта на [Въпросник за разполагане](https://aka.ms/provisionprojectoperations).

За това разполагане вижте [Регистрация за абонаменти за предварителен преглед](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) и [Осигуряване на нова среда](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json). 



