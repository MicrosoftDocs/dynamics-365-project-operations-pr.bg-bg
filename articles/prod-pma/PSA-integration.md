---
title: Общ преглед на Project Service Automation
description: Тази тема предоставя информация за решението за интеграция на Dynamics 365 Project Service Automation в Dynamics 365 Finance.
author: ruhercul
manager: AnnBe
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: ruhercul
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 1e1a963bccefd1552aab6e42d3b2d1dc63a82e8f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071961"
---
# <a name="project-service-automation-overview"></a><span data-ttu-id="faa2d-103">Общ преглед на Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="faa2d-103">Project Service Automation overview</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="faa2d-104">Решението за интеграция на Project Service Automation в Finance използва функцията за интегриране на данни, за да синхронизира данните между екземплярите на Dynamics 365 Finance и Dynamics 365 Project Service Automation чрез Common Data Service.</span><span class="sxs-lookup"><span data-stu-id="faa2d-104">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Dynamics 365 Finance and Dynamics 365 Project Service Automation via Common Data Service.</span></span> <span data-ttu-id="faa2d-105">Шаблони за интеграция, които се предлагат с функцията за интеграция на данни, позволяват потока от проекти, договори на проект и аспекти на договор по проект, контролни точки на проект, задачи по проект, категории на трансакция на разходи, прогнози за часове, и прогнози за разходи прогнозни разходи за проекти от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="faa2d-105">The integration templates that are available with the Data integration feature enable the flow of projects, project contracts, project contract lines, project contract line milestones, project tasks, expense transaction categories, hour estimates, and expense estimates from Project Service Automation to Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="faa2d-106">Ако използвате версия 7.3.0, трябва да инсталирате KB 4074835.</span><span class="sxs-lookup"><span data-stu-id="faa2d-106">If you're using version 7.3.0, you must install KB 4074835.</span></span> <span data-ttu-id="faa2d-107">След това ще можете да интегрирате проекти с фиксирана цена.</span><span class="sxs-lookup"><span data-stu-id="faa2d-107">You will then be able to integrate fixed price projects.</span></span>
> - <span data-ttu-id="faa2d-108">Ако използвате версия 7.3.0 и пренасяте транзакции с такси от Project Service Automation, трябва да инсталирате KB 4345320, за да включите тези такси във фактурата на проекта.</span><span class="sxs-lookup"><span data-stu-id="faa2d-108">If you're using version 7.3.0, and you are bringing fee transactions over from Project Service Automation, you must install KB 4345320 in order to include those fees in the project invoice.</span></span>
> - <span data-ttu-id="faa2d-109">Ако използвате версия 8.0, ще можете да използвате интеграция на проектни задачи, категории транзакции, прогнози за часове, оценки на разходите и заключване на функционалността.</span><span class="sxs-lookup"><span data-stu-id="faa2d-109">If you're using version 8.0, you will be able to use project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking.</span></span>
> - <span data-ttu-id="faa2d-110">Ако използвате версия 8.0.1 или по-нова, ще можете да синхронизирате актуални данни.</span><span class="sxs-lookup"><span data-stu-id="faa2d-110">If you're using version 8.0.1 or later, you will be able to synchronize actuals.</span></span>

<span data-ttu-id="faa2d-111">Преди да можете да интегрирате Project Service Automation Finance, трябва да конфигурирате параметрите за интеграция на Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="faa2d-111">Before you can integrate Project Service Automation Finance, you must configure the Project Service Automation integration parameters.</span></span> <span data-ttu-id="faa2d-112">За повече информация вижте [Параметри на интеграция на Project Service Automation](PSA-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="faa2d-112">For more information, see [Project Service Automation integration parameters](PSA-parameters.md).</span></span>

<span data-ttu-id="faa2d-113">Това решение за интеграция позволява директна синхронизация в следните сценарии:</span><span class="sxs-lookup"><span data-stu-id="faa2d-113">This integration solution enables direct synchronization in the following scenarios:</span></span>

- <span data-ttu-id="faa2d-114">Поддържайте договорите за проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="faa2d-114">Maintain project contracts in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="faa2d-115">Създаване на проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="faa2d-115">Create projects in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="faa2d-116">Поддържайте аспекти на договор за проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="faa2d-116">Maintain project contract lines in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="faa2d-117">Поддържайте контролни точки на аспекти на договор за проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="faa2d-117">Maintain project contract line milestones in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="faa2d-118">Поддържайте задачи на проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="faa2d-118">Maintain project tasks in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="faa2d-119">Поддържайте категории на трансакции на разход във Finance и ги синхронизирайте директно от Finance в Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="faa2d-119">Maintain expense transaction categories in Finance, and synchronize them directly from Finance to Project Service Automation.</span></span>
- <span data-ttu-id="faa2d-120">Създавайте прогнозни часове в проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="faa2d-120">Create project hour estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="faa2d-121">Създавайте прогнозни разходи на проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="faa2d-121">Create project expense estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="faa2d-122">Създайте действителни данни за времето, разходите и таксите на проект в Project Service Automation и създайте транзакции на проекти в дневника за интеграция на Project Service Automation, така че те да могат да бъдат публикувани във Finance.</span><span class="sxs-lookup"><span data-stu-id="faa2d-122">Create project time, expense, and fee actuals in Project Service Automation, and create project transactions in the Project Service Automation integration journal so that they can be posted in Finance.</span></span>

## <a name="data-synchronization"></a><span data-ttu-id="faa2d-123">Синхронизиране на данни</span><span class="sxs-lookup"><span data-stu-id="faa2d-123">Data synchronization</span></span>

<span data-ttu-id="faa2d-124">Следващата илюстрация показва как данните се синхронизират като част от интеграцията между Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="faa2d-124">The following illustration shows how data is synchronized as part of the integration between Project Service Automation and Finance.</span></span>

> [!NOTE]
> <span data-ttu-id="faa2d-125">Понастоящем не са налични всички шаблони.</span><span class="sxs-lookup"><span data-stu-id="faa2d-125">Not all templates are currently available.</span></span> <span data-ttu-id="faa2d-126">Шаблоните ще бъдат пуснати, когато бъдат завършени.</span><span class="sxs-lookup"><span data-stu-id="faa2d-126">Templates will be released as they are completed.</span></span>

<span data-ttu-id="faa2d-127">[![Интеграция на Project Service Automation с Finance](./media/PSA-integration.png)](./media/PSA-integration.png)</span><span class="sxs-lookup"><span data-stu-id="faa2d-127">[![Project Service Automation integration with Finance](./media/PSA-integration.png)](./media/PSA-integration.png)</span></span>

## <a name="system-requirements-for-finance"></a><span data-ttu-id="faa2d-128">Системни изисквания за финанси</span><span class="sxs-lookup"><span data-stu-id="faa2d-128">System requirements for Finance</span></span>

<span data-ttu-id="faa2d-129">За да използвате решението за интегриране на Project Service Automation за финансиране, трябва да инсталирате Enterprise Edition 7.3 с актуализация на платформа 12 или по-нова.</span><span class="sxs-lookup"><span data-stu-id="faa2d-129">To use the Project Service Automation to Finance integration solution, you must install Enterprise edition 7.3 with Platform update 12 or later.</span></span>

## <a name="system-requirements-for-project-service-automation"></a><span data-ttu-id="faa2d-130">Системни изисквания за Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="faa2d-130">System requirements for Project Service Automation</span></span>

<span data-ttu-id="faa2d-131">За да използвате решението за интегриране на Project Service Automation за финансиране, трябва да инсталирате следните компоненти:</span><span class="sxs-lookup"><span data-stu-id="faa2d-131">To use the Project Service Automation to Finance integration solution, you must install the following components:</span></span>

- <span data-ttu-id="faa2d-132">Dynamics 365 Project Service Automation версия 9.0.0.0 или по-нова</span><span class="sxs-lookup"><span data-stu-id="faa2d-132">Dynamics 365 Project Service Automation version 9.0.0.0 or later</span></span>
- <span data-ttu-id="faa2d-133">Решение за перспектива за пари за Dynamics 365 Sales, версия 1.14.0.0 (v14) или по-нова версия</span><span class="sxs-lookup"><span data-stu-id="faa2d-133">Prospect to cash solution for Dynamics 365 Sales, version 1.14.0.0 (v14) or later</span></span>
- <span data-ttu-id="faa2d-134">Решение за Project Service Automation към Finance за Dynamics 365 Project Service Automation версия 1.0.0.0 или по-нова</span><span class="sxs-lookup"><span data-stu-id="faa2d-134">Project Service Automation to Finance solution for Dynamics 365 Project Service Automation version 1.0.0.0 or later</span></span>

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a><span data-ttu-id="faa2d-135">Инсталирайте решението за интеграция на Project Service Automation във Finance във вашия екземпляр на Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="faa2d-135">Install the Project Service Automation to Finance integration solution in your Project Service Automation instance</span></span>

<span data-ttu-id="faa2d-136">Изтеглете решението за интеграция на Project Service Automation във Finance от [Център за изтегляне на Microsoft](https://www.microsoft.com/download/details.aspx?id=57016) и следвайте инструкциите, приложени към решението.</span><span class="sxs-lookup"><span data-stu-id="faa2d-136">Download the Project Service Automation to Finance integration solution from [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=57016), and follow the instructions that are included with the solution.</span></span>
