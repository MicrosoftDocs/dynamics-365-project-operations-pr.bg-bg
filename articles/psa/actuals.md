---
title: Общ преглед на действителни данни
description: Тази тема предоставя информация за действителни данни на проекта.
author: rumant
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
ms.openlocfilehash: 73f1b14bbb4cc53111a1b3a93756a86db04475ab
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014643"
---
# <a name="actuals-overview"></a><span data-ttu-id="7d67f-103">Общ преглед на действителни данни</span><span class="sxs-lookup"><span data-stu-id="7d67f-103">Actuals overview</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="7d67f-104">Действителните данни са количеството работа, завършена по даден проект.</span><span class="sxs-lookup"><span data-stu-id="7d67f-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="7d67f-105">Действителните данни на проекта могат да бъдат проследени обратно до техните изходни документи.</span><span class="sxs-lookup"><span data-stu-id="7d67f-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="7d67f-106">Тези изходни документи включват време, разходи и записи в счетоводния регистър, а също и фактури.</span><span class="sxs-lookup"><span data-stu-id="7d67f-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![Как се проследяват действителните данни на проекта до изходните документи](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="7d67f-108">Подаване на запис за време</span><span class="sxs-lookup"><span data-stu-id="7d67f-108">Submitting a time entry</span></span>

<span data-ttu-id="7d67f-109">В PSA при подаване на запис за време за проект, който се съпоставя с ред на договор от тип време и материали, се създават два счетоводни записа.</span><span class="sxs-lookup"><span data-stu-id="7d67f-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="7d67f-110">Единият запис е за разходи, а другият запис е за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="7d67f-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="7d67f-111">При подаване на запис за време за проект, който се съпоставя с ред на договор от тип с фиксирана цена, се създава счетоводен запис само за разходи.</span><span class="sxs-lookup"><span data-stu-id="7d67f-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="7d67f-112">Логиката за въвеждане на цени по подразбиране се намира в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="7d67f-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="7d67f-113">Всички стойности на полета от запис за време се копират в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="7d67f-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="7d67f-114">Тези полета включват датата на транзакцията, реда на договора, с който е съпоставен проектът, и резултата от валутата в съответната ценова листа.</span><span class="sxs-lookup"><span data-stu-id="7d67f-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="7d67f-115">Полетата, които влияят на цените по подразбиране, като например **Роля** и **Организационна единица**, водят до въвеждане на съответна цена по подразбиране в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="7d67f-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="7d67f-116">Ако добавите персонализирано поле в записа за време и искате стойността на полето да се попълни в действителните данни, създайте полето в обекта „Действителни данни“ и използвайте съпоставяния на полета, за да копирате полето от записа за време в действителните данни.</span><span class="sxs-lookup"><span data-stu-id="7d67f-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="7d67f-117">Подаване на запис за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-117">Submitting an expense entry</span></span>

<span data-ttu-id="7d67f-118">В PSA при подаване на запис за разходи за проект, който се съпоставя с ред на договор от тип време и материали, се създават два счетоводни записа.</span><span class="sxs-lookup"><span data-stu-id="7d67f-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="7d67f-119">Единият запис е за разходи, а другият запис е за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="7d67f-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="7d67f-120">При подаване на запис за разход за проект, който се съпоставя с ред на договор от тип с фиксирана цена, се създава счетоводен запис само за разходи.</span><span class="sxs-lookup"><span data-stu-id="7d67f-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="7d67f-121">Логиката за въвеждане на цени по подразбиране за разходи се базира на категорията разходи, която е избрана на страницата **Запис на разходи**.</span><span class="sxs-lookup"><span data-stu-id="7d67f-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="7d67f-122">Датата на транзакцията, редът на договора, с който е съпоставен проектът, и валутата се използват за определяне на съответната ценова листа.</span><span class="sxs-lookup"><span data-stu-id="7d67f-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="7d67f-123">За самата цена обаче сумата, въведена от потребителя, се задава директно в свързаните счетоводни записи за разходи и продажби по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="7d67f-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="7d67f-124">В текущата версия на PSA не е наличен базиран на категория запис на единични цени по подразбиране за записи за разходи.</span><span class="sxs-lookup"><span data-stu-id="7d67f-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="7d67f-125">Използване на счетоводни книги за записване на разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="7d67f-126">В PSA счетоводните книги за записи ви позволяват да записвате разходите или приходите в класовете материали, такси, време, разходи или данъчни транзакции.</span><span class="sxs-lookup"><span data-stu-id="7d67f-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="7d67f-127">Счетоводната книга има заглавка, редове и действие **Потвърждение**.</span><span class="sxs-lookup"><span data-stu-id="7d67f-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="7d67f-128">Ето някои сценарии, при които може да използвате счетоводна книга:</span><span class="sxs-lookup"><span data-stu-id="7d67f-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="7d67f-129">Трябва да записвате материални действителни данни за разходи и продажби по проект.</span><span class="sxs-lookup"><span data-stu-id="7d67f-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="7d67f-130">Трябва да преместите действителни данни от транзакции от друга система на PSA.</span><span class="sxs-lookup"><span data-stu-id="7d67f-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="7d67f-131">Трябва да запишете разходите, които са настъпили в друга система, като например разходи за доставки или подизпълнители.</span><span class="sxs-lookup"><span data-stu-id="7d67f-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7d67f-132">Използването на счетоводни книги за записи за създаване на действителни данни трябва да се извършва само от потребител, който е разбира напълно как ще се отразят действителните данни върху проекта.</span><span class="sxs-lookup"><span data-stu-id="7d67f-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="7d67f-133">Това е така, защото приложението не проверява типа на счетоводния запис или свързаното ценообразуване, въведено в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="7d67f-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="7d67f-134">Поради въздействието на този тип счетоводни книги, подбирайте внимателно на кого предоставяте достъп за създаване на счетоводни книги за записи.</span><span class="sxs-lookup"><span data-stu-id="7d67f-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="7d67f-135">Записване на действителни данни въз основа на проектни събития</span><span class="sxs-lookup"><span data-stu-id="7d67f-135">Recording actuals based on project events</span></span>

<span data-ttu-id="7d67f-136">PSA записва финансовите транзакции, които възникват по време на даден проект.</span><span class="sxs-lookup"><span data-stu-id="7d67f-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="7d67f-137">Тези транзакции се записват като **действителни данни**.</span><span class="sxs-lookup"><span data-stu-id="7d67f-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="7d67f-138">Следващите таблици показват различните видове действителни данни, които се създават в зависимост от това дали проектът е тип време и материали, или с фиксирана цена, дали е в етапа на предварителна продажба, или е вътрешен проект.</span><span class="sxs-lookup"><span data-stu-id="7d67f-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="7d67f-139">**Ресурсът принадлежи към същата организационна единица като единицата на проекта, сключваща договора**</span><span class="sxs-lookup"><span data-stu-id="7d67f-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="7d67f-140">Събитие</span><span class="sxs-lookup"><span data-stu-id="7d67f-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="7d67f-141">Платими или продадени проекти</span><span class="sxs-lookup"><span data-stu-id="7d67f-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="7d67f-142">Проект в етапа на предварителна продажба</span><span class="sxs-lookup"><span data-stu-id="7d67f-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="7d67f-143">Вътрешен проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="7d67f-144">Време и материали</span><span class="sxs-lookup"><span data-stu-id="7d67f-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="7d67f-145">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="7d67f-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="7d67f-146">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="7d67f-146">Actuals</span></span></th>
<th><span data-ttu-id="7d67f-147">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="7d67f-147">Transaction currency</span></span></th>
<th><span data-ttu-id="7d67f-148">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="7d67f-148">Fixed price</span></span></th>
<th><span data-ttu-id="7d67f-149">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="7d67f-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="7d67f-150">Създава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="7d67f-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="7d67f-151">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="7d67f-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-152">Подава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="7d67f-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="7d67f-153">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="7d67f-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7d67f-154">Времето се одобрява и не се получава промяна или увеличаване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="7d67f-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7d67f-155">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-155">Cost actual</span></span></td>
<td><span data-ttu-id="7d67f-156">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7d67f-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7d67f-157">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="7d67f-158">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7d67f-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="7d67f-159">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="7d67f-160">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-161">Нефактурирани действителни продажби – платими</span><span class="sxs-lookup"><span data-stu-id="7d67f-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="7d67f-162">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7d67f-163">Времето се одобрява и се получава намаляване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="7d67f-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7d67f-164">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-164">Cost actual</span></span></td>
<td><span data-ttu-id="7d67f-165">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7d67f-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7d67f-166">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="7d67f-167">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7d67f-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7d67f-168">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="7d67f-169">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-170">Нефактурирани действителни продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="7d67f-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7d67f-171">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-172">Нефактурирани действителни продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="7d67f-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7d67f-173">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7d67f-174">Потвърждава се фактура и не се получава промяна или увеличаване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="7d67f-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7d67f-175">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7d67f-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7d67f-176">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7d67f-177">Фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="7d67f-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="7d67f-178">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7d67f-179">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="7d67f-180">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-181">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7d67f-181">Billed sales</span></span></td>
<td><span data-ttu-id="7d67f-182">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7d67f-183">Потвърждава се фактура и се получава намаляване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="7d67f-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7d67f-184">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7d67f-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7d67f-185">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7d67f-186">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7d67f-187">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7d67f-188">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7d67f-189">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-190">Фактурирани продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="7d67f-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7d67f-191">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-192">Фактурирани продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="7d67f-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7d67f-193">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7d67f-194">Коригира се фактура, за да се увеличи платимото количество.</span><span class="sxs-lookup"><span data-stu-id="7d67f-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7d67f-195">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="7d67f-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7d67f-196">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="7d67f-197">Сторниране на фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="7d67f-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="7d67f-198">Промяна на състоянието на контролна точка от <strong>Фактурирано</strong> в <strong>Готово за фактуриране</strong></span><span class="sxs-lookup"><span data-stu-id="7d67f-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="7d67f-199">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7d67f-200">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="7d67f-201">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-202">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7d67f-202">Billed sales</span></span></td>
<td><span data-ttu-id="7d67f-203">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7d67f-204">Коригира се фактура, за да се намали платимото количество.</span><span class="sxs-lookup"><span data-stu-id="7d67f-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7d67f-205">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="7d67f-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7d67f-206">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-207">Фактурирани продажби за новото количество</span><span class="sxs-lookup"><span data-stu-id="7d67f-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="7d67f-208">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-209">Нефактурирани продажби – платими за разликата</span><span class="sxs-lookup"><span data-stu-id="7d67f-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="7d67f-210">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="7d67f-211">**Ресурсът принадлежи към организационна единица, която е различна от единицата на проекта, сключваща договора**</span><span class="sxs-lookup"><span data-stu-id="7d67f-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="7d67f-212">Събитие</span><span class="sxs-lookup"><span data-stu-id="7d67f-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="7d67f-213">Платими или продадени проекти</span><span class="sxs-lookup"><span data-stu-id="7d67f-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="7d67f-214">Проект в етапа на предварителна продажба</span><span class="sxs-lookup"><span data-stu-id="7d67f-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="7d67f-215">Вътрешен проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="7d67f-216">Време и материали</span><span class="sxs-lookup"><span data-stu-id="7d67f-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="7d67f-217">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="7d67f-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="7d67f-218">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="7d67f-218">Actuals</span></span></th>
<th><span data-ttu-id="7d67f-219">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="7d67f-219">Transaction currency</span></span></th>
<th><span data-ttu-id="7d67f-220">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="7d67f-220">Fixed price</span></span></th>
<th><span data-ttu-id="7d67f-221">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="7d67f-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="7d67f-222">Създава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="7d67f-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="7d67f-223">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="7d67f-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-224">Подава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="7d67f-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="7d67f-225">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="7d67f-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="7d67f-226">Времето се одобрява и не се получава промяна или увеличаване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="7d67f-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7d67f-227">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-227">Cost actual</span></span></td>
<td><span data-ttu-id="7d67f-228">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7d67f-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="7d67f-229">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="7d67f-230">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7d67f-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="7d67f-231">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="7d67f-232">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-233">Нефактурирани действителни продажби – платими</span><span class="sxs-lookup"><span data-stu-id="7d67f-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="7d67f-234">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-235">Разход на ресурсна единица</span><span class="sxs-lookup"><span data-stu-id="7d67f-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="7d67f-236">Валута на ресурсната единица</span><span class="sxs-lookup"><span data-stu-id="7d67f-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-237">Продажби между организации</span><span class="sxs-lookup"><span data-stu-id="7d67f-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="7d67f-238">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7d67f-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="7d67f-239">Времето се одобрява и се получава намаляване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="7d67f-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7d67f-240">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-240">Cost actual</span></span></td>
<td><span data-ttu-id="7d67f-241">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7d67f-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7d67f-242">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="7d67f-243">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7d67f-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7d67f-244">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="7d67f-245">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7d67f-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-246">Разход на ресурсна единица</span><span class="sxs-lookup"><span data-stu-id="7d67f-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="7d67f-247">Валута на ресурсната единица</span><span class="sxs-lookup"><span data-stu-id="7d67f-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-248">Продажби между организации</span><span class="sxs-lookup"><span data-stu-id="7d67f-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="7d67f-249">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7d67f-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-250">Нефактурирани действителни продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="7d67f-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7d67f-251">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-252">Нефактурирани действителни продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="7d67f-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7d67f-253">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7d67f-254">Потвърждава се фактура и не се получава промяна или увеличаване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="7d67f-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7d67f-255">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7d67f-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7d67f-256">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7d67f-257">Фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="7d67f-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="7d67f-258">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7d67f-259">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="7d67f-260">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-261">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7d67f-261">Billed sales</span></span></td>
<td><span data-ttu-id="7d67f-262">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7d67f-263">Потвърждава се фактура и се получава намаляване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="7d67f-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7d67f-264">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7d67f-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7d67f-265">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7d67f-266">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7d67f-267">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7d67f-268">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7d67f-269">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-270">Фактурирани продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="7d67f-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7d67f-271">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-272">Фактурирани продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="7d67f-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7d67f-273">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7d67f-274">Коригира се фактура, за да се увеличи платимото количество.</span><span class="sxs-lookup"><span data-stu-id="7d67f-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7d67f-275">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="7d67f-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7d67f-276">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="7d67f-277">Сторниране на фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="7d67f-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="7d67f-278">Промяна на състоянието на контролна точка от <strong>Фактурирано</strong> в <strong>Готово за фактуриране</strong></span><span class="sxs-lookup"><span data-stu-id="7d67f-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="7d67f-279">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7d67f-280">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="7d67f-281">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7d67f-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-282">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7d67f-282">Billed sales</span></span></td>
<td><span data-ttu-id="7d67f-283">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7d67f-284">Коригира се фактура, за да се намали платимото количество.</span><span class="sxs-lookup"><span data-stu-id="7d67f-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7d67f-285">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="7d67f-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7d67f-286">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-287">Фактурирани продажби за новото количество</span><span class="sxs-lookup"><span data-stu-id="7d67f-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="7d67f-288">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7d67f-289">Нефактурирани продажби – платими за разликата</span><span class="sxs-lookup"><span data-stu-id="7d67f-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="7d67f-290">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7d67f-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]