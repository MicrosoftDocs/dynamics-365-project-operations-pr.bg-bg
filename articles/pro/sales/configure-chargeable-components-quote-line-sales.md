---
title: Конфигуриране на платимите компоненти на ред на оферта
description: Тази тема предоставя информация за настройване на таксувани и неначисляеми компоненти на базирана на проект линия за оферти.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 1a9e1851bd8c5a4070df2774c945d1f3eabaaa8a
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858280"
---
# <a name="configure-the-chargeable-components-of-a-quote-line"></a><span data-ttu-id="85912-103">Конфигуриране на платимите компоненти на ред на оферта</span><span class="sxs-lookup"><span data-stu-id="85912-103">Configure the chargeable components of a quote line</span></span> 

<span data-ttu-id="85912-104">_**Отнася се за:** Олекотено внедряване – сделка към проформа фактуриране, Project Operations за сценарии, базирани на ресурси / без складови наличности_</span><span class="sxs-lookup"><span data-stu-id="85912-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="85912-105">Базовата линия на проекта има концепцията за *включени* компоненти и *таксуеми* компоненти.</span><span class="sxs-lookup"><span data-stu-id="85912-105">A project-based quote line has the concept of *included* components and *chargeable* components.</span></span>

<span data-ttu-id="85912-106">Включените компоненти са обект на:</span><span class="sxs-lookup"><span data-stu-id="85912-106">Included components are subject to:</span></span>

  - <span data-ttu-id="85912-107">Метод на фактуриране и разделяне на клиента</span><span class="sxs-lookup"><span data-stu-id="85912-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="85912-108">Ограничения, които да не се надвишават</span><span class="sxs-lookup"><span data-stu-id="85912-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="85912-109">Настройки на честотата на фактурите, дефинирани на базирана на проекта линия за оферти</span><span class="sxs-lookup"><span data-stu-id="85912-109">Invoice frequency settings defined on the project-based quote line</span></span>

<span data-ttu-id="85912-110">Подмножество от включените компоненти може да бъде маркирано като таксувано с помощта на полето **Тип фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="85912-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="85912-111">Полето **Тип фактуриране** е набор от опции, който позволява следните стойности в контекста на кавичка:</span><span class="sxs-lookup"><span data-stu-id="85912-111">The **Billing Type** field is an option-set that allows the following values in the context of a quote line:</span></span>

  - <span data-ttu-id="85912-112">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-112">Chargeable</span></span>
  - <span data-ttu-id="85912-113">Нетаксуеми</span><span class="sxs-lookup"><span data-stu-id="85912-113">Non-chargeable</span></span>

<span data-ttu-id="85912-114">Компонентите, които се заплащат, могат да бъдат дефинирани за задачи, роли и категории транзакции.</span><span class="sxs-lookup"><span data-stu-id="85912-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="85912-115">Плащаемостта се определя в задачите за котировъчен ред и се прилага за всички класове транзакции, включени в този ред.</span><span class="sxs-lookup"><span data-stu-id="85912-115">Chargeability is defined on the tasks for a quote line and applies to all transaction classes included on that line.</span></span> <span data-ttu-id="85912-116">Ако полето **Включете задачи** е зададено на **Цял проект** или оставено празно, разделът **Платими задачи** не е наличен.</span><span class="sxs-lookup"><span data-stu-id="85912-116">If the **Include Tasks** field is set to **Entire project** or left blank, the **Chargeable Tasks** tab isn't available.</span></span>

<span data-ttu-id="85912-117">Плащаемостта се определя в ролите за ред на оферта и се прилага само за класа трансакция **Време**.</span><span class="sxs-lookup"><span data-stu-id="85912-117">Chargeability is defined on roles for a quote line and only applies to the **Time** transaction class.</span></span> <span data-ttu-id="85912-118">Ако полето **Включете време** е зададено на **Не** на ред на оферта по проект разделът **Платими роли** не е наличен.</span><span class="sxs-lookup"><span data-stu-id="85912-118">If the field, **Include Time** is set to **No** on a project quote line, the **Chargeable Roles** tab isn't available.</span></span>

<span data-ttu-id="85912-119">Плащаемостта се определя в категориите трансакция за ред на оферта и се прилага само за класа трансакция **разход**.</span><span class="sxs-lookup"><span data-stu-id="85912-119">Chargeability is defined on transaction categories for a  quote line and only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="85912-120">Ако полето **Включете разходи** е зададено на **Не** на ред на оферта по проект разделът **Платими категории** не е наличен.</span><span class="sxs-lookup"><span data-stu-id="85912-120">If the field, **Include Expenses** is set to **No** on a project quote line, the **Chargeable Categories** tab isn't available.</span></span>

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="85912-121">Актуализирайте проектна задача, за да бъде таксувана или без такса</span><span class="sxs-lookup"><span data-stu-id="85912-121">Update a project task to be chargeable or non-chargeable</span></span>

<span data-ttu-id="85912-122">Проектната задача може да бъде таксувана или без такса в контекста на конкретен проект, базиран на котировка, което прави възможна следната настройка.</span><span class="sxs-lookup"><span data-stu-id="85912-122">A project task can be chargeable or non-chargeable in the context of a specific project-based quote line, which makes the following setup possible.</span></span>

<span data-ttu-id="85912-123">Ако ред на оферта, базиран на проект, включва **Време** и задачата **Т1**, задачата е свързана с ред на оферта като платена.</span><span class="sxs-lookup"><span data-stu-id="85912-123">If a project-based quote line includes **Time** and the task **T1**, the task is associated to the quote line as chargeable.</span></span> <span data-ttu-id="85912-124">Ако има втори ред, който включва **Разходи**, можете да свържете **Т1** задача на ред на оферта като без такса.</span><span class="sxs-lookup"><span data-stu-id="85912-124">If there is a second quote line that includes **Expenses**, you can associate the **T1** task on the quote line as non-chargeable.</span></span> <span data-ttu-id="85912-125">Резултатът е, че цялото време, записано в задачата, се заплаща и всички разходи, записани в задачата, не се заплащат.</span><span class="sxs-lookup"><span data-stu-id="85912-125">The result is that all time recorded on the task is chargeable and all expenses recorded on the task are non-chargeable.</span></span>

<span data-ttu-id="85912-126">Типът фактуриране на задачата може да се конфигурира в раздела **Платими задачи** базиран на проект ред на оферта чрез актуализиране на полето **Тип фактуриране** в подмрежата **Задачи на ред на оферта**.</span><span class="sxs-lookup"><span data-stu-id="85912-126">A task's billing type can be configured on the **Chargeable Tasks** tab of a project-based quote line by updating the **Billing Type** field on the **Quote Line Tasks** subgrid.</span></span> <span data-ttu-id="85912-127">Като алтернатива можете да актуализирате типа фактуриране за задача по проект в полето **Тип фактуриране** в подмрежата на настройката за фактуриране на задача по проект, което показва редовете на офертите, свързани със задача.</span><span class="sxs-lookup"><span data-stu-id="85912-127">Alternatively, you can update the billing type for a project task in the **Billing Type** field on the subgrid on the task billing setup of a project that shows the quote lines associated to a task.</span></span>

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="85912-128">Актуализирайте роля да бъде таксувана или без такса</span><span class="sxs-lookup"><span data-stu-id="85912-128">Update a role to be chargeable or non-chargeable</span></span>

<span data-ttu-id="85912-129">Ролята може да бъде изискуема или без такса в контекста на конкретен проект, базиран на котировка.</span><span class="sxs-lookup"><span data-stu-id="85912-129">A role can be chargeable or non-chargeable in the context of a specific project-based quote line.</span></span>

<span data-ttu-id="85912-130">Типът фактуриране на роля може да се конфигурира в раздела **Платими роли** на ред на оферта чрез актуализиране на полето **Тип фактуриране** в подмрежата **Платими роли**.</span><span class="sxs-lookup"><span data-stu-id="85912-130">A role's billing type can be configured on the **Chargeable Roles** tab of a quote line by updating the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="85912-131">Актуализирайте категорията на трансакция, за да бъде таксувана или без такса</span><span class="sxs-lookup"><span data-stu-id="85912-131">Update a transaction category to be chargeable or non-chargeable</span></span>

<span data-ttu-id="85912-132">Категорията на транзакциите може да бъде изискуема или без такса за определен ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="85912-132">A transaction category can be chargeable or non-chargeable on a specific quote line.</span></span>

<span data-ttu-id="85912-133">Типът фактуриране на трансакция може да се конфигурира в раздела **Платими категории** на ред на оферта чрез актуализиране на полето **Тип фактуриране** в подмрежата **Платими категории**.</span><span class="sxs-lookup"><span data-stu-id="85912-133">A transaction's billing type can be configured on the **Chargeable Categories** tab of a quote line by updating the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="85912-134">Решаване на възможността за фактуриране</span><span class="sxs-lookup"><span data-stu-id="85912-134">Resolve chargeability</span></span>
<span data-ttu-id="85912-135">Прогноза или действителни данни, създадени за време, ще се считат за изискуеми само ако:</span><span class="sxs-lookup"><span data-stu-id="85912-135">An estimate or actual created for time will only be considered chargeable if:</span></span>

   - <span data-ttu-id="85912-136">**Време** е включено в реда на оферта.</span><span class="sxs-lookup"><span data-stu-id="85912-136">**Time** is included on the quote line.</span></span>
   - <span data-ttu-id="85912-137">**Роля** се конфигурира като изискуема в реда на оферта.</span><span class="sxs-lookup"><span data-stu-id="85912-137">**Role** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="85912-138">**Включени задачи** е зададено на **Избрани задачи** в реда на оферта.</span><span class="sxs-lookup"><span data-stu-id="85912-138">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span> 

<span data-ttu-id="85912-139">Ако тези три неща са верни, **задача** също е конфигурирана като платена.</span><span class="sxs-lookup"><span data-stu-id="85912-139">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="85912-140">Прогноза или действително създаден за разход се счита за изискуем само ако:</span><span class="sxs-lookup"><span data-stu-id="85912-140">An estimate or actual created for expense is only considered chargeable if:</span></span> 

   - <span data-ttu-id="85912-141">**Разход** е включено в реда на оферта.</span><span class="sxs-lookup"><span data-stu-id="85912-141">**Expense** is included on the quote line.</span></span>
   - <span data-ttu-id="85912-142">**Категорията на трансакция** се конфигурира като изискуема в реда на оферта.</span><span class="sxs-lookup"><span data-stu-id="85912-142">**Transaction category** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="85912-143">**Включени задачи** е зададено на **Избрани задачи** в реда на оферта.</span><span class="sxs-lookup"><span data-stu-id="85912-143">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="85912-144">Ако тези три неща са верни, **задача** също е конфигурирана като платена.</span><span class="sxs-lookup"><span data-stu-id="85912-144">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="85912-145">Прогноза или действителни данни, създадени за материал, ще се считат за изискуеми само ако:</span><span class="sxs-lookup"><span data-stu-id="85912-145">An estimate or actual created for material will only be considered chargeable if:</span></span>

   - <span data-ttu-id="85912-146">**Материали** е включено в реда на оферта.</span><span class="sxs-lookup"><span data-stu-id="85912-146">**Materials** is included on the quote line.</span></span>
   - <span data-ttu-id="85912-147">**Включени задачи** е зададено на **Избрани задачи** в реда на оферта.</span><span class="sxs-lookup"><span data-stu-id="85912-147">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="85912-148">Ако тези две неща са верни, **задача** също трябва да е конфигурирана като платена.</span><span class="sxs-lookup"><span data-stu-id="85912-148">If these two things are true, the **Task** should also be configured as chargeable.</span></span> 


<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="85912-149">
                    <strong>Включва време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-149">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="85912-150">
                    <strong>Включва разход</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-150">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="85912-151">
                    <strong>Включва материал</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-151">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="85912-152">
                    <strong>Включени задачи</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-152">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="85912-153">
                    <strong>Роля</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-153">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="85912-154">
                    <strong>Категория</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-154">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="85912-155">
                    <strong>Задача</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-155">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="85912-156">
                    <strong>Въздействие на таксуемостта</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-156">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-157">Да</span><span class="sxs-lookup"><span data-stu-id="85912-157">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="85912-158">Да</span><span class="sxs-lookup"><span data-stu-id="85912-158">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="85912-159">Да</span><span class="sxs-lookup"><span data-stu-id="85912-159">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="85912-160">Целият проект</span><span class="sxs-lookup"><span data-stu-id="85912-160">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-161">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-161">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-162">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-162">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-163">Не може да се зададе</span><span class="sxs-lookup"><span data-stu-id="85912-163">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="85912-164">Таксуване по действително време: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-164">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="85912-165">Вид на фактурирането за действителни разходи: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-165">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="85912-166">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-166">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-167">Да</span><span class="sxs-lookup"><span data-stu-id="85912-167">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="85912-168">Да</span><span class="sxs-lookup"><span data-stu-id="85912-168">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="85912-169">Да</span><span class="sxs-lookup"><span data-stu-id="85912-169">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="85912-170">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="85912-170">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-171">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-171">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-172">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-172">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-173">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-173">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="85912-174">Таксуване по действително време: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-174">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="85912-175">Вид на фактурирането за действителни разходи: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-175">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="85912-176">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-176">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-177">Да</span><span class="sxs-lookup"><span data-stu-id="85912-177">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="85912-178">Да</span><span class="sxs-lookup"><span data-stu-id="85912-178">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="85912-179">Да</span><span class="sxs-lookup"><span data-stu-id="85912-179">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="85912-180">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="85912-180">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="85912-181">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-181">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-182">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-182">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-183">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-183">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="85912-184">Таксуване по действително време: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-184">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-185">Вид на фактурирането за действителни разходи: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-185">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="85912-186">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-186">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-187">Да</span><span class="sxs-lookup"><span data-stu-id="85912-187">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="85912-188">Да</span><span class="sxs-lookup"><span data-stu-id="85912-188">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="85912-189">Да</span><span class="sxs-lookup"><span data-stu-id="85912-189">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="85912-190">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="85912-190">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-191">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-191">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-192">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-192">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="85912-193">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-193">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="85912-194">Таксуване по действително време: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-194">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-195">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-195">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-196">Вид на фактурирането за действителни данни за материал: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-196">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-197">Да</span><span class="sxs-lookup"><span data-stu-id="85912-197">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="85912-198">Да</span><span class="sxs-lookup"><span data-stu-id="85912-198">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="85912-199">Да</span><span class="sxs-lookup"><span data-stu-id="85912-199">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="85912-200">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="85912-200">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="85912-201">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-201">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-202">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-202">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="85912-203">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-203">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="85912-204">Таксуване по действително време: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-204">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-205">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-205">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-206">Вид на фактурирането за действителни данни за материал: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-206">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-207">Да</span><span class="sxs-lookup"><span data-stu-id="85912-207">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="85912-208">Да</span><span class="sxs-lookup"><span data-stu-id="85912-208">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="85912-209">Да</span><span class="sxs-lookup"><span data-stu-id="85912-209">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="85912-210">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="85912-210">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="85912-211">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-211">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="85912-212">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-212">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-213">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-213">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="85912-214">Таксуване по действително време: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-214">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-215">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-215">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-216">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-216">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="85912-217">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-217">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="85912-218">Да</span><span class="sxs-lookup"><span data-stu-id="85912-218">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="85912-219">Да</span><span class="sxs-lookup"><span data-stu-id="85912-219">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="85912-220">Целият проект</span><span class="sxs-lookup"><span data-stu-id="85912-220">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-221">Не може да се зададе</span><span class="sxs-lookup"><span data-stu-id="85912-221">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="85912-222">
                    <strong>Платими</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-222">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-223">Не може да се зададе</span><span class="sxs-lookup"><span data-stu-id="85912-223">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="85912-224">Таксуване по действително време: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-224">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-225">Вид на фактурирането за действителни разходи: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-225">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="85912-226">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-226">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="85912-227">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-227">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="85912-228">Да</span><span class="sxs-lookup"><span data-stu-id="85912-228">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="85912-229">Да</span><span class="sxs-lookup"><span data-stu-id="85912-229">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="85912-230">Целият проект</span><span class="sxs-lookup"><span data-stu-id="85912-230">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-231">Не може да се зададе</span><span class="sxs-lookup"><span data-stu-id="85912-231">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="85912-232">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-232">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-233">Не може да се зададе</span><span class="sxs-lookup"><span data-stu-id="85912-233">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="85912-234">Таксуване по действително време: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-234">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-235">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-235">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-236">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-236">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-237">Да</span><span class="sxs-lookup"><span data-stu-id="85912-237">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="85912-238">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-238">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="85912-239">Да</span><span class="sxs-lookup"><span data-stu-id="85912-239">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="85912-240">Целият проект</span><span class="sxs-lookup"><span data-stu-id="85912-240">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-241">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-241">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-242">Не може да се зададе</span><span class="sxs-lookup"><span data-stu-id="85912-242">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-243">Не може да се зададе</span><span class="sxs-lookup"><span data-stu-id="85912-243">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="85912-244">Таксуване по действително време: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-244">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="85912-245">Вид на фактурирането за действителни разходи: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-245">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-246">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-246">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-247">Да</span><span class="sxs-lookup"><span data-stu-id="85912-247">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="85912-248">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-248">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="85912-249">Да</span><span class="sxs-lookup"><span data-stu-id="85912-249">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="85912-250">Целият проект</span><span class="sxs-lookup"><span data-stu-id="85912-250">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="85912-251">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-251">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-252">Не може да се зададе</span><span class="sxs-lookup"><span data-stu-id="85912-252">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-253">Не може да се зададе</span><span class="sxs-lookup"><span data-stu-id="85912-253">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="85912-254">Таксуване по действително време: <strong>Неплатимо </strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-254">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-255">Вид на фактурирането за действителни разходи: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-255">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-256">Вид на фактурирането за действителни данни за материал: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-256">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-257">Да</span><span class="sxs-lookup"><span data-stu-id="85912-257">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="85912-258">Да</span><span class="sxs-lookup"><span data-stu-id="85912-258">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="85912-259">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-259">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="85912-260">Целият проект</span><span class="sxs-lookup"><span data-stu-id="85912-260">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-261">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-261">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-262">Платими</span><span class="sxs-lookup"><span data-stu-id="85912-262">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-263">Не може да се зададе</span><span class="sxs-lookup"><span data-stu-id="85912-263">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="85912-264">Таксуване по действително време: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-264">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="85912-265">Вид на фактурирането за действителни разходи: Платимо</span><span class="sxs-lookup"><span data-stu-id="85912-265">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="85912-266">Вид на фактурирането за действителни данни за материали: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-266">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="85912-267">Да</span><span class="sxs-lookup"><span data-stu-id="85912-267">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="85912-268">Да</span><span class="sxs-lookup"><span data-stu-id="85912-268">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="85912-269">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-269">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="85912-270">Целият проект</span><span class="sxs-lookup"><span data-stu-id="85912-270">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="85912-271">
                    <strong>Нетаксуемо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-271">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="85912-272">
                    <strong>Нетаксуеми</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-272">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="85912-273">Не може да се зададе</span><span class="sxs-lookup"><span data-stu-id="85912-273">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="85912-274">Таксуване по действително време: <strong>Неплатимо </strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-274">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-275">Вид на фактурирането за действителни разходи: <strong>Неплатимо</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-275">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="85912-276">Вид на фактурирането за действителни данни за материали: <strong>Неналично</strong>
                </span><span class="sxs-lookup"><span data-stu-id="85912-276">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]
