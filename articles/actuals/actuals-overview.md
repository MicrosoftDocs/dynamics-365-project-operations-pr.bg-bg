---
title: Действителни данни
description: Тази тема предоставя информация за работата с действителни данни в Microsoft Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/16/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 13c429763fa805fae5324e4dcf1bf7669e842281
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126290"
---
# <a name="actuals"></a><span data-ttu-id="9d607-103">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="9d607-103">Actuals</span></span> 

<span data-ttu-id="9d607-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="9d607-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="9d607-105">Действителните данни са количеството работа, завършена по даден проект.</span><span class="sxs-lookup"><span data-stu-id="9d607-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="9d607-106">Те се създават в резултат на записи за време и разходи и записи в дневник и фактури.</span><span class="sxs-lookup"><span data-stu-id="9d607-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="9d607-107">Счетоводни записи и подаване на време</span><span class="sxs-lookup"><span data-stu-id="9d607-107">Journal lines and time submission</span></span>

<span data-ttu-id="9d607-108">За повече информация относно въвеждането на време вижте [Преглед на въвеждането на време](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="9d607-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="9d607-109">Време и материали</span><span class="sxs-lookup"><span data-stu-id="9d607-109">Time and materials</span></span>

<span data-ttu-id="9d607-110">Когато изпратеният запис за време е свързан с проект, който е съпоставен с ред за договор за време и материали, системата създава два реда на дневника, един за разходи и един за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="9d607-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="9d607-111">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="9d607-111">Fixed price</span></span>

<span data-ttu-id="9d607-112">При подаване на запис за време, който е свързан с проект, който се съпоставя с ред на договор от тип с фиксирана цена, системата създава един счетоводен запис за разходи.</span><span class="sxs-lookup"><span data-stu-id="9d607-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="9d607-113">Ценообразуване по подразбиране</span><span class="sxs-lookup"><span data-stu-id="9d607-113">Default pricing</span></span>

<span data-ttu-id="9d607-114">Логиката за създаване на цени по подразбиране се намира в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="9d607-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="9d607-115">Стойностите на полета от запис за време се копират в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="9d607-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="9d607-116">Тези стойности включват датата на транзакцията, реда на договора, с който е съпоставен проектът, и резултата от валутата в съответната ценова листа.</span><span class="sxs-lookup"><span data-stu-id="9d607-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="9d607-117">Полетата, които влияят на цените по подразбиране, като например **Роля** и **Организационна единица**, се използват за определяне на съответна цена по подразбиране в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="9d607-117">The fields that affect default pricing, such as **Role** and **Org Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="9d607-118">Можете да добавите персонализирано поле за въвеждане на час.</span><span class="sxs-lookup"><span data-stu-id="9d607-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="9d607-119">Ако искате стойността на полето да се попълни в действителните данни, създайте полето в обекта „Действителни данни“ и използвайте съпоставяния на полета, за да копирате полето от записа за време в действителните данни.</span><span class="sxs-lookup"><span data-stu-id="9d607-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="9d607-120">Редове на списания и представяне на основните разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="9d607-121">За повече информация относно запис за разходи вижте [Преглед на разход](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="9d607-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="9d607-122">Време и материали</span><span class="sxs-lookup"><span data-stu-id="9d607-122">Time and materials</span></span>

<span data-ttu-id="9d607-123">Когато основен запис за разход е свързан с проект, който е съпоставен с ред за договор за време и материали, системата създава два реда на дневника, един за разходи и един за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="9d607-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="9d607-124">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="9d607-124">Fixed price</span></span>

<span data-ttu-id="9d607-125">При основен запис за разход, който е свързан с проект, който се съпоставя с ред на договор от тип с фиксирана цена, системата създава един счетоводен запис за разходи.</span><span class="sxs-lookup"><span data-stu-id="9d607-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="9d607-126">Ценообразуване по подразбиране</span><span class="sxs-lookup"><span data-stu-id="9d607-126">Default pricing</span></span>

<span data-ttu-id="9d607-127">Логиката за въвеждане на цени по подразбиране за разходи се основава на категорията на разходите.</span><span class="sxs-lookup"><span data-stu-id="9d607-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="9d607-128">Датата на транзакцията, редът на договора, с който е съпоставен проектът, и валутата се използват за определяне на съответната ценова листа.</span><span class="sxs-lookup"><span data-stu-id="9d607-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="9d607-129">За самата цена обаче по подразбиране сумата, въведена за самата цена, се задава директно в свързаните счетоводни записи за разходи и продажби.</span><span class="sxs-lookup"><span data-stu-id="9d607-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="9d607-130">Базиран на категория запис на единични цени по подразбиране за записи за разходи.</span><span class="sxs-lookup"><span data-stu-id="9d607-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="9d607-131">Използване на счетоводни книги за записи за записване на разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-131">Use entry journals to record costs</span></span>

<span data-ttu-id="9d607-132">Можете да използвате журнали за вписване за записване на разходи или приходи в класовете материали, такси, време, разходи или данъчни транзакции.</span><span class="sxs-lookup"><span data-stu-id="9d607-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="9d607-133">Списанията могат да се използват за следните цели:</span><span class="sxs-lookup"><span data-stu-id="9d607-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="9d607-134">Записване на действителните разходи за материали и продажби по проект.</span><span class="sxs-lookup"><span data-stu-id="9d607-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="9d607-135">Преместете действителни данни от друга система в Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="9d607-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="9d607-136">Записвайте разходите, възникнали в друга система.</span><span class="sxs-lookup"><span data-stu-id="9d607-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="9d607-137">Тези разходи могат да включват разходи за поръчки или подизпълнители.</span><span class="sxs-lookup"><span data-stu-id="9d607-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9d607-138">Приложението не валидира типа на реда на дневника или свързаното с него ценообразуване, въведено в реда на дневника.</span><span class="sxs-lookup"><span data-stu-id="9d607-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="9d607-139">Следователно само потребител, който е напълно наясно счетоводното въздействие, което действителните имат върху проекта, трябва да използва дневници за въвеждане, за да създава действителни.</span><span class="sxs-lookup"><span data-stu-id="9d607-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="9d607-140">Поради въздействието на този тип списания, трябва внимателно да изберете кой има достъп за създаване на дневници за влизане.</span><span class="sxs-lookup"><span data-stu-id="9d607-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="9d607-141">Записване на действителни данни въз основа на проектни събития</span><span class="sxs-lookup"><span data-stu-id="9d607-141">Record actuals based on project events</span></span>

<span data-ttu-id="9d607-142">Project Operations записва финансовите транзакции, които възникват по време на даден проект.</span><span class="sxs-lookup"><span data-stu-id="9d607-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="9d607-143">Тези транзакции се записват като действителни данни.</span><span class="sxs-lookup"><span data-stu-id="9d607-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="9d607-144">Следващите таблици показват различните видове действителни данни, които се създават в зависимост от това дали проектът е тип време и материали, или с фиксирана цена, дали е в етапа на предварителна продажба, или е вътрешен проект.</span><span class="sxs-lookup"><span data-stu-id="9d607-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="9d607-145">Ресурсът принадлежи към същата организационна единица като единицата на проекта, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="9d607-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="9d607-146">Събитие</span><span class="sxs-lookup"><span data-stu-id="9d607-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="9d607-147">Платими или продадени проекти</span><span class="sxs-lookup"><span data-stu-id="9d607-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="9d607-148">Проект в етапа на предварителна продажба</span><span class="sxs-lookup"><span data-stu-id="9d607-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="9d607-149">Вътрешен проект</span><span class="sxs-lookup"><span data-stu-id="9d607-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="9d607-150">Време и материали</span><span class="sxs-lookup"><span data-stu-id="9d607-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="9d607-151">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="9d607-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="9d607-152">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="9d607-152">Actuals</span></span></th>
<th><span data-ttu-id="9d607-153">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="9d607-153">Transaction currency</span></span></th>
<th><span data-ttu-id="9d607-154">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="9d607-154">Fixed price</span></span></th>
<th><span data-ttu-id="9d607-155">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="9d607-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="9d607-156">Създава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="9d607-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="9d607-157">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="9d607-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-158">Подава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="9d607-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="9d607-159">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="9d607-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="9d607-160">Времето се одобрява и не се получава промяна или увеличаване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="9d607-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="9d607-161">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-161">Cost actual</span></span></td>
<td><span data-ttu-id="9d607-162">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="9d607-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="9d607-163">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="9d607-164">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="9d607-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="9d607-165">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="9d607-166">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-167">Нефактурирани действителни продажби – платими</span><span class="sxs-lookup"><span data-stu-id="9d607-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="9d607-168">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="9d607-169">Времето се одобрява и се получава намаляване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="9d607-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="9d607-170">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-170">Cost actual</span></span></td>
<td><span data-ttu-id="9d607-171">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="9d607-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="9d607-172">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="9d607-173">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="9d607-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="9d607-174">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="9d607-175">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-176">Нефактурирани действителни продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="9d607-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="9d607-177">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-178">Нефактурирани действителни продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="9d607-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="9d607-179">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="9d607-180">Потвърждава се фактура и не се получава промяна или увеличаване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="9d607-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="9d607-181">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="9d607-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="9d607-182">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="9d607-183">Фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="9d607-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="9d607-184">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="9d607-185">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="9d607-186">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-187">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="9d607-187">Billed sales</span></span></td>
<td><span data-ttu-id="9d607-188">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="9d607-189">Потвърждава се фактура и се получава намаляване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="9d607-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="9d607-190">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="9d607-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="9d607-191">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="9d607-192">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="9d607-193">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="9d607-194">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="9d607-195">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-196">Фактурирани продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="9d607-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="9d607-197">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-198">Фактурирани продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="9d607-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="9d607-199">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="9d607-200">Коригира се фактура, за да се увеличи платимото количество.</span><span class="sxs-lookup"><span data-stu-id="9d607-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="9d607-201">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="9d607-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="9d607-202">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="9d607-203">Сторниране на фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="9d607-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="9d607-204">Промяна на състоянието на контролна точка от <strong>Фактурирано</strong> в <strong>Готово за фактуриране</strong></span><span class="sxs-lookup"><span data-stu-id="9d607-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="9d607-205">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="9d607-206">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="9d607-207">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-208">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="9d607-208">Billed sales</span></span></td>
<td><span data-ttu-id="9d607-209">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="9d607-210">Коригира се фактура, за да се намали платимото количество.</span><span class="sxs-lookup"><span data-stu-id="9d607-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="9d607-211">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="9d607-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="9d607-212">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-213">Фактурирани продажби за новото количество</span><span class="sxs-lookup"><span data-stu-id="9d607-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="9d607-214">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-215">Нефактурирани продажби – платими за разликата</span><span class="sxs-lookup"><span data-stu-id="9d607-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="9d607-216">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="9d607-217">Ресурсът принадлежи към организационна единица, която е различна от единицата на проекта, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="9d607-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="9d607-218">Събитие</span><span class="sxs-lookup"><span data-stu-id="9d607-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="9d607-219">Платими или продадени проекти</span><span class="sxs-lookup"><span data-stu-id="9d607-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="9d607-220">Проект в етапа на предварителна продажба</span><span class="sxs-lookup"><span data-stu-id="9d607-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="9d607-221">Вътрешен проект</span><span class="sxs-lookup"><span data-stu-id="9d607-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="9d607-222">Време и материали</span><span class="sxs-lookup"><span data-stu-id="9d607-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="9d607-223">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="9d607-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="9d607-224">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="9d607-224">Actuals</span></span></th>
<th><span data-ttu-id="9d607-225">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="9d607-225">Transaction currency</span></span></th>
<th><span data-ttu-id="9d607-226">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="9d607-226">Fixed price</span></span></th>
<th><span data-ttu-id="9d607-227">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="9d607-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="9d607-228">Създава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="9d607-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="9d607-229">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="9d607-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-230">Подава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="9d607-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="9d607-231">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="9d607-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="9d607-232">Времето се одобрява и не се получава промяна или увеличаване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="9d607-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="9d607-233">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-233">Cost actual</span></span></td>
<td><span data-ttu-id="9d607-234">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="9d607-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="9d607-235">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="9d607-236">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="9d607-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="9d607-237">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="9d607-238">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-239">Нефактурирани действителни продажби – платими</span><span class="sxs-lookup"><span data-stu-id="9d607-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="9d607-240">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-241">Разход на ресурсна единица</span><span class="sxs-lookup"><span data-stu-id="9d607-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="9d607-242">Валута на ресурсната единица</span><span class="sxs-lookup"><span data-stu-id="9d607-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-243">Продажби между организации</span><span class="sxs-lookup"><span data-stu-id="9d607-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="9d607-244">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="9d607-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="9d607-245">Времето се одобрява и се получава намаляване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="9d607-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="9d607-246">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-246">Cost actual</span></span></td>
<td><span data-ttu-id="9d607-247">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="9d607-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="9d607-248">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="9d607-249">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="9d607-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="9d607-250">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="9d607-251">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="9d607-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-252">Разход на ресурсна единица</span><span class="sxs-lookup"><span data-stu-id="9d607-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="9d607-253">Валута на ресурсната единица</span><span class="sxs-lookup"><span data-stu-id="9d607-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-254">Продажби между организации</span><span class="sxs-lookup"><span data-stu-id="9d607-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="9d607-255">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="9d607-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-256">Нефактурирани действителни продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="9d607-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="9d607-257">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-258">Нефактурирани действителни продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="9d607-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="9d607-259">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="9d607-260">Потвърждава се фактура и не се получава промяна или увеличаване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="9d607-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="9d607-261">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="9d607-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="9d607-262">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="9d607-263">Фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="9d607-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="9d607-264">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="9d607-265">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="9d607-266">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-267">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="9d607-267">Billed sales</span></span></td>
<td><span data-ttu-id="9d607-268">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="9d607-269">Потвърждава се фактура и се получава намаляване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="9d607-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="9d607-270">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="9d607-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="9d607-271">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="9d607-272">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="9d607-273">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="9d607-274">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="9d607-275">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-276">Фактурирани продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="9d607-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="9d607-277">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-278">Фактурирани продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="9d607-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="9d607-279">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="9d607-280">Коригира се фактура, за да се увеличи платимото количество.</span><span class="sxs-lookup"><span data-stu-id="9d607-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="9d607-281">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="9d607-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="9d607-282">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="9d607-283">Сторниране на фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="9d607-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="9d607-284">Промяна на състоянието на контролна точка от <strong>Фактурирано</strong> в <strong>Готово за фактуриране</strong></span><span class="sxs-lookup"><span data-stu-id="9d607-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="9d607-285">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="9d607-286">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="9d607-287">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="9d607-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-288">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="9d607-288">Billed sales</span></span></td>
<td><span data-ttu-id="9d607-289">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="9d607-290">Коригира се фактура, за да се намали платимото количество.</span><span class="sxs-lookup"><span data-stu-id="9d607-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="9d607-291">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="9d607-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="9d607-292">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-293">Фактурирани продажби за новото количество</span><span class="sxs-lookup"><span data-stu-id="9d607-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="9d607-294">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="9d607-295">Нефактурирани продажби – платими за разликата</span><span class="sxs-lookup"><span data-stu-id="9d607-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="9d607-296">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="9d607-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
