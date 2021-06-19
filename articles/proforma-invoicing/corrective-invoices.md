---
title: Коригиращи базирани на проект фактури
description: Тази тема предоставя информация за това как да създавате и потвърждавате коригиращи фактури, базирани на проекти в Project Operations.
author: rumant
ms.date: 03/29/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f6b6670f823577bf7f784443f97f0b77e1e9a6aa
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012258"
---
# <a name="corrective-project-based-invoices"></a><span data-ttu-id="ef742-103">Коригиращи базирани на проект фактури</span><span class="sxs-lookup"><span data-stu-id="ef742-103">Corrective project-based invoices</span></span>

<span data-ttu-id="ef742-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="ef742-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="ef742-105">Потвърдена фактура за проект може да бъде коригирана, за да обработи промени или кредити, както е договорено с клиента и мениджъра на проекта.</span><span class="sxs-lookup"><span data-stu-id="ef742-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="ef742-106">За да редактирате потвърдена фактура, отворете потвърдената фактура и изберете **Коригирайте тази фактура**.</span><span class="sxs-lookup"><span data-stu-id="ef742-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="ef742-107">Този избор не е достъпен, освен ако фактура за проект не бъде потвърдена или фактурата, базирана на проекта, има аванси или фиксатори или съгласувания на аванси или фиксатори.</span><span class="sxs-lookup"><span data-stu-id="ef742-107">This selection isn't available unless a project invoice is confirmed or the project-based invoice has advances or retainers or reconciliations of advances or retainers.</span></span>

<span data-ttu-id="ef742-108">От потвърдената фактура се създава нов проект на фактура.</span><span class="sxs-lookup"><span data-stu-id="ef742-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="ef742-109">Всички подробности за реда за фактура от предварително потвърдената фактура се копират в новия проект.</span><span class="sxs-lookup"><span data-stu-id="ef742-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="ef742-110">По-долу са някои от ключовите моменти, които трябва да разберете относно подробностите за линията в новата коригирана фактура:</span><span class="sxs-lookup"><span data-stu-id="ef742-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="ef742-111">Всички количества са актуализирани до нула.</span><span class="sxs-lookup"><span data-stu-id="ef742-111">All quantities are updated to zero.</span></span> <span data-ttu-id="ef742-112">Dynamics 365 Project Operations приема, че всички фактурирани артикули са изцяло кредитирани.</span><span class="sxs-lookup"><span data-stu-id="ef742-112">Dynamics 365 Project Operations assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="ef742-113">Ако е необходимо, можете ръчно да актуализирате тези количества, за да отразят количеството, което се фактурира, а не количеството, което се кредитира.</span><span class="sxs-lookup"><span data-stu-id="ef742-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="ef742-114">Въз основа на въведеното количество, приложението изчислява кредитираното количество.</span><span class="sxs-lookup"><span data-stu-id="ef742-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="ef742-115">Тази сума се отразява в действителните факти, които се създават при потвърждаване на коригираната фактура.</span><span class="sxs-lookup"><span data-stu-id="ef742-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="ef742-116">Ако правите промени в данъчната сума, трябва да въведете правилната данъчна сума, а не сумата, която се кредитира.</span><span class="sxs-lookup"><span data-stu-id="ef742-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="ef742-117">Основните корекции винаги се обработват като пълни кредити.</span><span class="sxs-lookup"><span data-stu-id="ef742-117">Milestone corrections are always processed as full credits.</span></span>


> [!IMPORTANT]
> <span data-ttu-id="ef742-118">За подробности по реда за фактура, които представляват корекции на други вече фактурирани такси, **Корекция** полето е зададено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="ef742-118">For invoice line details that are corrections to other already invoiced charges, the **Correction** field is set to **Yes**.</span></span> <span data-ttu-id="ef742-119">За фактури, които имат коригирани подробности за реда на фактура, полето **Има корекции** е зададено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="ef742-119">For invoices that have corrected invoice line details, the **Has corrections** field is set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="ef742-120">Факти, създадени при потвърждаване на коригираща фактура</span><span class="sxs-lookup"><span data-stu-id="ef742-120">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="ef742-121">Следващата таблица изброява действителните факти, които се създават при потвърждаване на коригираща фактура.</span><span class="sxs-lookup"><span data-stu-id="ef742-121">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="ef742-122">
                    <strong>Сценарий</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ef742-122">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="ef742-123">
                    <strong>Действителни данни, създадени при потвърждение</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ef742-123">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ef742-124">Фактуриране на пълния кредит на предварително фактурирана транзакция във времето.</span><span class="sxs-lookup"><span data-stu-id="ef742-124">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-125">Обръщане на фактурирани продажби за часовете и сумата в детайла на оригиналната фактура за времето.</span><span class="sxs-lookup"><span data-stu-id="ef742-125">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-126">Нови действителни данни за нефактурирани продажби за часовете и сумата в детайла на оригиналната фактура за времето.</span><span class="sxs-lookup"><span data-stu-id="ef742-126">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="ef742-127">Фактуриране на частичния кредит по времева транзакция.</span><span class="sxs-lookup"><span data-stu-id="ef742-127">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-128">Обръщане на фактурирани продажби за часовете и сумата, фактурирана в подробностите на оригиналната фактура за времето.</span><span class="sxs-lookup"><span data-stu-id="ef742-128">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-129">Нова нефактурирана действителна продажба, която се заплаща за часовете и сумата в редактирания детайл на реда за фактура, сторниране на това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="ef742-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-130">Нова действителна нефактурирана продажба, която се дължи за оставащите часове и сума след приспадане на коригираните цифри в детайла на фактурата.</span><span class="sxs-lookup"><span data-stu-id="ef742-130">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ef742-131">Фактуриране на пълния кредит на предварително фактурирана транзакция за разход.</span><span class="sxs-lookup"><span data-stu-id="ef742-131">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-132">Обръщане на фактурирани продажби за количеството и сумата в подробностите на оригиналната фактура за разхода.</span><span class="sxs-lookup"><span data-stu-id="ef742-132">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-133">Нови действителни данни за нефактурирани продажби за количеството и сумата в подробностите на оригиналната фактура за разхода.</span><span class="sxs-lookup"><span data-stu-id="ef742-133">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="ef742-134">Фактуриране на частичния кредит на предварително фактурирана транзакция за разход.</span><span class="sxs-lookup"><span data-stu-id="ef742-134">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-135">Обръщане на фактурирани продажби за количеството и сумата, фактурирана в подробностите на оригиналната фактура за разход.</span><span class="sxs-lookup"><span data-stu-id="ef742-135">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-136">Нова нефактурирана действителна продажба, която се заплаща за количеството и сумата в редактирания детайл на реда на коригирана фактура, сторниране на това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="ef742-136">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-137">Нова действителна нефактурирана продажба, която се дължи за оставащото количество и сума след приспадане на коригираните цифри в детайла на фактурата.</span><span class="sxs-lookup"><span data-stu-id="ef742-137">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
                <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ef742-138">Фактуриране на пълния кредит на предварително фактурирана съществена транзакция.</span><span class="sxs-lookup"><span data-stu-id="ef742-138">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-139">Обръщане на фактурирани продажби за количеството и сумата в детайла на оригиналната фактура за материала.</span><span class="sxs-lookup"><span data-stu-id="ef742-139">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-140">Нови действителни данни за нефактурирани продажби за количеството и сумата в детайла на оригиналната фактура за материала.</span><span class="sxs-lookup"><span data-stu-id="ef742-140">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="ef742-141">Фактуриране на частичния кредит по съществена транзакция.</span><span class="sxs-lookup"><span data-stu-id="ef742-141">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-142">Обръщане на фактурирани продажби за фактурираното количество и сумата в детайла на оригиналната фактура за материала.</span><span class="sxs-lookup"><span data-stu-id="ef742-142">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-143">Нова нефактурирана действителна продажба, която се дължи за количеството и сумата в редактирания детайл на фактурата, сторниране на това и еквивалентна фактурирана действителна продажба.</span><span class="sxs-lookup"><span data-stu-id="ef742-143">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-144">Нова действителна нефактурирана продажба, която се дължи за оставащото количество и сума след приспадане на коригираните цифри в детайла на фактурата.</span><span class="sxs-lookup"><span data-stu-id="ef742-144">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ef742-145">Фактуриране на пълния кредит на предварително фактурирана транзакция на такса.</span><span class="sxs-lookup"><span data-stu-id="ef742-145">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-146">Обръщане на фактурирани продажби за количеството и сумата в подробностите на оригиналната фактура за таксата.</span><span class="sxs-lookup"><span data-stu-id="ef742-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-147">Нови действителни данни за нефактурирани продажби за количеството и сумата в подробностите на оригиналната фактура за таксата.</span><span class="sxs-lookup"><span data-stu-id="ef742-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ef742-148">Фактуриране на частичния кредит на предварително фактурирана транзакция на такса.</span><span class="sxs-lookup"><span data-stu-id="ef742-148">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-149">Обръщане на фактурирани продажби за количеството и сумата, фактурирана в подробностите на оригиналната фактура за таксата.</span><span class="sxs-lookup"><span data-stu-id="ef742-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-150">Нова нефактурирана действителна продажба, която се заплаща за количеството и сумата в редактирания детайл на реда на редактирана коригираща фактура, сторниране на това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="ef742-150">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="ef742-151">Фактуриране на пълния кредит на предварително фактурирана контролна точка.</span><span class="sxs-lookup"><span data-stu-id="ef742-151">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-152">Обръщане на фактурирани продажби за сумата в детайла на оригиналната фактура за контролната точка.</span><span class="sxs-lookup"><span data-stu-id="ef742-152">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="ef742-153">Състоянието на фактурата на етапа се актуализира от <b>Фактура на клиента публикувана</b> на <b>Готови за фактуриране</b>.</span><span class="sxs-lookup"><span data-stu-id="ef742-153">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="ef742-154">Фактуриране на частичния кредит на предварително фактурирана контролна точка.</span><span class="sxs-lookup"><span data-stu-id="ef742-154">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="ef742-155">Този сценарий не се поддържа.</span><span class="sxs-lookup"><span data-stu-id="ef742-155">This scenario isn't supported.</span></span>
                </p>
            </td>
        </tr>       
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
