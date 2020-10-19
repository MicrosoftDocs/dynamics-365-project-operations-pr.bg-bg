---
title: Внедряване на Project Operations Lite – фактуриране на сделката към проформа
description: Тази тема предоставя информация за това как да инсталирате внедряване на Project Operations lite - сделка за проформа фактуриране.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: e938876d459b3f6dfedd90e57e3042cda96bffb7
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948746"
---
# <a name="deploy-project-operations-lite-deployment--deal-to-proforma-invoicing"></a><span data-ttu-id="7b28a-103">Внедряване на Project Operations Lite – фактуриране на сделката към проформа</span><span class="sxs-lookup"><span data-stu-id="7b28a-103">Deploy Project Operations Lite deployment – deal to proforma invoicing</span></span>

<span data-ttu-id="7b28a-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="7b28a-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7b28a-105">Project Operations поддържа множество модели за разполагане.</span><span class="sxs-lookup"><span data-stu-id="7b28a-105">Project Operations supports multiple deployment models.</span></span> <span data-ttu-id="7b28a-106">За да определите най-добрия модел за внедряване, вижте [Видове внедряване](determine-deployment-type.md).</span><span class="sxs-lookup"><span data-stu-id="7b28a-106">To determine the best deployment model, see [Deployment types](determine-deployment-type.md).</span></span>


> [!IMPORTANT]
> <span data-ttu-id="7b28a-107">Това внедряване, олекотено внедряване - сделка за проформа фактуриране, води до внедряване само в **Common Data Service на Project Operations**.</span><span class="sxs-lookup"><span data-stu-id="7b28a-107">This deployment, Lite deployment – deal to proforma invoicing, results in a **Common Data Service-only deployment of Project Operations**.</span></span>

- [<span data-ttu-id="7b28a-108">Инсталиране на Project Operations в нова среда на CDS</span><span class="sxs-lookup"><span data-stu-id="7b28a-108">Install Project Operations into a new CDS environment</span></span>](#new)
- [<span data-ttu-id="7b28a-109">Инсталирайте в съществуваща CDS среда</span><span class="sxs-lookup"><span data-stu-id="7b28a-109">Install into an existing CDS environment</span></span>](#existing)



## <a name="install-project-operations-to-a-new-cds-environment"></a><a name="new"></a><span data-ttu-id="7b28a-110">Инсталиране на Project Operations в нова среда на CDS</span><span class="sxs-lookup"><span data-stu-id="7b28a-110">Install Project Operations to a new CDS environment</span></span>

1. <span data-ttu-id="7b28a-111">Като [Глобален или Power Platform Администратор](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) с лиценз за Project Operations, създайте нова среда на CDS в [Административен център на PowerPlatform](https://admin.powerplatform.com).</span><span class="sxs-lookup"><span data-stu-id="7b28a-111">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, create a new CDS environment in the [PowerPlatform admin center](https://admin.powerplatform.com).</span></span> <span data-ttu-id="7b28a-112">Уверете се, че **CDS база данни** и **Приложения на Dynamics 365** са активирани.</span><span class="sxs-lookup"><span data-stu-id="7b28a-112">Make sure that **CDS database** and **Dynamics 365 Apps** are enabled.</span></span> <span data-ttu-id="7b28a-113">За повече информация вижте [Създаване и управляване на среди в центъра за администриране на Power Platform](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span><span class="sxs-lookup"><span data-stu-id="7b28a-113">For more information, see [Create and manage environments in the Power Platform admin center](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span></span>
2. <span data-ttu-id="7b28a-114">Изберете **Microsoft Dynamics 365 Project Operations** от списъка за внедряване на приложения на Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="7b28a-114">Select **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span>


## <a name="install-project-operations-to-an-existing-cds-environment"></a><a name="existing"></a><span data-ttu-id="7b28a-115">Инсталиране на Project Operations в съществуваща среда на CDS</span><span class="sxs-lookup"><span data-stu-id="7b28a-115">Install Project Operations to an existing CDS environment</span></span>

1. <span data-ttu-id="7b28a-116">Като [глобален или Power Platform Администратор](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) с лиценз за Project Operations, намерете среда в [Административен център на PowerPlatform](https://admin.powerplatform.com), където искате да инсталирате Project Operations.</span><span class="sxs-lookup"><span data-stu-id="7b28a-116">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, locate the environment in the [PowerPlatform admin center](https://admin.powerplatform.com) where you want to install Project Operations.</span></span>
2. <span data-ttu-id="7b28a-117">Инсталирайте **Microsoft Dynamics 365 Project Operations** от списъка за внедряване на приложения на Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="7b28a-117">Install **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span> <span data-ttu-id="7b28a-118">За повече информация вижте [Управление на приложения на Dynamics 365](https://docs.microsoft.com/power-platform/admin/manage-apps).</span><span class="sxs-lookup"><span data-stu-id="7b28a-118">For more information, see [Manage Dynamics 365 apps](https://docs.microsoft.com/power-platform/admin/manage-apps).</span></span>


