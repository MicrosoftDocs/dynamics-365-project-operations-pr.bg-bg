---
title: Потвърждение на проформа фактура
description: Тази тема предоставя информация за потвърждаване на проформа фактура.
author: rumant
manager: AnnBe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: fa1e6c17fbda76a283c2ec68760a00e846decf83
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128090"
---
# <a name="confirm-a-proforma-invoice"></a><span data-ttu-id="63cce-103">Потвърждение на проформа фактура</span><span class="sxs-lookup"><span data-stu-id="63cce-103">Confirm a proforma invoice</span></span>

<span data-ttu-id="63cce-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="63cce-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="63cce-105">След като се потвърди проформа фактура, състоянието на фактурата на проекта се актуализира до **Потвърдено**.</span><span class="sxs-lookup"><span data-stu-id="63cce-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="63cce-106">Когато фактурата бъде потвърдена, тя става само за четене.</span><span class="sxs-lookup"><span data-stu-id="63cce-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="63cce-107">Занапред фактурата може да бъде коригирана само ако има инициирани от клиента корекции или кредити или когато е означена като платена.</span><span class="sxs-lookup"><span data-stu-id="63cce-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, or when it's marked as paid.</span></span>

<span data-ttu-id="63cce-108">Следващата таблица изброява действителните факти, създадени от системата.</span><span class="sxs-lookup"><span data-stu-id="63cce-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="63cce-109">Тези фактически данни се създават, когато се извършват определени операции върху проекта на фактура за проект, преди той да бъде потвърден.</span><span class="sxs-lookup"><span data-stu-id="63cce-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="416" valign="top">
                <p><span data-ttu-id="63cce-110">
                    <strong>Сценарий</strong>
                </span><span class="sxs-lookup"><span data-stu-id="63cce-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="608" valign="top">
                <p><span data-ttu-id="63cce-111">
                    <strong>Действителни данни, създадени при потвърждение</strong>
                </span><span class="sxs-lookup"><span data-stu-id="63cce-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="63cce-112">Фактуриране на транзакция във времето без никакви редакции в проектофактурата.</span><span class="sxs-lookup"><span data-stu-id="63cce-112">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-113">Обръщане на нефактурирани продажби за часовете и сумата в детайла на първоначалното одобрение на време.</span><span class="sxs-lookup"><span data-stu-id="63cce-113">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-114">Действителни данни за фактурирани продажби за часовете и сумата в детайла на първоначалното одобрение на време.</span><span class="sxs-lookup"><span data-stu-id="63cce-114">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="63cce-115">Фактуриране на транзакция във времето, която е редактирана, за да се намали количеството.</span><span class="sxs-lookup"><span data-stu-id="63cce-115">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-116">Обръщане на нефактурирани продажби за часовете и сумата в детайла на първоначалното одобрение на време.</span><span class="sxs-lookup"><span data-stu-id="63cce-116">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-117">Нова нефактурирана действителна продажба, която се заплаща за часовете и сумата в редактирания детайл на реда за фактура, сторниране на действителните данни за нефактурирани продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="63cce-117">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-118">Нова нефактурирана действителна продажба, която не се заплаща за оставащите часовете и сумата след изваждане на коригираните суми в редактирания детайл на реда за фактура, сторниране на действителните данни за нефактурирани продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="63cce-118">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="63cce-119">Фактуриране на транзакция във времето, която е редактирана, за да се увеличи количеството.</span><span class="sxs-lookup"><span data-stu-id="63cce-119">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-120">Обръщане на нефактурирани продажби за часовете и сумата в детайла на първоначалното одобрение на време.</span><span class="sxs-lookup"><span data-stu-id="63cce-120">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-121">Нова нефактурирана действителна продажба, която се заплаща за часовете и сумата в редактирания детайл на реда за фактура, сторниране на действителните данни за нефактурирани продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="63cce-121">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="63cce-122">Фактуриране на транзакция за разход без никакви редакции в проектофактурата.</span><span class="sxs-lookup"><span data-stu-id="63cce-122">Invoicing an expense transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-123">Обръщане на нефактурирани продажби за количеството и сумата в детайла на първоначалното одобрение на разход.</span><span class="sxs-lookup"><span data-stu-id="63cce-123">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-124">Действителни данни за фактурирана продажба за количеството и сумата в детайла на първоначалното одобрение на разход.</span><span class="sxs-lookup"><span data-stu-id="63cce-124">A billed sales actual for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="63cce-125">Фактуриране на транзакция за разход, която е редактирана, за да се намали количеството.</span><span class="sxs-lookup"><span data-stu-id="63cce-125">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-126">Обръщане на нефактурирани продажби за количеството и сумата в детайла на първоначалното одобрение на разход.</span><span class="sxs-lookup"><span data-stu-id="63cce-126">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-127">Нова нефактурирана действителна продажба, която се заплаща за количеството и сумата в редактирания детайл на реда за фактура, сторниране на действителните данни за нефактурирани продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="63cce-127">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-128">Нова нефактурирана действителна продажба, която не се заплаща за оставащото количество часовете и сумата след изваждане на коригираните суми в редактирания детайл на реда за фактура, сторниране на действителните данни за нефактурирани продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="63cce-128">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent of the billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="63cce-129">Фактуриране на транзакция за разход, която е редактирана, за да се увеличи количеството.</span><span class="sxs-lookup"><span data-stu-id="63cce-129">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-130">Обръщане на нефактурирани продажби за количеството и сумата в детайла на първоначалното одобрение на разход.</span><span class="sxs-lookup"><span data-stu-id="63cce-130">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-131">Нова нефактурирана действителна продажба, която се заплаща за количеството и сумата в редактирания детайл на реда за фактура, сторниране на неозаглавени действителни данни за нефактурирани продажби това и еквивалентна действителна фактурирана продажба.</span><span class="sxs-lookup"><span data-stu-id="63cce-131">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the untilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="63cce-132">Фактуриране на такса.</span><span class="sxs-lookup"><span data-stu-id="63cce-132">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-133">Обръщане на нефактурирани продажби за сумата на такса в първоначалния счетоводен запис.</span><span class="sxs-lookup"><span data-stu-id="63cce-133">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-134">Действителни данни за фактурирана продажба за количеството и сумата в детайла на първоначалния счетоводен запис за такса.</span><span class="sxs-lookup"><span data-stu-id="63cce-134">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="63cce-135">Фактурирането на контролна точка.</span><span class="sxs-lookup"><span data-stu-id="63cce-135">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="63cce-136">Действителни данни на фактурирани продажби за сумата на контролна точка на първоначалната контролна точка в аспекти на договор по проект.</span><span class="sxs-lookup"><span data-stu-id="63cce-136">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>
