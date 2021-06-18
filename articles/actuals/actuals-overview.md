---
title: Действителни данни
description: Тази тема предоставя информация за това как да работите с актуални данни в Microsoft Dynamics 365 Project Operations.
author: rumant
ms.date: 04/01/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 78c7a9486d0338adfd7770447f21d17509e654f7
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996598"
---
# <a name="actuals"></a><span data-ttu-id="b1acb-103">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="b1acb-103">Actuals</span></span> 

<span data-ttu-id="b1acb-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="b1acb-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b1acb-105">Фактите представляват прегледания и одобрен финансов и графичен напредък по даден проект.</span><span class="sxs-lookup"><span data-stu-id="b1acb-105">Actuals represent the reviewed and approved financial and schedule progress on a project.</span></span> <span data-ttu-id="b1acb-106">Те са създадени в резултат на одобрение на време, разходи, записи за използване на материали и записи в дневник и фактури.</span><span class="sxs-lookup"><span data-stu-id="b1acb-106">They are created as a result of approval of time, expense, material usage entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="b1acb-107">Счетоводни записи и подаване на време</span><span class="sxs-lookup"><span data-stu-id="b1acb-107">Journal lines and time submission</span></span>

<span data-ttu-id="b1acb-108">За повече информация относно въвеждането на време вижте [Преглед на въвеждането на време](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="b1acb-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="b1acb-109">Време и материали</span><span class="sxs-lookup"><span data-stu-id="b1acb-109">Time and materials</span></span>

<span data-ttu-id="b1acb-110">Когато изпратеният запис за време е свързан с проект, който е съпоставен с ред за договор за време и материали, системата създава два реда на дневника, един за разходи и един за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="b1acb-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="b1acb-111">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="b1acb-111">Fixed price</span></span>

<span data-ttu-id="b1acb-112">При подаване на запис за време, който е свързан с проект, който се съпоставя с ред на договор от тип с фиксирана цена, системата създава един счетоводен запис за разходи.</span><span class="sxs-lookup"><span data-stu-id="b1acb-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="b1acb-113">Ценообразуване по подразбиране</span><span class="sxs-lookup"><span data-stu-id="b1acb-113">Default pricing</span></span>

<span data-ttu-id="b1acb-114">Логиката за създаване на цени по подразбиране се намира в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="b1acb-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="b1acb-115">Стойностите на полета от запис за време се копират в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="b1acb-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="b1acb-116">Тези стойности включват датата на транзакцията, реда на договора, с който е съпоставен проектът, и резултата от валутата в съответната ценова листа.</span><span class="sxs-lookup"><span data-stu-id="b1acb-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="b1acb-117">Полетата, които влияят на ценообразуването по подразбиране, като например **Роля** и **Ресурсна единица**, се използват за определяне на съответна цена по подразбиране в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="b1acb-117">The fields that affect default pricing, such as **Role** and **Resourcing Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="b1acb-118">Можете да добавите персонализирано поле за въвеждане на час.</span><span class="sxs-lookup"><span data-stu-id="b1acb-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="b1acb-119">Ако искате стойността на полето да се разпространява към действителни, създайте полето в таблиците **Действителни данни** и **счетоводен запис**.</span><span class="sxs-lookup"><span data-stu-id="b1acb-119">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="b1acb-120">Използвайте персонализиран код, за да разпространите избраната стойност на полето от Time Entry към Actuals през реда на дневника, като използвате източници на транзакции.</span><span class="sxs-lookup"><span data-stu-id="b1acb-120">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="b1acb-121">За повече информация относно произхода на транзакциите и връзките вижте [Свързване на факти с оригинални записи](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="b1acb-121">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="b1acb-122">Редове на списания и представяне на основните разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-122">Journal lines and basic expense submission</span></span>

<span data-ttu-id="b1acb-123">За повече информация относно запис за разходи вижте [Преглед на разход](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="b1acb-123">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="b1acb-124">Време и материали</span><span class="sxs-lookup"><span data-stu-id="b1acb-124">Time and materials</span></span>

<span data-ttu-id="b1acb-125">Когато основен запис за разход е свързан с проект, който е съпоставен с ред за договор за време и материали, системата създава два реда на дневника, един за разходи и един за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="b1acb-125">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="b1acb-126">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="b1acb-126">Fixed price</span></span>

<span data-ttu-id="b1acb-127">Когато подаден запис за основен разход е свързан към проект, който се съпоставя с ред на договор от тип с фиксирана цена, системата създава един счетоводен запис за разходи.</span><span class="sxs-lookup"><span data-stu-id="b1acb-127">When a submitted basic expense entry is linked to a project that's mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="b1acb-128">Ценообразуване по подразбиране</span><span class="sxs-lookup"><span data-stu-id="b1acb-128">Default pricing</span></span>

<span data-ttu-id="b1acb-129">Логиката за въвеждане на цени по подразбиране за разходи се основава на категорията на разходите.</span><span class="sxs-lookup"><span data-stu-id="b1acb-129">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="b1acb-130">Датата на транзакцията, редът на договора, с който е съпоставен проектът, и валутата се използват за определяне на съответната ценова листа.</span><span class="sxs-lookup"><span data-stu-id="b1acb-130">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="b1acb-131">Полетата, които влияят на ценообразуването по подразбиране, като например **Категория на трансакция** и **Ресурсна единица**, се използват за определяне на съответна цена по подразбиране в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="b1acb-131">The fields that affect default pricing, such as **Transaction Category** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="b1acb-132">Това обаче работи само когато методът за ценообразуване в ценовата листа е **единична цена**.</span><span class="sxs-lookup"><span data-stu-id="b1acb-132">However, this only works when the pricing method in the price list is **Price per unit**.</span></span> <span data-ttu-id="b1acb-133">Ако методът на ценообразуване е **На цена** или **Надценка над разходите**, цената, въведена при създаване на запис на разходите, се използва за себестойност и цената в реда на дневника за продажби се изчислява въз основа на метода на ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="b1acb-133">If pricing method is **At cost** or **Markup over cost**, the price entered when the expense entry is created is used for cost and the price on the sales journal line is calculated based on the pricing method.</span></span> 

<span data-ttu-id="b1acb-134">Можете да добавите персонализирано поле към записа за разходи.</span><span class="sxs-lookup"><span data-stu-id="b1acb-134">You can add a custom field on the expense entry.</span></span> <span data-ttu-id="b1acb-135">Ако искате стойността на полето да се разпространява към действителни, създайте полето в таблиците **Действителни данни** и **счетоводен запис**.</span><span class="sxs-lookup"><span data-stu-id="b1acb-135">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="b1acb-136">Използвайте персонализиран код, за да разпространите избраната стойност на полето от Time Entry към Actuals през реда на дневника, като използвате източници на транзакции.</span><span class="sxs-lookup"><span data-stu-id="b1acb-136">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="b1acb-137">За повече информация относно произхода на транзакциите и връзките вижте [Свързване на факти с оригинални записи](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="b1acb-137">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-material-usage-log-submission"></a><span data-ttu-id="b1acb-138">Редове на списания и подаване на дневник за използване на материали</span><span class="sxs-lookup"><span data-stu-id="b1acb-138">Journal lines and material usage log submission</span></span>

<span data-ttu-id="b1acb-139">За повече информация относно записването на разходите вижте [Дневник на използването на материала](../material/material-usage-log.md).</span><span class="sxs-lookup"><span data-stu-id="b1acb-139">For more information about expense entry, see [Material Usage Log](../material/material-usage-log.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="b1acb-140">Време и материали</span><span class="sxs-lookup"><span data-stu-id="b1acb-140">Time and materials</span></span>

<span data-ttu-id="b1acb-141">Когато изпратеният запис в дневника за използване на материали е свързан с проект, който е съпоставен с ред за договор за време и материали, системата създава два реда на дневника, един за разходи и един за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="b1acb-141">When a submitted material usage log entry is linked to a project that is mapped to a time and materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="b1acb-142">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="b1acb-142">Fixed price</span></span>

<span data-ttu-id="b1acb-143">Когато подаден запис на регистрационен файл за използване на материал е свързан към проект, който се съпоставя с ред на договор от тип с фиксирана цена, системата създава един счетоводен запис за разходи.</span><span class="sxs-lookup"><span data-stu-id="b1acb-143">When a submitted material usage log entry is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="b1acb-144">Ценообразуване по подразбиране</span><span class="sxs-lookup"><span data-stu-id="b1acb-144">Default pricing</span></span>

<span data-ttu-id="b1acb-145">Логиката за въвеждане на цени по подразбиране за материал се основава на комбинацията от продукт и единица.</span><span class="sxs-lookup"><span data-stu-id="b1acb-145">The logic for entering default prices for material is based on the product and unit combination.</span></span> <span data-ttu-id="b1acb-146">Датата на транзакцията, редът на договора, с който е съпоставен проектът, и валутата се използват за определяне на съответната ценова листа.</span><span class="sxs-lookup"><span data-stu-id="b1acb-146">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="b1acb-147">Полетата, които влияят на ценообразуването по подразбиране, като например **ИД на продукт** и **единица**, се използват за определяне на съответна цена по подразбиране в счетоводния запис.</span><span class="sxs-lookup"><span data-stu-id="b1acb-147">The fields that affect default pricing, such as **Product ID** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="b1acb-148">Това обаче работи само за каталожни продукти.</span><span class="sxs-lookup"><span data-stu-id="b1acb-148">However, this only works for catalog products.</span></span> <span data-ttu-id="b1acb-149">За продукти за вписване, цената, въведена при създаване на запис в дневника за използване на материали, се използва за себестойност и продажна цена в редовете на дневника.</span><span class="sxs-lookup"><span data-stu-id="b1acb-149">For write-in products, the price entered when the material usage log entry is created is used for cost and sales price on the journal lines.</span></span> 

<span data-ttu-id="b1acb-150">Можете да добавите персонализирано поле към записа **Регистрационен файл за използване на материал**.</span><span class="sxs-lookup"><span data-stu-id="b1acb-150">You can add a custom field on the **Material Usage Log** entry.</span></span> <span data-ttu-id="b1acb-151">Ако искате стойността на полето да се разпространява към действителни, създайте полето в таблиците **Действителни данни** и **счетоводен запис**.</span><span class="sxs-lookup"><span data-stu-id="b1acb-151">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="b1acb-152">Използвайте персонализиран код, за да разпространите избраната стойност на полето от Time Entry към Actuals през реда на дневника, като използвате източници на транзакции.</span><span class="sxs-lookup"><span data-stu-id="b1acb-152">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="b1acb-153">За повече информация относно произхода на транзакциите и връзките вижте [Свързване на факти с оригинални записи](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="b1acb-153">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="b1acb-154">Използване на счетоводни книги за записи за записване на разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-154">Use entry journals to record costs</span></span>

<span data-ttu-id="b1acb-155">Можете да използвате журнали за вписване за записване на разходи или приходи в класовете материали, такси, време, разходи или данъчни транзакции.</span><span class="sxs-lookup"><span data-stu-id="b1acb-155">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="b1acb-156">Списанията могат да се използват за следните цели:</span><span class="sxs-lookup"><span data-stu-id="b1acb-156">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="b1acb-157">Преместване на действителни данни от транзакции от друга система в Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="b1acb-157">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="b1acb-158">Записвайте разходите, възникнали в друга система.</span><span class="sxs-lookup"><span data-stu-id="b1acb-158">Record costs that occurred in another system.</span></span> <span data-ttu-id="b1acb-159">Тези разходи могат да включват разходи за поръчки или подизпълнители.</span><span class="sxs-lookup"><span data-stu-id="b1acb-159">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b1acb-160">Приложението не валидира типа на реда на дневника или свързаното с него ценообразуване, въведено в реда на дневника.</span><span class="sxs-lookup"><span data-stu-id="b1acb-160">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="b1acb-161">Следователно само потребител, който е напълно наясно счетоводното въздействие, което действителните имат върху проекта, трябва да използва дневници за въвеждане, за да създава действителни.</span><span class="sxs-lookup"><span data-stu-id="b1acb-161">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="b1acb-162">Поради въздействието на този тип списания, трябва внимателно да изберете кой има достъп за създаване на дневници за влизане.</span><span class="sxs-lookup"><span data-stu-id="b1acb-162">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>

## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="b1acb-163">Записване на действителни данни въз основа на проектни събития</span><span class="sxs-lookup"><span data-stu-id="b1acb-163">Record actuals based on project events</span></span>

<span data-ttu-id="b1acb-164">Project Operations записва финансовите транзакции, които възникват по време на даден проект.</span><span class="sxs-lookup"><span data-stu-id="b1acb-164">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="b1acb-165">Тези транзакции се записват като действителни данни.</span><span class="sxs-lookup"><span data-stu-id="b1acb-165">These transactions are recorded as actuals.</span></span> <span data-ttu-id="b1acb-166">Следващите таблици показват различните видове действителни данни, които се създават в зависимост от това дали проектът е тип време и материали, или с фиксирана цена, дали е в етапа на предварителна продажба, или е вътрешен проект.</span><span class="sxs-lookup"><span data-stu-id="b1acb-166">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="b1acb-167">Ресурсът принадлежи към същата организационна единица като единицата на проекта, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="b1acb-167">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="b1acb-168">Събитие</span><span class="sxs-lookup"><span data-stu-id="b1acb-168">Event</span></span></th>
<th colspan="4"><span data-ttu-id="b1acb-169">Платими или продадени проекти</span><span class="sxs-lookup"><span data-stu-id="b1acb-169">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="b1acb-170">Проект в етапа на предварителна продажба</span><span class="sxs-lookup"><span data-stu-id="b1acb-170">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="b1acb-171">Вътрешен проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-171">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="b1acb-172">Време и материали</span><span class="sxs-lookup"><span data-stu-id="b1acb-172">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="b1acb-173">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="b1acb-173">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="b1acb-174">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="b1acb-174">Actuals</span></span></th>
<th><span data-ttu-id="b1acb-175">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="b1acb-175">Transaction currency</span></span></th>
<th><span data-ttu-id="b1acb-176">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="b1acb-176">Fixed price</span></span></th>
<th><span data-ttu-id="b1acb-177">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="b1acb-177">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="b1acb-178">Създава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="b1acb-178">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="b1acb-179">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="b1acb-179">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-180">Подава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="b1acb-180">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="b1acb-181">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="b1acb-181">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="b1acb-182">Времето се одобрява и не се получава промяна или увеличаване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="b1acb-182">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="b1acb-183">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-183">Cost actual</span></span></td>
<td><span data-ttu-id="b1acb-184">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="b1acb-184">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="b1acb-185">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-185">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="b1acb-186">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="b1acb-186">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="b1acb-187">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-187">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="b1acb-188">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-188">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-189">Нефактурирани действителни продажби – платими</span><span class="sxs-lookup"><span data-stu-id="b1acb-189">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="b1acb-190">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="b1acb-191">Времето се одобрява и се получава намаляване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="b1acb-191">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="b1acb-192">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-192">Cost actual</span></span></td>
<td><span data-ttu-id="b1acb-193">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="b1acb-193">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="b1acb-194">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-194">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="b1acb-195">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="b1acb-195">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="b1acb-196">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-196">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="b1acb-197">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-197">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-198">Нефактурирани действителни продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="b1acb-198">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="b1acb-199">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-199">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-200">Нефактурирани действителни продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="b1acb-200">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="b1acb-201">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-201">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="b1acb-202">Потвърждава се фактура и не се получава промяна или увеличаване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="b1acb-202">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="b1acb-203">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="b1acb-203">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="b1acb-204">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-204">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="b1acb-205">Фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="b1acb-205">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="b1acb-206">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-206">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="b1acb-207">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-207">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="b1acb-208">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-208">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-209">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="b1acb-209">Billed sales</span></span></td>
<td><span data-ttu-id="b1acb-210">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-210">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="b1acb-211">Потвърждава се фактура и се получава намаляване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="b1acb-211">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="b1acb-212">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="b1acb-212">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="b1acb-213">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-213">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="b1acb-214">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-214">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="b1acb-215">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-215">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="b1acb-216">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-216">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="b1acb-217">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-217">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-218">Фактурирани продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="b1acb-218">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="b1acb-219">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-219">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-220">Фактурирани продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="b1acb-220">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="b1acb-221">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-221">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="b1acb-222">Коригира се фактура, за да се увеличи платимото количество.</span><span class="sxs-lookup"><span data-stu-id="b1acb-222">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="b1acb-223">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="b1acb-223">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="b1acb-224">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-224">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="b1acb-225">Сторниране на фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="b1acb-225">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="b1acb-226">Промяна на състоянието на контролна точка от <strong>Фактурирано</strong> в <strong>Готово за фактуриране</strong></span><span class="sxs-lookup"><span data-stu-id="b1acb-226">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="b1acb-227">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-227">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="b1acb-228">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-228">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="b1acb-229">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-229">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-230">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="b1acb-230">Billed sales</span></span></td>
<td><span data-ttu-id="b1acb-231">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-231">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="b1acb-232">Коригира се фактура, за да се намали платимото количество.</span><span class="sxs-lookup"><span data-stu-id="b1acb-232">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="b1acb-233">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="b1acb-233">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="b1acb-234">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-235">Фактурирани продажби за новото количество</span><span class="sxs-lookup"><span data-stu-id="b1acb-235">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="b1acb-236">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-236">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-237">Нефактурирани продажби – платими за разликата</span><span class="sxs-lookup"><span data-stu-id="b1acb-237">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="b1acb-238">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-238">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="b1acb-239">Ресурсът принадлежи към организационна единица, която е различна от единицата на проекта, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="b1acb-239">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="b1acb-240">Събитие</span><span class="sxs-lookup"><span data-stu-id="b1acb-240">Event</span></span></th>
<th colspan="4"><span data-ttu-id="b1acb-241">Платими или продадени проекти</span><span class="sxs-lookup"><span data-stu-id="b1acb-241">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="b1acb-242">Проект в етапа на предварителна продажба</span><span class="sxs-lookup"><span data-stu-id="b1acb-242">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="b1acb-243">Вътрешен проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-243">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="b1acb-244">Време и материали</span><span class="sxs-lookup"><span data-stu-id="b1acb-244">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="b1acb-245">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="b1acb-245">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="b1acb-246">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="b1acb-246">Actuals</span></span></th>
<th><span data-ttu-id="b1acb-247">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="b1acb-247">Transaction currency</span></span></th>
<th><span data-ttu-id="b1acb-248">Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="b1acb-248">Fixed price</span></span></th>
<th><span data-ttu-id="b1acb-249">Валута на транзакцията</span><span class="sxs-lookup"><span data-stu-id="b1acb-249">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="b1acb-250">Създава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="b1acb-250">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="b1acb-251">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="b1acb-251">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-252">Подава се запис за време.</span><span class="sxs-lookup"><span data-stu-id="b1acb-252">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="b1acb-253">Няма дейност в обекта „Действителни данни“</span><span class="sxs-lookup"><span data-stu-id="b1acb-253">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="b1acb-254">Времето се одобрява и не се получава промяна или увеличаване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="b1acb-254">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="b1acb-255">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-255">Cost actual</span></span></td>
<td><span data-ttu-id="b1acb-256">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="b1acb-256">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="b1acb-257">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-257">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="b1acb-258">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="b1acb-258">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="b1acb-259">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-259">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="b1acb-260">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-260">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-261">Нефактурирани действителни продажби – платими</span><span class="sxs-lookup"><span data-stu-id="b1acb-261">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="b1acb-262">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-262">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-263">Разход на ресурсна единица</span><span class="sxs-lookup"><span data-stu-id="b1acb-263">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="b1acb-264">Валута на ресурсната единица</span><span class="sxs-lookup"><span data-stu-id="b1acb-264">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-265">Продажби между организации</span><span class="sxs-lookup"><span data-stu-id="b1acb-265">Interorganizational sales</span></span></td>
<td><span data-ttu-id="b1acb-266">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="b1acb-266">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="b1acb-267">Времето се одобрява и се получава намаляване на платимите часове по време на одобрение.</span><span class="sxs-lookup"><span data-stu-id="b1acb-267">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="b1acb-268">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-268">Cost actual</span></span></td>
<td><span data-ttu-id="b1acb-269">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="b1acb-269">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="b1acb-270">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-270">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="b1acb-271">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="b1acb-271">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="b1acb-272">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-272">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="b1acb-273">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="b1acb-273">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-274">Разход на ресурсна единица</span><span class="sxs-lookup"><span data-stu-id="b1acb-274">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="b1acb-275">Валута на ресурсната единица</span><span class="sxs-lookup"><span data-stu-id="b1acb-275">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-276">Продажби между организации</span><span class="sxs-lookup"><span data-stu-id="b1acb-276">Interorganizational sales</span></span></td>
<td><span data-ttu-id="b1acb-277">Валута на единицата, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="b1acb-277">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-278">Нефактурирани действителни продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="b1acb-278">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="b1acb-279">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-279">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-280">Нефактурирани действителни продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="b1acb-280">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="b1acb-281">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-281">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="b1acb-282">Потвърждава се фактура и не се получава промяна или увеличаване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="b1acb-282">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="b1acb-283">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="b1acb-283">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="b1acb-284">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-284">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="b1acb-285">Фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="b1acb-285">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="b1acb-286">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-286">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="b1acb-287">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-287">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="b1acb-288">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-288">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-289">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="b1acb-289">Billed sales</span></span></td>
<td><span data-ttu-id="b1acb-290">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-290">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="b1acb-291">Потвърждава се фактура и се получава намаляване на платимите часове.</span><span class="sxs-lookup"><span data-stu-id="b1acb-291">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="b1acb-292">Сторниране на нефактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="b1acb-292">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="b1acb-293">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-293">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="b1acb-294">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-294">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="b1acb-295">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-295">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="b1acb-296">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-296">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="b1acb-297">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-297">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-298">Фактурирани продажби – платими за новото количество</span><span class="sxs-lookup"><span data-stu-id="b1acb-298">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="b1acb-299">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-299">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-300">Фактурирани продажби – неплатими за разликата</span><span class="sxs-lookup"><span data-stu-id="b1acb-300">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="b1acb-301">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-301">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="b1acb-302">Коригира се фактура, за да се увеличи платимото количество.</span><span class="sxs-lookup"><span data-stu-id="b1acb-302">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="b1acb-303">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="b1acb-303">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="b1acb-304">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-304">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="b1acb-305">Сторниране на фактурирани продажби за контролна точка</span><span class="sxs-lookup"><span data-stu-id="b1acb-305">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="b1acb-306">Промяна на състоянието на контролна точка от <strong>Фактурирано</strong> в <strong>Готово за фактуриране</strong></span><span class="sxs-lookup"><span data-stu-id="b1acb-306">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="b1acb-307">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-307">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="b1acb-308">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-308">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="b1acb-309">Неприложимо</span><span class="sxs-lookup"><span data-stu-id="b1acb-309">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-310">Фактурирани продажби</span><span class="sxs-lookup"><span data-stu-id="b1acb-310">Billed sales</span></span></td>
<td><span data-ttu-id="b1acb-311">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-311">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="b1acb-312">Коригира се фактура, за да се намали платимото количество.</span><span class="sxs-lookup"><span data-stu-id="b1acb-312">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="b1acb-313">Фактурирани продажби – сторниране</span><span class="sxs-lookup"><span data-stu-id="b1acb-313">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="b1acb-314">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-314">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-315">Фактурирани продажби за новото количество</span><span class="sxs-lookup"><span data-stu-id="b1acb-315">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="b1acb-316">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-316">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="b1acb-317">Нефактурирани продажби – платими за разликата</span><span class="sxs-lookup"><span data-stu-id="b1acb-317">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="b1acb-318">Валута на договор по проект</span><span class="sxs-lookup"><span data-stu-id="b1acb-318">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
