---
title: Създаване на разширени договори за фактуриране въз основа на напредъка
description: Тази тема обяснява как да създадете проектни договори, така че да можете да генерирате фактури за клиенти въз основа на процент от завършената работа.
author: RadhikaRS
ms.date: 03/26/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 3b445488100e0a8335a05505405953b173ff836c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999658"
---
# <a name="create-advanced-contracts-for-billing-based-on-progress"></a><span data-ttu-id="d617f-103">Създаване на разширени договори за фактуриране въз основа на напредъка</span><span class="sxs-lookup"><span data-stu-id="d617f-103">Create advanced contracts for billing based on progress</span></span>
[!include [banner](../includes/banner.md)]

<span data-ttu-id="d617f-104">Тази тема обяснява как да създадете проектни договори, така че да можете да създавате фактури за клиенти въз основа на процент от завършената работа.</span><span class="sxs-lookup"><span data-stu-id="d617f-104">This topic explains how to create project contracts so that you can create invoices for customers, based on a percentage of completed work.</span></span> <span data-ttu-id="d617f-105">Сумите на фактурите се изчисляват автоматично за бюджетните категории работа, които сте настроили за даден проект.</span><span class="sxs-lookup"><span data-stu-id="d617f-105">Invoice amounts are automatically calculated for the budget categories of work that you set up for a project.</span></span> <span data-ttu-id="d617f-106">Времето за фактура се задава, когато договаряте договора за проект с клиента.</span><span class="sxs-lookup"><span data-stu-id="d617f-106">The invoice timing is set when you negotiate the project contract with the customer.</span></span>

<span data-ttu-id="d617f-107">Използвайте процедурите в тази тема, за да създадете договор, асоцииран проект и правила за фактуриране, които изчисляват сумите на фактурите за бюджетните категории работа, които сте настроили за проекта.</span><span class="sxs-lookup"><span data-stu-id="d617f-107">Use the procedures in this topic to set up a contract, an associated project, and the billing rules that calculate invoice amounts for the budget categories of work that you set up for the project.</span></span>

<span data-ttu-id="d617f-108">След като създадете договора и проекта, можете да настроите подробностите за проекта.</span><span class="sxs-lookup"><span data-stu-id="d617f-108">After you've created the contract and the project, you can set up the details of the project.</span></span> <span data-ttu-id="d617f-109">Например можете да дефинирате дейности и да назначите работници към проекта.</span><span class="sxs-lookup"><span data-stu-id="d617f-109">For example, you can define activities and assign workers to the project.</span></span>

## <a name="example"></a><span data-ttu-id="d617f-110">Пример</span><span class="sxs-lookup"><span data-stu-id="d617f-110">Example</span></span>

<span data-ttu-id="d617f-111">Вашата организация е фирма за разработка на софтуер.</span><span class="sxs-lookup"><span data-stu-id="d617f-111">Your organization is a software development firm.</span></span> <span data-ttu-id="d617f-112">Вие се съгласявате да разработите пакет за отчитане на заплати за клиент на обща такса от 20 000 щатски долара (USD).</span><span class="sxs-lookup"><span data-stu-id="d617f-112">You agree to develop a payroll accounting package for a customer for a total fee of 20,000 US dollars (USD).</span></span> <span data-ttu-id="d617f-113">Вашата организация се съгласява да фактурира клиента, докато попълвате конкретни проценти от проекта.</span><span class="sxs-lookup"><span data-stu-id="d617f-113">Your organization agrees to invoice the customer as you complete specific percentages of the project.</span></span> <span data-ttu-id="d617f-114">Настройвате следните категории проекти за работата, така че да можете да ги използвате в процеса на фактуриране:</span><span class="sxs-lookup"><span data-stu-id="d617f-114">You set up the following project categories for the work, so that you can use them in the billing process:</span></span>

- <span data-ttu-id="d617f-115">Консултиране</span><span class="sxs-lookup"><span data-stu-id="d617f-115">Consulting</span></span>
- <span data-ttu-id="d617f-116">Проектиране</span><span class="sxs-lookup"><span data-stu-id="d617f-116">Design</span></span>
- <span data-ttu-id="d617f-117">Инсталиране</span><span class="sxs-lookup"><span data-stu-id="d617f-117">Installation</span></span>

<span data-ttu-id="d617f-118">Настройвате също правила за таксуване, които автоматично изчисляват сумите на фактурите за процента на завършена работа по проекта във всяка категория.</span><span class="sxs-lookup"><span data-stu-id="d617f-118">You also set up billing rules that automatically calculate the invoice amounts for the percentage of project work that is completed in each category.</span></span>

<span data-ttu-id="d617f-119">Управителят на бюджета създава бюджет за категориите проекти.</span><span class="sxs-lookup"><span data-stu-id="d617f-119">The budget manager creates a budget for the project categories.</span></span> <span data-ttu-id="d617f-120">Количеството завършена работа се изчислява автоматично като процент от действителната работа в сравнение с предвидените в бюджета суми.</span><span class="sxs-lookup"><span data-stu-id="d617f-120">The amount of completed work is automatically calculated as a percentage of actual work in comparison to the budgeted amounts.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d617f-121">Предварителни изисквания</span><span class="sxs-lookup"><span data-stu-id="d617f-121">Prerequisites</span></span>

<span data-ttu-id="d617f-122">Преди да създадете проект, който използва правила за фактуриране, трябва да настроите последователностите от числа за правилата за фактуриране и дневник за такси, който се използва за осчетоводяване на фактуриране на напредъка.</span><span class="sxs-lookup"><span data-stu-id="d617f-122">Before you create a project that uses billing rules, you must set up the number sequences for billing rules and a fee journal that is used to post progress billings.</span></span>

1. <span data-ttu-id="d617f-123">Отидете на **Управление на проекти и счетоводство** \> **Настройка** \> **Управление на проекти и счетоводни параметри**.</span><span class="sxs-lookup"><span data-stu-id="d617f-123">Go to **Project management and accounting** \> **Setup** \> **Project management and accounting parameters**.</span></span>
2. <span data-ttu-id="d617f-124">На страницата **Управление на проекти и счетоводни параметри** в раздела **Брой последователности** задайте числовата последователност, която искате да използвате, когато се създават правила за таксуване.</span><span class="sxs-lookup"><span data-stu-id="d617f-124">On the **Project management and accounting parameters** page, on the **Number sequences** tab, set up the number sequence that you want to use when billing rules are created.</span></span>
3. <span data-ttu-id="d617f-125">Отидете на **Управление на проекти и счетоводство** \> **Журнали** \> **Такса**.</span><span class="sxs-lookup"><span data-stu-id="d617f-125">Go to **Project management and accounting** \> **Journals** \> **Fee**.</span></span>
4. <span data-ttu-id="d617f-126">На страницата **Журнал на таксите** изберете **Създаване** и въведете името на дневника.</span><span class="sxs-lookup"><span data-stu-id="d617f-126">On the **Fee journal** page, select **New**, and enter the journal name.</span></span>

## <a name="create-a-contract-for-progress-billings"></a><span data-ttu-id="d617f-127">Създайте договор за фактуриране на напредъка</span><span class="sxs-lookup"><span data-stu-id="d617f-127">Create a contract for progress billings</span></span>

<span data-ttu-id="d617f-128">Използвайте тази процедура, за да създадете договор за проект за проект с фиксирана цена.</span><span class="sxs-lookup"><span data-stu-id="d617f-128">Use this procedure to create a project contract for a fixed-price project.</span></span> <span data-ttu-id="d617f-129">Създавате фактура за проект, когато работата, завършена по проекта, достигне определен процент.</span><span class="sxs-lookup"><span data-stu-id="d617f-129">You create a project invoice when the work that is completed on the project reaches a specified percentage.</span></span>

1. <span data-ttu-id="d617f-130">Отидете на **Управление на проекти и счетоводство** \> **Проекти** \> **Договори за проекти**.</span><span class="sxs-lookup"><span data-stu-id="d617f-130">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="d617f-131">На страницата **договори на проект** изберете **Нов**.</span><span class="sxs-lookup"><span data-stu-id="d617f-131">On the **Project contracts** page, select **New**.</span></span>
3. <span data-ttu-id="d617f-132">В диалоговия прозорец **Нов договор за проект**, задайте следните полета:</span><span class="sxs-lookup"><span data-stu-id="d617f-132">In the **New project contract** dialog box, set the following fields:</span></span>

    - <span data-ttu-id="d617f-133">**Име**</span><span class="sxs-lookup"><span data-stu-id="d617f-133">**Name**</span></span>
    - <span data-ttu-id="d617f-134">**Тип финансиране**</span><span class="sxs-lookup"><span data-stu-id="d617f-134">**Funding type**</span></span>
    - <span data-ttu-id="d617f-135">**Източник на финансиране**</span><span class="sxs-lookup"><span data-stu-id="d617f-135">**Funding source**</span></span>
    - <span data-ttu-id="d617f-136">**Валута на продажбите** - По подразбиране тази валута се използва за фактури на клиенти, които са свързани с договор за проект.</span><span class="sxs-lookup"><span data-stu-id="d617f-136">**Sales currency** – By default, this currency is used for customer invoices that are associated with the project contract.</span></span> <span data-ttu-id="d617f-137">Можете обаче да промените валутата на продажбите на конкретна фактура на клиента.</span><span class="sxs-lookup"><span data-stu-id="d617f-137">However, you can change the sales currency on a specific customer invoice.</span></span>

4. <span data-ttu-id="d617f-138">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="d617f-138">Select **OK**.</span></span> <span data-ttu-id="d617f-139">Информацията се копира в заглавката на страницата **Договори за проекти**.</span><span class="sxs-lookup"><span data-stu-id="d617f-139">The information is copied to the header of the **Project contracts** page.</span></span>
5. <span data-ttu-id="d617f-140">На страницата **Договори за проекти** попълнете останалата част от необходимата информация за проекта.</span><span class="sxs-lookup"><span data-stu-id="d617f-140">On the **Project contracts** page, fill in the rest of the required information for the project.</span></span>

## <a name="create-a-project-for-progress-billings"></a><span data-ttu-id="d617f-141">Създайте проект за фактуриране на напредъка</span><span class="sxs-lookup"><span data-stu-id="d617f-141">Create a project for progress billings</span></span>

<span data-ttu-id="d617f-142">Следвайте тези стъпки, за да създадете проект и всички подпроекти, свързани с договор за проект.</span><span class="sxs-lookup"><span data-stu-id="d617f-142">Follow these steps to create a project and any subprojects that are associated with a project contract.</span></span>

1. <span data-ttu-id="d617f-143">Отидете на **Управление на проекти и счетоводство** \> **Проекти** \> **Всички проекти**.</span><span class="sxs-lookup"><span data-stu-id="d617f-143">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="d617f-144">На страницата **Всички проекти** изберете **Създаване**.</span><span class="sxs-lookup"><span data-stu-id="d617f-144">On the **All projects** page, select **New**.</span></span>
3. <span data-ttu-id="d617f-145">В диалоговия прозорец **Нов проект** в полето **Тип на проекта** изберете **Време и материал**.</span><span class="sxs-lookup"><span data-stu-id="d617f-145">In the **New project** dialog box, in the **Project type** field, select **Time and material**.</span></span>
4. <span data-ttu-id="d617f-146">Избор на група на проекта.</span><span class="sxs-lookup"><span data-stu-id="d617f-146">Select a project group.</span></span> <span data-ttu-id="d617f-147">Проектната група определя информацията за осчетоводяване за проектите, които са възложени на групата.</span><span class="sxs-lookup"><span data-stu-id="d617f-147">A project group defines the posting information for the projects that are assigned to the group.</span></span>
5. <span data-ttu-id="d617f-148">Изберете **Създаване на проект**.</span><span class="sxs-lookup"><span data-stu-id="d617f-148">Select **Create project**.</span></span>
6. <span data-ttu-id="d617f-149">След като проектът е създаден, задайте етапа на проекта на **В процес**.</span><span class="sxs-lookup"><span data-stu-id="d617f-149">After the project is created, set the project stage to **In process**.</span></span>

## <a name="create-a-budget-for-a-project"></a><span data-ttu-id="d617f-150">Създаване на бюджет за проект</span><span class="sxs-lookup"><span data-stu-id="d617f-150">Create a budget for a project</span></span>

<span data-ttu-id="d617f-151">Категориите на бюджет се използват за автоматично изчисляване на сумите на фактурите за процента на завършена работа за всяка категория.</span><span class="sxs-lookup"><span data-stu-id="d617f-151">Budget categories are used to automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="d617f-152">Следвайте тези стъпки, за да създадете бюджетни категории за прогнозните разходи.</span><span class="sxs-lookup"><span data-stu-id="d617f-152">Follow these steps to create budget categories for the estimated costs.</span></span>

1. <span data-ttu-id="d617f-153">Отидете на **Управление на проекти и счетоводство** \> **Проекти** \> **Всички проекти**.</span><span class="sxs-lookup"><span data-stu-id="d617f-153">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="d617f-154">На страницата **Всички проекти** изберете и отворете желания от вас проект.</span><span class="sxs-lookup"><span data-stu-id="d617f-154">On the **All projects** page, select and open the project that you want.</span></span>
3. <span data-ttu-id="d617f-155">На страницата **Проекти** в панела за действие, на раздела **План** в групата **Бюджет** изберете **Бюджет на проекта**.</span><span class="sxs-lookup"><span data-stu-id="d617f-155">On the **Projects** page, on the Action Pane, on the **Plan** tab, in the **Budget** group, select **Project budget**.</span></span>
4. <span data-ttu-id="d617f-156">На страница **Бюджет на проекта** въведете приблизителни разходи за всяка категория в проекта.</span><span class="sxs-lookup"><span data-stu-id="d617f-156">On the **Project budget** page, enter an estimated cost for each category in the project.</span></span>

## <a name="create-billing-rules-for-progress-billings"></a><span data-ttu-id="d617f-157">Създайте правила за фактуриране за фактуриране на напредъка</span><span class="sxs-lookup"><span data-stu-id="d617f-157">Create billing rules for progress billings</span></span>

1. <span data-ttu-id="d617f-158">Отидете на **Управление на проекти и счетоводство** \> **Проекти** \> **Договори за проекти**.</span><span class="sxs-lookup"><span data-stu-id="d617f-158">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="d617f-159">На страницата **Договори по проект** изберете и отворете договор по проект.</span><span class="sxs-lookup"><span data-stu-id="d617f-159">On the **Project contracts** page, select and open a project contract.</span></span>
3. <span data-ttu-id="d617f-160">На страницата за договор за проект, на FastTab **Правила за фактуриране** изберете **Добавяне**.</span><span class="sxs-lookup"><span data-stu-id="d617f-160">On the project contract page, on the **Billing rules** FastTab, select **Add**.</span></span>
4. <span data-ttu-id="d617f-161">На страницата **Правило за таксуване** в полето **Тип линия** изберете **Напредък**.</span><span class="sxs-lookup"><span data-stu-id="d617f-161">On the **Billing rule** page, in the **Line type** field, select **Progress**.</span></span>
5. <span data-ttu-id="d617f-162">На FastTab **Подробности за правилото за таксуване** в полето **Стойност на договора** въведете общата стойност на договора.</span><span class="sxs-lookup"><span data-stu-id="d617f-162">On the **Billing rule line details** FastTab, in the **Contract value** field, enter the total value of the contract.</span></span>
6. <span data-ttu-id="d617f-163">В полето **Категория** изберете категорията, в която да публикувате транзакцията с такса.</span><span class="sxs-lookup"><span data-stu-id="d617f-163">In the **Category** field, select the category to post the fee transaction to.</span></span>
7. <span data-ttu-id="d617f-164">В полето **Проект** изберете проекта, който използва това правило за фактуриране.</span><span class="sxs-lookup"><span data-stu-id="d617f-164">In the **Project** field, select the project that uses this billing rule.</span></span>
8. <span data-ttu-id="d617f-165">По избор: Присвойте правилото за фактуриране на допълнителни проекти.</span><span class="sxs-lookup"><span data-stu-id="d617f-165">Optional: Assign the billing rule to additional projects.</span></span> <span data-ttu-id="d617f-166">Във FastTab **Проект** в секцията **Налични проекти** проект и след това изберете бутона със стрелка надясно, за да добавите проекта към секцията **Избрани проекти**.</span><span class="sxs-lookup"><span data-stu-id="d617f-166">On the **Project** FastTab, in the **Available projects** section, select a project, and then select the right arrow button to add the project to the **Selected projects** section.</span></span>
9. <span data-ttu-id="d617f-167">По избор: Изчислете процентната сума, която клиентът удържа от плащания по фактура.</span><span class="sxs-lookup"><span data-stu-id="d617f-167">Optional: Calculate the percentage amount that the customer withholds from payments on an invoice.</span></span> <span data-ttu-id="d617f-168">На FastTab **Условия за задържане на плащане** изберете източника на финансиране и след това в полето **Процент на задържане** въведете процента на задържане.</span><span class="sxs-lookup"><span data-stu-id="d617f-168">On the **Payment retention terms** FastTab, select the funding source, and then, in the **Retention percentage** field, enter the retention percentage.</span></span>
10. <span data-ttu-id="d617f-169">Повторете тези стъпки, за да създадете допълнителни правила за фактуриране за проектния договор.</span><span class="sxs-lookup"><span data-stu-id="d617f-169">Repeat these steps to create additional billing rules for the project contract.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]