---
title: Потвърждение на базирана на проект проформа фактура
description: Тази тема предоставя информация за това как да потвърдите проформа фактура, базирана на проект.
author: rumant
manager: AnnBe
ms.date: 04/05/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 53c647dca506822312053fb5c9b086a2947974c2
ms.sourcegitcommit: ca0fc078d1a12484eca193fe051b8442c0559db8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/07/2021
ms.locfileid: "5867115"
---
# <a name="confirm-a-proforma-project-based-invoice"></a><span data-ttu-id="67744-103">Потвърждение на базирана на проект проформа фактура</span><span class="sxs-lookup"><span data-stu-id="67744-103">Confirm a proforma project-based invoice</span></span>

<span data-ttu-id="67744-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="67744-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="67744-105">След като се потвърди проформа фактура, състоянието на фактурата на проекта се актуализира до **Потвърдено**.</span><span class="sxs-lookup"><span data-stu-id="67744-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="67744-106">Когато фактурата бъде потвърдена, тя става само за четене.</span><span class="sxs-lookup"><span data-stu-id="67744-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="67744-107">Занапред фактурата може да бъде коригирана само ако има инициирани от клиента корекции или кредити.</span><span class="sxs-lookup"><span data-stu-id="67744-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits.</span></span>

<span data-ttu-id="67744-108">Следващата таблица изброява действителните факти, създадени от системата.</span><span class="sxs-lookup"><span data-stu-id="67744-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="67744-109">Тези фактически данни се създават, когато се извършват определени операции върху проекта на фактура за проект, преди той да бъде потвърден.</span><span class="sxs-lookup"><span data-stu-id="67744-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="67744-110">
                    <strong>Сценарий</strong>
                </span><span class="sxs-lookup"><span data-stu-id="67744-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="67744-111">
                    <strong>Действителни данни, създадени при потвърждение</strong>
                </span><span class="sxs-lookup"><span data-stu-id="67744-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="67744-112">Фактуриране на капаро или аванс</span><span class="sxs-lookup"><span data-stu-id="67744-112">Invoicing an advance or retainer</span></span> </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-113">Фактурирани продажби, действителни от типа <strong>Капаро</strong> се създава за сумата по аванса или фиксатора.</span><span class="sxs-lookup"><span data-stu-id="67744-113">A billed sales actual of type, <strong>Retainer</strong> is created for the amount on the advance or retainer.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-114">Нефактурирани продажби, действителни с отрицателна сума на фиксатора или аванс, който да се използва за съгласуване.</span><span class="sxs-lookup"><span data-stu-id="67744-114">An unbilled sales actual with a negative amount of the retainer or advance to be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="67744-115">След пълно съгласуване на фиксатор или аванс по фактура.</span><span class="sxs-lookup"><span data-stu-id="67744-115">After fully reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-116">Нефактулирано обръщане на продажбите на фиксатора или аванса, създаден за помирение.</span><span class="sxs-lookup"><span data-stu-id="67744-116">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="67744-117">Тази сума е положителна, тъй като има за цел да анулира отрицателното, създадено при фактуриране на фиксатора или аванса.</span><span class="sxs-lookup"><span data-stu-id="67744-117">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-118">Фактурирани действителни данни на продажби за сумата в тази фактура.</span><span class="sxs-lookup"><span data-stu-id="67744-118">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="67744-119">След частично съгласуване на фиксатор или аванс по фактура.</span><span class="sxs-lookup"><span data-stu-id="67744-119">After partially reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-120">Нефактулирано обръщане на продажбите на фиксатора или аванса, създаден за помирение.</span><span class="sxs-lookup"><span data-stu-id="67744-120">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="67744-121">Тази сума е положителна, тъй като има за цел да анулира отрицателното, създадено при фактуриране на фиксатора или аванса.</span><span class="sxs-lookup"><span data-stu-id="67744-121">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-122">Фактурирани действителни данни на продажби за сумата в тази фактура.</span><span class="sxs-lookup"><span data-stu-id="67744-122">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-123">Отрицателни действителни данни на нефактурирани продажби на оставащата сума на капарото или аванса за използване за съгласуване за бъдещи фактури.</span><span class="sxs-lookup"><span data-stu-id="67744-123">A negative unbilled sales actual of the remaining retainer or advance amount to be used for reconciliation on future invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="67744-124">Фактуриране на транзакция във времето без никакви редакции в проектофактурата.</span><span class="sxs-lookup"><span data-stu-id="67744-124">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-125">Обръщане на нефактурирани продажби за часовете и сумата в детайла на първоначалното одобрение на време.</span><span class="sxs-lookup"><span data-stu-id="67744-125">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-126">Действителни данни за фактурирани продажби за часовете и сумата в детайла на първоначалното одобрение на време.</span><span class="sxs-lookup"><span data-stu-id="67744-126">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="67744-127">Фактуриране на транзакция във времето, която е редактирана, за да се намали количеството.</span><span class="sxs-lookup"><span data-stu-id="67744-127">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-128">Обръщане на нефактурирани продажби за часовете и сумата в детайла на първоначалното одобрение на време.</span><span class="sxs-lookup"><span data-stu-id="67744-128">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-129">Нова нефактурирана действителна продажба, която се заплаща за часовете и сумата в редактирания детайл на реда за фактура, сторниране на действителните данни за продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="67744-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-130">Нова нефактурирана действителна продажба, която не се начислява за оставащите часове и сума след приспадане на коригираните цифри в редактирания детайл на фактурата, сторниране на действителните продажби и еквивалентна фактурирана действителна продажба.</span><span class="sxs-lookup"><span data-stu-id="67744-130">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="67744-131">Фактуриране на транзакция във времето, която е редактирана, за да се увеличи количеството.</span><span class="sxs-lookup"><span data-stu-id="67744-131">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-132">Обръщане на нефактурирани продажби за часовете и сумата в детайла на първоначалното одобрение на време.</span><span class="sxs-lookup"><span data-stu-id="67744-132">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-133">Нова нефактурирана действителна продажба, която се заплаща за часовете и сумата в редактирания детайл на реда за фактура, сторниране на действителните данни за нефактурирани продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="67744-133">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="67744-134">Фактуриране на транзакция за разход без никакви редакции в проектофактурата.</span><span class="sxs-lookup"><span data-stu-id="67744-134">Invoicing an expense transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-135">Обръщане на нефактурирани продажби за количеството и сумата в детайла на първоначалното одобрение на разход.</span><span class="sxs-lookup"><span data-stu-id="67744-135">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-136">Действителни данни за фактурирана продажба за количеството и сумата в детайла на първоначалното одобрение на разход.</span><span class="sxs-lookup"><span data-stu-id="67744-136">A billed sales actual for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="67744-137">Фактуриране на транзакция за разход, която е редактирана, за да се намали количеството.</span><span class="sxs-lookup"><span data-stu-id="67744-137">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-138">Обръщане на нефактурирани продажби за количеството и сумата в детайла на първоначалното одобрение на разход.</span><span class="sxs-lookup"><span data-stu-id="67744-138">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-139">Нова нефактурирана действителна продажба, която се заплаща за количеството и сумата в редактирания детайл на реда за фактура, сторниране на действителните данни за нефактурирани продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="67744-139">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-140">Нова нефактурирана действителна продажба, която не се заплаща за оставащото количество часовете и сумата след изваждане на коригираните суми в редактирания детайл на реда за фактура, сторниране на действителните данни за нефактурирани продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="67744-140">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="67744-141">Фактуриране на транзакция за разход, която е редактирана, за да се увеличи количеството.</span><span class="sxs-lookup"><span data-stu-id="67744-141">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-142">Обръщане на нефактурирани продажби за количеството и сумата в детайла на първоначалното одобрение на разход.</span><span class="sxs-lookup"><span data-stu-id="67744-142">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-143">Нова нефактурирана действителна продажба, която се заплаща за количеството и сумата в редактирания детайл на реда за фактура, сторниране на действителни данни за нефактурирани продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="67744-143">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="67744-144">Фактуриране на съществена транзакция без никакви редакции в проектофактурата.</span><span class="sxs-lookup"><span data-stu-id="67744-144">Invoicing a material transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-145">Сторниране на нефактурирани продажби за количеството и сумата в детайла на първоначалното одобряване на използване на материал.</span><span class="sxs-lookup"><span data-stu-id="67744-145">An unbilled sales reversal for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-146">Действителни данни за фактурирани продажби за количеството и сумата в детайла на първоначалното одобряване на използване на материал.</span><span class="sxs-lookup"><span data-stu-id="67744-146">A billed sales actual for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="67744-147">Фактуриране на съществена транзакция, която е редактирана, за да се намали количеството.</span><span class="sxs-lookup"><span data-stu-id="67744-147">Invoicing a material transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-148">Сторниране на нефактурирани продажби за количеството и сумата в детайла на първоначалното одобряване за време.</span><span class="sxs-lookup"><span data-stu-id="67744-148">An unbilled sales reversal for the quantity and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-149">Нова нефактурирана действителна продажба, която се заплаща за количеството и сумата в редактирания детайл на реда за фактура, сторниране на действителните данни за нефактурирани продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="67744-149">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-150">Нова нефактурирана действителна продажба, която не се заплаща за оставащото количество часовете и сумата след изваждане на коригираните суми в редактирания детайл на реда за фактура, сторниране на действителните данни за нефактурирани продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="67744-150">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="67744-151">Фактуриране на съществена транзакция, която е редактирана, за да се увеличи количеството.</span><span class="sxs-lookup"><span data-stu-id="67744-151">Invoicing a material transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-152">Сторниране на нефактурирани продажби за количеството и сумата в детайла на първоначалното одобряване на използване на материал.</span><span class="sxs-lookup"><span data-stu-id="67744-152">An unbilled sales reversal for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-153">Нова нефактурирана действителна продажба, която се заплаща за количеството и сумата в редактирания детайл на реда за фактура, сторниране на действителните данни за нефактурирани продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="67744-153">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="67744-154">Фактуриране на такса.</span><span class="sxs-lookup"><span data-stu-id="67744-154">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-155">Обръщане на нефактурирани продажби за сумата на такса в първоначалния счетоводен запис.</span><span class="sxs-lookup"><span data-stu-id="67744-155">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-156">Действителни данни за фактурирана продажба за количеството и сумата в детайла на първоначалния счетоводен запис за такса.</span><span class="sxs-lookup"><span data-stu-id="67744-156">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="67744-157">Фактурирането на контролна точка.</span><span class="sxs-lookup"><span data-stu-id="67744-157">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="67744-158">Действителни данни на фактурирани продажби за сумата на контролна точка на първоначалната контролна точка в аспекти на договор по проект.</span><span class="sxs-lookup"><span data-stu-id="67744-158">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
       
    </tbody>
</table>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
