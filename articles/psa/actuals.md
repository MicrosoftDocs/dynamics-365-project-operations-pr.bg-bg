---
title: Общ преглед на действителни данни
description: Тази тема предоставя информация за действителни данни на проекта.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 08/03/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c4a3424bed704243dfb5524fa541c3fcc0899e57
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285605"
---
# <a name="actuals-overview"></a><span data-ttu-id="4feb4-103">Общ преглед на действителни данни</span><span class="sxs-lookup"><span data-stu-id="4feb4-103">Actuals overview</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="4feb4-104">Действителните данни са количеството работа, завършена по даден проект.</span><span class="sxs-lookup"><span data-stu-id="4feb4-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="4feb4-105">Действителните данни на проекта могат да бъдат проследени обратно до техните изходни документи.</span><span class="sxs-lookup"><span data-stu-id="4feb4-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="4feb4-106">Тези изходни документи включват време, разходи и записи в счетоводния регистър, а също и фактури.</span><span class="sxs-lookup"><span data-stu-id="4feb4-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![Как се проследяват действителните данни на проекта до изходните документи](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="4feb4-108">Подаване на запис за време</span><span class="sxs-lookup"><span data-stu-id="4feb4-108">Submitting a time entry</span></span>

<span data-ttu-id="4feb4-109">В PSA при подаване на запис за време за проект, който се съпоставя с ред на договор от тип време и материали, се създават два счетоводни записа.</span><span class="sxs-lookup"><span data-stu-id="4feb4-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="4feb4-110">Единият запис е за разходи, а другият запис е за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="4feb4-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="4feb4-111">При подаване на запис за време за проект, който се съпоставя с ред на договор от тип с фиксирана цена, се създава счетоводен запис само за разходи.</span><span class="sxs-lookup"><span data-stu-id="4feb4-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="4feb4-112">Логиката за въвеждане на цени по подразбиране се намира в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="4feb4-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="4feb4-113">Всички стойности на полета от запис за време се копират в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="4feb4-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="4feb4-114">Тези полета включват датата на транзакцията, реда на договора, с който е съпоставен проектът, и резултата от валутата в съответната ценова листа.</span><span class="sxs-lookup"><span data-stu-id="4feb4-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="4feb4-115">Полетата, които влияят на цените по подразбиране, като например **Роля** и **Организационна единица**, водят до въвеждане на съответна цена по подразбиране в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="4feb4-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="4feb4-116">Ако добавите персонализирано поле в записа за време и искате стойността на полето да се попълни в действителните данни, създайте полето в обекта „Действителни данни“ и използвайте съпоставяния на полета, за да копирате полето от записа за време в действителните данни.</span><span class="sxs-lookup"><span data-stu-id="4feb4-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="4feb4-117">Подаване на запис за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-117">Submitting an expense entry</span></span>

<span data-ttu-id="4feb4-118">В PSA при подаване на запис за разходи за проект, който се съпоставя с ред на договор от тип време и материали, се създават два счетоводни записа.</span><span class="sxs-lookup"><span data-stu-id="4feb4-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="4feb4-119">Единият запис е за разходи, а другият запис е за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="4feb4-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="4feb4-120">При подаване на запис за разход за проект, който се съпоставя с ред на договор от тип с фиксирана цена, се създава счетоводен запис само за разходи.</span><span class="sxs-lookup"><span data-stu-id="4feb4-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="4feb4-121">Логиката за въвеждане на цени по подразбиране за разходи се базира на категорията разходи, която е избрана на страницата **Запис на разходи**.</span><span class="sxs-lookup"><span data-stu-id="4feb4-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="4feb4-122">Датата на транзакцията, редът на договора, с който е съпоставен проектът, и валутата се използват за определяне на съответната ценова листа.</span><span class="sxs-lookup"><span data-stu-id="4feb4-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="4feb4-123">За самата цена обаче сумата, въведена от потребителя, се задава директно в свързаните счетоводни записи за разходи и продажби по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="4feb4-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="4feb4-124">В текущата версия на PSA не е наличен базиран на категория запис на единични цени по подразбиране за записи за разходи.</span><span class="sxs-lookup"><span data-stu-id="4feb4-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="4feb4-125">Използване на счетоводни книги за записване на разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="4feb4-126">В PSA счетоводните книги за записи ви позволяват да записвате разходите или приходите в класовете материали, такси, време, разходи или данъчни транзакции.</span><span class="sxs-lookup"><span data-stu-id="4feb4-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="4feb4-127">Счетоводната книга има заглавка, редове и действие **Потвърждение**.</span><span class="sxs-lookup"><span data-stu-id="4feb4-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="4feb4-128">Ето някои сценарии, при които може да използвате счетоводна книга:</span><span class="sxs-lookup"><span data-stu-id="4feb4-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="4feb4-129">Трябва да записвате материални действителни данни за разходи и продажби по проект.</span><span class="sxs-lookup"><span data-stu-id="4feb4-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="4feb4-130">Трябва да преместите действителни данни от транзакции от друга система на PSA.</span><span class="sxs-lookup"><span data-stu-id="4feb4-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="4feb4-131">Трябва да запишете разходите, които са настъпили в друга система, като например разходи за доставки или подизпълнители.</span><span class="sxs-lookup"><span data-stu-id="4feb4-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4feb4-132">Използването на счетоводни книги за записи за създаване на действителни данни трябва да се извършва само от потребител, който е разбира напълно как ще се отразят действителните данни върху проекта.</span><span class="sxs-lookup"><span data-stu-id="4feb4-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="4feb4-133">Това е така, защото приложението не проверява типа на счетоводния запис или свързаното ценообразуване, въведено в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="4feb4-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="4feb4-134">Поради въздействието на този тип счетоводни книги, подбирайте внимателно на кого предоставяте достъп за създаване на счетоводни книги за записи.</span><span class="sxs-lookup"><span data-stu-id="4feb4-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="4feb4-135">Записване на действителни данни въз основа на проектни събития</span><span class="sxs-lookup"><span data-stu-id="4feb4-135">Recording actuals based on project events</span></span>

<span data-ttu-id="4feb4-136">PSA записва финансовите транзакции, които възникват по време на даден проект.</span><span class="sxs-lookup"><span data-stu-id="4feb4-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="4feb4-137">Тези транзакции се записват като **действителни данни**.</span><span class="sxs-lookup"><span data-stu-id="4feb4-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="4feb4-138">Следващите таблици показват различните видове действителни данни, които се създават в зависимост от това дали проектът е тип време и материали, или с фиксирана цена, дали е в етапа на предварителна продажба, или е вътрешен проект.</span><span class="sxs-lookup"><span data-stu-id="4feb4-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="4feb4-139">**Ресурсът принадлежи към същата организационна единица като единицата на проекта, сключваща договора**</span><span class="sxs-lookup"><span data-stu-id="4feb4-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="4feb4-140">Събитие</span><span class="sxs-lookup"><span data-stu-id="4feb4-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="4feb4-141">Платими или продадени проекти</span><span class="sxs-lookup"><span data-stu-id="4feb4-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="4feb4-142">Проект в етапа на предварителна продажба</span><span class="sxs-lookup"><span data-stu-id="4feb4-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="4feb4-143">Вътрешен проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="4feb4-144">Време и материали</span><span class="sxs-lookup"><span data-stu-id="4feb4-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="4feb4-145">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="4feb4-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="4feb4-146">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="4feb4-146">Actuals</span></span></th>
<th><span data-ttu-id="4feb4-147">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="4feb4-147">Transaction currency</span></span></th>
<th><span data-ttu-id="4feb4-148">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="4feb4-148">Fixed price</span></span></th>
<th><span data-ttu-id="4feb4-149">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="4feb4-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="4feb4-150">Създава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="4feb4-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="4feb4-151">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="4feb4-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-152">Подава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="4feb4-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="4feb4-153">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="4feb4-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4feb4-154">Времето се одобрява и не се получава промяна или увеличаване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="4feb4-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="4feb4-155">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-155">Cost actual</span></span></td>
<td><span data-ttu-id="4feb4-156">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="4feb4-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4feb4-157">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="4feb4-158">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="4feb4-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="4feb4-159">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="4feb4-160">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-161">Нефактурирани действителни продажби – платими</span><span class="sxs-lookup"><span data-stu-id="4feb4-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="4feb4-162">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4feb4-163">Времето се одобрява и се получава намаляване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="4feb4-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="4feb4-164">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-164">Cost actual</span></span></td>
<td><span data-ttu-id="4feb4-165">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="4feb4-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="4feb4-166">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="4feb4-167">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="4feb4-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="4feb4-168">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="4feb4-169">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-170">Нефактурирани действителни продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="4feb4-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="4feb4-171">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-172">Нефактурирани действителни продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="4feb4-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="4feb4-173">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4feb4-174">Потвърждава се фактура и не се получава промяна или увеличаване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="4feb4-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="4feb4-175">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="4feb4-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="4feb4-176">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4feb4-177">Фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="4feb4-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="4feb4-178">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4feb4-179">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="4feb4-180">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-181">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="4feb4-181">Billed sales</span></span></td>
<td><span data-ttu-id="4feb4-182">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4feb4-183">Потвърждава се фактура и се получава намаляване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="4feb4-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="4feb4-184">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="4feb4-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="4feb4-185">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="4feb4-186">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4feb4-187">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4feb4-188">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4feb4-189">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-190">Фактурирани продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="4feb4-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="4feb4-191">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-192">Фактурирани продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="4feb4-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="4feb4-193">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4feb4-194">Коригира се фактура, за да се увеличи платимото количество.</span><span class="sxs-lookup"><span data-stu-id="4feb4-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="4feb4-195">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="4feb4-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="4feb4-196">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="4feb4-197">Сторниране на фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="4feb4-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="4feb4-198">Промяна на състоянието на контролна точка от <strong>Фактурирано</strong> в <strong>Готово за фактуриране</strong></span><span class="sxs-lookup"><span data-stu-id="4feb4-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="4feb4-199">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="4feb4-200">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="4feb4-201">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-202">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="4feb4-202">Billed sales</span></span></td>
<td><span data-ttu-id="4feb4-203">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4feb4-204">Коригира се фактура, за да се намали платимото количество.</span><span class="sxs-lookup"><span data-stu-id="4feb4-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="4feb4-205">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="4feb4-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="4feb4-206">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-207">Фактурирани продажби за новото количество</span><span class="sxs-lookup"><span data-stu-id="4feb4-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="4feb4-208">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-209">Нефактурирани продажби – платими за разликата</span><span class="sxs-lookup"><span data-stu-id="4feb4-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="4feb4-210">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="4feb4-211">**Ресурсът принадлежи към организационна единица, която е различна от единицата на проекта, сключваща договора**</span><span class="sxs-lookup"><span data-stu-id="4feb4-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="4feb4-212">Събитие</span><span class="sxs-lookup"><span data-stu-id="4feb4-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="4feb4-213">Платими или продадени проекти</span><span class="sxs-lookup"><span data-stu-id="4feb4-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="4feb4-214">Проект в етапа на предварителна продажба</span><span class="sxs-lookup"><span data-stu-id="4feb4-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="4feb4-215">Вътрешен проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="4feb4-216">Време и материали</span><span class="sxs-lookup"><span data-stu-id="4feb4-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="4feb4-217">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="4feb4-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="4feb4-218">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="4feb4-218">Actuals</span></span></th>
<th><span data-ttu-id="4feb4-219">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="4feb4-219">Transaction currency</span></span></th>
<th><span data-ttu-id="4feb4-220">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="4feb4-220">Fixed price</span></span></th>
<th><span data-ttu-id="4feb4-221">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="4feb4-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="4feb4-222">Създава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="4feb4-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="4feb4-223">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="4feb4-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-224">Подава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="4feb4-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="4feb4-225">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="4feb4-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="4feb4-226">Времето се одобрява и не се получава промяна или увеличаване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="4feb4-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="4feb4-227">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-227">Cost actual</span></span></td>
<td><span data-ttu-id="4feb4-228">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="4feb4-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="4feb4-229">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="4feb4-230">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="4feb4-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="4feb4-231">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="4feb4-232">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-233">Нефактурирани действителни продажби – платими</span><span class="sxs-lookup"><span data-stu-id="4feb4-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="4feb4-234">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-235">Разход на ресурсна единица</span><span class="sxs-lookup"><span data-stu-id="4feb4-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="4feb4-236">Валута на ресурсната единица</span><span class="sxs-lookup"><span data-stu-id="4feb4-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-237">Продажби между организации</span><span class="sxs-lookup"><span data-stu-id="4feb4-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="4feb4-238">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="4feb4-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="4feb4-239">Времето се одобрява и се получава намаляване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="4feb4-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="4feb4-240">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-240">Cost actual</span></span></td>
<td><span data-ttu-id="4feb4-241">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="4feb4-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="4feb4-242">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="4feb4-243">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="4feb4-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="4feb4-244">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="4feb4-245">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="4feb4-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-246">Разход на ресурсна единица</span><span class="sxs-lookup"><span data-stu-id="4feb4-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="4feb4-247">Валута на ресурсната единица</span><span class="sxs-lookup"><span data-stu-id="4feb4-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-248">Продажби между организации</span><span class="sxs-lookup"><span data-stu-id="4feb4-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="4feb4-249">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="4feb4-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-250">Нефактурирани действителни продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="4feb4-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="4feb4-251">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-252">Нефактурирани действителни продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="4feb4-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="4feb4-253">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4feb4-254">Потвърждава се фактура и не се получава промяна или увеличаване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="4feb4-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="4feb4-255">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="4feb4-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="4feb4-256">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4feb4-257">Фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="4feb4-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="4feb4-258">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="4feb4-259">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="4feb4-260">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-261">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="4feb4-261">Billed sales</span></span></td>
<td><span data-ttu-id="4feb4-262">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4feb4-263">Потвърждава се фактура и се получава намаляване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="4feb4-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="4feb4-264">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="4feb4-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="4feb4-265">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="4feb4-266">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4feb4-267">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4feb4-268">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="4feb4-269">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-270">Фактурирани продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="4feb4-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="4feb4-271">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-272">Фактурирани продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="4feb4-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="4feb4-273">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="4feb4-274">Коригира се фактура, за да се увеличи платимото количество.</span><span class="sxs-lookup"><span data-stu-id="4feb4-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="4feb4-275">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="4feb4-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="4feb4-276">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="4feb4-277">Сторниране на фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="4feb4-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="4feb4-278">Промяна на състоянието на контролна точка от <strong>Фактурирано</strong> в <strong>Готово за фактуриране</strong></span><span class="sxs-lookup"><span data-stu-id="4feb4-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="4feb4-279">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="4feb4-280">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="4feb4-281">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="4feb4-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-282">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="4feb4-282">Billed sales</span></span></td>
<td><span data-ttu-id="4feb4-283">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="4feb4-284">Коригира се фактура, за да се намали платимото количество.</span><span class="sxs-lookup"><span data-stu-id="4feb4-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="4feb4-285">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="4feb4-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="4feb4-286">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-287">Фактурирани продажби за новото количество</span><span class="sxs-lookup"><span data-stu-id="4feb4-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="4feb4-288">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="4feb4-289">Нефактурирани продажби – платими за разликата</span><span class="sxs-lookup"><span data-stu-id="4feb4-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="4feb4-290">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="4feb4-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]