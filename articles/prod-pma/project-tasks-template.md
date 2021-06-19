---
title: Синхронизирайте проектните задачи директно от Project Service Automation с Finance and Operations
description: Тази тема описва шаблона и основните задачи, които се използват за синхронизиране на прогнозни часове на задачи за проект директно от Microsoft Dynamics 365 Project Service Automation във Dynamics 365 Finance.
author: Yowelle
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 16cd38f2f190414d7be9c93e8ab90d55006f47e1
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6009963"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="8fc0e-103">Синхронизирайте проектните задачи директно от Project Service Automation с Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="8fc0e-103">Synchronize project tasks directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="8fc0e-104">Тази тема описва шаблона и основните задачи, които се използват за синхронизиране на прогнозни часове на задачи за проект директно от Dynamics 365 Project Service Automation във Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-104">This topic describes the template and underlying task that are used to synchronize project tasks directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="8fc0e-105">Интеграция на проектни задачи, категории транзакции, прогнози за часове, оценки на разходите и заключване на функционалността е налична във версия 8.0.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="8fc0e-106">Ако използвате Enterprise Edition 7.3.0, след като инсталирате KB 4132657 и KB 4132660, ще можете да използвате шаблоните за интегриране на проектни задачи, категории на транзакционни транзакции, часови прогнози, прогнозни разходи и актуални данни и да конфигурирате заключване на функционалността.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-106">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="8fc0e-107">Ако трябва да нулирате счетоводните разпределения, препоръчваме да инсталирате и KB 4131710.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-107">If you must reset the accounting distributions, we recommended that you also install KB 4131710.</span></span>
> - <span data-ttu-id="8fc0e-108">Интегрирането на действителни данни е достъпно от версия 8.0.1.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-108">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="8fc0e-109">Поток от данни за Project Service Automation към Finance</span><span class="sxs-lookup"><span data-stu-id="8fc0e-109">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="8fc0e-110">Решението за интеграция на Project Service Automation to Finance използва функцията за интегриране на данни, за да синхронизира данните между копията на Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-110">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="8fc0e-111">Шаблонът за интеграция, които се предлагат с функцията за интеграция на данни, позволяват потока от данни за задачи на проекта от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-111">The integration template that is available with the Data integration feature enables the flow of data about project tasks from Project Service Automation to Finance.</span></span>

<span data-ttu-id="8fc0e-112">Следващата илюстрация показва как данните се синхронизират между Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-112">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="8fc0e-113">[![Поток от данни за интеграция на Project Service Automation с Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span><span class="sxs-lookup"><span data-stu-id="8fc0e-113">[![Data flow for Project Service Automation integration with Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span></span>

## <a name="template-and-task"></a><span data-ttu-id="8fc0e-114">Шаблони и задача</span><span class="sxs-lookup"><span data-stu-id="8fc0e-114">Template and task</span></span>

<span data-ttu-id="8fc0e-115">За достъп до шаблона, в администраторски център на Microsoft Power Apps, изберете **Проекти** и след това в горния десен ъгъл изберете **Нов проект**, за да изберете публични шаблони.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-115">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="8fc0e-116">Следният шаблон и основна задача се използват за синхронизиране на задачи на проекта от Project Service Automation към Finance:</span><span class="sxs-lookup"><span data-stu-id="8fc0e-116">The following template and underlying task are used to synchronize project tasks from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="8fc0e-117">**Име на шаблона в Интегриране на данни:** Задачи на проект (PSA до Fin и Ops)</span><span class="sxs-lookup"><span data-stu-id="8fc0e-117">**Name of the template in Data integration:** Project tasks (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="8fc0e-118">**Име на задача в проекта:** Задачи на проекта</span><span class="sxs-lookup"><span data-stu-id="8fc0e-118">**Name of the task in the project:** Project tasks</span></span>

<span data-ttu-id="8fc0e-119">Преди да може да се случи синхронизиране на задачи на проект, трябва да синхронизирате договорите на проект и проектите.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-119">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="entity-set"></a><span data-ttu-id="8fc0e-120">Набор от обекти</span><span class="sxs-lookup"><span data-stu-id="8fc0e-120">Entity set</span></span>

| <span data-ttu-id="8fc0e-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="8fc0e-121">Project Service Automation</span></span> | <span data-ttu-id="8fc0e-122">Finance</span><span class="sxs-lookup"><span data-stu-id="8fc0e-122">Finance</span></span>                             |
|----------------------------|-------------------------------------|
| <span data-ttu-id="8fc0e-123">Задачи от проекти</span><span class="sxs-lookup"><span data-stu-id="8fc0e-123">Project Tasks</span></span>              | <span data-ttu-id="8fc0e-124">Интеграционен обект за задача на проект</span><span class="sxs-lookup"><span data-stu-id="8fc0e-124">Integration entity for project task</span></span> |

## <a name="entity-flow"></a><span data-ttu-id="8fc0e-125">Поток на обекта</span><span class="sxs-lookup"><span data-stu-id="8fc0e-125">Entity flow</span></span>

<span data-ttu-id="8fc0e-126">Задачите по проект за часовете на проекта се управляват в Project Service Automation и се синхронизират с Finance като дейности на проект.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-126">Project tasks are managed in Project Service Automation, and they are synchronized to Finance as project activities.</span></span>

## <a name="prerequisites-and-mapping-setup"></a><span data-ttu-id="8fc0e-127">Предпоставки и настройка на картографиране</span><span class="sxs-lookup"><span data-stu-id="8fc0e-127">Prerequisites and mapping setup</span></span>

<span data-ttu-id="8fc0e-128">Преди да може да се случи синхронизиране на задачи на проект, трябва да синхронизирате договорите на проект и проектите.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-128">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="power-query"></a><span data-ttu-id="8fc0e-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="8fc0e-129">Power Query</span></span>

<span data-ttu-id="8fc0e-130">Трябва да използвате Microsoft Power Query за Excel, за да филтрирате данни, ако това условие е изпълнено:</span><span class="sxs-lookup"><span data-stu-id="8fc0e-130">You must use Microsoft Power Query for Excel to filter data if this condition is met:</span></span>

- <span data-ttu-id="8fc0e-131">Имате специфични за ресурсите записи в проектна задача.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-131">You have resource-specific records in a project task.</span></span>

<span data-ttu-id="8fc0e-132">Ако трябва да използвате Power Query, следвайте това указание:</span><span class="sxs-lookup"><span data-stu-id="8fc0e-132">If you must use Power Query, follow this guideline:</span></span>

- <span data-ttu-id="8fc0e-133">Шаблонът за проектни задачи (PSA до Fin и Ops) има филтър по подразбиране, който изключва специфични за ресурсите записи от проектна задача, като зададе филтъра на **IsLineTask** на **Невярно**.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-133">The Project tasks (PSA to Fin and Ops) template has a default filter that excludes resource-specific records from a project task by setting the filter on **IsLineTask** to **False**.</span></span> <span data-ttu-id="8fc0e-134">Ако създадете свой собствен шаблон, трябва да добавите този филтър.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-134">If you create your own template, you must add this filter.</span></span>

## <a name="template-mapping-in-data-integration"></a><span data-ttu-id="8fc0e-135">Съпоставяне на шаблони при интеграция на данни</span><span class="sxs-lookup"><span data-stu-id="8fc0e-135">Template mapping in Data integration</span></span>

<span data-ttu-id="8fc0e-136">Следващата илюстрация показва пример за съпоставяния на задача на шаблон при интеграция на данни.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-136">The following illustration shows an example of the template task mappings in Data integration.</span></span> <span data-ttu-id="8fc0e-137">Картографирането показва информация за полето, която ще бъде синхронизирана от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="8fc0e-137">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="8fc0e-138">[![Съпоставяне на шаблони](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span><span class="sxs-lookup"><span data-stu-id="8fc0e-138">[![Template mapping](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]