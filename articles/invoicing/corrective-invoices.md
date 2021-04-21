---
title: Създаване на коригиращи базирани на проект фактури
description: Тази тема предоставя информация за корективни фактури за проекти в Project Operations.
author: rumant
manager: Annbe
ms.date: 03/29/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 32772d64b3fc77f0af9618edff40e3b295593454
ms.sourcegitcommit: 504c09365bf404c1f1aa9b5034c1e1e5bc9d0d54
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788832"
---
# <a name="create-corrective-project-based-invoices"></a><span data-ttu-id="2fc74-103">Създаване на коригиращи базирани на проект фактури</span><span class="sxs-lookup"><span data-stu-id="2fc74-103">Create corrective project-based invoices</span></span> 

<span data-ttu-id="2fc74-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="2fc74-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="2fc74-105">Потвърдена фактура за проект може да бъде коригирана, за да обработи промени или кредити, както е договорено с клиента и мениджъра на проекта.</span><span class="sxs-lookup"><span data-stu-id="2fc74-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="2fc74-106">За да редактирате потвърдена фактура, отворете потвърдената фактура и изберете **Коригирайте тази фактура**.</span><span class="sxs-lookup"><span data-stu-id="2fc74-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="2fc74-107">Този избор не е наличен, освен ако не бъде потвърдена фактура за проект.</span><span class="sxs-lookup"><span data-stu-id="2fc74-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="2fc74-108">От потвърдената фактура се създава нов проект на фактура.</span><span class="sxs-lookup"><span data-stu-id="2fc74-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="2fc74-109">Всички подробности за реда за фактура от предварително потвърдената фактура се копират в новия проект.</span><span class="sxs-lookup"><span data-stu-id="2fc74-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="2fc74-110">Следват някои ключови моменти, които ще ви помогнат да разберете повече за подробностите за реда в новата коригирана фактура:</span><span class="sxs-lookup"><span data-stu-id="2fc74-110">The following are some key points to help you understand more about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="2fc74-111">Всички количества са актуализирани до нула.</span><span class="sxs-lookup"><span data-stu-id="2fc74-111">All quantities are updated to zero.</span></span> <span data-ttu-id="2fc74-112">Това приема, че всички фактурирани артикули са изцяло кредитирани.</span><span class="sxs-lookup"><span data-stu-id="2fc74-112">This assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="2fc74-113">Ако е необходимо, можете ръчно да актуализирате тези количества, за да отразят количеството, което се фактурира, а не количеството, което се кредитира.</span><span class="sxs-lookup"><span data-stu-id="2fc74-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="2fc74-114">Въз основа на въведеното количество, приложението изчислява кредитираното количество.</span><span class="sxs-lookup"><span data-stu-id="2fc74-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="2fc74-115">Тази сума се отразява в действителните факти, които се създават при потвърждаване на коригираната фактура.</span><span class="sxs-lookup"><span data-stu-id="2fc74-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="2fc74-116">Ако правите промени в данъчната сума, трябва да въведете правилната данъчна сума, а не сумата, която се кредитира.</span><span class="sxs-lookup"><span data-stu-id="2fc74-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="2fc74-117">Основните корекции винаги се обработват като пълни кредити.</span><span class="sxs-lookup"><span data-stu-id="2fc74-117">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="2fc74-118">Сумите за фиксиране или аванс могат да бъдат коригирани, ако клиентът е бил фактуриран за неправилна сума.</span><span class="sxs-lookup"><span data-stu-id="2fc74-118">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="2fc74-119">Съпоставянията на задържащите и авансовите плащания могат да бъдат коригирани, ако е използвана неправилна сума за изравняване на таксите по предварително потвърдена фактура.</span><span class="sxs-lookup"><span data-stu-id="2fc74-119">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2fc74-120">Подробности за ред на фактура, които представляват корекции на други вече фактурирани такси, имат поле **Корекция** зададено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="2fc74-120">Invoice line details that are corrections to other already invoiced charges have the **Correction** field set to **Yes**.</span></span> <span data-ttu-id="2fc74-121">Фактурите, които са коригирали данните за реда на фактурата, имат поле, наречено **Има корекции** и също е настроено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="2fc74-121">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a><span data-ttu-id="2fc74-122">Факти, създадени при потвърждаване на коригираща фактура</span><span class="sxs-lookup"><span data-stu-id="2fc74-122">Actuals created on confirmation of a corrective invoice</span></span>

<span data-ttu-id="2fc74-123">Следващата таблица изброява действителните факти, които се създават при потвърждаване на коригираща фактура.</span><span class="sxs-lookup"><span data-stu-id="2fc74-123">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="2fc74-124">
                    <strong>Сценарий</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2fc74-124">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="2fc74-125">
                    <strong>Действителни данни, създадени при потвърждение</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2fc74-125">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="2fc74-126">Потвърдете корекцията на фактуриран аванс или фиксатор.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="2fc74-126">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-127">Нефактулирано обръщане на продажбите на фиксатора или аванса, създаден за помирение.</span><span class="sxs-lookup"><span data-stu-id="2fc74-127">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="2fc74-128">Тази сума е положителна, тъй като има за цел да анулира отрицателното, създадено при фактуриране на фиксатора или аванса.</span><span class="sxs-lookup"><span data-stu-id="2fc74-128">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-129">Създава се действително обръщане на фактурирани продажби за сумата върху фиксатора или аванс за обръщане на първоначалните фактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="2fc74-129">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-130">Създава се нова актуална таксувана продажба за коригираната сума на фиксатора или коригирана фактура на базата на аванс.</span><span class="sxs-lookup"><span data-stu-id="2fc74-130">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-131">Нефактурирани продажби, действителни с отрицателна сума на фиксатора или коригирана линия на фактура, базирана на аванс, която ще се използва за съгласуване.</span><span class="sxs-lookup"><span data-stu-id="2fc74-131">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="2fc74-132">Потвърждение за корекцията на предварително примирен фиксатор или аванс.</span><span class="sxs-lookup"><span data-stu-id="2fc74-132">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-133">Нефактулирано обръщане на продажбите на фиксатора или аванса, създаден за помирение.</span><span class="sxs-lookup"><span data-stu-id="2fc74-133">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="2fc74-134">Тази сума е положителна и има за цел да анулира отрицателното, създадено при възникването на предишно уравняване.</span><span class="sxs-lookup"><span data-stu-id="2fc74-134">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-135">Фактурирано обръщане на продажби, действително за сумата от предходната фактура.</span><span class="sxs-lookup"><span data-stu-id="2fc74-135">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-136">Създава се нови действителни данни за таксувани продажби за коригираната сума на капаро, която се прилага за коригирана фактура.</span><span class="sxs-lookup"><span data-stu-id="2fc74-136">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-137">Нефактурирани действителни данни за продажби с отрицателна сума от коригиран останал аванс или капаро, които ще се използват за уравняване на по-нататъшни фактури.</span><span class="sxs-lookup"><span data-stu-id="2fc74-137">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2fc74-138">Фактуриране на пълния кредит на предварително фактурирана транзакция във времето.</span><span class="sxs-lookup"><span data-stu-id="2fc74-138">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-139">Обръщане на фактурирани продажби за часовете и сумата в детайла на оригиналната фактура за времето.</span><span class="sxs-lookup"><span data-stu-id="2fc74-139">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-140">Нови действителни данни за нефактурирани продажби за часовете и сумата в детайла на оригиналната фактура за времето.</span><span class="sxs-lookup"><span data-stu-id="2fc74-140">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="2fc74-141">Фактуриране на частичния кредит по времева транзакция.</span><span class="sxs-lookup"><span data-stu-id="2fc74-141">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-142">Обръщане на фактурирани продажби за часовете и сумата, фактурирана в подробностите на оригиналната фактура за времето.</span><span class="sxs-lookup"><span data-stu-id="2fc74-142">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-143">Нова нефактурирана действителна продажба, която се заплаща за часовете и сумата в редактирания детайл на реда за фактура, сторниране на това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="2fc74-143">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-144">Нова действителна нефактурирана продажба, която се дължи за оставащите часове и сума след приспадане на коригираните цифри в детайла на фактурата.</span><span class="sxs-lookup"><span data-stu-id="2fc74-144">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2fc74-145">Фактуриране на пълния кредит на предварително фактурирана транзакция за разход.</span><span class="sxs-lookup"><span data-stu-id="2fc74-145">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-146">Обръщане на фактурирани продажби за количеството и сумата в подробностите на оригиналната фактура за разхода.</span><span class="sxs-lookup"><span data-stu-id="2fc74-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-147">Нови действителни данни за нефактурирани продажби за количеството и сумата в подробностите на оригиналната фактура за разхода.</span><span class="sxs-lookup"><span data-stu-id="2fc74-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="2fc74-148">Фактуриране на частичния кредит на предварително фактурирана транзакция за разход.</span><span class="sxs-lookup"><span data-stu-id="2fc74-148">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-149">Обръщане на фактурирани продажби за количеството и сумата, фактурирана в подробностите на оригиналната фактура за разход.</span><span class="sxs-lookup"><span data-stu-id="2fc74-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-150">Нова нефактурирана действителна продажба, която се заплаща за количеството и сумата в редактирания детайл на реда на коригирана фактура, сторниране на това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="2fc74-150">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-151">Нова действителна нефактурирана продажба, която се дължи за оставащото количество и сума след приспадане на коригираните цифри в детайла на фактурата.</span><span class="sxs-lookup"><span data-stu-id="2fc74-151">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2fc74-152">Фактуриране на пълния кредит на предварително фактурирана транзакция на такса.</span><span class="sxs-lookup"><span data-stu-id="2fc74-152">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-153">Обръщане на фактурирани продажби за количеството и сумата в подробностите на оригиналната фактура за таксата.</span><span class="sxs-lookup"><span data-stu-id="2fc74-153">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-154">Нови действителни данни за нефактурирани продажби за количеството и сумата в подробностите на оригиналната фактура за таксата.</span><span class="sxs-lookup"><span data-stu-id="2fc74-154">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2fc74-155">Фактуриране на частичния кредит на предварително фактурирана транзакция на такса.</span><span class="sxs-lookup"><span data-stu-id="2fc74-155">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-156">Обръщане на фактурирани продажби за количеството и сумата, фактурирана в подробностите на оригиналната фактура за таксата.</span><span class="sxs-lookup"><span data-stu-id="2fc74-156">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-157">Нова нефактурирана действителна продажба, която се заплаща за количеството и сумата в редактирания детайл на реда на редактирана коригираща фактура, сторниране на това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="2fc74-157">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="2fc74-158">Фактуриране на пълния кредит на предварително фактурирана контролна точка.</span><span class="sxs-lookup"><span data-stu-id="2fc74-158">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-159">Обръщане на фактурирани продажби за сумата в детайла на оригиналната фактура за контролната точка.</span><span class="sxs-lookup"><span data-stu-id="2fc74-159">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="2fc74-160">Състоянието на фактурата на етапа се актуализира от <b>Публикувана фактура на клиент</b> на <b>Готови за фактуриране</b>.</span><span class="sxs-lookup"><span data-stu-id="2fc74-160">The invoice status on the milestone is updated from <b>Customer invoice posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="2fc74-161">Фактуриране на частичния кредит на предварително фактурирана контролна точка.</span><span class="sxs-lookup"><span data-stu-id="2fc74-161">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="2fc74-162">Неподдържано</span><span class="sxs-lookup"><span data-stu-id="2fc74-162">Unsupported</span></span> </p>
            </td>
        </tr>        
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
