---
title: Внедряване на Project Operations – олекотено
description: Тази статия предоставя информация за това как да инсталирате внедряване на Project Operations lite - сделка за проформа фактуриране.
author: stsporen
ms.date: 02/28/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 86293b725e86db3d4b8bdaf5810b16b7c670e8a3
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930305"
---
# <a name="deploy-project-operations---lite"></a>Внедряване на Project Operations – олекотено

_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_



Project Operations поддържа множество модели за разполагане. За да определите най-добрия модел за внедряване, вижте [Видове внедряване](determine-deployment-type.md).


> [!IMPORTANT]
> Това внедряване, олекотено внедряване - сделка за проформа фактуриране, води до внедряване само в **Dataverse на Project Operations**.

- [Инсталиране на Project Operations в нова среда на Dataverse](#new)
- [Инсталирайте в съществуваща среда на Dataverse](#existing)



## <a name="install-project-operations-to-a-new-dataverse-environment"></a><a name="new"></a>Инсталиране на Project Operations в нова среда на Dataverse

1. Като [Глобален или Power Platform Администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) с лиценз за Project Operations, създайте нова среда на Dataverse в [Административен център на PowerPlatform](https://admin.powerplatform.com). Уверете се, че **Създайте база данни за тази среда** и **Приложения на Dynamics 365** са активирани. За повече информация вижте [Създаване и управляване на среди в центъра за администриране на Power Platform](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
2. Изберете **Microsoft Dynamics 365 Project Operations** от списъка с внедрявания на приложения на Dynamics 365.


## <a name="install-project-operations-to-an-existing-dataverse-environment"></a><a name="existing"></a>Инсталиране на Project Operations в съществуваща среда на Dataverse
1. Уверете се, че средата не е конфигурирана с [двойно писане](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-overview), тъй като инсталацията ще инсталира [Project Operations за сценарии, базирани на ресурси/неналичност](project-operations-integrated-deployment-overview.md) възможности.
2. Като [глобален или Power Platform Администратор](/power-platform/admin/global-service-administrators-can-administer-without-license) с лиценз за Project Operations, намерете среда в [Административен център на PowerPlatform](https://admin.powerplatform.com), където искате да инсталирате Project Operations.
3. Инсталирайте **Microsoft Dynamics 365 Project Operations** от списъка с внедрявания на приложения на Dynamics 365. За повече информация вижте [Управление на приложения на Dynamics 365](/power-platform/admin/manage-apps).




[!INCLUDE[footer-include](../includes/footer-banner.md)]
