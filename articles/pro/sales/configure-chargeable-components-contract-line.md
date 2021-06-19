---
title: Конфигуриране на платими компоненти на базирани на проект аспекти на договор
description: Тази тема предоставя информация за това как да добавите таксуеми компоненти към договорни линии в Project Operations.
author: rumant
ms.date: 10/08/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b29c912828aa4af2d2d9cb47869012087cb834b4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003708"
---
# <a name="configure-chargeable-components-of-a-project-based-contract-line"></a><span data-ttu-id="b51c4-103">Конфигуриране на платими компоненти на базирани на проект аспекти на договор</span><span class="sxs-lookup"><span data-stu-id="b51c4-103">Configure chargeable components of a project-based contract line</span></span>

<span data-ttu-id="b51c4-104">_**Отнася се за:** Олекотено внедряване – сделка към проформа фактуриране, Project Operations за сценарии, базирани на ресурси / без складови наличности_</span><span class="sxs-lookup"><span data-stu-id="b51c4-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="b51c4-105">Базираните на проект аспекти на договор имат *включени* компоненти и *таксуеми* компоненти.</span><span class="sxs-lookup"><span data-stu-id="b51c4-105">A project-based contract line has *included* components and *chargeable* components.</span></span>

<span data-ttu-id="b51c4-106">Включените компоненти са компоненти, които са обект на:</span><span class="sxs-lookup"><span data-stu-id="b51c4-106">Included components are components that are subject to:</span></span>

  - <span data-ttu-id="b51c4-107">Метод на фактуриране и разделяне на клиента</span><span class="sxs-lookup"><span data-stu-id="b51c4-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="b51c4-108">Ограничения, които да не се надвишават</span><span class="sxs-lookup"><span data-stu-id="b51c4-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="b51c4-109">Настройки на честотата на фактурите, дефинирани на базиран на проекта ред на оферта</span><span class="sxs-lookup"><span data-stu-id="b51c4-109">Invoice frequency settings defined on the project-based contract line</span></span>

<span data-ttu-id="b51c4-110">Подмножество от включените компоненти може да бъде маркирано като таксувано с помощта на полето **Тип фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="b51c4-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="b51c4-111">Полето **Тип фактуриране** е набор от опции, който позволява следните стойности в контекста на аспекти на договор:</span><span class="sxs-lookup"><span data-stu-id="b51c4-111">The **Billing Type** field is an option-set that allows the following values in the context of a contract line:</span></span>

  - <span data-ttu-id="b51c4-112">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-112">Chargeable</span></span>
  - <span data-ttu-id="b51c4-113">Нетаксуеми</span><span class="sxs-lookup"><span data-stu-id="b51c4-113">Non-chargeable</span></span>

<span data-ttu-id="b51c4-114">Компонентите, които се заплащат, могат да бъдат дефинирани за задачи, роли и категории транзакции.</span><span class="sxs-lookup"><span data-stu-id="b51c4-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="b51c4-115">Плащаемостта се определя в задачите за аспекти на договор по проект и се прилага за всички класове транзакции, включени в реда.</span><span class="sxs-lookup"><span data-stu-id="b51c4-115">Chargeability is defined on tasks for a project contract line and applies to all transaction classes included on the line.</span></span> <span data-ttu-id="b51c4-116">Ако полето **Включване на задачи** в аспекти на договор е празно или зададено на **Цял проект**, разделът **Платими задачи** няма да е наличен.</span><span class="sxs-lookup"><span data-stu-id="b51c4-116">If the **Include Tasks** field on a contract line is blank or set to **Entire project**, the **Chargeable tasks** tab will not be available.</span></span>

<span data-ttu-id="b51c4-117">Плащаемостта се определя в ролите за аспекти на договор по проект и се прилага само за класа трансакция **Време**.</span><span class="sxs-lookup"><span data-stu-id="b51c4-117">Chargeability defined on roles for a project contract line only applies to the **Time** transaction class.</span></span> <span data-ttu-id="b51c4-118">Ако полето на аспекти на договор **Включете време** е зададено на **Не**, разделът **Платими роли** не е наличен.</span><span class="sxs-lookup"><span data-stu-id="b51c4-118">If the **Include Time** field on a contract line is set to **No**, the **Chargeable roles** tab will not be available.</span></span>

<span data-ttu-id="b51c4-119">Плащаемостта се определя в категориите трансакция за аспекти на договор по проект и се прилага само за класа трансакция **разход**.</span><span class="sxs-lookup"><span data-stu-id="b51c4-119">Chargeability defined on transaction categories for a project contract line only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="b51c4-120">Ако полето на аспекти на договор **Включете разход** е зададено на **Не**, разделът **Платими категории** не е наличен.</span><span class="sxs-lookup"><span data-stu-id="b51c4-120">If the **Include Expenses** field is set to **No**, the **Chargeable Categories** tab will not be available.</span></span>

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a><span data-ttu-id="b51c4-121">Актуализирайте проектна задача, за да бъде таксувана или без такса</span><span class="sxs-lookup"><span data-stu-id="b51c4-121">Update a project task as chargeable or non-chargeable</span></span>

<span data-ttu-id="b51c4-122">Проектната задача може да бъде таксувана или без такса на специфични аспекти на договор, което прави възможна следната настройка:</span><span class="sxs-lookup"><span data-stu-id="b51c4-122">A project task can be chargeable or non-chargeable on a specific contract line, which makes the following setup possible:</span></span>

<span data-ttu-id="b51c4-123">Ако договорната линия, базирана на проект, включва **Време** и определена задача, **Т1** е свързано с него като изискуемо.</span><span class="sxs-lookup"><span data-stu-id="b51c4-123">If a project-based contract line includes **Time** and a certain task, **T1** is associated to it as chargeable.</span></span> <span data-ttu-id="b51c4-124">Ако има втори ред на договор, който включва **Разходи**, можете да свържете Т1 задача на ред на договор като без такса.</span><span class="sxs-lookup"><span data-stu-id="b51c4-124">If there is a second contract line that includes **Expense**, you can associate the T1 task on the contract line as non-chargeable.</span></span> <span data-ttu-id="b51c4-125">Резултатът е, че цялото време, записано в задачата, се заплаща и всички разходи не се заплащат.</span><span class="sxs-lookup"><span data-stu-id="b51c4-125">The result is that all of the time recorded on the task is chargeable and all expenses are non-chargeable.</span></span>

<span data-ttu-id="b51c4-126">Типът фактуриране на задачата може да се конфигурира в раздела **Платими задачи** в аспектите на договора чрез актуализиране на полето **Тип фактуриране** в подмрежата за задачи на аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="b51c4-126">A task's billing type can be configured on the **Chargeable Tasks** tab of the contract line by updating the **Billing Type** field on the contract line tasks subgrid.</span></span> <span data-ttu-id="b51c4-127">Като алтернатива можете да актуализирате полето **Тип фактуриране** в подмрежата на настройката за фактуриране на задача по проект, което показва аспектите на договора, свързани със задача.</span><span class="sxs-lookup"><span data-stu-id="b51c4-127">Alternatively, you can update the **Billing Type** field on the subgrid of the task Billing setup of a project that shows the contract lines associated to a task.</span></span>

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a><span data-ttu-id="b51c4-128">Актуализирайте роля да бъде таксувана или без такса</span><span class="sxs-lookup"><span data-stu-id="b51c4-128">Update a role as chargeable or non-chargeable</span></span>

<span data-ttu-id="b51c4-129">Роля може да бъде изискуема или без такса за определен ред на договор.</span><span class="sxs-lookup"><span data-stu-id="b51c4-129">A role can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="b51c4-130">Типът таксуване на роля може да бъде конфигуриран на раздела **Платими роли** на договорна линия.</span><span class="sxs-lookup"><span data-stu-id="b51c4-130">A role's billing type can be configured on the **Chargeable Roles** tab of a contract line.</span></span> <span data-ttu-id="b51c4-131">За да направите това, актуализирайте полето **Тип фактуриране** в подмрежата **Платими роли**.</span><span class="sxs-lookup"><span data-stu-id="b51c4-131">To do this, update the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a><span data-ttu-id="b51c4-132">Актуализирайте категорията на трансакция, за да бъде таксувана или без такса</span><span class="sxs-lookup"><span data-stu-id="b51c4-132">Update a transaction category as chargeable or non-chargeable</span></span>

<span data-ttu-id="b51c4-133">Категорията на транзакциите може да бъде изискуема или без такса за определен ред на договор.</span><span class="sxs-lookup"><span data-stu-id="b51c4-133">A transaction category can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="b51c4-134">Типът таксуване на трансакция може да бъде конфигуриран на раздела **Платими категории** на базиран на проект ред на договор.</span><span class="sxs-lookup"><span data-stu-id="b51c4-134">A transaction's billing type can be configured on the **Chargeable Categories** tab of a project-based contract line.</span></span> <span data-ttu-id="b51c4-135">За да направите това, актуализирайте полето **Тип фактуриране** в подмрежата **Платими категории**.</span><span class="sxs-lookup"><span data-stu-id="b51c4-135">To do this, update the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="b51c4-136">Решаване на възможността за фактуриране</span><span class="sxs-lookup"><span data-stu-id="b51c4-136">Resolve chargeability</span></span>

<span data-ttu-id="b51c4-137">Прогноза или действително създаден за времето се счита за изискуем само ако:</span><span class="sxs-lookup"><span data-stu-id="b51c4-137">An estimate or actual created for time is only considered chargeable if:</span></span>

   - <span data-ttu-id="b51c4-138">**Време** е включено в аспектите на договор.</span><span class="sxs-lookup"><span data-stu-id="b51c4-138">**Time** is included on the contract line.</span></span>
   - <span data-ttu-id="b51c4-139">**Роля** се конфигурира като изискуема в аспектите на договор.</span><span class="sxs-lookup"><span data-stu-id="b51c4-139">**Role** is configured as chargeable on the contract line.</span></span>
   - <span data-ttu-id="b51c4-140">**Включени задачи** е зададено на **Избрани задачи** на аспектите на договор.</span><span class="sxs-lookup"><span data-stu-id="b51c4-140">**Included Tasks** is set to **Selected tasks** on the contract line.</span></span>
 
 <span data-ttu-id="b51c4-141">Ако тези три неща са верни, задачата е конфигурирана като платена.</span><span class="sxs-lookup"><span data-stu-id="b51c4-141">If these three things are true, the task is configured as chargeable.</span></span> 

<span data-ttu-id="b51c4-142">Прогноза или действително създаден за разход се счита за изискуем само ако:</span><span class="sxs-lookup"><span data-stu-id="b51c4-142">An estimate or actual created for expense is only considered chargeable if:</span></span>

   - <span data-ttu-id="b51c4-143">**Разход** е включен в аспектите на договор</span><span class="sxs-lookup"><span data-stu-id="b51c4-143">**Expense** is included on the contract line</span></span>
   - <span data-ttu-id="b51c4-144">**Категорията на трансакция** се конфигурира като изискуема в аспектите на договор</span><span class="sxs-lookup"><span data-stu-id="b51c4-144">**Transaction category** is configured as chargeable on the contract line</span></span>
   - <span data-ttu-id="b51c4-145">**Включени задачи** е зададено на **Избрани задачи** на аспектите на договор</span><span class="sxs-lookup"><span data-stu-id="b51c4-145">**Included Tasks** is set to **Selected task** on the contract line</span></span>
  
 <span data-ttu-id="b51c4-146">Ако тези три неща са верни, **задача** е конфигурирана като платена.</span><span class="sxs-lookup"><span data-stu-id="b51c4-146">If these three things are true, the **Task** is configured as chargeable.</span></span> 

<span data-ttu-id="b51c4-147">Прогноза или действително създаден за материал се счита за изискуем само ако:</span><span class="sxs-lookup"><span data-stu-id="b51c4-147">An estimate or actual created for material is only considered chargeable if:</span></span>

   - <span data-ttu-id="b51c4-148">**Материали** е включено в аспектите на договор</span><span class="sxs-lookup"><span data-stu-id="b51c4-148">**Materials** is included on the contract line</span></span>
   - <span data-ttu-id="b51c4-149">**Включени задачи** е зададено на **Избрани задачи** на аспектите на договор</span><span class="sxs-lookup"><span data-stu-id="b51c4-149">**Included Tasks** is set to **Selected tasks** on the contract line</span></span>

<span data-ttu-id="b51c4-150">Ако тези две неща са верни, **задача** е конфигурирана като платена.</span><span class="sxs-lookup"><span data-stu-id="b51c4-150">If these two things are true, the **Task** is configured as chargeable.</span></span> 

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="b51c4-151">
                    <strong>Включва време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-151">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="b51c4-152">
                    <strong>Включва разход</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-152">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="b51c4-153">
                    <strong>Включва материал</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-153">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="b51c4-154">
                    <strong>Включени задачи</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-154">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b51c4-155">
                    <strong>Роля</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-155">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="b51c4-156">
                    <strong>Категория</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-156">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b51c4-157">
                    <strong>Задача</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-157">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="b51c4-158">
                    <strong>Въздействие на таксуемостта</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-158">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-159">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-159">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b51c4-160">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-160">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b51c4-161">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-161">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b51c4-162">Целият проект</span><span class="sxs-lookup"><span data-stu-id="b51c4-162">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-163">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-163">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-164">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-164">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-165">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="b51c4-165">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b51c4-166">Таксуване по действително време: <strong>Платимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-166">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-167">Вид на фактурирането за действителни разходи: <strong>Платимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-167">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-168">Вид на фактурирането за действителни данни за материал: <strong>Платимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-168">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-169">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-169">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b51c4-170">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-170">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b51c4-171">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-171">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b51c4-172">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="b51c4-172">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-173">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-173">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-174">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-174">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-175">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-175">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b51c4-176">Таксуване по действително време: <strong>Платимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-176">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-177">Вид на фактурирането за действителни разходи: <strong>Платимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-177">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-178">Вид на фактурирането за действителни данни за материал: <strong>Платимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-178">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-179">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-179">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b51c4-180">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-180">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b51c4-181">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-181">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b51c4-182">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="b51c4-182">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b51c4-183">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-183">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-184">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-184">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-185">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-185">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b51c4-186">Таксуване по действително време: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-186">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-187">Вид на фактурирането за действителни разходи: Платимо</span><span class="sxs-lookup"><span data-stu-id="b51c4-187">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b51c4-188">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="b51c4-188">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-189">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-189">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b51c4-190">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-190">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b51c4-191">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-191">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b51c4-192">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="b51c4-192">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-193">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-193">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-194">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-194">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b51c4-195">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-195">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b51c4-196">Таксуване по действително време: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-196">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-197">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-197">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-198">Вид на фактурирането за действителни данни за материал: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-198">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-199">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-199">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b51c4-200">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-200">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b51c4-201">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-201">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b51c4-202">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="b51c4-202">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b51c4-203">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-203">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-204">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-204">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b51c4-205">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-205">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b51c4-206">Таксуване по действително време: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-206">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-207">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-207">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-208">Вид на фактурирането за действителни данни за материал: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-208">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-209">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-209">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b51c4-210">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-210">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b51c4-211">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-211">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b51c4-212">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="b51c4-212">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b51c4-213">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-213">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="b51c4-214">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-214">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-215">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-215">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b51c4-216">Таксуване по действително време: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-216">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-217">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-217">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-218">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="b51c4-218">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="b51c4-219">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-219">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b51c4-220">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-220">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b51c4-221">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-221">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b51c4-222">Целият проект</span><span class="sxs-lookup"><span data-stu-id="b51c4-222">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-223">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="b51c4-223">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="b51c4-224">
                    <strong>Платими</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-224">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-225">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="b51c4-225">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b51c4-226">Таксуване по действително време: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-226">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-227">Вид на фактурирането за действителни разходи: Платимо</span><span class="sxs-lookup"><span data-stu-id="b51c4-227">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b51c4-228">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="b51c4-228">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="b51c4-229">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-229">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b51c4-230">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-230">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b51c4-231">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-231">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b51c4-232">Целият проект</span><span class="sxs-lookup"><span data-stu-id="b51c4-232">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-233">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="b51c4-233">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="b51c4-234">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-234">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-235">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="b51c4-235">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b51c4-236">Таксуване по действително време: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-236">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-237">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-237">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-238">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="b51c4-238">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-239">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-239">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="b51c4-240">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-240">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b51c4-241">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-241">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b51c4-242">Целият проект</span><span class="sxs-lookup"><span data-stu-id="b51c4-242">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-243">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-243">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-244">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="b51c4-244">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-245">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="b51c4-245">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b51c4-246">Таксуване по действително време: Платимо</span><span class="sxs-lookup"><span data-stu-id="b51c4-246">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b51c4-247">Вид на фактурирането за действителни разходи: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-247">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-248">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="b51c4-248">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-249">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-249">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="b51c4-250">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-250">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b51c4-251">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-251">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b51c4-252">Целият проект</span><span class="sxs-lookup"><span data-stu-id="b51c4-252">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b51c4-253">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-253">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-254">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="b51c4-254">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-255">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="b51c4-255">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b51c4-256">Таксуване по действително време: <strong>Неплатимо </strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-256">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-257">Вид на фактурирането за действителни разходи: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-257">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-258">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="b51c4-258">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-259">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-259">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b51c4-260">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-260">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="b51c4-261">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-261">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b51c4-262">Целият проект</span><span class="sxs-lookup"><span data-stu-id="b51c4-262">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-263">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-263">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-264">Платими</span><span class="sxs-lookup"><span data-stu-id="b51c4-264">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-265">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="b51c4-265">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b51c4-266">Таксуване по действително време: Платимо</span><span class="sxs-lookup"><span data-stu-id="b51c4-266">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b51c4-267">Вид на фактурирането за действителни разходи: Платимо</span><span class="sxs-lookup"><span data-stu-id="b51c4-267">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b51c4-268">Вид на фактурирането за действителни данни за материали: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-268">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b51c4-269">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-269">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b51c4-270">Да</span><span class="sxs-lookup"><span data-stu-id="b51c4-270">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="b51c4-271">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-271">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b51c4-272">Целият проект</span><span class="sxs-lookup"><span data-stu-id="b51c4-272">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b51c4-273">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-273">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="b51c4-274">
                    <strong>Нетаксуеми</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-274">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b51c4-275">Не може да бъде зададено</span><span class="sxs-lookup"><span data-stu-id="b51c4-275">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b51c4-276">Таксуване по действително време: <strong>Неплатимо </strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-276">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-277">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-277">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="b51c4-278">Вид на фактурирането за действителни данни за материали: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b51c4-278">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>





[!INCLUDE[footer-include](../../includes/footer-banner.md)]
