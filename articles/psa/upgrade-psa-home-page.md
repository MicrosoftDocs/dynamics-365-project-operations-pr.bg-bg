---
title: Начална страница за надстройка
description: Тази тема показва къде да намерите важна информация за новите и променените функции в Dynamics 365 Project Service Automation и процеса за надстройване до най-новата версия.
manager: kfend
ms.prod: ''
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 05/30/2019
ms.topic: article
author: rumant
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 838eecb1229ea20106c7d5487dc37a81e8df501b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281690"
---
# <a name="upgrade-home-page"></a><span data-ttu-id="621f4-103">Начална страница за надстройка</span><span class="sxs-lookup"><span data-stu-id="621f4-103">Upgrade home page</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

## <a name="upgrade-from-psa-version-2x-or-1x-to-version-3x"></a><span data-ttu-id="621f4-104">Надстройка от PSA, версия 2.x или 1.x до версия 3.x</span><span class="sxs-lookup"><span data-stu-id="621f4-104">Upgrade from PSA version 2.x or 1.x to version 3.x</span></span>

### <a name="new-instances"></a><span data-ttu-id="621f4-105">Нови екземпляри</span><span class="sxs-lookup"><span data-stu-id="621f4-105">New instances</span></span>

<span data-ttu-id="621f4-106">От 17 май 2019 г., когато Project Service Automation се избере по време на обезпечаване на нов екземпляр, версия 3.x се инсталира по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="621f4-106">As of May 17, 2019, when Project Service Automation is selected during the provisioning of a new instance, version 3.x is installed by default.</span></span>

### <a name="existing-instances"></a><span data-ttu-id="621f4-107">Съществуващи екземпляри</span><span class="sxs-lookup"><span data-stu-id="621f4-107">Existing instances</span></span>

<span data-ttu-id="621f4-108">Преди клиенти, които имат екземпляр на PSA версия 2.x и трябваше да надстроят до версия 3.x, която е версия на PSA, базирана на Унифициран интерфейс на клиент (UCI), трябваше да се свържат с поддръжката на Microsoft и да предоставят подробности за техния екземпляр, така че поддръжката да може да разреши надстройване на екземпляра до версия 3.x например.</span><span class="sxs-lookup"><span data-stu-id="621f4-108">Previously, customers who have an instance of PSA version 2.x and needed to upgrade to version 3.x, which is the Unified client interface-based (UCI) version of PSA, had to contact Microsoft Support and provide the details of their instance so that support could enable the instance for upgrade to version 3.x.</span></span> <span data-ttu-id="621f4-109">От 1 март 2020 г. клиентите, които имат екземпляр на PSA версия 2.x и трябва да надстроят до версия 3.x, ще могат да надстроят своите копия директно от портала на администратор, без да се налага да се свързват с поддръжката на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="621f4-109">As of March 1, 2020, customers who have an instance of PSA version 2.x and need to upgrade to version 3.x, will able to upgrade their instances directly from the Admin portal without having to contact Microsoft Support.</span></span>  

> [!NOTE]
> <span data-ttu-id="621f4-110">PSA версия 3.x включва значителни промени.</span><span class="sxs-lookup"><span data-stu-id="621f4-110">PSA version 3.x includes significant changes.</span></span> <span data-ttu-id="621f4-111">Тя е изградена върху рамката на Унифицирания интерфейс, за да помогне за осигуряване на подобрено потребителско изживяване.</span><span class="sxs-lookup"><span data-stu-id="621f4-111">It has been built on the Unified Interface framework to help provide an improved user experience.</span></span> <span data-ttu-id="621f4-112">Преработеното приложение предоставя последователен, унифициран потребителски интерфейс (UI) и следва принципите на адаптивния дизайн за оптимален изглед върху всякакъв размер на екрана или устройство.</span><span class="sxs-lookup"><span data-stu-id="621f4-112">The redesigned app delivers a consistent, uniform user interface (UI), and it follows responsive design principles for optimal viewing on any screen size or device.</span></span> <span data-ttu-id="621f4-113">В приложението има и други промени.</span><span class="sxs-lookup"><span data-stu-id="621f4-113">There have been other changes throughout the application.</span></span> <span data-ttu-id="621f4-114">Някои от променените области включват ценообразуване, резервиране и присвояване на ресурси, време, разходи и одобрения.</span><span class="sxs-lookup"><span data-stu-id="621f4-114">Some of the areas that have been changed include pricing, booking and assigning resources, time, expenses, and approvals.</span></span>

<span data-ttu-id="621f4-115">Преди да започнете процеса на надстройване, ви препоръчваме да изпълните следните задачи:</span><span class="sxs-lookup"><span data-stu-id="621f4-115">Before you begin the upgrade process, we recommend that you complete the following tasks:</span></span>

- <span data-ttu-id="621f4-116">Проверете дали Dynamics 365 Field Service и Project Service Automation са инсталирани на идентифицирания екземпляра.</span><span class="sxs-lookup"><span data-stu-id="621f4-116">Verify whether both Dynamics 365 Field Service and Project Service Automation are installed on the identified instance.</span></span> <span data-ttu-id="621f4-117">Ако и двете решения са инсталирани, трябва да планирате да надстроите и двете, преди да подновите обичайната употреба на екземпляра.</span><span class="sxs-lookup"><span data-stu-id="621f4-117">If both solutions are installed, you should plan to upgrade both before you resume regular use of the instance.</span></span>
- <span data-ttu-id="621f4-118">Внимателно прегледайте следните теми.</span><span class="sxs-lookup"><span data-stu-id="621f4-118">Carefully review the following topics.</span></span> <span data-ttu-id="621f4-119">Познаването и разбирането на промените между версиите ще ви помогне при процеса на надстройване.</span><span class="sxs-lookup"><span data-stu-id="621f4-119">Awareness and understanding of the changes between versions will help you with the upgrade process.</span></span> <span data-ttu-id="621f4-120">Тези теми предоставят информация за основните промени в PSA заедно със съображения и препоръки за планиране на надстройката до версия 3.x.</span><span class="sxs-lookup"><span data-stu-id="621f4-120">These topics provide information about the major changes in PSA, together with considerations and recommendations for planning your upgrade to version 3.x.</span></span>

    - [<span data-ttu-id="621f4-121">Какво е новото или промененото в Project Service Automation версия 3</span><span class="sxs-lookup"><span data-stu-id="621f4-121">What's new or changed in Project Service Automation version 3</span></span>](whats-new-changed-v3.md)
    - [<span data-ttu-id="621f4-122">Съображения за надстройка – Project Service Automation версия 2.x или 1.x до версия 3</span><span class="sxs-lookup"><span data-stu-id="621f4-122">Upgrade considerations - Project Service Automation version 2.x or 1.x to version 3</span></span>](upgrade-v3.md)

- <span data-ttu-id="621f4-123">Надстройте екземпляра си в ограничителен режим, за да оцените промените във внедряването, преди да надстроите производствения си екземпляр.</span><span class="sxs-lookup"><span data-stu-id="621f4-123">Upgrade your sandbox instance to evaluate the changes in your implementation before you upgrade your production instance.</span></span>

<span data-ttu-id="621f4-124">След като сте прегледали темите, споменати по-горе, и сте готови да надстроите до PSA версия 3.x или версия, базирана на UCI, подайте заявка до поддръжката на Microsoft, за да направите надстройката налична от центъра за администриране.</span><span class="sxs-lookup"><span data-stu-id="621f4-124">After you've reviewed the topics that were mentioned earlier and are ready to upgrade to PSA version 3.x or the UCI-based version, submit a request to Microsoft support to make the upgrade available from Admin center.</span></span> <span data-ttu-id="621f4-125">В заявката си посочете подробностите за вашия екземпляр.</span><span class="sxs-lookup"><span data-stu-id="621f4-125">In your request, provide the details of your instance.</span></span>

## <a name="older-versions-of-psa-psa-version-2x-in-a-newly-created-instance"></a><span data-ttu-id="621f4-126">По-стари версии на PSA (PSA версия 2.x) в новосъздаден екземпляр</span><span class="sxs-lookup"><span data-stu-id="621f4-126">Older versions of PSA (PSA version 2.x) in a newly created instance</span></span>

<span data-ttu-id="621f4-127">От 17 май 2019 г. всички нови екземпляри ще имат UCI като клиент по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="621f4-127">As of May 17, 2019, all new instances will have UCI as the default client.</span></span> <span data-ttu-id="621f4-128">За съгласуване с тази промяна PSA версия 3.x и Field Service версия 8.x ще бъдат осигурявани по подразбиране, тъй като тези версии са проектирани да работят с UCI клиента.</span><span class="sxs-lookup"><span data-stu-id="621f4-128">For alignment with this change, PSA version 3.x and Field Service version 8.x will be provisioned by default, because these versions are designed to work with the UCI client.</span></span>

<span data-ttu-id="621f4-129">От 1 март 2020 г. клиентите на Dynamics PSA вече няма да могат да създават нова среда с по-стари версии на PSA, например PSA версия 2.x или по-ниска.</span><span class="sxs-lookup"><span data-stu-id="621f4-129">Starting March 1, 2020, customers of Dynamics PSA will no longer be able to create a new environment with older versions of PSA, for example PSA version 2.x or lower.</span></span> <span data-ttu-id="621f4-130">Всяка нова среда ще бъде да получите само версия 3.x на PSA.</span><span class="sxs-lookup"><span data-stu-id="621f4-130">Any new environment will be to get only version 3.x of PSA.</span></span>

> [!NOTE]
> <span data-ttu-id="621f4-131">За най-добро изживяване, когато използвате по-стари версии на приложенията Field Service и PSA, отидете на страницата **Системни настройки** и за полето **Използване само на новия Унифициран интерфейс (препоръчително)** изберете **Не**, тъй като тези версии не са проектирани да се зареждат правилно в UCI.</span><span class="sxs-lookup"><span data-stu-id="621f4-131">For the best experience when you use older versions of the Field Service and PSA applications, go to the **System settings** page and for the field, **Use the new Unified Interface only (recommended)** field, select **No** as these versions aren't designed to be correctly loaded in UCI.</span></span> <span data-ttu-id="621f4-132">След като изключите UCI, можете да отваряте и изпълнявате тези версии на Field Service и PSA, като използвате стария уеб клиент.</span><span class="sxs-lookup"><span data-stu-id="621f4-132">After you have turned off UCI, you can open and run these versions of Field Service and PSA by using the old web client.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]