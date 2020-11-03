---
title: Кредити и коригирани фактури
description: Тази тема предоставя информация за коригирани фактури в Project Operations
author: rumant
manager: Annbe
ms.date: 10/15/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d2187627439d42b37222dce0a491c62dafc358d5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071931"
---
# <a name="credits-and-corrected-invoices"></a><span data-ttu-id="7f36f-103">Кредити и коригирани фактури</span><span class="sxs-lookup"><span data-stu-id="7f36f-103">Credits and corrected invoices</span></span>

<span data-ttu-id="7f36f-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="7f36f-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7f36f-105">Потвърдена фактура за проект може да бъде коригирана, за да обработи промени или кредити, както е договорено с клиента и мениджъра на проекта.</span><span class="sxs-lookup"><span data-stu-id="7f36f-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="7f36f-106">За да редактирате потвърдена фактура, отворете потвърдената фактура и изберете **Коригирайте тази фактура**.</span><span class="sxs-lookup"><span data-stu-id="7f36f-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="7f36f-107">Този избор не е наличен, освен ако не бъде потвърдена фактура за проект.</span><span class="sxs-lookup"><span data-stu-id="7f36f-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="7f36f-108">От потвърдената фактура се създава нов проект на фактура.</span><span class="sxs-lookup"><span data-stu-id="7f36f-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="7f36f-109">Всички подробности за реда за фактура от предварително потвърдената фактура се копират в новия проект.</span><span class="sxs-lookup"><span data-stu-id="7f36f-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="7f36f-110">По-долу са някои от ключовите моменти, които трябва да разберете относно подробностите за линията в новата коригирана фактура:</span><span class="sxs-lookup"><span data-stu-id="7f36f-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="7f36f-111">Всички количества са актуализирани до нула.</span><span class="sxs-lookup"><span data-stu-id="7f36f-111">All quantities are updated to zero.</span></span> <span data-ttu-id="7f36f-112">Приложението приема, че всички фактурирани артикули са изцяло кредитирани.</span><span class="sxs-lookup"><span data-stu-id="7f36f-112">The application assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="7f36f-113">Ако е необходимо, можете ръчно да актуализирате тези количества, за да отразят количеството, което се фактурира, а не количеството, което се кредитира.</span><span class="sxs-lookup"><span data-stu-id="7f36f-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="7f36f-114">Въз основа на въведеното количество, приложението изчислява кредитираното количество.</span><span class="sxs-lookup"><span data-stu-id="7f36f-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="7f36f-115">Тази сума се отразява в действителните факти, които се създават при потвърждаване на коригираната фактура.</span><span class="sxs-lookup"><span data-stu-id="7f36f-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="7f36f-116">Ако правите промени в данъчната сума, трябва да въведете правилната данъчна сума, а не сумата, която се кредитира.</span><span class="sxs-lookup"><span data-stu-id="7f36f-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="7f36f-117">По-рано потвърдените продуктови договорени редове не се копират.</span><span class="sxs-lookup"><span data-stu-id="7f36f-117">Previously confirmed product-based contract lines are not copied over.</span></span> <span data-ttu-id="7f36f-118">Обработката на корекции на фактура за проект, базирана на продукт, не се поддържа.</span><span class="sxs-lookup"><span data-stu-id="7f36f-118">Processing corrections on a product-based project invoice is not supported.</span></span>
- <span data-ttu-id="7f36f-119">Основните корекции винаги се обработват като пълни кредити.</span><span class="sxs-lookup"><span data-stu-id="7f36f-119">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="7f36f-120">Сумите за фиксиране или аванс могат да бъдат коригирани, ако клиентът е бил фактуриран за неправилна сума.</span><span class="sxs-lookup"><span data-stu-id="7f36f-120">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="7f36f-121">Съпоставянията на задържащите и авансовите плащания могат да бъдат коригирани, ако е използвана неправилна сума за изравняване на таксите по предварително потвърдена фактура.</span><span class="sxs-lookup"><span data-stu-id="7f36f-121">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7f36f-122">Подробности за реда за фактури, които представляват корекции на други вече фактурирани такси, имат полето **Корекция** , зададено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="7f36f-122">Invoice line details that are corrections to other already invoiced charges have the field **Correction** set to **Yes**.</span></span> <span data-ttu-id="7f36f-123">Фактурите, които са коригирали данните за реда на фактурата, имат поле, наречено **Има корекции** и също е настроено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="7f36f-123">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a><span data-ttu-id="7f36f-124">Факти, създадени при потвърждаване на коригираща фактура:</span><span class="sxs-lookup"><span data-stu-id="7f36f-124">Actuals created on Confirmation of a corrective invoice:</span></span>

<span data-ttu-id="7f36f-125">По-долу са действителните, създадени от приложението за потвърждаване на коректив въз основа на извършените операции върху проекта на коригираща фактура преди потвърждение.</span><span class="sxs-lookup"><span data-stu-id="7f36f-125">Below are the actuals created by the application on confirmation of a corrective based on the operations performed on the draft corrective invoice before confirmation.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="7f36f-126">
                    <strong>Сценарий</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f36f-126">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="7f36f-127">
                    <strong>Действителни данни, създадени при потвърждение</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f36f-127">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="7f36f-128">Потвърдете корекцията на фактуриран аванс или фиксатор.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f36f-128">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-129">Нефактулирано обръщане на продажбите на фиксатора или аванса, създаден за помирение.</span><span class="sxs-lookup"><span data-stu-id="7f36f-129">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="7f36f-130">Тази сума е положителна, тъй като има за цел да анулира отрицателното, създадено при фактуриране на фиксатора или аванса.</span><span class="sxs-lookup"><span data-stu-id="7f36f-130">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-131">Създава се действително обръщане на фактурирани продажби за сумата върху фиксатора или аванс за обръщане на първоначалните фактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="7f36f-131">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-132">Създава се нова актуална таксувана продажба за коригираната сума на фиксатора или коригирана фактура на базата на аванс.</span><span class="sxs-lookup"><span data-stu-id="7f36f-132">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-133">Нефактурирани продажби, действителни с отрицателна сума на фиксатора или коригирана линия на фактура, базирана на аванс, която ще се използва за съгласуване.</span><span class="sxs-lookup"><span data-stu-id="7f36f-133">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="7f36f-134">Потвърждение за корекцията на предварително примирен фиксатор или аванс.</span><span class="sxs-lookup"><span data-stu-id="7f36f-134">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-135">Нефактулирано обръщане на продажбите на фиксатора или аванса, създаден за помирение.</span><span class="sxs-lookup"><span data-stu-id="7f36f-135">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="7f36f-136">Тази сума е положителна и има за цел да анулира отрицателното, създадено при възникването на предишно уравняване.</span><span class="sxs-lookup"><span data-stu-id="7f36f-136">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-137">Фактурирано обръщане на продажби, действително за сумата от предходната фактура.</span><span class="sxs-lookup"><span data-stu-id="7f36f-137">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-138">Създава се нови действителни данни за таксувани продажби за коригираната сума на капаро, която се прилага за коригирана фактура.</span><span class="sxs-lookup"><span data-stu-id="7f36f-138">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-139">Нефактурирани действителни данни за продажби с отрицателна сума от коригиран останал аванс или капаро, които ще се използват за уравняване на по-нататъшни фактури.</span><span class="sxs-lookup"><span data-stu-id="7f36f-139">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f36f-140">Фактуриране на пълния кредит на предварително фактурирана транзакция във времето.</span><span class="sxs-lookup"><span data-stu-id="7f36f-140">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-141">Обръщане на фактурирани продажби за часовете и сумата в детайла на оригиналната фактура за времето.</span><span class="sxs-lookup"><span data-stu-id="7f36f-141">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-142">Нови действителни данни за нефактурирани продажби за часовете и сумата в детайла на оригиналната фактура за времето.</span><span class="sxs-lookup"><span data-stu-id="7f36f-142">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="7f36f-143">Фактуриране на частичния кредит по времева транзакция.</span><span class="sxs-lookup"><span data-stu-id="7f36f-143">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-144">Обръщане на фактурирани продажби за часовете и сумата, фактурирана в подробностите на оригиналната фактура за времето.</span><span class="sxs-lookup"><span data-stu-id="7f36f-144">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-145">Нова нефактурирана действителна продажба, която се заплаща за часовете и сумата в редактирания детайл на реда за фактура, сторниране на това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="7f36f-145">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-146">Нова действителна нефактурирана продажба, която се дължи за оставащите часове и сума след приспадане на коригираните цифри в детайла на фактурата.</span><span class="sxs-lookup"><span data-stu-id="7f36f-146">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f36f-147">Фактуриране на пълния кредит на предварително фактурирана транзакция за разход.</span><span class="sxs-lookup"><span data-stu-id="7f36f-147">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-148">Обръщане на фактурирани продажби за количеството и сумата в подробностите на оригиналната фактура за разхода.</span><span class="sxs-lookup"><span data-stu-id="7f36f-148">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-149">Нови действителни данни за нефактурирани продажби за количеството и сумата в подробностите на оригиналната фактура за разхода.</span><span class="sxs-lookup"><span data-stu-id="7f36f-149">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="7f36f-150">Фактуриране на частичния кредит на предварително фактурирана транзакция за разход.</span><span class="sxs-lookup"><span data-stu-id="7f36f-150">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-151">Обръщане на фактурирани продажби за количеството и сумата, фактурирана в подробностите на оригиналната фактура за разход.</span><span class="sxs-lookup"><span data-stu-id="7f36f-151">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-152">Нова нефактурирана действителна продажба, която се заплаща за количеството и сумата в редактирания детайл на реда на коригирана фактура, сторниране на това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="7f36f-152">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-153">Нова действителна нефактурирана продажба, която се дължи за оставащото количество и сума след приспадане на коригираните цифри в детайла на фактурата.</span><span class="sxs-lookup"><span data-stu-id="7f36f-153">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f36f-154">Фактуриране на пълния кредит на предварително фактурирана транзакция на такса.</span><span class="sxs-lookup"><span data-stu-id="7f36f-154">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-155">Обръщане на фактурирани продажби за количеството и сумата в подробностите на оригиналната фактура за таксата.</span><span class="sxs-lookup"><span data-stu-id="7f36f-155">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-156">Нови действителни данни за нефактурирани продажби за количеството и сумата в подробностите на оригиналната фактура за таксата.</span><span class="sxs-lookup"><span data-stu-id="7f36f-156">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f36f-157">Фактуриране на частичния кредит на предварително фактурирана транзакция на такса.</span><span class="sxs-lookup"><span data-stu-id="7f36f-157">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-158">Обръщане на фактурирани продажби за количеството и сумата, фактурирана в подробностите на оригиналната фактура за таксата.</span><span class="sxs-lookup"><span data-stu-id="7f36f-158">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-159">Нова нефактурирана действителна продажба, която се заплаща за количеството и сумата в редактирания детайл на реда на редактирана коригираща фактура, сторниране на това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="7f36f-159">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="7f36f-160">Фактуриране на пълния кредит на предварително фактурирана контролна точка.</span><span class="sxs-lookup"><span data-stu-id="7f36f-160">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-161">Обръщане на фактурирани продажби за сумата в детайла на оригиналната фактура за контролната точка.</span><span class="sxs-lookup"><span data-stu-id="7f36f-161">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="7f36f-162">Състоянието на фактурата или фактурата на етапа по реда на договора за проект се актуализира до **Готови за фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="7f36f-162">The milestone invoice or billing status on the project contract line is updated to **Ready to Invoice**.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="7f36f-163">Фактуриране на частичния кредит на предварително фактурирана контролна точка.</span><span class="sxs-lookup"><span data-stu-id="7f36f-163">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-164">Неподдържано</span><span class="sxs-lookup"><span data-stu-id="7f36f-164">Unsupported</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="7f36f-165">Кредити и корекции на предварително фактурирана продуктови аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="7f36f-165">Credits and corrections of a previously invoiced product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="7f36f-166">Неподдържано</span><span class="sxs-lookup"><span data-stu-id="7f36f-166">Unsupported</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>
