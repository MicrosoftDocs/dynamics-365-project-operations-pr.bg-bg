---
title: Действителни данни
description: Тази тема предоставя информация за това как да работите с актуални данни в Microsoft Dynamics 365 Project Operations.
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
ms.openlocfilehash: 6a94bd143b0d0dad2a08511a34e592a057b6d2a1
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291786"
---
# <a name="actuals"></a><span data-ttu-id="7706f-103">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="7706f-103">Actuals</span></span> 

<span data-ttu-id="7706f-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="7706f-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="7706f-105">Действителните данни са количеството работа, завършена по даден проект.</span><span class="sxs-lookup"><span data-stu-id="7706f-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="7706f-106">Те се създават в резултат на записи за време и разходи и записи в дневник и фактури.</span><span class="sxs-lookup"><span data-stu-id="7706f-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="7706f-107">Счетоводни записи и подаване на време</span><span class="sxs-lookup"><span data-stu-id="7706f-107">Journal lines and time submission</span></span>

<span data-ttu-id="7706f-108">За повече информация относно въвеждането на време вижте [Преглед на въвеждането на време](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="7706f-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="7706f-109">Време и материали</span><span class="sxs-lookup"><span data-stu-id="7706f-109">Time and materials</span></span>

<span data-ttu-id="7706f-110">Когато изпратеният запис за време е свързан с проект, който е съпоставен с ред за договор за време и материали, системата създава два реда на дневника, един за разходи и един за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="7706f-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="7706f-111">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="7706f-111">Fixed price</span></span>

<span data-ttu-id="7706f-112">При подаване на запис за време, който е свързан с проект, който се съпоставя с ред на договор от тип с фиксирана цена, системата създава един счетоводен запис за разходи.</span><span class="sxs-lookup"><span data-stu-id="7706f-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="7706f-113">Ценообразуване по подразбиране</span><span class="sxs-lookup"><span data-stu-id="7706f-113">Default pricing</span></span>

<span data-ttu-id="7706f-114">Логиката за създаване на цени по подразбиране се намира в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="7706f-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="7706f-115">Стойностите на полета от запис за време се копират в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="7706f-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="7706f-116">Тези стойности включват датата на транзакцията, реда на договора, с който е съпоставен проектът, и резултата от валутата в съответната ценова листа.</span><span class="sxs-lookup"><span data-stu-id="7706f-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="7706f-117">Полетата, които влияят на цените по подразбиране, като например **Роля** и **Организационна единица**, се използват за определяне на съответна цена по подразбиране в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="7706f-117">The fields that affect default pricing, such as **Role** and **Org Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="7706f-118">Можете да добавите персонализирано поле за въвеждане на час.</span><span class="sxs-lookup"><span data-stu-id="7706f-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="7706f-119">Ако искате стойността на полето да се попълни в действителните данни, създайте полето в обекта „Действителни данни“ и използвайте съпоставяния на полета, за да копирате полето от записа за време в действителните данни.</span><span class="sxs-lookup"><span data-stu-id="7706f-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="7706f-120">Редове на списания и представяне на основните разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="7706f-121">За повече информация относно запис за разходи вижте [Преглед на разход](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="7706f-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="7706f-122">Време и материали</span><span class="sxs-lookup"><span data-stu-id="7706f-122">Time and materials</span></span>

<span data-ttu-id="7706f-123">Когато основен запис за разход е свързан с проект, който е съпоставен с ред за договор за време и материали, системата създава два реда на дневника, един за разходи и един за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="7706f-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="7706f-124">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="7706f-124">Fixed price</span></span>

<span data-ttu-id="7706f-125">При основен запис за разход, който е свързан с проект, който се съпоставя с ред на договор от тип с фиксирана цена, системата създава един счетоводен запис за разходи.</span><span class="sxs-lookup"><span data-stu-id="7706f-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="7706f-126">Ценообразуване по подразбиране</span><span class="sxs-lookup"><span data-stu-id="7706f-126">Default pricing</span></span>

<span data-ttu-id="7706f-127">Логиката за въвеждане на цени по подразбиране за разходи се основава на категорията на разходите.</span><span class="sxs-lookup"><span data-stu-id="7706f-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="7706f-128">Датата на транзакцията, редът на договора, с който е съпоставен проектът, и валутата се използват за определяне на съответната ценова листа.</span><span class="sxs-lookup"><span data-stu-id="7706f-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="7706f-129">За самата цена обаче по подразбиране сумата, въведена за самата цена, се задава директно в свързаните счетоводни записи за разходи и продажби.</span><span class="sxs-lookup"><span data-stu-id="7706f-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="7706f-130">Базиран на категория запис на единични цени по подразбиране за записи за разходи.</span><span class="sxs-lookup"><span data-stu-id="7706f-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="7706f-131">Използване на счетоводни книги за записи за записване на разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-131">Use entry journals to record costs</span></span>

<span data-ttu-id="7706f-132">Можете да използвате журнали за вписване за записване на разходи или приходи в класовете материали, такси, време, разходи или данъчни транзакции.</span><span class="sxs-lookup"><span data-stu-id="7706f-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="7706f-133">Списанията могат да се използват за следните цели:</span><span class="sxs-lookup"><span data-stu-id="7706f-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="7706f-134">Записване на действителните разходи за материали и продажби по проект.</span><span class="sxs-lookup"><span data-stu-id="7706f-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="7706f-135">Преместване на действителни данни от транзакции от друга система в Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="7706f-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="7706f-136">Записвайте разходите, възникнали в друга система.</span><span class="sxs-lookup"><span data-stu-id="7706f-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="7706f-137">Тези разходи могат да включват разходи за поръчки или подизпълнители.</span><span class="sxs-lookup"><span data-stu-id="7706f-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7706f-138">Приложението не валидира типа на реда на дневника или свързаното с него ценообразуване, въведено в реда на дневника.</span><span class="sxs-lookup"><span data-stu-id="7706f-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="7706f-139">Следователно само потребител, който е напълно наясно счетоводното въздействие, което действителните имат върху проекта, трябва да използва дневници за въвеждане, за да създава действителни.</span><span class="sxs-lookup"><span data-stu-id="7706f-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="7706f-140">Поради въздействието на този тип списания, трябва внимателно да изберете кой има достъп за създаване на дневници за влизане.</span><span class="sxs-lookup"><span data-stu-id="7706f-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="7706f-141">Записване на действителни данни въз основа на проектни събития</span><span class="sxs-lookup"><span data-stu-id="7706f-141">Record actuals based on project events</span></span>

<span data-ttu-id="7706f-142">Project Operations записва финансовите транзакции, които възникват по време на даден проект.</span><span class="sxs-lookup"><span data-stu-id="7706f-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="7706f-143">Тези транзакции се записват като действителни данни.</span><span class="sxs-lookup"><span data-stu-id="7706f-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="7706f-144">Следващите таблици показват различните видове действителни данни, които се създават в зависимост от това дали проектът е тип време и материали, или с фиксирана цена, дали е в етапа на предварителна продажба, или е вътрешен проект.</span><span class="sxs-lookup"><span data-stu-id="7706f-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="7706f-145">Ресурсът принадлежи към същата организационна единица като единицата на проекта, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7706f-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="7706f-146">Събитие</span><span class="sxs-lookup"><span data-stu-id="7706f-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="7706f-147">Платими или продадени проекти</span><span class="sxs-lookup"><span data-stu-id="7706f-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="7706f-148">Проект в етапа на предварителна продажба</span><span class="sxs-lookup"><span data-stu-id="7706f-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="7706f-149">Вътрешен проект</span><span class="sxs-lookup"><span data-stu-id="7706f-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="7706f-150">Време и материали</span><span class="sxs-lookup"><span data-stu-id="7706f-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="7706f-151">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="7706f-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="7706f-152">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="7706f-152">Actuals</span></span></th>
<th><span data-ttu-id="7706f-153">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="7706f-153">Transaction currency</span></span></th>
<th><span data-ttu-id="7706f-154">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="7706f-154">Fixed price</span></span></th>
<th><span data-ttu-id="7706f-155">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="7706f-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="7706f-156">Създава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="7706f-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="7706f-157">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="7706f-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-158">Подава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="7706f-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="7706f-159">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="7706f-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7706f-160">Времето се одобрява и не се получава промяна или увеличаване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="7706f-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7706f-161">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-161">Cost actual</span></span></td>
<td><span data-ttu-id="7706f-162">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7706f-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7706f-163">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="7706f-164">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7706f-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="7706f-165">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="7706f-166">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-167">Нефактурирани действителни продажби – платими</span><span class="sxs-lookup"><span data-stu-id="7706f-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="7706f-168">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7706f-169">Времето се одобрява и се получава намаляване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="7706f-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7706f-170">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-170">Cost actual</span></span></td>
<td><span data-ttu-id="7706f-171">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7706f-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7706f-172">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="7706f-173">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7706f-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7706f-174">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="7706f-175">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-176">Нефактурирани действителни продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="7706f-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7706f-177">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-178">Нефактурирани действителни продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="7706f-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7706f-179">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7706f-180">Потвърждава се фактура и не се получава промяна или увеличаване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="7706f-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7706f-181">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7706f-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7706f-182">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7706f-183">Фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="7706f-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="7706f-184">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7706f-185">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="7706f-186">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-187">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7706f-187">Billed sales</span></span></td>
<td><span data-ttu-id="7706f-188">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7706f-189">Потвърждава се фактура и се получава намаляване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="7706f-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7706f-190">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7706f-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7706f-191">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7706f-192">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7706f-193">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7706f-194">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7706f-195">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-196">Фактурирани продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="7706f-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7706f-197">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-198">Фактурирани продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="7706f-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7706f-199">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7706f-200">Коригира се фактура, за да се увеличи платимото количество.</span><span class="sxs-lookup"><span data-stu-id="7706f-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7706f-201">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="7706f-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7706f-202">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="7706f-203">Сторниране на фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="7706f-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="7706f-204">Промяна на състоянието на контролна точка от <strong>Фактурирано</strong> в <strong>Готово за фактуриране</strong></span><span class="sxs-lookup"><span data-stu-id="7706f-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="7706f-205">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7706f-206">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="7706f-207">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-208">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7706f-208">Billed sales</span></span></td>
<td><span data-ttu-id="7706f-209">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7706f-210">Коригира се фактура, за да се намали платимото количество.</span><span class="sxs-lookup"><span data-stu-id="7706f-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7706f-211">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="7706f-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7706f-212">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-213">Фактурирани продажби за новото количество</span><span class="sxs-lookup"><span data-stu-id="7706f-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="7706f-214">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-215">Нефактурирани продажби – платими за разликата</span><span class="sxs-lookup"><span data-stu-id="7706f-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="7706f-216">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="7706f-217">Ресурсът принадлежи към организационна единица, която е различна от единицата на проекта, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7706f-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="7706f-218">Събитие</span><span class="sxs-lookup"><span data-stu-id="7706f-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="7706f-219">Платими или продадени проекти</span><span class="sxs-lookup"><span data-stu-id="7706f-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="7706f-220">Проект в етапа на предварителна продажба</span><span class="sxs-lookup"><span data-stu-id="7706f-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="7706f-221">Вътрешен проект</span><span class="sxs-lookup"><span data-stu-id="7706f-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="7706f-222">Време и материали</span><span class="sxs-lookup"><span data-stu-id="7706f-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="7706f-223">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="7706f-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="7706f-224">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="7706f-224">Actuals</span></span></th>
<th><span data-ttu-id="7706f-225">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="7706f-225">Transaction currency</span></span></th>
<th><span data-ttu-id="7706f-226">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="7706f-226">Fixed price</span></span></th>
<th><span data-ttu-id="7706f-227">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="7706f-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="7706f-228">Създава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="7706f-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="7706f-229">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="7706f-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-230">Подава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="7706f-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="7706f-231">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="7706f-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="7706f-232">Времето се одобрява и не се получава промяна или увеличаване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="7706f-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7706f-233">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-233">Cost actual</span></span></td>
<td><span data-ttu-id="7706f-234">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7706f-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="7706f-235">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="7706f-236">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7706f-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="7706f-237">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="7706f-238">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-239">Нефактурирани действителни продажби – платими</span><span class="sxs-lookup"><span data-stu-id="7706f-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="7706f-240">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-241">Разход на ресурсна единица</span><span class="sxs-lookup"><span data-stu-id="7706f-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="7706f-242">Валута на ресурсната единица</span><span class="sxs-lookup"><span data-stu-id="7706f-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-243">Продажби между организации</span><span class="sxs-lookup"><span data-stu-id="7706f-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="7706f-244">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7706f-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="7706f-245">Времето се одобрява и се получава намаляване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="7706f-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7706f-246">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-246">Cost actual</span></span></td>
<td><span data-ttu-id="7706f-247">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7706f-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7706f-248">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="7706f-249">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7706f-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7706f-250">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="7706f-251">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="7706f-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-252">Разход на ресурсна единица</span><span class="sxs-lookup"><span data-stu-id="7706f-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="7706f-253">Валута на ресурсната единица</span><span class="sxs-lookup"><span data-stu-id="7706f-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-254">Продажби между организации</span><span class="sxs-lookup"><span data-stu-id="7706f-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="7706f-255">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="7706f-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-256">Нефактурирани действителни продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="7706f-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7706f-257">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-258">Нефактурирани действителни продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="7706f-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7706f-259">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7706f-260">Потвърждава се фактура и не се получава промяна или увеличаване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="7706f-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7706f-261">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7706f-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7706f-262">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7706f-263">Фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="7706f-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="7706f-264">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7706f-265">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="7706f-266">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-267">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7706f-267">Billed sales</span></span></td>
<td><span data-ttu-id="7706f-268">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7706f-269">Потвърждава се фактура и се получава намаляване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="7706f-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7706f-270">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7706f-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7706f-271">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7706f-272">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7706f-273">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7706f-274">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7706f-275">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-276">Фактурирани продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="7706f-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7706f-277">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-278">Фактурирани продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="7706f-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7706f-279">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7706f-280">Коригира се фактура, за да се увеличи платимото количество.</span><span class="sxs-lookup"><span data-stu-id="7706f-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7706f-281">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="7706f-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7706f-282">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="7706f-283">Сторниране на фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="7706f-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="7706f-284">Промяна на състоянието на контролна точка от <strong>Фактурирано</strong> в <strong>Готово за фактуриране</strong></span><span class="sxs-lookup"><span data-stu-id="7706f-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="7706f-285">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7706f-286">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="7706f-287">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="7706f-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-288">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="7706f-288">Billed sales</span></span></td>
<td><span data-ttu-id="7706f-289">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7706f-290">Коригира се фактура, за да се намали платимото количество.</span><span class="sxs-lookup"><span data-stu-id="7706f-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7706f-291">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="7706f-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7706f-292">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-293">Фактурирани продажби за новото количество</span><span class="sxs-lookup"><span data-stu-id="7706f-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="7706f-294">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7706f-295">Нефактурирани продажби – платими за разликата</span><span class="sxs-lookup"><span data-stu-id="7706f-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="7706f-296">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="7706f-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]