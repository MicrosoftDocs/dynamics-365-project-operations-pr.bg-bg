---
title: Синхронизирайте категориите разходи за проекти между Finance and Operations и Project Service Automation
description: Тази тема описва шаблон и основните задачи, които се използват за синхронизиране на категории на разход по проект между Microsoft Dynamics 365 Finance и Dynamics 365 Project Service Automation.
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
ms.assetid: 7dd914dc-1913-45eb-8a67-e897b00089fa
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 757fe1dbc804b986fc3334ebae7254a3f0491f59
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749313"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a><span data-ttu-id="2cd9c-103">Синхронизирайте категориите разходи за проекти между Finance and Operations и Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="2cd9c-103">Synchronize project expense categories between Finance and Operations and Project Service Automation</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="2cd9c-104">Тази тема описва шаблон и основните задачи, които се използват за синхронизиране на категории на разход по проект между Dynamics 365 Finance и Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-104">This topic describes the templates and underlying tasks that are used to synchronize project expense categories between Dynamics 365 Finance and Dynamics 365 Project Service Automation.</span></span>

> [!NOTE]
> - <span data-ttu-id="2cd9c-105">Интеграция на проектни задачи, категории транзакции, прогнози за часове, оценки на разходите и заключване на функционалността е налична във версия 8.0.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="2cd9c-106">Интегрирането на действителни данни е достъпно от версия 8.0.1.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-106">Actuals integration is available in version 8.0.1 or later.</span></span>
> - <span data-ttu-id="2cd9c-107">Ако използвате Enterprise Edition 7.3.0, след като инсталирате KB 4132657 и KB 4132660, ще можете да използвате шаблоните за интегриране на проектни задачи, категории на транзакционни транзакции, часови прогнози, прогнозни разходи и актуални данни и да конфигурирате заключване на функционалността.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-107">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="2cd9c-108">Ако трябва да нулирате счетоводните разпределения, препоръчваме да инсталирате и KB 4131710.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-108">If you must reset the accounting distributions, we recommend that you also install KB 4131710.</span></span>

## <a name="data-flow-for-project-service-automation-and-finance"></a><span data-ttu-id="2cd9c-109">Поток от данни за Project Service Automation и Finance</span><span class="sxs-lookup"><span data-stu-id="2cd9c-109">Data flow for Project Service Automation and Finance</span></span>

<span data-ttu-id="2cd9c-110">Решението за интеграция на Project Service Automation и Finance използва функцията за интегриране на данни, за да синхронизира данните между копията на Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-110">The Project Service Automation and Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="2cd9c-111">Шаблоните за интеграция, които се предлагат с функцията за интеграция на данни, позволяват потока от данни за категории на трансакция на прогнозни часови прогнози на проекта и прогнозни разходи за проекти между Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-111">The integration templates that are available with the Data integration feature enable the flow of data about project expense transaction categories between Finance and Project Service Automation.</span></span>

<span data-ttu-id="2cd9c-112">Ако категориите проектни разходи са усвоени във Finance, интеграционният поток е първо от Finance към Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-112">If the project expense categories are mastered in Finance, the integration flow is first from Finance to Project Service Automation.</span></span> <span data-ttu-id="2cd9c-113">Идентификационните идентификатори на категориите на разходите по проекта след това се актуализират чрез синхронизиране от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-113">The integration IDs of the project expense categories are then updated through synchronization from Project Service Automation to Finance.</span></span>

<span data-ttu-id="2cd9c-114">Ако категориите проектни разходи са усвоени в Project Service Automation, интеграционният поток е първо от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-114">If the project expense categories are mastered in Project Service Automation, the integration flow is first from Project Service Automation to Finance.</span></span> <span data-ttu-id="2cd9c-115">Категориите на проектите вече трябва да бъдат конфигурирани във Finance преди синхронизирането от Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-115">The project categories must already be configured in Finance before the synchronization from Project Service Automation.</span></span> <span data-ttu-id="2cd9c-116">След това синхронизирайте от Finance обратно към Project Service Automation и след това от Project Service Automation към Finance отново.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-116">Then synchronize from Finance back to Project Service Automation, and then from Project Service Automation to Finance again.</span></span> <span data-ttu-id="2cd9c-117">По този начин помагате да гарантирате, че категориите са свързани и че не се създават дубликати.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-117">In this way, you help guarantee that the categories are linked, and that no duplicates are created.</span></span>

> [!NOTE]
> <span data-ttu-id="2cd9c-118">Обикновено категориите разходи за проекти се усвояват във Finance.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-118">Typically, the project expense categories are mastered in Finance.</span></span> <span data-ttu-id="2cd9c-119">Ако обаче не са или ако категориите разходи вече са създадени в Project Service Automation, първо трябва да синхронизирате с помощта на шаблона за категории транзакции на категории на проекта (PSA към Fin и Ops).</span><span class="sxs-lookup"><span data-stu-id="2cd9c-119">However, if they aren't, or if expense categories have already been created in Project Service Automation, you must first synchronize by using the Project expense transaction categories (PSA to Fin and Ops) template.</span></span> <span data-ttu-id="2cd9c-120">След това синхронизирайте, като използвате шаблона за категории транзакции на проекта (Fin и Ops към PSA).</span><span class="sxs-lookup"><span data-stu-id="2cd9c-120">Then synchronize by using the Project expense transaction categories (Fin and Ops to PSA) template.</span></span> <span data-ttu-id="2cd9c-121">След това трябва да стартирате синхронизирането от Project Service Automation към Finance още веднъж.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-121">You should then run the synchronization from Project Service Automation to Finance one more time.</span></span>
>
> <span data-ttu-id="2cd9c-122">Ако първо синхронизирате от Project Service Automation, трябва да бъдат изпълнени следните изисквания във Finance, преди да се стартира синхронизацията:</span><span class="sxs-lookup"><span data-stu-id="2cd9c-122">If you synchronize first from Project Service Automation, the following requirements must be met in Finance before the synchronization is run:</span></span>
>
> - <span data-ttu-id="2cd9c-123">Споделената категория, която съответства на категорията на проекта, която е настроена в Project Service Automation, трябва да съществува и трябва да бъде активирана и за двете **Проект** и **Разход**.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-123">The shared category that matches the project category that is set up in Project Service Automation must exist, and it must be enabled for both **Project** and **Expense**.</span></span>
> - <span data-ttu-id="2cd9c-124">За всяко юридическо лице по финанси, с което трябва да се интегрира, трябва да съществуват следните категории проекти:</span><span class="sxs-lookup"><span data-stu-id="2cd9c-124">For each Finance legal entity that must be integrated with, the following project categories must exist:</span></span>
>
>     - <span data-ttu-id="2cd9c-125">**Категория на проекта** съществува.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-125">**Project category** exists.</span></span> 
>     - <span data-ttu-id="2cd9c-126">**Използвайте в разходи** е активирано.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-126">**Use in Expense** is enabled.</span></span>
>     - <span data-ttu-id="2cd9c-127">**Активен в журнала** е активирано.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-127">**Active in journal** is enabled.</span></span>
>     - <span data-ttu-id="2cd9c-128">**Тип транзакция** е зададено на **Разход**.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-128">**Transaction type** is set to **Expense**.</span></span>

<span data-ttu-id="2cd9c-129">Следващата илюстрация показва как данните се синхронизират между Project Service Automation и Finance.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-129">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="2cd9c-130">[![Поток от данни за интеграция на Project Service Automation с Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="2cd9c-130">[![Data flow for Project Service Automation integration with Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span></span>

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a><span data-ttu-id="2cd9c-131">Синхронизиране на категория на разход по проекта между Finance и Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="2cd9c-131">Project expense category synchronization from Finance to Project Service Automation</span></span>

### <a name="template-and-task"></a><span data-ttu-id="2cd9c-132">Шаблони и задача</span><span class="sxs-lookup"><span data-stu-id="2cd9c-132">Template and task</span></span>

<span data-ttu-id="2cd9c-133">За достъп до шаблона, в администраторски център на Microsoft Power Apps, изберете **Проекти** и след това в горния десен ъгъл изберете **Нов проект**, за да изберете публични шаблони.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-133">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="2cd9c-134">Следният шаблон и основните задачи се използват за синхронизиране на категории на разходи на проекта от Finance към Project Service Automation:</span><span class="sxs-lookup"><span data-stu-id="2cd9c-134">The following template and underlying task are used to synchronize project expense categories from Finance to Project Service Automation:</span></span>

- <span data-ttu-id="2cd9c-135">**Име на шаблона в Интегриране на данни:** Категории на трансакция на разходи по проект (Fin и Ops към PSA)</span><span class="sxs-lookup"><span data-stu-id="2cd9c-135">**Name of the template in Data integration:** Project expense transaction categories (Fin and Ops to PSA)</span></span>
- <span data-ttu-id="2cd9c-136">**Име на задачата в проекта:** Синхронизирайте категории с PSA</span><span class="sxs-lookup"><span data-stu-id="2cd9c-136">**Name of the task in the project:** Sync categories to PSA</span></span>

### <a name="entity-set"></a><span data-ttu-id="2cd9c-137">Набор от обекти</span><span class="sxs-lookup"><span data-stu-id="2cd9c-137">Entity set</span></span>

| <span data-ttu-id="2cd9c-138">Finance</span><span class="sxs-lookup"><span data-stu-id="2cd9c-138">Finance</span></span>                           | <span data-ttu-id="2cd9c-139">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="2cd9c-139">Project Service Automation</span></span> |
|-----------------------------------|----------------------------|
| <span data-ttu-id="2cd9c-140">Интеграционен обект за категории</span><span class="sxs-lookup"><span data-stu-id="2cd9c-140">Integration entity for categories</span></span> | <span data-ttu-id="2cd9c-141">Категории трансакция</span><span class="sxs-lookup"><span data-stu-id="2cd9c-141">Transaction categories</span></span>     |

### <a name="entity-flow"></a><span data-ttu-id="2cd9c-142">Поток на обекта</span><span class="sxs-lookup"><span data-stu-id="2cd9c-142">Entity flow</span></span>

<span data-ttu-id="2cd9c-143">Категориите на разходи на проекта се управляват във Finance и се синхронизират с Project Service Automation като категории на трансакция.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-143">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="2cd9c-144">Power Query</span><span class="sxs-lookup"><span data-stu-id="2cd9c-144">Power Query</span></span>

<span data-ttu-id="2cd9c-145">Когато синхронизирате с Project Service Automation, трябва да използвате Microsoft Power Query за Excel, за да зададете типа на таксуване в категорията на транзакциите.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-145">When you're synchronizing to Project Service Automation, you must use Microsoft Power Query for Excel to set the billing type on the transaction category.</span></span> <span data-ttu-id="2cd9c-146">Категориите на транзакционните категории на проекта (Fin и Ops към PSA) предоставят колона и картографиране по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-146">The Project expense transaction categories (Fin and Ops to PSA) template provides a default column and mapping.</span></span> <span data-ttu-id="2cd9c-147">Ако създадете свой собствен шаблон, трябва да добавите тази условна колона в Power Query.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-147">If you create your own template, you must add a conditional column in Power Query.</span></span> <span data-ttu-id="2cd9c-148">Следвайте тези стъпки.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-148">Follow these steps.</span></span>

1. <span data-ttu-id="2cd9c-149">Щракнете върху стрелката, за да отворите задачата за картографиране на категорията на разходите за проекта в шаблона за категории на транзакции за проект (Fin и Ops към PSA).</span><span class="sxs-lookup"><span data-stu-id="2cd9c-149">Click the arrow to open the mapping of the project expense categories task in the Project expense transaction categories (Fin and Ops to PSA) template.</span></span>
2. <span data-ttu-id="2cd9c-150">Щракнете върху връзката **Разширени заявки и филтриране**, за да отворите Power Query.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-150">Click the **Advance Query and Filtering** link to open Power Query.</span></span>
2. <span data-ttu-id="2cd9c-151">Изберете **Добавете условна колона**.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-151">Select **Add Conditional Column**.</span></span>
3. <span data-ttu-id="2cd9c-152">Въведете име за новата колона, като например **BillingType**.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-152">Enter a name for the new column, such as **BillingType**.</span></span>
4. <span data-ttu-id="2cd9c-153">Въведете следното условие: **ако CATEGORYID не е равно на нула, тогава 19235001, в противен случай е нула**.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-153">Enter the following condition: **if CATEGORYID not equal to null then 19235001, Otherwise null**.</span></span>
5. <span data-ttu-id="2cd9c-154">Щракнете върху **OK** на колоната.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-154">Click **OK** on the column.</span></span>
6. <span data-ttu-id="2cd9c-155">Не забравяйте да картографирате тази нова колона на страницата за картографиране.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-155">Be sure to map this new column on the mapping page.</span></span>

<span data-ttu-id="2cd9c-156">Следващата илюстрация показва пример за съпоставяне на задача на шаблон при интеграция на данни.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-156">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="2cd9c-157">Картографирането показва информация за полето, която ще бъде синхронизирана от Finance в Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-157">The mapping shows the field information that will be synchronized from Finance to Project Service Automation.</span></span>

<span data-ttu-id="2cd9c-158">[![Съпоставяне на шаблони](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="2cd9c-158">[![Template mapping](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span></span>

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a><span data-ttu-id="2cd9c-159">Синхронизиране на категория на разход по проекта между Finance и Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="2cd9c-159">Project expense category synchronization from Project Service Automation to Finance</span></span>

### <a name="template-and-task"></a><span data-ttu-id="2cd9c-160">Шаблони и задача</span><span class="sxs-lookup"><span data-stu-id="2cd9c-160">Template and task</span></span>

<span data-ttu-id="2cd9c-161">Следният шаблон и основните задачи се използват за синхронизиране на категории на разходи на проекта от Project Service Automation към Finance:</span><span class="sxs-lookup"><span data-stu-id="2cd9c-161">The following template and underlying task are used to synchronize project expense categories from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="2cd9c-162">**Име на шаблона в Интегриране на данни:** Категории на трансакция на разходи по проект (PSA към Fin и Ops)</span><span class="sxs-lookup"><span data-stu-id="2cd9c-162">**Name of the template in Data integration:** Project expense transaction categories (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="2cd9c-163">**Име на задачата в проекта:** Синхронизирайте категории с Fin Ops</span><span class="sxs-lookup"><span data-stu-id="2cd9c-163">**Name of the task in the project:** Sync categories to Fin Ops</span></span>

### <a name="entity-set"></a><span data-ttu-id="2cd9c-164">Набор от обекти</span><span class="sxs-lookup"><span data-stu-id="2cd9c-164">Entity set</span></span>

| <span data-ttu-id="2cd9c-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="2cd9c-165">Project Service Automation</span></span> | <span data-ttu-id="2cd9c-166">Finance</span><span class="sxs-lookup"><span data-stu-id="2cd9c-166">Finance</span></span>                           |
|----------------------------|-----------------------------------|
| <span data-ttu-id="2cd9c-167">Категории трансакция</span><span class="sxs-lookup"><span data-stu-id="2cd9c-167">Transaction categories</span></span>     | <span data-ttu-id="2cd9c-168">Интеграционен обект за категории</span><span class="sxs-lookup"><span data-stu-id="2cd9c-168">Integration entity for categories</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="2cd9c-169">Поток на обекта</span><span class="sxs-lookup"><span data-stu-id="2cd9c-169">Entity flow</span></span>

<span data-ttu-id="2cd9c-170">Категориите на разходи на проекта се управляват във Finance и се синхронизират с Project Service Automation като категории на трансакция.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-170">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span> <span data-ttu-id="2cd9c-171">Обратната синхронизация с актуализации на Finance в категорията ба проект във Finance с ИД на интеграция от Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-171">The synchronization back to Finance updates the project category in Finance with the integration ID from Project Service Automation.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="2cd9c-172">Съпоставяне на шаблони при интеграция на данни</span><span class="sxs-lookup"><span data-stu-id="2cd9c-172">Template mapping in Data integration</span></span>

<span data-ttu-id="2cd9c-173">Следващата илюстрация показва пример за съпоставяне на задача на шаблон при интеграция на данни.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-173">The following illustration shows an example of the template task mapping in Data integration.</span></span>

> [!NOTE]
> <span data-ttu-id="2cd9c-174">Картографирането показва информация за полето, която ще бъде синхронизирана от Project Service Automation към Finance.</span><span class="sxs-lookup"><span data-stu-id="2cd9c-174">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="2cd9c-175">[![Съпоставяне на шаблони](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="2cd9c-175">[![Template mapping](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span></span>
