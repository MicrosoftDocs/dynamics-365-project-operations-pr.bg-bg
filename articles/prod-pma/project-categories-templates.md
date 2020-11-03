---
title: Синхронизирайте категориите разходи за проекти между Finance and Operations и Project Service Automation
description: Тази тема описва шаблон и основните задачи, които се използват за синхронизиране на категории на разход по проект между Microsoft Dynamics 365 Finance и Dynamics 365 Project Service Automation.
author: Yowelle
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
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: ed7ca3c85d3f99b7eefe10f4ddec822b9aeb1684
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071959"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a><span data-ttu-id="f66a6-103">Синхронизирайте категориите разходи за проекти между Finance and Operations и Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f66a6-103">Synchronize project expense categories between Finance and Operations and Project Service Automation</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="f66a6-104">Тази тема описва шаблон и основните задачи, които се използват за синхронизиране на категории на разход по проект между Dynamics 365 Finance и Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f66a6-104">This topic describes the templates and underlying tasks that are used to synchronize project expense categories between Dynamics 365 Finance and Dynamics 365 Project Service Automation.</span></span>

> [!NOTE]
> - <span data-ttu-id="f66a6-105">Интеграция на проектни задачи, категории транзакции, прогнози за часове, оценки на разходите и заключване на функционалността е налична във версия 8.0.</span><span class="sxs-lookup"><span data-stu-id="f66a6-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="f66a6-106">Интегрирането на действителни данни е достъпно от версия 8.0.1.</span><span class="sxs-lookup"><span data-stu-id="f66a6-106">Actuals integration is available in version 8.0.1 or later.</span></span>
> - <span data-ttu-id="f66a6-107">Ако използвате Enterprise Edition 7.3.0, след като инсталирате KB 4132657 и KB 4132660, ще можете да използвате шаблоните за интегриране на проектни задачи, категории на транзакционни транзакции, часови прогнози, прогнозни разходи и актуални данни и да конфигурирате заключване на функционалността.</span><span class="sxs-lookup"><span data-stu-id="f66a6-107">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="f66a6-108">Ако трябва да нулирате счетоводните разпределения, препоръчваме да инсталирате и KB 4131710.</span><span class="sxs-lookup"><span data-stu-id="f66a6-108">If you must reset the accounting distributions, we recommend that you also install KB 4131710.</span></span>

## <a name="data-flow-for-project-service-automation-and-finance"></a><span data-ttu-id="f66a6-109">Поток от данни за Project Service Automation и Finance</span><span class="sxs-lookup"><span data-stu-id="f66a6-109">Data flow for Project Service Automation and Finance</span></span>

<span data-ttu-id="f66a6-110">Решението за интеграция на Project Service Automation и Finance използва функцията за интегриране на данни, за да синхронизира данните между копията на Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="f66a6-110">The Project Service Automation and Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="f66a6-111">Шаблоните за интеграция, които се предлагат с функцията за интеграция на данни, позволяват потока от данни за категории на трансакция на прогнозни часови прогнози на проекта и прогнозни разходи за проекти между Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="f66a6-111">The integration templates that are available with the Data integration feature enable the flow of data about project expense transaction categories between Finance and Project Service Automation.</span></span>

<span data-ttu-id="f66a6-112">Ако категориите проектни разходи са усвоени във Finance, интеграционният поток е първо от Finance към Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f66a6-112">If the project expense categories are mastered in Finance, the integration flow is first from Finance to Project Service Automation.</span></span> <span data-ttu-id="f66a6-113">Идентификационните идентификатори на категориите на разходите по проекта след това се актуализират чрез синхронизиране от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="f66a6-113">The integration IDs of the project expense categories are then updated through synchronization from Project Service Automation to Finance.</span></span>

<span data-ttu-id="f66a6-114">Ако категориите проектни разходи са усвоени в Project Service Automation, интеграционният поток е първо от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="f66a6-114">If the project expense categories are mastered in Project Service Automation, the integration flow is first from Project Service Automation to Finance.</span></span> <span data-ttu-id="f66a6-115">Категориите на проектите вече трябва да бъдат конфигурирани във Finance преди синхронизирането от Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f66a6-115">The project categories must already be configured in Finance before the synchronization from Project Service Automation.</span></span> <span data-ttu-id="f66a6-116">След това синхронизирайте от Finance обратно към Project Service Automation и след това от Project Service Automation към Finance отново.</span><span class="sxs-lookup"><span data-stu-id="f66a6-116">Then synchronize from Finance back to Project Service Automation, and then from Project Service Automation to Finance again.</span></span> <span data-ttu-id="f66a6-117">По този начин помагате да гарантирате, че категориите са свързани и че не се създават дубликати.</span><span class="sxs-lookup"><span data-stu-id="f66a6-117">In this way, you help guarantee that the categories are linked, and that no duplicates are created.</span></span>

> [!NOTE]
> <span data-ttu-id="f66a6-118">Обикновено категориите разходи за проекти се усвояват във Finance.</span><span class="sxs-lookup"><span data-stu-id="f66a6-118">Typically, the project expense categories are mastered in Finance.</span></span> <span data-ttu-id="f66a6-119">Ако обаче не са или ако категориите разходи вече са създадени в Project Service Automation, първо трябва да синхронизирате с помощта на шаблона за категории транзакции на категории на проекта (PSA към Fin и Ops).</span><span class="sxs-lookup"><span data-stu-id="f66a6-119">However, if they aren't, or if expense categories have already been created in Project Service Automation, you must first synchronize by using the Project expense transaction categories (PSA to Fin and Ops) template.</span></span> <span data-ttu-id="f66a6-120">След това синхронизирайте, като използвате шаблона за категории транзакции на проекта (Fin и Ops към PSA).</span><span class="sxs-lookup"><span data-stu-id="f66a6-120">Then synchronize by using the Project expense transaction categories (Fin and Ops to PSA) template.</span></span> <span data-ttu-id="f66a6-121">След това трябва да стартирате синхронизирането от Project Service Automation към Finance още веднъж.</span><span class="sxs-lookup"><span data-stu-id="f66a6-121">You should then run the synchronization from Project Service Automation to Finance one more time.</span></span>
>
> <span data-ttu-id="f66a6-122">Ако първо синхронизирате от Project Service Automation, трябва да бъдат изпълнени следните изисквания във Finance, преди да се стартира синхронизацията:</span><span class="sxs-lookup"><span data-stu-id="f66a6-122">If you synchronize first from Project Service Automation, the following requirements must be met in Finance before the synchronization is run:</span></span>
>
> - <span data-ttu-id="f66a6-123">Споделената категория, която съответства на категорията на проекта, която е настроена в Project Service Automation, трябва да съществува и трябва да бъде активирана и за двете **Проект** и **Разход**.</span><span class="sxs-lookup"><span data-stu-id="f66a6-123">The shared category that matches the project category that is set up in Project Service Automation must exist, and it must be enabled for both **Project** and **Expense**.</span></span>
> - <span data-ttu-id="f66a6-124">За всяко юридическо лице по финанси, с което трябва да се интегрира, трябва да съществуват следните категории проекти:</span><span class="sxs-lookup"><span data-stu-id="f66a6-124">For each Finance legal entity that must be integrated with, the following project categories must exist:</span></span>
>
>     - <span data-ttu-id="f66a6-125">**Категория на проекта** съществува.</span><span class="sxs-lookup"><span data-stu-id="f66a6-125">**Project category** exists.</span></span> 
>     - <span data-ttu-id="f66a6-126">**Използвайте в разходи** е активирано.</span><span class="sxs-lookup"><span data-stu-id="f66a6-126">**Use in Expense** is enabled.</span></span>
>     - <span data-ttu-id="f66a6-127">**Активен в журнала** е активирано.</span><span class="sxs-lookup"><span data-stu-id="f66a6-127">**Active in journal** is enabled.</span></span>
>     - <span data-ttu-id="f66a6-128">**Тип транзакция** е зададено на **Разход**.</span><span class="sxs-lookup"><span data-stu-id="f66a6-128">**Transaction type** is set to **Expense**.</span></span>

<span data-ttu-id="f66a6-129">Следващата илюстрация показва как данните се синхронизират между Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="f66a6-129">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="f66a6-130">[![Поток от данни за интеграция на Project Service Automation с Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="f66a6-130">[![Data flow for Project Service Automation integration with Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span></span>

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a><span data-ttu-id="f66a6-131">Синхронизиране на категория на разход по проекта между Finance и Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f66a6-131">Project expense category synchronization from Finance to Project Service Automation</span></span>

### <a name="template-and-task"></a><span data-ttu-id="f66a6-132">Шаблони и задача</span><span class="sxs-lookup"><span data-stu-id="f66a6-132">Template and task</span></span>

<span data-ttu-id="f66a6-133">За достъп до шаблона, в администраторски център на Microsoft Power Apps, изберете **Проекти** и след това в горния десен ъгъл изберете **Нов проект** , за да изберете публични шаблони.</span><span class="sxs-lookup"><span data-stu-id="f66a6-133">To access the template, in the Microsoft Power Apps admin center, select **Projects** , and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="f66a6-134">Следният шаблон и основните задачи се използват за синхронизиране на категории на разходи на проекта от Finance към Project Service Automation:</span><span class="sxs-lookup"><span data-stu-id="f66a6-134">The following template and underlying task are used to synchronize project expense categories from Finance to Project Service Automation:</span></span>

- <span data-ttu-id="f66a6-135">**Име на шаблона в Интегриране на данни:** Категории на трансакция на разходи по проект (Fin и Ops към PSA)</span><span class="sxs-lookup"><span data-stu-id="f66a6-135">**Name of the template in Data integration:** Project expense transaction categories (Fin and Ops to PSA)</span></span>
- <span data-ttu-id="f66a6-136">**Име на задачата в проекта:** Синхронизирайте категории с PSA</span><span class="sxs-lookup"><span data-stu-id="f66a6-136">**Name of the task in the project:** Sync categories to PSA</span></span>

### <a name="entity-set"></a><span data-ttu-id="f66a6-137">Набор от обекти</span><span class="sxs-lookup"><span data-stu-id="f66a6-137">Entity set</span></span>

| <span data-ttu-id="f66a6-138">Finance</span><span class="sxs-lookup"><span data-stu-id="f66a6-138">Finance</span></span>                           | <span data-ttu-id="f66a6-139">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f66a6-139">Project Service Automation</span></span> |
|-----------------------------------|----------------------------|
| <span data-ttu-id="f66a6-140">Интеграционен обект за категории</span><span class="sxs-lookup"><span data-stu-id="f66a6-140">Integration entity for categories</span></span> | <span data-ttu-id="f66a6-141">Категории трансакция</span><span class="sxs-lookup"><span data-stu-id="f66a6-141">Transaction categories</span></span>     |

### <a name="entity-flow"></a><span data-ttu-id="f66a6-142">Поток на обекта</span><span class="sxs-lookup"><span data-stu-id="f66a6-142">Entity flow</span></span>

<span data-ttu-id="f66a6-143">Категориите на разходи на проекта се управляват във Finance и се синхронизират с Project Service Automation като категории на трансакция.</span><span class="sxs-lookup"><span data-stu-id="f66a6-143">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="f66a6-144">Power Query</span><span class="sxs-lookup"><span data-stu-id="f66a6-144">Power Query</span></span>

<span data-ttu-id="f66a6-145">Когато синхронизирате с Project Service Automation, трябва да използвате Microsoft Power Query за Excel, за да зададете типа на таксуване в категорията на транзакциите.</span><span class="sxs-lookup"><span data-stu-id="f66a6-145">When you're synchronizing to Project Service Automation, you must use Microsoft Power Query for Excel to set the billing type on the transaction category.</span></span> <span data-ttu-id="f66a6-146">Категориите на транзакционните категории на проекта (Fin и Ops към PSA) предоставят колона и картографиране по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="f66a6-146">The Project expense transaction categories (Fin and Ops to PSA) template provides a default column and mapping.</span></span> <span data-ttu-id="f66a6-147">Ако създадете свой собствен шаблон, трябва да добавите тази условна колона в Power Query.</span><span class="sxs-lookup"><span data-stu-id="f66a6-147">If you create your own template, you must add a conditional column in Power Query.</span></span> <span data-ttu-id="f66a6-148">Следвайте тези стъпки.</span><span class="sxs-lookup"><span data-stu-id="f66a6-148">Follow these steps.</span></span>

1. <span data-ttu-id="f66a6-149">Щракнете върху стрелката, за да отворите задачата за картографиране на категорията на разходите за проекта в шаблона за категории на транзакции за проект (Fin и Ops към PSA).</span><span class="sxs-lookup"><span data-stu-id="f66a6-149">Click the arrow to open the mapping of the project expense categories task in the Project expense transaction categories (Fin and Ops to PSA) template.</span></span>
2. <span data-ttu-id="f66a6-150">Щракнете върху връзката **Разширени заявки и филтриране** , за да отворите Power Query.</span><span class="sxs-lookup"><span data-stu-id="f66a6-150">Click the **Advance Query and Filtering** link to open Power Query.</span></span>
2. <span data-ttu-id="f66a6-151">Изберете **Добавете условна колона**.</span><span class="sxs-lookup"><span data-stu-id="f66a6-151">Select **Add Conditional Column**.</span></span>
3. <span data-ttu-id="f66a6-152">Въведете име за новата колона, като например **BillingType**.</span><span class="sxs-lookup"><span data-stu-id="f66a6-152">Enter a name for the new column, such as **BillingType**.</span></span>
4. <span data-ttu-id="f66a6-153">Въведете следното условие: **ако CATEGORYID не е равно на нула, тогава 19235001, в противен случай е нула**.</span><span class="sxs-lookup"><span data-stu-id="f66a6-153">Enter the following condition: **if CATEGORYID not equal to null then 19235001, Otherwise null**.</span></span>
5. <span data-ttu-id="f66a6-154">Щракнете върху **OK** на колоната.</span><span class="sxs-lookup"><span data-stu-id="f66a6-154">Click **OK** on the column.</span></span>
6. <span data-ttu-id="f66a6-155">Не забравяйте да картографирате тази нова колона на страницата за картографиране.</span><span class="sxs-lookup"><span data-stu-id="f66a6-155">Be sure to map this new column on the mapping page.</span></span>

<span data-ttu-id="f66a6-156">Следващата илюстрация показва пример за съпоставяне на задача на шаблон при интеграция на данни.</span><span class="sxs-lookup"><span data-stu-id="f66a6-156">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="f66a6-157">Картографирането показва информация за полето, която ще бъде синхронизирана от Finance в Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f66a6-157">The mapping shows the field information that will be synchronized from Finance to Project Service Automation.</span></span>

<span data-ttu-id="f66a6-158">[![Съпоставяне на шаблон за категория на разход по проекта и Project Service Automation](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="f66a6-158">[![Project expense category to Project Service Automation template mapping](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span></span>

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a><span data-ttu-id="f66a6-159">Синхронизиране на категория на разход по проекта между Finance и Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f66a6-159">Project expense category synchronization from Project Service Automation to Finance</span></span>

### <a name="template-and-task"></a><span data-ttu-id="f66a6-160">Шаблони и задача</span><span class="sxs-lookup"><span data-stu-id="f66a6-160">Template and task</span></span>

<span data-ttu-id="f66a6-161">Следният шаблон и основните задачи се използват за синхронизиране на категории на разходи на проекта от Project Service Automation към Finance:</span><span class="sxs-lookup"><span data-stu-id="f66a6-161">The following template and underlying task are used to synchronize project expense categories from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="f66a6-162">**Име на шаблона в Интегриране на данни:** Категории на трансакция на разходи по проект (PSA към Fin и Ops)</span><span class="sxs-lookup"><span data-stu-id="f66a6-162">**Name of the template in Data integration:** Project expense transaction categories (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="f66a6-163">**Име на задачата в проекта:** Синхронизирайте категории с Fin Ops</span><span class="sxs-lookup"><span data-stu-id="f66a6-163">**Name of the task in the project:** Sync categories to Fin Ops</span></span>

### <a name="entity-set"></a><span data-ttu-id="f66a6-164">Набор от обекти</span><span class="sxs-lookup"><span data-stu-id="f66a6-164">Entity set</span></span>

| <span data-ttu-id="f66a6-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f66a6-165">Project Service Automation</span></span> | <span data-ttu-id="f66a6-166">Finance</span><span class="sxs-lookup"><span data-stu-id="f66a6-166">Finance</span></span>                           |
|----------------------------|-----------------------------------|
| <span data-ttu-id="f66a6-167">Категории трансакция</span><span class="sxs-lookup"><span data-stu-id="f66a6-167">Transaction categories</span></span>     | <span data-ttu-id="f66a6-168">Интеграционен обект за категории</span><span class="sxs-lookup"><span data-stu-id="f66a6-168">Integration entity for categories</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="f66a6-169">Поток на обекта</span><span class="sxs-lookup"><span data-stu-id="f66a6-169">Entity flow</span></span>

<span data-ttu-id="f66a6-170">Категориите на разходи на проекта се управляват във Finance и се синхронизират с Project Service Automation като категории на трансакция.</span><span class="sxs-lookup"><span data-stu-id="f66a6-170">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span> <span data-ttu-id="f66a6-171">Обратната синхронизация с актуализации на Finance в категорията ба проект във Finance с ИД на интеграция от Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f66a6-171">The synchronization back to Finance updates the project category in Finance with the integration ID from Project Service Automation.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="f66a6-172">Съпоставяне на шаблони при интеграция на данни</span><span class="sxs-lookup"><span data-stu-id="f66a6-172">Template mapping in Data integration</span></span>

<span data-ttu-id="f66a6-173">Следващата илюстрация показва пример за съпоставяне на задача на шаблон при интеграция на данни.</span><span class="sxs-lookup"><span data-stu-id="f66a6-173">The following illustration shows an example of the template task mapping in Data integration.</span></span>

> [!NOTE]
> <span data-ttu-id="f66a6-174">Картографирането показва информация за полето, която ще бъде синхронизирана от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="f66a6-174">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="f66a6-175">[![Съпоставяне на Project Service Automation с шаблон на Finance](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="f66a6-175">[![Project Service Automation to Finance template mapping](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span></span>
