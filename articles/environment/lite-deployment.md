---
title: Внедряване на Project Operations – олекотено
description: Тази тема предоставя информация за това как да инсталирате внедряване на Project Operations lite - сделка за проформа фактуриране.
author: stsporen
ms.date: 02/28/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: e33506504665f2e7ef7ad48469082f9f64a2a44b
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/14/2022
ms.locfileid: "8580719"
---
# <a name="deploy-project-operations---lite"></a>Внедряване на Project Operations – олекотено

_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_



Project Operations поддържа множество модели за разполагане. За да определите най-добрия модел за внедряване, вижте [Видове внедряване](determine-deployment-type.md).


> [!IMPORTANT]
> Това внедряване, олекотено внедряване - сделка за проформа фактуриране, води до внедряване само в **Dataverse на Project Operations**.

- [Инсталиране на операции на проекта в нова Dataverse среда](#new)
- [Инсталиране в съществуваща Dataverse среда](#existing)



## <a name="install-project-operations-to-a-new-dataverse-environment"></a><a name="new"></a> Инсталиране на операции на проект в нова Dataverse среда

1. Като [глобален или Power Platform администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) с лиценз за Операции по проекта създайте нова Dataverse среда в центъра [за администриране на](https://admin.powerplatform.com) PowerPlatform. Уверете се, че **създаване на база данни за тази среда** и **Приложения** на Dynamics 365 са разрешени. За повече информация вижте [Създаване и управляване на среди в центъра за администриране на Power Platform](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
2. Изберете **Microsoft Dynamics 365 Project Operations** от списъка с внедрявания на приложения на Dynamics 365.


## <a name="install-project-operations-to-an-existing-dataverse-environment"></a><a name="existing"></a> Инсталиране на операции на проект в съществуваща Dataverse среда
1. Осигурете, че средата не е конфигурирана с [двойно записване](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-overview) като инсталация след това ще инсталира [проект операции за ресурси/не-заредени](project-operations-integrated-deployment-overview.md) базирани сценарии възможности.
2. Като [глобален или Power Platform Администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) с лиценз за Project Operations, намерете среда в [Административен център на PowerPlatform](https://admin.powerplatform.com), където искате да инсталирате Project Operations.
3. Инсталирайте **Microsoft Dynamics 365 Project Operations** от списъка с внедрявания на приложения на Dynamics 365. За повече информация вижте [Управление на приложения на Dynamics 365](/power-platform/admin/manage-apps).




[!INCLUDE[footer-include](../includes/footer-banner.md)]
