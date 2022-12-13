---
title: Внедряване на операции по проекти Lite
description: Тази статия предоставя информация за това как да инсталирате внедряване на Project Operations lite - сделка за проформа фактуриране.
author: stsporen
ms.date: 11/29/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 2c508f56b3018b6a86fea78bcf9ee4136e90f385
ms.sourcegitcommit: 38cb012502cbd640abbc21a0912b195112b27ccb
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/30/2022
ms.locfileid: "9810965"
---
# <a name="deploy-project-operations-lite"></a>Внедряване на операции по проекти Lite

_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_



Project Operations поддържа множество модели за разполагане. За да определите най-добрия модел за внедряване, вижте [Видове внедряване](determine-deployment-type.md).


> [!IMPORTANT]
> Това внедряване, олекотено внедряване - сделка за проформа фактуриране, води до внедряване само в **Dataverse на Project Operations**.

- [Инсталиране на Project Operations в нова среда на Dataverse](#new)
- [Инсталирайте в съществуваща среда на Dataverse](#existing)
- [Инсталиране в съществуваща Dataverse среда, която има компоненти за двоен запис](#existingdw)



## <a name="install-project-operations-lite-to-a-new-dataverse-environment"></a><a name="new"></a> Инсталиране на Project Operations Lite в нова Dataverse среда

1. Като [Глобален или Power Platform Администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) с лиценз за Project Operations, създайте нова среда на Dataverse в [Административен център на PowerPlatform](https://admin.powerplatform.com). Уверете се, че **Създайте база данни за тази среда** и **Приложения на Dynamics 365** са активирани. За повече информация вижте [Създаване и управляване на среди в центъра за администриране на Power Platform](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
1. Изберете **Microsoft Dynamics 365 Project Operations** от списъка с внедрявания на приложения на Dynamics 365.


## <a name="install-project-operations-lite-to-an-existing-dataverse-environment"></a><a name="existing"></a> Инсталиране на Project Operations Lite в съществуваща Dataverse среда 
1. Като [глобален или Power Platform Администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) с лиценз за Project Operations, намерете среда в [Административен център на PowerPlatform](https://admin.powerplatform.com), където искате да инсталирате Project Operations.
1. Инсталирайте **Microsoft Dynamics 365 Project Operations** от списъка с внедрявания на приложения на Dynamics 365. За повече информация вижте [Управление на приложения на Dynamics 365](/power-platform/admin/manage-apps).

## <a name="install-project-operations-lite-to-an-existing-dataverse-environment-where-dual-write-solutions-are-already-present"></a><a name="existingdw"></a> Инсталирайте Project Operations Lite в съществуваща Dataverse среда, където вече има решения за двойно писане

Ако искате да продължите да изпълнявате операции по проекта в режим на олекотено разполагане, трябва да изпълните следните стъпки:

1. Като [глобален или Power Platform Администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) с лиценз за Project Operations, намерете среда в [Административен център на PowerPlatform](https://admin.powerplatform.com), където искате да инсталирате Project Operations.
1. Инсталирайте **Microsoft Dynamics 365 Project Operations** от списъка с внедрявания на приложения на Dynamics 365. За повече информация вижте [Управление на приложения на Dynamics 365](/power-platform/admin/manage-apps).
1. Тъй като вашата среда има инсталирани компоненти за двойно писане, които помагат при интегрирането на приложения за финансиране и операции, инсталацията на Project Operations също ще инсталира възможностите и разширенията, необходими за интегриране на данни, свързани с проекта, към приложения за финансиране и операции. Тъй като искате да стартирате Project Operations in Lite разполагане, тези компоненти за интеграция трябва да бъдат премахнати, тъй като те ще създадат ограничения и режийни разходи за Lite сценарии за разполагане. Ръчно деинсталирайте решенията **Dynamics 365 Project Operations Dual Write и** Dual Write **Dynamics 365 Project Operations Entity Maps**, за да премахнете тези компоненти.
1. Отидете на Операции на **проекта -> Настройки -> параметри**. Отворете страницата с подробни данни за параметрите **на проекта и задайте полето Поведение** при **надстройка на решение само на**  **Lite**. Това гарантира, че всички последващи подобрения на операциите по проекта няма да върнат интеграционните компоненти в операциите по проекта.  

[!INCLUDE[footer-include](../includes/footer-banner.md)]
