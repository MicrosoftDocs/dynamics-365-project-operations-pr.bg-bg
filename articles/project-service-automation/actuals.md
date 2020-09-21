---
title: Действителни данни
description: Тази тема предоставя информация за действителни данни на проекта.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 44c6e85f-5b21-4e24-999c-15a2f065d977
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8291e0eb8531e8e9690368675f333c44b6e92e48
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749347"
---
# <a name="actuals"></a><span data-ttu-id="29c9a-103">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="29c9a-103">Actuals</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="29c9a-104">Действителните данни са количеството работа, завършена по даден проект.</span><span class="sxs-lookup"><span data-stu-id="29c9a-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="29c9a-105">Действителните данни на проекта могат да бъдат проследени обратно до техните изходни документи.</span><span class="sxs-lookup"><span data-stu-id="29c9a-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="29c9a-106">Тези изходни документи включват време, разходи и записи в счетоводния регистър, а също и фактури.</span><span class="sxs-lookup"><span data-stu-id="29c9a-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![Как се проследяват действителните данни на проекта до изходните документи](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="29c9a-108">Подаване на запис за време</span><span class="sxs-lookup"><span data-stu-id="29c9a-108">Submitting a time entry</span></span>

<span data-ttu-id="29c9a-109">В PSA при подаване на запис за време за проект, който се съпоставя с ред на договор от тип време и материали, се създават два счетоводни записа.</span><span class="sxs-lookup"><span data-stu-id="29c9a-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="29c9a-110">Единият запис е за разходи, а другият запис е за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="29c9a-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="29c9a-111">При подаване на запис за време за проект, който се съпоставя с ред на договор от тип с фиксирана цена, се създава счетоводен запис само за разходи.</span><span class="sxs-lookup"><span data-stu-id="29c9a-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="29c9a-112">Логиката за въвеждане на цени по подразбиране се намира в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="29c9a-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="29c9a-113">Всички стойности на полета от запис за време се копират в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="29c9a-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="29c9a-114">Тези полета включват датата на транзакцията, реда на договора, с който е съпоставен проектът, и резултата от валутата в съответната ценова листа.</span><span class="sxs-lookup"><span data-stu-id="29c9a-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="29c9a-115">Полетата, които влияят на цените по подразбиране, като например **Роля** и **Организационна единица**, водят до въвеждане на съответна цена по подразбиране в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="29c9a-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="29c9a-116">Ако добавите персонализирано поле в записа за време и искате стойността на полето да се попълни в действителните данни, създайте полето в обекта „Действителни данни“ и използвайте съпоставяния на полета, за да копирате полето от записа за време в действителните данни.</span><span class="sxs-lookup"><span data-stu-id="29c9a-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="29c9a-117">Подаване на запис за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-117">Submitting an expense entry</span></span>

<span data-ttu-id="29c9a-118">В PSA при подаване на запис за разходи за проект, който се съпоставя с ред на договор от тип време и материали, се създават два счетоводни записа.</span><span class="sxs-lookup"><span data-stu-id="29c9a-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="29c9a-119">Единият запис е за разходи, а другият запис е за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="29c9a-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="29c9a-120">При подаване на запис за разход за проект, който се съпоставя с ред на договор от тип с фиксирана цена, се създава счетоводен запис само за разходи.</span><span class="sxs-lookup"><span data-stu-id="29c9a-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="29c9a-121">Логиката за въвеждане на цени по подразбиране за разходи се базира на категорията разходи, която е избрана на страницата **Запис на разходи**.</span><span class="sxs-lookup"><span data-stu-id="29c9a-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="29c9a-122">Датата на транзакцията, редът на договора, с който е съпоставен проектът, и валутата се използват за определяне на съответната ценова листа.</span><span class="sxs-lookup"><span data-stu-id="29c9a-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="29c9a-123">За самата цена обаче сумата, въведена от потребителя, се задава директно в свързаните счетоводни записи за разходи и продажби по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="29c9a-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="29c9a-124">В текущата версия на PSA не е наличен базиран на категория запис на единични цени по подразбиране за записи за разходи.</span><span class="sxs-lookup"><span data-stu-id="29c9a-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-journals-to-record-costs"></a><span data-ttu-id="29c9a-125">Използване на счетоводни книги за записване на разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-125">Using journals to record costs</span></span>

<span data-ttu-id="29c9a-126">В PSA счетоводните книги ви позволяват да записвате разходи или приходи в класовете материали, такси, време, разходи или данъчни транзакции.</span><span class="sxs-lookup"><span data-stu-id="29c9a-126">In PSA, journals let you record cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="29c9a-127">Счетоводната книга има заглавка, редове и действие **Потвърждение**.</span><span class="sxs-lookup"><span data-stu-id="29c9a-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="29c9a-128">Ето някои сценарии, при които може да използвате счетоводна книга:</span><span class="sxs-lookup"><span data-stu-id="29c9a-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="29c9a-129">Трябва да записвате материални действителни данни за разходи и продажби по проект.</span><span class="sxs-lookup"><span data-stu-id="29c9a-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="29c9a-130">Трябва да преместите действителни данни от транзакции от друга система на PSA.</span><span class="sxs-lookup"><span data-stu-id="29c9a-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="29c9a-131">Трябва да запишете разходите, които са настъпили в друга система, като например разходи за доставки или подизпълнители.</span><span class="sxs-lookup"><span data-stu-id="29c9a-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="29c9a-132">Записване на действителни данни въз основа на проектни събития</span><span class="sxs-lookup"><span data-stu-id="29c9a-132">Recording actuals based on project events</span></span>

<span data-ttu-id="29c9a-133">PSA записва финансовите транзакции, които възникват по време на даден проект.</span><span class="sxs-lookup"><span data-stu-id="29c9a-133">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="29c9a-134">Тези транзакции се записват като **действителни данни**.</span><span class="sxs-lookup"><span data-stu-id="29c9a-134">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="29c9a-135">Следващите таблици показват различните видове действителни данни, които се създават в зависимост от това дали проектът е тип време и материали, или с фиксирана цена, дали е в етапа на предварителна продажба, или е вътрешен проект.</span><span class="sxs-lookup"><span data-stu-id="29c9a-135">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="29c9a-136">**Ресурсът принадлежи към същата организационна единица като единицата на проекта, сключваща договора**</span><span class="sxs-lookup"><span data-stu-id="29c9a-136">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="29c9a-137">Събитие</span><span class="sxs-lookup"><span data-stu-id="29c9a-137">Event</span></span></th>
<th colspan="4"><span data-ttu-id="29c9a-138">Платими или продадени проекти</span><span class="sxs-lookup"><span data-stu-id="29c9a-138">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="29c9a-139">Проект в етапа на предварителна продажба</span><span class="sxs-lookup"><span data-stu-id="29c9a-139">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="29c9a-140">Вътрешен проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-140">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="29c9a-141">Време и материали</span><span class="sxs-lookup"><span data-stu-id="29c9a-141">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="29c9a-142">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="29c9a-142">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="29c9a-143">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="29c9a-143">Actuals</span></span></th>
<th><span data-ttu-id="29c9a-144">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="29c9a-144">Transaction currency</span></span></th>
<th><span data-ttu-id="29c9a-145">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="29c9a-145">Fixed price</span></span></th>
<th><span data-ttu-id="29c9a-146">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="29c9a-146">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="29c9a-147">Създава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="29c9a-147">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="29c9a-148">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="29c9a-148">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-149">Подава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="29c9a-149">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="29c9a-150">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="29c9a-150">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="29c9a-151">Времето се одобрява и не се получава промяна или увеличаване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="29c9a-151">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="29c9a-152">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-152">Cost actual</span></span></td>
<td><span data-ttu-id="29c9a-153">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="29c9a-153">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="29c9a-154">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-154">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="29c9a-155">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="29c9a-155">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="29c9a-156">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-156">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="29c9a-157">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-157">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-158">Нефактурирани действителни продажби – платими</span><span class="sxs-lookup"><span data-stu-id="29c9a-158">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="29c9a-159">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-159">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="29c9a-160">Времето се одобрява и се получава намаляване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="29c9a-160">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="29c9a-161">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-161">Cost actual</span></span></td>
<td><span data-ttu-id="29c9a-162">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="29c9a-162">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="29c9a-163">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-163">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="29c9a-164">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="29c9a-164">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="29c9a-165">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-165">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="29c9a-166">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-167">Нефактурирани действителни продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="29c9a-167">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="29c9a-168">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-168">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-169">Нефактурирани действителни продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="29c9a-169">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="29c9a-170">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-170">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="29c9a-171">Потвърждава се фактура и не се получава промяна или увеличаване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="29c9a-171">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="29c9a-172">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="29c9a-172">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="29c9a-173">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-173">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="29c9a-174">Фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="29c9a-174">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="29c9a-175">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-175">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="29c9a-176">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-176">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="29c9a-177">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-177">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-178">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="29c9a-178">Billed sales</span></span></td>
<td><span data-ttu-id="29c9a-179">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="29c9a-180">Потвърждава се фактура и се получава намаляване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="29c9a-180">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="29c9a-181">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="29c9a-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="29c9a-182">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-182">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="29c9a-183">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-183">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="29c9a-184">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-184">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="29c9a-185">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-185">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="29c9a-186">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-187">Фактурирани продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="29c9a-187">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="29c9a-188">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-188">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-189">Фактурирани продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="29c9a-189">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="29c9a-190">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="29c9a-191">Коригира се фактура, за да се увеличи платимото количество.</span><span class="sxs-lookup"><span data-stu-id="29c9a-191">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="29c9a-192">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="29c9a-192">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="29c9a-193">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-193">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="29c9a-194">Сторниране на фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="29c9a-194">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="29c9a-195">Промяна на състоянието на контролна точка от <strong>Фактурирано</strong> в <strong>Готово за фактуриране</strong></span><span class="sxs-lookup"><span data-stu-id="29c9a-195">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="29c9a-196">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-196">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="29c9a-197">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-197">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="29c9a-198">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-198">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-199">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="29c9a-199">Billed sales</span></span></td>
<td><span data-ttu-id="29c9a-200">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-200">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="29c9a-201">Коригира се фактура, за да се намали платимото количество.</span><span class="sxs-lookup"><span data-stu-id="29c9a-201">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="29c9a-202">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="29c9a-202">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="29c9a-203">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-203">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-204">Фактурирани продажби за новото количество</span><span class="sxs-lookup"><span data-stu-id="29c9a-204">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="29c9a-205">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-205">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-206">Нефактурирани продажби – платими за разликата</span><span class="sxs-lookup"><span data-stu-id="29c9a-206">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="29c9a-207">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-207">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="29c9a-208">**Ресурсът принадлежи към организационна единица, която е различна от единицата на проекта, сключваща договора**</span><span class="sxs-lookup"><span data-stu-id="29c9a-208">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="29c9a-209">Събитие</span><span class="sxs-lookup"><span data-stu-id="29c9a-209">Event</span></span></th>
<th colspan="4"><span data-ttu-id="29c9a-210">Платими или продадени проекти</span><span class="sxs-lookup"><span data-stu-id="29c9a-210">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="29c9a-211">Проект в етапа на предварителна продажба</span><span class="sxs-lookup"><span data-stu-id="29c9a-211">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="29c9a-212">Вътрешен проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-212">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="29c9a-213">Време и материали</span><span class="sxs-lookup"><span data-stu-id="29c9a-213">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="29c9a-214">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="29c9a-214">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="29c9a-215">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="29c9a-215">Actuals</span></span></th>
<th><span data-ttu-id="29c9a-216">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="29c9a-216">Transaction currency</span></span></th>
<th><span data-ttu-id="29c9a-217">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="29c9a-217">Fixed price</span></span></th>
<th><span data-ttu-id="29c9a-218">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="29c9a-218">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="29c9a-219">Създава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="29c9a-219">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="29c9a-220">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="29c9a-220">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-221">Подава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="29c9a-221">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="29c9a-222">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="29c9a-222">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="29c9a-223">Времето се одобрява и не се получава промяна или увеличаване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="29c9a-223">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="29c9a-224">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-224">Cost actual</span></span></td>
<td><span data-ttu-id="29c9a-225">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="29c9a-225">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="29c9a-226">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-226">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="29c9a-227">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="29c9a-227">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="29c9a-228">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-228">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="29c9a-229">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-229">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-230">Нефактурирани действителни продажби – платими</span><span class="sxs-lookup"><span data-stu-id="29c9a-230">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="29c9a-231">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-231">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-232">Разход на ресурсна единица</span><span class="sxs-lookup"><span data-stu-id="29c9a-232">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="29c9a-233">Валута на ресурсната единица</span><span class="sxs-lookup"><span data-stu-id="29c9a-233">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-234">Продажби между организации</span><span class="sxs-lookup"><span data-stu-id="29c9a-234">Interorganizational sales</span></span></td>
<td><span data-ttu-id="29c9a-235">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="29c9a-235">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="29c9a-236">Времето се одобрява и се получава намаляване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="29c9a-236">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="29c9a-237">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-237">Cost actual</span></span></td>
<td><span data-ttu-id="29c9a-238">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="29c9a-238">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="29c9a-239">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-239">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="29c9a-240">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="29c9a-240">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="29c9a-241">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-241">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="29c9a-242">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="29c9a-242">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-243">Разход на ресурсна единица</span><span class="sxs-lookup"><span data-stu-id="29c9a-243">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="29c9a-244">Валута на ресурсната единица</span><span class="sxs-lookup"><span data-stu-id="29c9a-244">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-245">Продажби между организации</span><span class="sxs-lookup"><span data-stu-id="29c9a-245">Interorganizational sales</span></span></td>
<td><span data-ttu-id="29c9a-246">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="29c9a-246">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-247">Нефактурирани действителни продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="29c9a-247">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="29c9a-248">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-248">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-249">Нефактурирани действителни продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="29c9a-249">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="29c9a-250">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-250">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="29c9a-251">Потвърждава се фактура и не се получава промяна или увеличаване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="29c9a-251">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="29c9a-252">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="29c9a-252">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="29c9a-253">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-253">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="29c9a-254">Фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="29c9a-254">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="29c9a-255">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-255">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="29c9a-256">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-256">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="29c9a-257">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-257">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-258">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="29c9a-258">Billed sales</span></span></td>
<td><span data-ttu-id="29c9a-259">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="29c9a-260">Потвърждава се фактура и се получава намаляване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="29c9a-260">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="29c9a-261">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="29c9a-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="29c9a-262">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-262">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="29c9a-263">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-263">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="29c9a-264">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-264">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="29c9a-265">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-265">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="29c9a-266">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-267">Фактурирани продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="29c9a-267">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="29c9a-268">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-268">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-269">Фактурирани продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="29c9a-269">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="29c9a-270">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-270">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="29c9a-271">Коригира се фактура, за да се увеличи платимото количество.</span><span class="sxs-lookup"><span data-stu-id="29c9a-271">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="29c9a-272">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="29c9a-272">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="29c9a-273">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-273">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="29c9a-274">Сторниране на фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="29c9a-274">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="29c9a-275">Промяна на състоянието на контролна точка от <strong>Фактурирано</strong> в <strong>Готово за фактуриране</strong></span><span class="sxs-lookup"><span data-stu-id="29c9a-275">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="29c9a-276">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-276">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="29c9a-277">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-277">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="29c9a-278">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="29c9a-278">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-279">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="29c9a-279">Billed sales</span></span></td>
<td><span data-ttu-id="29c9a-280">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-280">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="29c9a-281">Коригира се фактура, за да се намали платимото количество.</span><span class="sxs-lookup"><span data-stu-id="29c9a-281">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="29c9a-282">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="29c9a-282">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="29c9a-283">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-283">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-284">Фактурирани продажби за новото количество</span><span class="sxs-lookup"><span data-stu-id="29c9a-284">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="29c9a-285">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-285">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="29c9a-286">Нефактурирани продажби – платими за разликата</span><span class="sxs-lookup"><span data-stu-id="29c9a-286">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="29c9a-287">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="29c9a-287">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
