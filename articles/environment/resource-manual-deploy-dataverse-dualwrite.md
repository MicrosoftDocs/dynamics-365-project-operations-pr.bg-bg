---
title: Ръчно внедряване на приложението Project Operations Dataverse с поддръжка на двойно писане
description: Тази тема обяснява как да разгърнете ръчно приложението Project Operations Dataverse, така че да поддържа двойно писане.
author: stsporen
ms.date: 06/18/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 2ad147da542fc9e7a2705da7a834d1a6512907e5
ms.sourcegitcommit: 205a94ab4168de25b102f31d00a691c8205ba63e
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/18/2021
ms.locfileid: "6273995"
---
# <a name="manually-deploy-the-project-operations-dataverse-app-with-dual-write-support"></a><span data-ttu-id="82f39-103">Ръчно внедряване на приложението Project Operations Dataverse с поддръжка на двойно писане</span><span class="sxs-lookup"><span data-stu-id="82f39-103">Manually deploy the Project Operations Dataverse app with dual-write support</span></span>

<span data-ttu-id="82f39-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="82f39-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="82f39-105">Тази тема обяснява как да разгърнете ръчно Microsoft Dynamics 365 Project Operations в Microsoft Dataverse, така че да поддържа двойно писане.</span><span class="sxs-lookup"><span data-stu-id="82f39-105">This topic explains how to manually deploy Microsoft Dynamics 365 Project Operations in Microsoft Dataverse so that it supports dual-write.</span></span> <span data-ttu-id="82f39-106">Project Operations открива конфигурацията на средата и добавя допълнителна поддръжка за двойно писане, ако са изпълнени предпоставките.</span><span class="sxs-lookup"><span data-stu-id="82f39-106">Project Operations detects the environment's configuration and adds additional support for dual-write if the prerequisites are met.</span></span>

<span data-ttu-id="82f39-107">По време на разполагането чрез Microsoft Dynamics Lifecycle Services (LCS), ако сте следвали инструкциите в тази тема, можете да пропуснете разполагането на интеграция на Microsoft Power Platform (известна преди като среда на Common Data Service).</span><span class="sxs-lookup"><span data-stu-id="82f39-107">During deployment through Microsoft Dynamics Lifecycle Services (LCS), if you've followed the instructions in this topic, you can skip the deployment of the Microsoft Power Platform integration (previously known as the Common Data Service environment).</span></span>

<span data-ttu-id="82f39-108">Процесът на внедряване на Project Operations в Dataverse така че да поддържа двойно писане има четири основни стъпки:</span><span class="sxs-lookup"><span data-stu-id="82f39-108">The process of deploying Project Operations in Dataverse so that it supports dual-write has four main steps:</span></span>

1. <span data-ttu-id="82f39-109">[Създайте нова среда в Dataverse, която поддържа двойно писане](#create).</span><span class="sxs-lookup"><span data-stu-id="82f39-109">[Create a new environment in Dataverse that supports dual-write](#create).</span></span>
2. <span data-ttu-id="82f39-110">[Добавете двойни условия за запис в средата](#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="82f39-110">[Add dual-write prerequisites to the environment](#prerequisites).</span></span>
3. <span data-ttu-id="82f39-111">[Добавете приложението Project Operations Dataverse](#dataverse).</span><span class="sxs-lookup"><span data-stu-id="82f39-111">[Add the Project Operations Dataverse app](#dataverse).</span></span>
4. <span data-ttu-id="82f39-112">[Връзка към средите ви](#link).</span><span class="sxs-lookup"><span data-stu-id="82f39-112">[Link your environments](#link).</span></span>

## <a name="create-a-new-environment-in-dataverse-that-supports-dual-write"></a><a name="create"></a><span data-ttu-id="82f39-113">Създайте нова среда в Dataverse, която поддържа двойно писане</span><span class="sxs-lookup"><span data-stu-id="82f39-113">Create a new environment in Dataverse that supports dual-write</span></span>

<span data-ttu-id="82f39-114">За да завършите тази процедура, трябва да влезете като администратор.</span><span class="sxs-lookup"><span data-stu-id="82f39-114">To complete this procedure, you must sign in as an administrator.</span></span>

1. <span data-ttu-id="82f39-115">Отворете [Център за администриране на Power Platform](https://admin.powerplatform.com) и влезте като администратор.</span><span class="sxs-lookup"><span data-stu-id="82f39-115">Open the [Power Platform admin center](https://admin.powerplatform.com), and sign in as an administrator.</span></span>
2. <span data-ttu-id="82f39-116">Създайте нова среда и я наименувайте.</span><span class="sxs-lookup"><span data-stu-id="82f39-116">Create a new environment, and name it.</span></span>
3. <span data-ttu-id="82f39-117">Избор на тип среда.</span><span class="sxs-lookup"><span data-stu-id="82f39-117">Select the environment type.</span></span> <span data-ttu-id="82f39-118">Ако сте се регистрирали за пробната оферта, изберете **Пробен период (базиран на абонамент)**.</span><span class="sxs-lookup"><span data-stu-id="82f39-118">If you signed up for the trial offer, select **Trial (subscription-based)**.</span></span>
4. <span data-ttu-id="82f39-119">Потвърдете региона за разполагане.</span><span class="sxs-lookup"><span data-stu-id="82f39-119">Confirm the deployment region.</span></span>
5. <span data-ttu-id="82f39-120">Активирайте **Създайте база данни за тази среда** опция.</span><span class="sxs-lookup"><span data-stu-id="82f39-120">Enable the **Create a database for this environment** option.</span></span> 
6. <span data-ttu-id="82f39-121">Потвърдете езика и след това потвърдете, че валутата съответства на валутата за вашите приложения на Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="82f39-121">Confirm the language, and then confirm that the currency matches the currency for your Finance and Operations apps.</span></span>
7. <span data-ttu-id="82f39-122">Активирайте **Приложения на Dynamics 365** и потвърдете, че **Автоматично внедряване на тези приложения** полето е зададено на **Няма**.</span><span class="sxs-lookup"><span data-stu-id="82f39-122">Enable the **Dynamics 365 apps** option, and confirm that the **Automatically deploy these apps** field is set to **None**.</span></span>
8. <span data-ttu-id="82f39-123">Добавете група за защита, ако се изисква група за защита.</span><span class="sxs-lookup"><span data-stu-id="82f39-123">Add a security group, if a security group is required.</span></span>
9. <span data-ttu-id="82f39-124">Изберете **Запиши**, за да създадете средата.</span><span class="sxs-lookup"><span data-stu-id="82f39-124">Select **Save** to create the environment.</span></span>
10. <span data-ttu-id="82f39-125">Изчакайте, докато внедряването завърши и средата достигне състояние **Готово**.</span><span class="sxs-lookup"><span data-stu-id="82f39-125">Wait until the deployment is completed and the environment reaches the **Ready** state.</span></span>

## <a name="add-dual-write-prerequisites-to-the-environment"></a><a name="prerequisites"></a><span data-ttu-id="82f39-126">Добавете двойни условия за запис в средата</span><span class="sxs-lookup"><span data-stu-id="82f39-126">Add dual-write prerequisites to the environment</span></span>

<span data-ttu-id="82f39-127">Поддръжката на двойно писане включва допълнителни полета, които се добавят към ключови обекти, като например обект **фирма**.</span><span class="sxs-lookup"><span data-stu-id="82f39-127">Dual-write support includes additional fields that are added to key entities, such as the **Company** entity.</span></span> <span data-ttu-id="82f39-128">Ако добавяте поддръжка за двойно писане към съществуваща среда, може да се наложи да актуализирате данните, за да активирате поддръжката.</span><span class="sxs-lookup"><span data-stu-id="82f39-128">If you're adding dual-write support to an existing environment, you might have to update the data to enable the support.</span></span> <span data-ttu-id="82f39-129">За информация как да стартирате данните вижте [Данни за Bootstrap фирма](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data).</span><span class="sxs-lookup"><span data-stu-id="82f39-129">For information about how to bootstrap the data, see [Bootstrap company data](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data).</span></span> <span data-ttu-id="82f39-130">За повече информация относно двойното писане вижте [Системни изисквания за двойно записване](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).</span><span class="sxs-lookup"><span data-stu-id="82f39-130">For more information about dual-write, see [Dual-write system requirements](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).</span></span>

<span data-ttu-id="82f39-131">Завършете тази процедура, за да добавите предпоставките за двойно писане към вашата среда.</span><span class="sxs-lookup"><span data-stu-id="82f39-131">Complete this procedure to add the dual-write prerequisites to your environment.</span></span>

1. <span data-ttu-id="82f39-132">Отворете средата, която току-що създадохте, и след това отидете на **Ресурс** \> **Приложения на Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="82f39-132">Open the environment that you just created, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="82f39-133">Изберете **Основно решение с двойно записване** в списъка с приложения и го инсталирайте.</span><span class="sxs-lookup"><span data-stu-id="82f39-133">Select **Dual-write core solution** in the app list, and install it.</span></span>
3. <span data-ttu-id="82f39-134">Изчакайте, докато инсталацията приключи.</span><span class="sxs-lookup"><span data-stu-id="82f39-134">Wait until the installation is completed.</span></span> <span data-ttu-id="82f39-135">След това изберете **Решение за управление на приложение с двойно записване** в списъка с приложения и го инсталирайте.</span><span class="sxs-lookup"><span data-stu-id="82f39-135">Then select **Dual-write application orchestration solution** in the app list, and install it.</span></span>

## <a name="add-the-project-operations-dataverse-app"></a><a name="dataverse"></a><span data-ttu-id="82f39-136">Добавете приложението Project Operations Dataverse</span><span class="sxs-lookup"><span data-stu-id="82f39-136">Add the Project Operations Dataverse app</span></span>

<span data-ttu-id="82f39-137">Можете да завършите тази процедура само ако сте изпълнили предишните процедури, преди да сте инсталирали Project Operations.</span><span class="sxs-lookup"><span data-stu-id="82f39-137">You can complete this procedure only if you completed the previous procedures before you installed Project Operations.</span></span> <span data-ttu-id="82f39-138">По време на инсталацията системата анализира конфигурацията на средата и добавя поддръжка за двойно писане, ако е необходимо.</span><span class="sxs-lookup"><span data-stu-id="82f39-138">During installation, the system analyzes the environment configuration and adds support for dual-write if it's required.</span></span>

1. <span data-ttu-id="82f39-139">Отворете средата, която създадохте по-рано, и след това отидете на **Ресурс** \> **Приложения на Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="82f39-139">Open the environment that you created earlier, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="82f39-140">Изберете **Microsoft Dynamics 365 Project Operations** в списъка с приложения и го инсталирайте.</span><span class="sxs-lookup"><span data-stu-id="82f39-140">Select **Microsoft Dynamics 365 Project Operations** in the app list, and install it.</span></span>

## <a name="link-your-environments"></a><a name="link"></a><span data-ttu-id="82f39-141">Връзка към средите ви</span><span class="sxs-lookup"><span data-stu-id="82f39-141">Link your environments</span></span>

<span data-ttu-id="82f39-142">След внедряването на Dataverse среда, можете да настроите връзката във вашите приложения на Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="82f39-142">After the Dataverse environment is deployed, you can set up the link in your Finance and Operations apps.</span></span> <span data-ttu-id="82f39-143">Следвайте стъпките в [Използвайте съветника за двойно писане, за да свържете вашата среда](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).</span><span class="sxs-lookup"><span data-stu-id="82f39-143">Follow the steps in [Use the dual-write wizard to link your environments](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).</span></span>
