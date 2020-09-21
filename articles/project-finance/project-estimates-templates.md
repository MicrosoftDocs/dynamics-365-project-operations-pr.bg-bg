---
title: Синхронизирайте проектните оценки директно от Project Service Automation с Finance and Operations
description: Тази тема описва шаблоните и основните задачи, които се използват за синхронизиране на прогнозни часове на проекта и прогнозни разходи за проекти директно от Microsoft Dynamics 365 Project Service Automation да се Dynamics 365 Finance.
author: KimANelson
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: d688ce9a-41e3-4ebe-952e-700f8351fbe9
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: a24a967d82c2e005e61234d34da8a583b61ff7b1
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749273"
---
# <a name="synchronize-project-estimates-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="e6786-103">Синхронизирайте проектните оценки директно от Project Service Automation с Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="e6786-103">Synchronize project estimates directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="e6786-104">Тази тема описва шаблоните и основните задачи, които се използват за синхронизиране на прогнозни часове на проекта и прогнозни разходи за проекти директно от Dynamics 365 Project Service Automation да се Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="e6786-104">This topic describes the templates and underlying tasks that are used to synchronize project hour estimates and project expense estimates directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="e6786-105">Интеграция на проектни задачи, категории транзакции, прогнози за часове, оценки на разходите и заключване на функционалността е налична във версия 8.0.</span><span class="sxs-lookup"><span data-stu-id="e6786-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking is available in version 8.0.</span></span>
> - <span data-ttu-id="e6786-106">Интегрирането на действителни данни е достъпно от версия 8.0.1.</span><span class="sxs-lookup"><span data-stu-id="e6786-106">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="e6786-107">Поток от данни за Project Service Automation към Finance</span><span class="sxs-lookup"><span data-stu-id="e6786-107">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="e6786-108">Решението за интеграция на Project Service Automation to Finance използва функцията за интегриране на данни, за да синхронизира данните между копията на Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="e6786-108">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="e6786-109">Шаблоните за интеграция, които се предлагат с функцията за интеграция на данни, позволяват потока от данни за прогнозни часови прогнози на проекта и прогнозни разходи за проекти от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="e6786-109">The integration templates that are available with the Data integration feature enable the flow of data about project hour estimates and project expense estimates from Project Service Automation to Finance.</span></span>

<span data-ttu-id="e6786-110">Следващата илюстрация показва как данните се синхронизират между Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="e6786-110">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="e6786-111">[![Поток от данни за интеграция на Project Service Automation с Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="e6786-111">[![Data flow for Project Service Automation integration with Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span></span>

## <a name="project-hour-estimates"></a><span data-ttu-id="e6786-112">Прогнозни оценки на часове</span><span class="sxs-lookup"><span data-stu-id="e6786-112">Project hour estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="e6786-113">Шаблони и задачи</span><span class="sxs-lookup"><span data-stu-id="e6786-113">Template and tasks</span></span>

<span data-ttu-id="e6786-114">За достъп до наличните шаблони, в администраторски център на Microsoft Power Apps, изберете **Проекти** и след това в горния десен ъгъл изберете **Нов проект**, за да изберете публични шаблони.</span><span class="sxs-lookup"><span data-stu-id="e6786-114">To access the available templates, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="e6786-115">Следният шаблон и основните задачи се използват за синхронизиране на прогнозите за часовете на проекта от Project Service Automation към Finance:</span><span class="sxs-lookup"><span data-stu-id="e6786-115">The following template and underlying tasks are used to synchronize project hour estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="e6786-116">**Име на шаблона в Интегриране на данни:** Приблизителни прогнозни часове (PSA до Fin и Ops)</span><span class="sxs-lookup"><span data-stu-id="e6786-116">**Name of the template in Data integration:** Project hour estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="e6786-117">**Име на задачите в проекта:**</span><span class="sxs-lookup"><span data-stu-id="e6786-117">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="e6786-118">Релации на трансакция</span><span class="sxs-lookup"><span data-stu-id="e6786-118">Transaction relationships</span></span>
    - <span data-ttu-id="e6786-119">Прогнози за разноски</span><span class="sxs-lookup"><span data-stu-id="e6786-119">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="e6786-120">Набор от обекти</span><span class="sxs-lookup"><span data-stu-id="e6786-120">Entity set</span></span>

| <span data-ttu-id="e6786-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="e6786-121">Project Service Automation</span></span> | <span data-ttu-id="e6786-122">Finance</span><span class="sxs-lookup"><span data-stu-id="e6786-122">Finance</span></span>                                       |
|----------------------------|-----------------------------------------------|
| <span data-ttu-id="e6786-123">Задачи от проекти</span><span class="sxs-lookup"><span data-stu-id="e6786-123">Project tasks</span></span>              | <span data-ttu-id="e6786-124">Интеграционен обект за прогнозни часови оценки на проекта</span><span class="sxs-lookup"><span data-stu-id="e6786-124">Integration entity for project hour estimates</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="e6786-125">Поток на обекта</span><span class="sxs-lookup"><span data-stu-id="e6786-125">Entity flow</span></span>

<span data-ttu-id="e6786-126">Прогнозите за часовете на проекта се управляват в Project Service Automation и се синхронизират с Finance като прогнози за часовете на проекта.</span><span class="sxs-lookup"><span data-stu-id="e6786-126">Project hour estimates are managed in Project Service Automation, and they are synchronized to Finance as project hour forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="e6786-127">Предварителни изисквания</span><span class="sxs-lookup"><span data-stu-id="e6786-127">Prerequisites</span></span>

<span data-ttu-id="e6786-128">Преди да може да се извърши синхронизиране на прогнозни часови оценки на проекта, трябва да синхронизирате проекти, проектни задачи и категории транзакции на проектни разходи.</span><span class="sxs-lookup"><span data-stu-id="e6786-128">Before synchronization of project hour estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="e6786-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="e6786-129">Power Query</span></span>

<span data-ttu-id="e6786-130">В шаблона за прогнозни часове на проекта трябва да използвате Microsoft Power Query за Excel, за да изпълните тези задачи:</span><span class="sxs-lookup"><span data-stu-id="e6786-130">In the project hour estimates template, you must use Microsoft Power Query for Excel to complete these tasks:</span></span>

- <span data-ttu-id="e6786-131">Задайте идентификатора на модела за прогноза по подразбиране, който ще се използва, когато интеграцията създава нови часови прогнози.</span><span class="sxs-lookup"><span data-stu-id="e6786-131">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="e6786-132">Филтрирайте всички специфични за ресурса записи в задачата, които ще пропуснат интеграцията в прогнози за час.</span><span class="sxs-lookup"><span data-stu-id="e6786-132">Filter out any resource-specific records in the task that will fail the integration into hour forecasts.</span></span>
- <span data-ttu-id="e6786-133">Филтрирайте всички празни редове от категории транзакции.</span><span class="sxs-lookup"><span data-stu-id="e6786-133">Filter out any empty transaction category rows.</span></span> <span data-ttu-id="e6786-134">Неизпълнението на тази задача може да доведе до неправилни прогнози за часа.</span><span class="sxs-lookup"><span data-stu-id="e6786-134">Failure to complete this task might result in incorrect hour forecasts.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="e6786-135">Задайте стандартния идентификатор на модела за прогноза</span><span class="sxs-lookup"><span data-stu-id="e6786-135">Set the default forecast model ID</span></span>

<span data-ttu-id="e6786-136">За да актуализирате идентификатора на модела по подразбиране в шаблона, щракнете върху стрелката **Карта**, за да отворите картографирането.</span><span class="sxs-lookup"><span data-stu-id="e6786-136">To update the default forecast model ID in the template, click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="e6786-137">След това изберете връзката **Разширени заявки и филтриране**.</span><span class="sxs-lookup"><span data-stu-id="e6786-137">Then select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="e6786-138">Ако използвате шаблона за прогнозни часове на проекта (PSA до Fin и Ops) по подразбиране, изберете **Вмъкнато състояние** в списъка на **Приложени стъпки**.</span><span class="sxs-lookup"><span data-stu-id="e6786-138">If you're using the default Project hour estimates (PSA to Fin and Ops) template, select the **Inserted Condition** in the list of **Applied Steps**.</span></span> <span data-ttu-id="e6786-139">Във **Функцията** влизане, замяна **О\_прогноза** с името на идентификатора на прогнозния модел, който трябва да се използва с интеграцията.</span><span class="sxs-lookup"><span data-stu-id="e6786-139">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="e6786-140">Шаблонът по подразбиране има идентификационен номер на прогнозен модел от демонстрационните данни.</span><span class="sxs-lookup"><span data-stu-id="e6786-140">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="e6786-141">Ако създавате нов шаблон, трябва да добавите тази колона.</span><span class="sxs-lookup"><span data-stu-id="e6786-141">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="e6786-142">В Power Query изберете **Добавете условна колона** и въведете име за новата колона, като например **ModelID**.</span><span class="sxs-lookup"><span data-stu-id="e6786-142">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="e6786-143">Въведете условието за колоната, където, ако задачата на проекта не е нула, тогава \<въведете идентификатора на модела за прогноза\>; иначе е нула.</span><span class="sxs-lookup"><span data-stu-id="e6786-143">Enter the condition for the column, where, if Project task is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="filter-out-resource-specific-records"></a><span data-ttu-id="e6786-144">Филтрирайте специфичните за ресурсите записи</span><span class="sxs-lookup"><span data-stu-id="e6786-144">Filter out resource-specific records</span></span>

<span data-ttu-id="e6786-145">Шаблонът за прогнозни часове на проекта (PSA до Fin и Ops) има филтър по подразбиране, който премахва всички специфични за ресурса записи.</span><span class="sxs-lookup"><span data-stu-id="e6786-145">The Project hour estimates (PSA to Fin and Ops) template has a default filter that removes any resource-specific records.</span></span> <span data-ttu-id="e6786-146">Ако създадете свой собствен шаблон, трябва да добавите този филтър.</span><span class="sxs-lookup"><span data-stu-id="e6786-146">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="e6786-147">Изберете **Разширени заявки и филтриране** връзка за филтриране на **msdyn\_islinetask** колона, така че само записите **Невярно** са включени.</span><span class="sxs-lookup"><span data-stu-id="e6786-147">Select the **Advanced Query and Filtering** link to filter on the **msdyn\_islinetask** column so that only **False** records are included.</span></span>

#### <a name="filter-out-empty-transaction-category-rows"></a><span data-ttu-id="e6786-148">Филтрирайте празни редове от категории транзакции</span><span class="sxs-lookup"><span data-stu-id="e6786-148">Filter out empty transaction category rows</span></span>

<span data-ttu-id="e6786-149">Трябва да добавите филтър, за да премахнете всички редове, които имат празни категории транзакции.</span><span class="sxs-lookup"><span data-stu-id="e6786-149">You must add a filter to remove any rows that have empty transaction categories.</span></span> <span data-ttu-id="e6786-150">Тази задача е задължителна, независимо дали използвате шаблона по подразбиране или създавате свой собствен шаблон.</span><span class="sxs-lookup"><span data-stu-id="e6786-150">This task is required, regardless of whether you're using the default template or creating your own template.</span></span> <span data-ttu-id="e6786-151">Този филтър премахва всички обобщени редове от Project Service Automation, които могат да доведат до неправилни прогнози за часа във Finance.</span><span class="sxs-lookup"><span data-stu-id="e6786-151">This filter removes any summary rows from Project Service Automation that might cause the hour forecasts in Finance to be incorrect.</span></span> <span data-ttu-id="e6786-152">Изберете връзката **Разширени заявки и филтриране** за филтриране на нулеви записи в **msdyn\_категория на транзакциите\_стойност** колона.</span><span class="sxs-lookup"><span data-stu-id="e6786-152">Select **Advanced Query and Filtering** link to filter out null records in the **msdyn\_transactioncategory\_value** column.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="e6786-153">Съпоставяне на шаблони при интеграция на данни</span><span class="sxs-lookup"><span data-stu-id="e6786-153">Template mapping in Data integration</span></span>

<span data-ttu-id="e6786-154">Следващата илюстрация показва пример за съпоставяне на задача на шаблон при интеграция на данни.</span><span class="sxs-lookup"><span data-stu-id="e6786-154">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="e6786-155">Картографирането показва информация за полето, която ще бъде синхронизирана от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="e6786-155">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="e6786-156">[![Съпоставяне на шаблони](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="e6786-156">[![Template mapping](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span></span>

## <a name="project-expense-estimates"></a><span data-ttu-id="e6786-157">Прогнози за разход по проект</span><span class="sxs-lookup"><span data-stu-id="e6786-157">Project expense estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="e6786-158">Шаблони и задачи</span><span class="sxs-lookup"><span data-stu-id="e6786-158">Template and tasks</span></span>

<span data-ttu-id="e6786-159">Следният шаблон и основните задачи се използват за синхронизиране на прогнозите за разходи на проекта от Project Service Automation към Finance:</span><span class="sxs-lookup"><span data-stu-id="e6786-159">The following template and underlying tasks are used to synchronize project expense estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="e6786-160">**Име на шаблона в Интегриране на данни:** Приблизителни прогнозни разходи (PSA до Fin и Ops)</span><span class="sxs-lookup"><span data-stu-id="e6786-160">**Name of the template in Data integration:** Project expense estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="e6786-161">**Име на задачите в проекта:**</span><span class="sxs-lookup"><span data-stu-id="e6786-161">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="e6786-162">Релации на трансакция</span><span class="sxs-lookup"><span data-stu-id="e6786-162">Transaction relationships</span></span> 
    - <span data-ttu-id="e6786-163">Прогнози за разноски</span><span class="sxs-lookup"><span data-stu-id="e6786-163">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="e6786-164">Набор от обекти</span><span class="sxs-lookup"><span data-stu-id="e6786-164">Entity set</span></span>

| <span data-ttu-id="e6786-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="e6786-165">Project Service Automation</span></span> | <span data-ttu-id="e6786-166">Finance</span><span class="sxs-lookup"><span data-stu-id="e6786-166">Finance</span></span>                                                  |
|----------------------------|----------------------------------------------------------|
| <span data-ttu-id="e6786-167">Връзки на транзакции</span><span class="sxs-lookup"><span data-stu-id="e6786-167">Transaction Connections</span></span>    | <span data-ttu-id="e6786-168">Интеграционен обект за взаимоотношения на проектни транзакции</span><span class="sxs-lookup"><span data-stu-id="e6786-168">Integration entity for project transaction relationships</span></span> |
| <span data-ttu-id="e6786-169">Редове за оценки</span><span class="sxs-lookup"><span data-stu-id="e6786-169">Estimate Lines</span></span>             | <span data-ttu-id="e6786-170">Интеграционен обект за прогнозни разходи на проекта</span><span class="sxs-lookup"><span data-stu-id="e6786-170">Integration entity for project expense estimates</span></span>         |

### <a name="entity-flow"></a><span data-ttu-id="e6786-171">Поток на обекта</span><span class="sxs-lookup"><span data-stu-id="e6786-171">Entity flow</span></span>

<span data-ttu-id="e6786-172">Прогнозите за разходи на проекта се управляват в Project Service Automation и се синхронизират с Finance като прогнози за разходи на проекта.</span><span class="sxs-lookup"><span data-stu-id="e6786-172">Project expense estimates are managed in Project Service Automation, and they are synchronized to Finance as project expense forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="e6786-173">Предварителни изисквания</span><span class="sxs-lookup"><span data-stu-id="e6786-173">Prerequisites</span></span>

<span data-ttu-id="e6786-174">Преди да може да се извърши синхронизиране на прогнозни разходи проекта, трябва да синхронизирате проекти, проектни задачи и категории транзакции на проектни разходи.</span><span class="sxs-lookup"><span data-stu-id="e6786-174">Before synchronization of project expense estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="e6786-175">Power Query</span><span class="sxs-lookup"><span data-stu-id="e6786-175">Power Query</span></span>

<span data-ttu-id="e6786-176">В шаблона за прогнозни разходи на проекта трябва да използвате Power Query за Excel, за да изпълните следните задачи:</span><span class="sxs-lookup"><span data-stu-id="e6786-176">In the project expense estimates template, you must use Power Query to complete the following tasks:</span></span>

- <span data-ttu-id="e6786-177">Филтрирайте, за да включите само редовите записи за оценка на разходите.</span><span class="sxs-lookup"><span data-stu-id="e6786-177">Filter to include only expense estimate line records.</span></span>
- <span data-ttu-id="e6786-178">Задайте идентификатора на модела за прогноза по подразбиране, който ще се използва, когато интеграцията създава нови часови прогнози.</span><span class="sxs-lookup"><span data-stu-id="e6786-178">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="e6786-179">Трансформирайте видовете фактуриране.</span><span class="sxs-lookup"><span data-stu-id="e6786-179">Transform the billing types.</span></span>
- <span data-ttu-id="e6786-180">Трансформирайте видовете трансакция.</span><span class="sxs-lookup"><span data-stu-id="e6786-180">Transform the transaction types.</span></span>

#### <a name="filter-to-include-only-expense-estimate-lines"></a><span data-ttu-id="e6786-181">Филтрирайте, за да включите само редовите прогнози за разходи</span><span class="sxs-lookup"><span data-stu-id="e6786-181">Filter to include only expense estimate lines</span></span>

<span data-ttu-id="e6786-182">Шаблонът за прогнозни разходи за проекта (PSA към Fin и Ops) има филтър по подразбиране, който включва само разходни редове в интеграцията.</span><span class="sxs-lookup"><span data-stu-id="e6786-182">The Project expense estimates (PSA to Fin and Ops) template has a default filter that includes only expense lines in the integration.</span></span> <span data-ttu-id="e6786-183">Ако създадете свой собствен шаблон, трябва да добавите този филтър.</span><span class="sxs-lookup"><span data-stu-id="e6786-183">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="e6786-184">Изберете **Транзакционни отношения** и след това щракнете върху стрелката **Карта**, за да отворите картографирането.</span><span class="sxs-lookup"><span data-stu-id="e6786-184">Select the **Transaction relationships** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="e6786-185">Изберете връзката **Разширени заявки и филтриране**.</span><span class="sxs-lookup"><span data-stu-id="e6786-185">Select the **Advanced Query and Filtering** link.</span></span> <span data-ttu-id="e6786-186">Филтрирайте колона **msdyn\_transactiontype1**, така че да включва само **msdyn\_estimateline**.</span><span class="sxs-lookup"><span data-stu-id="e6786-186">Filter the **msdyn\_transactiontype1** column so that it includes only **msdyn\_estimateline**.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="e6786-187">Задайте стандартния идентификатор на модела за прогноза</span><span class="sxs-lookup"><span data-stu-id="e6786-187">Set the default forecast model ID</span></span>

<span data-ttu-id="e6786-188">За да актуализирате идентификатора на модела по подразбиране в шаблона, изберете задача **Прогнози за разходи** и след това щракнете върху стрелката **Карта**, за да отворите картографирането.</span><span class="sxs-lookup"><span data-stu-id="e6786-188">To update the default forecast model ID in the template, select the **Expense estimates** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="e6786-189">Изберете връзката **Разширени заявки и филтриране**.</span><span class="sxs-lookup"><span data-stu-id="e6786-189">Select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="e6786-190">Ако използвате шаблона за прогнозни разходи на проекта (PSA до Fin и Ops) по подразбиране, в Power Query изберете първо формуляра **Вмъкнато състояние** в секцията **Приложени стъпки**.</span><span class="sxs-lookup"><span data-stu-id="e6786-190">If you're using the default Project expense estimates (PSA to Fin and Ops) template, in Power Query, select the first **Inserted Condition** from the **Applied Steps** section.</span></span> <span data-ttu-id="e6786-191">Във **Функцията** влизане, замяна **О\_прогноза** с името на идентификатора на прогнозния модел, който трябва да се използва с интеграцията.</span><span class="sxs-lookup"><span data-stu-id="e6786-191">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="e6786-192">Шаблонът по подразбиране има идентификационен номер на прогнозен модел от демонстрационните данни.</span><span class="sxs-lookup"><span data-stu-id="e6786-192">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="e6786-193">Ако създавате нов шаблон, трябва да добавите тази колона.</span><span class="sxs-lookup"><span data-stu-id="e6786-193">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="e6786-194">В Power Query изберете **Добавете условна колона** и въведете име за новата колона, като например **ModelID**.</span><span class="sxs-lookup"><span data-stu-id="e6786-194">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="e6786-195">Въведете условието за колоната, където, ако ИД на ред на прогноза не е нула, тогава \<въведете идентификатора на модела за прогноза\>; иначе е нула.</span><span class="sxs-lookup"><span data-stu-id="e6786-195">Enter the condition for the column, where, if Estimate line ID is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="transform-the-billing-types"></a><span data-ttu-id="e6786-196">Трансформирайте видовете фактуриране</span><span class="sxs-lookup"><span data-stu-id="e6786-196">Transform the billing types</span></span>

<span data-ttu-id="e6786-197">Шаблонът за прогнозни разходи за проект (PSA към Fin и Ops) включва условна колона, която се използва за трансформиране на типовете фактури, получени от Project Service Automation по време на интеграцията.</span><span class="sxs-lookup"><span data-stu-id="e6786-197">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the billing types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="e6786-198">Ако създадете свой собствен шаблон, трябва да добавите тази условна колона.</span><span class="sxs-lookup"><span data-stu-id="e6786-198">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="e6786-199">Изберете **Разширени заявки и филтриране** връзка и след това изберете **Добавете условна колона**.</span><span class="sxs-lookup"><span data-stu-id="e6786-199">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="e6786-200">Въведете име за новата колона, като например **BillingType**.</span><span class="sxs-lookup"><span data-stu-id="e6786-200">Enter a name for the new column, such as **BillingType**.</span></span> <span data-ttu-id="e6786-201">След това въведете следното условие:</span><span class="sxs-lookup"><span data-stu-id="e6786-201">Then enter the following condition:</span></span>

<span data-ttu-id="e6786-202">Ако **msdyn\_тип фактуриране** = 192350000, тогава **NonChargeable**</span><span class="sxs-lookup"><span data-stu-id="e6786-202">If **msdyn\_billingtype** = 192350000, then **NonChargeable**</span></span>  
<span data-ttu-id="e6786-203">иначе ако **msdyn\_тип фактуриране** = 192350001, тогава **Chargeable**</span><span class="sxs-lookup"><span data-stu-id="e6786-203">else if **msdyn\_billingtype** = 192350001, then **Chargeable**</span></span>  
<span data-ttu-id="e6786-204">иначе ако **msdyn\_тип фактуриране** = 192350002, тогава **Complimentary**</span><span class="sxs-lookup"><span data-stu-id="e6786-204">else if **msdyn\_billingtype** = 192350002, then **Complimentary**</span></span>  
<span data-ttu-id="e6786-205">друго **NotAvailable**</span><span class="sxs-lookup"><span data-stu-id="e6786-205">else **NotAvailable**</span></span>

#### <a name="transform-the-transaction-types"></a><span data-ttu-id="e6786-206">Трансформирайте видовете трансакция</span><span class="sxs-lookup"><span data-stu-id="e6786-206">Transform the transaction types</span></span>

<span data-ttu-id="e6786-207">Шаблонът за прогнозни разходи за проект (PSA към Fin и Ops) включва условна колона, която се използва за трансформиране на типовете трансакции, получени от Project Service Automation по време на интеграцията.</span><span class="sxs-lookup"><span data-stu-id="e6786-207">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the transaction types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="e6786-208">Ако създадете свой собствен шаблон, трябва да добавите тази условна колона.</span><span class="sxs-lookup"><span data-stu-id="e6786-208">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="e6786-209">Изберете **Разширени заявки и филтриране** връзка и след това изберете **Добавете условна колона**.</span><span class="sxs-lookup"><span data-stu-id="e6786-209">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="e6786-210">Въведете име за новата колона, като например **TransactionType**.</span><span class="sxs-lookup"><span data-stu-id="e6786-210">Enter a name for the new column, such as **TransactionType**.</span></span> <span data-ttu-id="e6786-211">След това въведете следното условие:</span><span class="sxs-lookup"><span data-stu-id="e6786-211">Then enter the following condition:</span></span>

<span data-ttu-id="e6786-212">Ако **msdyn\_код на транзакцията** = 192350000, тогава **Разходи**</span><span class="sxs-lookup"><span data-stu-id="e6786-212">If **msdyn\_transactiontypecode** = 192350000, then **Cost**</span></span>  
<span data-ttu-id="e6786-213">иначе ако **msdyn\_код на транзакцията** = 192350005, тогава **Продажби**</span><span class="sxs-lookup"><span data-stu-id="e6786-213">else if **msdyn\_transactiontypecode** = 192350005, then **Sales**</span></span>  
<span data-ttu-id="e6786-214">иначе **нула**</span><span class="sxs-lookup"><span data-stu-id="e6786-214">else **null**</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="e6786-215">Съпоставяне на шаблони при интеграция на данни</span><span class="sxs-lookup"><span data-stu-id="e6786-215">Template mapping in Data integration</span></span>

<span data-ttu-id="e6786-216">Следните илюстрации показват примери на нанасяне на задача за съпоставяне в интеграция на данни.</span><span class="sxs-lookup"><span data-stu-id="e6786-216">The following illustrations show examples of the template task mappings in Data integration.</span></span> <span data-ttu-id="e6786-217">Картографирането показва информация за полето, която ще бъде синхронизирана от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="e6786-217">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="e6786-218">[![Съпоставяне на шаблони](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="e6786-218">[![Template mapping](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span></span>

<span data-ttu-id="e6786-219">[![Съпоставяне на шаблони](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="e6786-219">[![Template mapping](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span></span>
