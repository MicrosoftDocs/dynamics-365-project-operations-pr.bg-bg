---
title: Отмяна на преди това одобрени записи за време и разходи
description: Тази тема предоставя информация за това как да отмените одобрена транзакция за време и разход по проект.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/07/2019
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
ms.openlocfilehash: 84fc057599dd98162320d6104ed4a7612e894ecb
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4123320"
---
# <a name="cancel-previously-approved-time-or-expense-entries"></a><span data-ttu-id="e1a34-103">Отмяна на преди това одобрени записи за време или разходи</span><span class="sxs-lookup"><span data-stu-id="e1a34-103">Cancel previously approved time or expense entries</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="e1a34-104">В най-новата версия на Dynamics 365 Project Service Automation одобряващите могат да анулират записи за време или разходи, които преди това са одобрили.</span><span class="sxs-lookup"><span data-stu-id="e1a34-104">In the latest version of Dynamics 365 Project Service Automation, approvers can cancel time or expense entries that they previously approved.</span></span>

## <a name="cancel-a-previously-approved-time-or-expense-entry"></a><span data-ttu-id="e1a34-105">Отмяна на преди това одобрен запис за време или разходи</span><span class="sxs-lookup"><span data-stu-id="e1a34-105">Cancel a previously approved time or expense entry</span></span>

<span data-ttu-id="e1a34-106">Следвайте тези стъпки, за да отмените запис за време или разход, който сте одобрили преди това.</span><span class="sxs-lookup"><span data-stu-id="e1a34-106">Follow these steps to cancel a time or expense entry that you previously approved.</span></span>

1. <span data-ttu-id="e1a34-107">Отидете на **Проекти** \> **Моята работа** \> **Одобрения**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-107">Go to **Projects** \> **My Work** \> **Approvals**.</span></span>
2. <span data-ttu-id="e1a34-108">На страницата със списъка **Одобрения** променете изгледа на **Моите минали одобрения**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-108">On the **Approvals** list page, change the view to **My past approvals**.</span></span> <span data-ttu-id="e1a34-109">Показва се списък на записите за време и разходи, които преди това сте одобрили.</span><span class="sxs-lookup"><span data-stu-id="e1a34-109">A list of the time and expense entries that you previously approved is shown.</span></span>
3. <span data-ttu-id="e1a34-110">Изберете един или повече записи и след това изберете **Отмяна на одобрение**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-110">Select one or more entries, and then select **Cancel approval**.</span></span> <span data-ttu-id="e1a34-111">Получавате предупредително съобщение.</span><span class="sxs-lookup"><span data-stu-id="e1a34-111">You receive a warning message.</span></span>
4. <span data-ttu-id="e1a34-112">Изберете **ОК**, за да отмените одобрението.</span><span class="sxs-lookup"><span data-stu-id="e1a34-112">Select **OK** to cancel the approval.</span></span>

## <a name="understand-the-impact-of-canceling-a-time-or-expense-entry-approval"></a><span data-ttu-id="e1a34-113">Разбиране на въздействието от отмяната на одобрение на запис за време или разходи</span><span class="sxs-lookup"><span data-stu-id="e1a34-113">Understand the impact of canceling a time or expense entry approval</span></span>

<span data-ttu-id="e1a34-114">Когато се отмени одобрение, въздействието е оперативно и финансово.</span><span class="sxs-lookup"><span data-stu-id="e1a34-114">When an approval is canceled, there is both operational impact and financial impact.</span></span>

### <a name="operational-impact"></a><span data-ttu-id="e1a34-115">Оперативно въздействие</span><span class="sxs-lookup"><span data-stu-id="e1a34-115">Operational impact</span></span>

<span data-ttu-id="e1a34-116">От страна на операциите, когато дадено одобрение бъде отменено, състоянието на записа се връща към **Чернова** и одобрението вече не се появява в изгледа **Моите минали одобрения**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-116">On the operations side, when an approval is canceled, the status of the record is reset to **Draft**, and the approval no longer appears in the **My past approvals** view.</span></span> <span data-ttu-id="e1a34-117">Вместо това отмененото одобрение се появява или в изгледа **Записи за време за одобрение**, или в изгледа **Записи за разходи за одобрение**, в зависимост от това дали е запис за време или запис на разходи.</span><span class="sxs-lookup"><span data-stu-id="e1a34-117">Instead, the canceled approval appears in either the **Time entries for approval** view or the **Expense entries for approval** view, depending on whether it was a time entry or an expense entry.</span></span> <span data-ttu-id="e1a34-118">Освен това състоянието на свързания запис за време или разходи се променя на **Подадено**, така че свързаният запис да е в съответствие с одобренията, които имат състояние **Чернова**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-118">Additionally, the status of the related time or expense entry is changed to **Submitted**, so that the related entry is consistent with approvals that have a status of **Draft**.</span></span>

<span data-ttu-id="e1a34-119">Като одобряващ можете да редактирате някои от полетата на одобрение, което има състояние **Чернова**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-119">As an approver, you can edit some of the fields of an approval that has a status of **Draft**.</span></span> <span data-ttu-id="e1a34-120">Тези полета включват **Тип фактуриране** и **Платими часове за записи за време**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-120">These fields include **Billing Type** and **Billable Hours for Time Entries**.</span></span> <span data-ttu-id="e1a34-121">След като направите промени, можете да одобрите записа отново.</span><span class="sxs-lookup"><span data-stu-id="e1a34-121">After you make changes, you can approve the record again.</span></span> <span data-ttu-id="e1a34-122">Или можете да отхвърлите записа.</span><span class="sxs-lookup"><span data-stu-id="e1a34-122">Alternatively, you can reject the entry.</span></span> <span data-ttu-id="e1a34-123">Ако отхвърлите одобрението на запис за време, състоянието на записа се променя на **Върнато**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-123">If you reject the approval of a time entry, the status of the entry is changed to **Returned**.</span></span> <span data-ttu-id="e1a34-124">Ако отхвърлите одобрението на запис за разходи, състоянието се променя на **Отхвърлено**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-124">If you reject the approval of an expense entry, the status is changed to **Rejected**.</span></span> <span data-ttu-id="e1a34-125">Функционално, върнатите и отхвърлени записи се държат като запис, който има състояние **Чернова**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-125">Functionally, both returned and rejected entries behave the same as an entry that has a status of **Draft**.</span></span> <span data-ttu-id="e1a34-126">Член на екипа на проекта може да направи всички необходими промени в записа и след това да го подаде отново за одобрение или да изтрие изцяло записа.</span><span class="sxs-lookup"><span data-stu-id="e1a34-126">A project team member can either make any required changes to the entry and then resubmit it for approval, or delete the entry entirely.</span></span>

### <a name="financial-impact"></a><span data-ttu-id="e1a34-127">Финансово въздействие</span><span class="sxs-lookup"><span data-stu-id="e1a34-127">Financial impact</span></span>

<span data-ttu-id="e1a34-128">Проектът се засяга също и финансово, когато дадено одобрение бъде отменено.</span><span class="sxs-lookup"><span data-stu-id="e1a34-128">A project is also affected financially when an approval is canceled.</span></span> <span data-ttu-id="e1a34-129">Първо, съответните действителни данни за разходите и продажбите се актуализират по следния начин:</span><span class="sxs-lookup"><span data-stu-id="e1a34-129">First, the corresponding actuals for cost and sales are updated in the following manner:</span></span>

- <span data-ttu-id="e1a34-130">Състоянието на корекцията се задава на **Коригирано**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-130">The adjustment status is set to **Adjusted**.</span></span>
- <span data-ttu-id="e1a34-131">Състоянието на фактуриране се задава на **Отменено**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-131">The billing status is set to **Canceled**.</span></span>

<span data-ttu-id="e1a34-132">След това се създават записи за сторниране в таблицата „Действителни данни“.</span><span class="sxs-lookup"><span data-stu-id="e1a34-132">Next, reversal entries are created in the Actuals table.</span></span> <span data-ttu-id="e1a34-133">За да създадете записи за сторниране, системата копира отгоре стойностите на полето от първоначалните действителни данни.</span><span class="sxs-lookup"><span data-stu-id="e1a34-133">To create reversal entries, the system copies over the field values from the original actuals.</span></span> <span data-ttu-id="e1a34-134">Единствените стойности, които не се копират, са количествените стойности.</span><span class="sxs-lookup"><span data-stu-id="e1a34-134">The only values that aren't copied over are the quantity values.</span></span> <span data-ttu-id="e1a34-135">Вместо това тези стойности се сторнират.</span><span class="sxs-lookup"><span data-stu-id="e1a34-135">These values are reversed instead.</span></span> <span data-ttu-id="e1a34-136">Сторнирани действителни данни се създават за действителни данни **Разходи** и **Нефактурирани продажби**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-136">Reversed actuals are created for both **Cost** and **Unbilled Sales** actuals.</span></span> <span data-ttu-id="e1a34-137">Полето **Състояние на корекцията** на сторнирани действителни данни се задава на **Некоректируемо**, а състоянието на фактуриране се задава на **Отменено**.</span><span class="sxs-lookup"><span data-stu-id="e1a34-137">The **Adjustment Status** field on the reversed actuals is set to **Unadjustable**, and the billing status is set to **Canceled**.</span></span>

<span data-ttu-id="e1a34-138">След като тези промени бъдат направени, сумата, която е записана като изразходвана по проекта, и натрупаните приходи по проекта вече няма да отчитат сумите, които тези действителни данни представляват.</span><span class="sxs-lookup"><span data-stu-id="e1a34-138">After these changes are made, the amount that is recorded as spent on the project and the revenue backlog on the project will longer account for the amounts that these actuals represent.</span></span>
