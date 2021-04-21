---
title: Конфигуриране на платими компоненти на базирани на проект аспекти на договор
description: Тази тема предоставя информация за това как да добавите таксуеми компоненти към договорни линии в Project Operations.
author: rumant
manager: Annbe
ms.date: 10/08/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ddada2cb412ba7370fb0a750325a84772937d8d0
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858460"
---
# <a name="configure-chargeable-components-of-a-project-based-contract-line"></a><span data-ttu-id="0442a-103">Конфигуриране на платими компоненти на базирани на проект аспекти на договор</span><span class="sxs-lookup"><span data-stu-id="0442a-103">Configure chargeable components of a project-based contract line</span></span>

<span data-ttu-id="0442a-104">_**Отнася се за:** Олекотено внедряване – сделка към проформа фактуриране, Project Operations за сценарии, базирани на ресурси / без складови наличности_</span><span class="sxs-lookup"><span data-stu-id="0442a-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="0442a-105">Базираните на проект аспекти на договор имат *включени* компоненти и *таксуеми* компоненти.</span><span class="sxs-lookup"><span data-stu-id="0442a-105">A project-based contract line has *included* components and *chargeable* components.</span></span>

<span data-ttu-id="0442a-106">Включените компоненти са компоненти, които са обект на:</span><span class="sxs-lookup"><span data-stu-id="0442a-106">Included components are components that are subject to:</span></span>

  - <span data-ttu-id="0442a-107">Метод на фактуриране и разделяне на клиента</span><span class="sxs-lookup"><span data-stu-id="0442a-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="0442a-108">Ограничения, които да не се надвишават</span><span class="sxs-lookup"><span data-stu-id="0442a-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="0442a-109">Настройки на честотата на фактурите, дефинирани на базиран на проекта ред на оферта</span><span class="sxs-lookup"><span data-stu-id="0442a-109">Invoice frequency settings defined on the project-based contract line</span></span>

<span data-ttu-id="0442a-110">Подмножество от включените компоненти може да бъде маркирано като таксувано с помощта на полето **Тип фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="0442a-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="0442a-111">Полето **Тип фактуриране** е набор от опции, който позволява следните стойности в контекста на аспекти на договор:</span><span class="sxs-lookup"><span data-stu-id="0442a-111">The **Billing Type** field is an option-set that allows the following values in the context of a contract line:</span></span>

  - <span data-ttu-id="0442a-112">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-112">Chargeable</span></span>
  - <span data-ttu-id="0442a-113">Нетаксуеми</span><span class="sxs-lookup"><span data-stu-id="0442a-113">Non-chargeable</span></span>

<span data-ttu-id="0442a-114">Компонентите, които се заплащат, могат да бъдат дефинирани за задачи, роли и категории транзакции.</span><span class="sxs-lookup"><span data-stu-id="0442a-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="0442a-115">Плащаемостта се определя в задачите за аспекти на договор по проект и се прилага за всички класове транзакции, включени в реда.</span><span class="sxs-lookup"><span data-stu-id="0442a-115">Chargeability is defined on tasks for a project contract line and applies to all transaction classes included on the line.</span></span> <span data-ttu-id="0442a-116">Ако полето **Включване на задачи** в аспекти на договор е празно или зададено на **Цял проект**, разделът **Платими задачи** няма да е наличен.</span><span class="sxs-lookup"><span data-stu-id="0442a-116">If the **Include Tasks** field on a contract line is blank or set to **Entire project**, the **Chargeable tasks** tab will not be available.</span></span>

<span data-ttu-id="0442a-117">Плащаемостта се определя в ролите за аспекти на договор по проект и се прилага само за класа трансакция **Време**.</span><span class="sxs-lookup"><span data-stu-id="0442a-117">Chargeability defined on roles for a project contract line only applies to the **Time** transaction class.</span></span> <span data-ttu-id="0442a-118">Ако полето на аспекти на договор **Включете време** е зададено на **Не**, разделът **Платими роли** не е наличен.</span><span class="sxs-lookup"><span data-stu-id="0442a-118">If the **Include Time** field on a contract line is set to **No**, the **Chargeable roles** tab will not be available.</span></span>

<span data-ttu-id="0442a-119">Плащаемостта се определя в категориите трансакция за аспекти на договор по проект и се прилага само за класа трансакция **разход**.</span><span class="sxs-lookup"><span data-stu-id="0442a-119">Chargeability defined on transaction categories for a project contract line only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="0442a-120">Ако полето на аспекти на договор **Включете разход** е зададено на **Не**, разделът **Платими категории** не е наличен.</span><span class="sxs-lookup"><span data-stu-id="0442a-120">If the **Include Expenses** field is set to **No**, the **Chargeable Categories** tab will not be available.</span></span>

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a><span data-ttu-id="0442a-121">Актуализирайте проектна задача, за да бъде таксувана или без такса</span><span class="sxs-lookup"><span data-stu-id="0442a-121">Update a project task as chargeable or non-chargeable</span></span>

<span data-ttu-id="0442a-122">Проектната задача може да бъде таксувана или без такса на специфични аспекти на договор, което прави възможна следната настройка:</span><span class="sxs-lookup"><span data-stu-id="0442a-122">A project task can be chargeable or non-chargeable on a specific contract line, which makes the following setup possible:</span></span>

<span data-ttu-id="0442a-123">Ако договорната линия, базирана на проект, включва **Време** и определена задача, **Т1** е свързано с него като изискуемо.</span><span class="sxs-lookup"><span data-stu-id="0442a-123">If a project-based contract line includes **Time** and a certain task, **T1** is associated to it as chargeable.</span></span> <span data-ttu-id="0442a-124">Ако има втори ред на договор, който включва **Разходи**, можете да свържете Т1 задача на ред на договор като без такса.</span><span class="sxs-lookup"><span data-stu-id="0442a-124">If there is a second contract line that includes **Expense**, you can associate the T1 task on the contract line as non-chargeable.</span></span> <span data-ttu-id="0442a-125">Резултатът е, че цялото време, записано в задачата, се заплаща и всички разходи не се заплащат.</span><span class="sxs-lookup"><span data-stu-id="0442a-125">The result is that all of the time recorded on the task is chargeable and all expenses are non-chargeable.</span></span>

<span data-ttu-id="0442a-126">Типът фактуриране на задачата може да се конфигурира в раздела **Платими задачи** в аспектите на договора чрез актуализиране на полето **Тип фактуриране** в подмрежата за задачи на аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="0442a-126">A task's billing type can be configured on the **Chargeable Tasks** tab of the contract line by updating the **Billing Type** field on the contract line tasks subgrid.</span></span> <span data-ttu-id="0442a-127">Като алтернатива можете да актуализирате полето **Тип фактуриране** в подмрежата на настройката за фактуриране на задача по проект, което показва аспектите на договора, свързани със задача.</span><span class="sxs-lookup"><span data-stu-id="0442a-127">Alternatively, you can update the **Billing Type** field on the subgrid of the task Billing setup of a project that shows the contract lines associated to a task.</span></span>

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a><span data-ttu-id="0442a-128">Актуализирайте роля да бъде таксувана или без такса</span><span class="sxs-lookup"><span data-stu-id="0442a-128">Update a role as chargeable or non-chargeable</span></span>

<span data-ttu-id="0442a-129">Роля може да бъде изискуема или без такса за определен ред на договор.</span><span class="sxs-lookup"><span data-stu-id="0442a-129">A role can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="0442a-130">Типът таксуване на роля може да бъде конфигуриран на раздела **Платими роли** на договорна линия.</span><span class="sxs-lookup"><span data-stu-id="0442a-130">A role's billing type can be configured on the **Chargeable Roles** tab of a contract line.</span></span> <span data-ttu-id="0442a-131">За да направите това, актуализирайте полето **Тип фактуриране** в подмрежата **Платими роли**.</span><span class="sxs-lookup"><span data-stu-id="0442a-131">To do this, update the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a><span data-ttu-id="0442a-132">Актуализирайте категорията на трансакция, за да бъде таксувана или без такса</span><span class="sxs-lookup"><span data-stu-id="0442a-132">Update a transaction category as chargeable or non-chargeable</span></span>

<span data-ttu-id="0442a-133">Категорията на транзакциите може да бъде изискуема или без такса за определен ред на договор.</span><span class="sxs-lookup"><span data-stu-id="0442a-133">A transaction category can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="0442a-134">Типът таксуване на трансакция може да бъде конфигуриран на раздела **Платими категории** на базиран на проект ред на договор.</span><span class="sxs-lookup"><span data-stu-id="0442a-134">A transaction's billing type can be configured on the **Chargeable Categories** tab of a project-based contract line.</span></span> <span data-ttu-id="0442a-135">За да направите това, актуализирайте полето **Тип фактуриране** в подмрежата **Платими категории**.</span><span class="sxs-lookup"><span data-stu-id="0442a-135">To do this, update the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="0442a-136">Решаване на възможността за фактуриране</span><span class="sxs-lookup"><span data-stu-id="0442a-136">Resolve chargeability</span></span>

<span data-ttu-id="0442a-137">Прогноза или действително създаден за времето се счита за изискуем само ако:</span><span class="sxs-lookup"><span data-stu-id="0442a-137">An estimate or actual created for time is only considered chargeable if:</span></span>

   - <span data-ttu-id="0442a-138">**Време** е включено в аспектите на договор.</span><span class="sxs-lookup"><span data-stu-id="0442a-138">**Time** is included on the contract line.</span></span>
   - <span data-ttu-id="0442a-139">**Роля** се конфигурира като изискуема в аспектите на договор.</span><span class="sxs-lookup"><span data-stu-id="0442a-139">**Role** is configured as chargeable on the contract line.</span></span>
   - <span data-ttu-id="0442a-140">**Включени задачи** е зададено на **Избрани задачи** на аспектите на договор.</span><span class="sxs-lookup"><span data-stu-id="0442a-140">**Included Tasks** is set to **Selected tasks** on the contract line.</span></span>
 
 <span data-ttu-id="0442a-141">Ако тези три неща са верни, задачата е конфигурирана като платена.</span><span class="sxs-lookup"><span data-stu-id="0442a-141">If these three things are true, the task is configured as chargeable.</span></span> 

<span data-ttu-id="0442a-142">Прогноза или действително създаден за разход се счита за изискуем само ако:</span><span class="sxs-lookup"><span data-stu-id="0442a-142">An estimate or actual created for expense is only considered chargeable if:</span></span>

   - <span data-ttu-id="0442a-143">**Разход** е включен в аспектите на договор</span><span class="sxs-lookup"><span data-stu-id="0442a-143">**Expense** is included on the contract line</span></span>
   - <span data-ttu-id="0442a-144">**Категорията на трансакция** се конфигурира като изискуема в аспектите на договор</span><span class="sxs-lookup"><span data-stu-id="0442a-144">**Transaction category** is configured as chargeable on the contract line</span></span>
   - <span data-ttu-id="0442a-145">**Включени задачи** е зададено на **Избрани задачи** на аспектите на договор</span><span class="sxs-lookup"><span data-stu-id="0442a-145">**Included Tasks** is set to **Selected task** on the contract line</span></span>
  
 <span data-ttu-id="0442a-146">Ако тези три неща са верни, **задача** е конфигурирана като платена.</span><span class="sxs-lookup"><span data-stu-id="0442a-146">If these three things are true, the **Task** is configured as chargeable.</span></span> 

<span data-ttu-id="0442a-147">Прогноза или действително създаден за материал се счита за изискуем само ако:</span><span class="sxs-lookup"><span data-stu-id="0442a-147">An estimate or actual created for material is only considered chargeable if:</span></span>

   - <span data-ttu-id="0442a-148">**Материали** е включено в аспектите на договор</span><span class="sxs-lookup"><span data-stu-id="0442a-148">**Materials** is included on the contract line</span></span>
   - <span data-ttu-id="0442a-149">**Включени задачи** е зададено на **Избрани задачи** на аспектите на договор</span><span class="sxs-lookup"><span data-stu-id="0442a-149">**Included Tasks** is set to **Selected tasks** on the contract line</span></span>

<span data-ttu-id="0442a-150">Ако тези две неща са верни, **задача** е конфигурирана като платена.</span><span class="sxs-lookup"><span data-stu-id="0442a-150">If these two things are true, the **Task** is configured as chargeable.</span></span> 

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="0442a-151">
                    <strong>Включва време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-151">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="0442a-152">
                    <strong>Включва разход</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-152">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="0442a-153">
                    <strong>Включва материал</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-153">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="0442a-154">
                    <strong>Включени задачи</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-154">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="0442a-155">
                    <strong>Роля</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-155">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="0442a-156">
                    <strong>Категория</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-156">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="0442a-157">
                    <strong>Задача</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-157">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="0442a-158">
                    <strong>Въздействие на таксуемостта</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-158">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-159">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-159">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="0442a-160">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-160">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="0442a-161">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-161">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="0442a-162">Целият проект</span><span class="sxs-lookup"><span data-stu-id="0442a-162">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-163">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-163">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-164">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-164">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-165">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="0442a-165">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="0442a-166">Таксуване по действително време: <strong>Платимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-166">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-167">Вид на фактурирането за действителни разходи: <strong>Платимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-167">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-168">Вид на фактурирането за действителни данни за материал: <strong>Платимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-168">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-169">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-169">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="0442a-170">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-170">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="0442a-171">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-171">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="0442a-172">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="0442a-172">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-173">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-173">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-174">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-174">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-175">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-175">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="0442a-176">Таксуване по действително време: <strong>Платимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-176">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-177">Вид на фактурирането за действителни разходи: <strong>Платимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-177">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-178">Вид на фактурирането за действителни данни за материал: <strong>Платимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-178">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-179">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-179">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="0442a-180">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-180">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="0442a-181">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-181">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="0442a-182">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="0442a-182">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="0442a-183">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-183">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-184">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-184">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-185">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-185">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="0442a-186">Таксуване по действително време: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-186">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-187">Вид на фактурирането за действителни разходи: Платимо</span><span class="sxs-lookup"><span data-stu-id="0442a-187">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="0442a-188">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="0442a-188">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-189">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-189">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="0442a-190">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-190">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="0442a-191">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-191">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="0442a-192">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="0442a-192">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-193">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-193">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-194">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-194">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="0442a-195">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-195">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="0442a-196">Таксуване по действително време: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-196">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-197">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-197">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-198">Вид на фактурирането за действителни данни за материал: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-198">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-199">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-199">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="0442a-200">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-200">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="0442a-201">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-201">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="0442a-202">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="0442a-202">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="0442a-203">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-203">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-204">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-204">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="0442a-205">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-205">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="0442a-206">Таксуване по действително време: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-206">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-207">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-207">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-208">Вид на фактурирането за действителни данни за материал: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-208">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-209">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-209">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="0442a-210">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-210">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="0442a-211">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-211">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="0442a-212">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="0442a-212">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="0442a-213">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-213">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="0442a-214">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-214">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-215">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-215">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="0442a-216">Таксуване по действително време: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-216">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-217">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-217">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-218">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="0442a-218">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="0442a-219">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-219">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="0442a-220">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-220">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="0442a-221">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-221">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="0442a-222">Целият проект</span><span class="sxs-lookup"><span data-stu-id="0442a-222">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-223">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="0442a-223">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="0442a-224">
                    <strong>Платими</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-224">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-225">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="0442a-225">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="0442a-226">Таксуване по действително време: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-226">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-227">Вид на фактурирането за действителни разходи: Платимо</span><span class="sxs-lookup"><span data-stu-id="0442a-227">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="0442a-228">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="0442a-228">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="0442a-229">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-229">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="0442a-230">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-230">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="0442a-231">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-231">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="0442a-232">Целият проект</span><span class="sxs-lookup"><span data-stu-id="0442a-232">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-233">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="0442a-233">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="0442a-234">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-234">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-235">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="0442a-235">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="0442a-236">Таксуване по действително време: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-236">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-237">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-237">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-238">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="0442a-238">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-239">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-239">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="0442a-240">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-240">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="0442a-241">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-241">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="0442a-242">Целият проект</span><span class="sxs-lookup"><span data-stu-id="0442a-242">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-243">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-243">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-244">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="0442a-244">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-245">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="0442a-245">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="0442a-246">Таксуване по действително време: Платимо</span><span class="sxs-lookup"><span data-stu-id="0442a-246">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="0442a-247">Вид на фактурирането за действителни разходи: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-247">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-248">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="0442a-248">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-249">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-249">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="0442a-250">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-250">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="0442a-251">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-251">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="0442a-252">Целият проект</span><span class="sxs-lookup"><span data-stu-id="0442a-252">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="0442a-253">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-253">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-254">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="0442a-254">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-255">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="0442a-255">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="0442a-256">Таксуване по действително време: <strong>Неплатимо </strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-256">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-257">Вид на фактурирането за действителни разходи: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-257">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-258">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="0442a-258">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-259">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-259">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="0442a-260">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-260">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="0442a-261">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-261">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="0442a-262">Целият проект</span><span class="sxs-lookup"><span data-stu-id="0442a-262">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-263">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-263">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-264">Платими</span><span class="sxs-lookup"><span data-stu-id="0442a-264">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-265">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="0442a-265">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="0442a-266">Таксуване по действително време: Платимо</span><span class="sxs-lookup"><span data-stu-id="0442a-266">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="0442a-267">Вид на фактурирането за действителни разходи: Платимо</span><span class="sxs-lookup"><span data-stu-id="0442a-267">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="0442a-268">Вид на фактурирането за действителни данни за материали: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-268">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="0442a-269">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-269">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="0442a-270">Да</span><span class="sxs-lookup"><span data-stu-id="0442a-270">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="0442a-271">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-271">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="0442a-272">Целият проект</span><span class="sxs-lookup"><span data-stu-id="0442a-272">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="0442a-273">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-273">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="0442a-274">
                    <strong>Нетаксуеми</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-274">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="0442a-275">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="0442a-275">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="0442a-276">Таксуване по действително време: <strong>Неплатимо </strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-276">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-277">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-277">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="0442a-278">Вид на фактурирането за действителни данни за материали: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0442a-278">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>





[!INCLUDE[footer-include](../../includes/footer-banner.md)]
