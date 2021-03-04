---
title: Оттегляне на одобрени записи за време или разходи
description: Тази тема предоставя информация за това как да оттеглите преди това одобрена транзакция за време или разход.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom: ''
ms.author: rumant
ms.date: 03/08/2019
ms.topic: article
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: f9bb25ac9ef7b400063c5f958311e475de6f6506
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147820"
---
# <a name="recall-approved-time-or-expense-entries"></a><span data-ttu-id="80056-103">Оттегляне на одобрени записи за време или разходи</span><span class="sxs-lookup"><span data-stu-id="80056-103">Recall approved time or expense entries</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="80056-104">Член на екипа по проекта или друго лице, което подаде запис за време или разход, може да оттегли този запис за време или разход, след като е бил одобрен.</span><span class="sxs-lookup"><span data-stu-id="80056-104">A project team member or an other person who submits a time or expense entry can recall that time or expense entry after it has been approved.</span></span> <span data-ttu-id="80056-105">Процесът на оттегляне на одобрен запис за време или разход има две стъпки:</span><span class="sxs-lookup"><span data-stu-id="80056-105">The process for recalling an approved time or expense entry has two steps:</span></span>

1. <span data-ttu-id="80056-106">Подателят заявява оттегляне.</span><span class="sxs-lookup"><span data-stu-id="80056-106">A submitter requests a recall.</span></span>
2. <span data-ttu-id="80056-107">Одобряващият одобрява оттеглянето.</span><span class="sxs-lookup"><span data-stu-id="80056-107">An approver approves the recall.</span></span>

## <a name="request-a-recall"></a><span data-ttu-id="80056-108">Заявка за оттегляне</span><span class="sxs-lookup"><span data-stu-id="80056-108">Request a recall</span></span>

<span data-ttu-id="80056-109">Следвайте тези стъпки, за да заявите оттегляне на одобрен запис за време или разход.</span><span class="sxs-lookup"><span data-stu-id="80056-109">Follow these steps to request a recall of an approved time or expense entry.</span></span>

1. <span data-ttu-id="80056-110">За записи за време отидете на **Проекти** \> **Моята работа** \> **Запис за време**.</span><span class="sxs-lookup"><span data-stu-id="80056-110">For time entries, go to **Projects** \> **My Work** \> **Time Entry**.</span></span>

    <span data-ttu-id="80056-111">–или–</span><span class="sxs-lookup"><span data-stu-id="80056-111">–or–</span></span>

    <span data-ttu-id="80056-112">За записи за разходи отидете на **Проекти** \> **Моята работа** \> **Разходи**.</span><span class="sxs-lookup"><span data-stu-id="80056-112">For expense entries, go to **Projects** \> **My Work** \> **Expenses**.</span></span>

2. <span data-ttu-id="80056-113">За записи за време изберете всички записи за време за конкретна комбинация от проект и задача.</span><span class="sxs-lookup"><span data-stu-id="80056-113">For time entries, select all the time entries for a specific combination of a project and a task.</span></span> <span data-ttu-id="80056-114">Или в мрежата изберете отделните клетки за време на конкретна дата за конкретен проект.</span><span class="sxs-lookup"><span data-stu-id="80056-114">Alternatively, in the grid, select the individual cells for time on a specific date for a specific project.</span></span>

    <span data-ttu-id="80056-115">–или–</span><span class="sxs-lookup"><span data-stu-id="80056-115">–or–</span></span>

    <span data-ttu-id="80056-116">За записи за разходи изберете реда на записа за разход за оттегляне.</span><span class="sxs-lookup"><span data-stu-id="80056-116">For expense entries, select the row for the expense entry to recall.</span></span>

3. <span data-ttu-id="80056-117">Изберете **Оттегляне**.</span><span class="sxs-lookup"><span data-stu-id="80056-117">Select **Recall**.</span></span> <span data-ttu-id="80056-118">Появява се диалогов прозорец за потвърждение.</span><span class="sxs-lookup"><span data-stu-id="80056-118">A confirmation dialog box appears.</span></span> <span data-ttu-id="80056-119">Ако избраните записи за време и разходи са вече одобрени, ще получите подкана да въведете причина за оттеглянето.</span><span class="sxs-lookup"><span data-stu-id="80056-119">If the selected time and expense entries were already approved, you're prompted to enter a reason for the recall.</span></span>
4. <span data-ttu-id="80056-120">Въведете причина за оттеглянето и след това изберете **OK**, за да потвърдите операцията.</span><span class="sxs-lookup"><span data-stu-id="80056-120">Enter a reason for the recall, and then select **OK** to confirm the operation.</span></span> <span data-ttu-id="80056-121">Системата изпраща на лицето, което е одобрило записите, заявка за одобрение на изтеглянето.</span><span class="sxs-lookup"><span data-stu-id="80056-121">The system sends the person who approved the entries a request to approve the recall.</span></span>

> [!NOTE]
> <span data-ttu-id="80056-122">Въпреки че одобрените записи за време и разходи могат да се оттеглят, ако дадено одобрено време или разход вече са били фактурирани на клиента, не може да бъде създадена заявка за оттегляне.</span><span class="sxs-lookup"><span data-stu-id="80056-122">Although approved time and expense entries can be recalled, if an approved time or expense has already been invoiced to the customer, a recall request can't be created.</span></span> <span data-ttu-id="80056-123">Потребител, който се опитва да създаде заявка за оттегляне, ще получи съобщение, че времето или разходите не могат да бъдат оттеглени, защото вече са фактурирани.</span><span class="sxs-lookup"><span data-stu-id="80056-123">A user who tries to create a recall request will receive a message that states that the time or expense can't be recalled because it was already invoiced.</span></span>

## <a name="approve-or-reject-a-recall-request"></a><span data-ttu-id="80056-124">Одобряване или отхвърляне на заявка за оттегляне</span><span class="sxs-lookup"><span data-stu-id="80056-124">Approve or reject a recall request</span></span>

<span data-ttu-id="80056-125">Изпълнете следните стъпки, за да одобрите или отхвърлите заявка за оттегляне.</span><span class="sxs-lookup"><span data-stu-id="80056-125">Follow these steps to approve or reject a recall request.</span></span>

1. <span data-ttu-id="80056-126">Отидете на **Проекти** \> **Моята работа** \> **Одобрения**.</span><span class="sxs-lookup"><span data-stu-id="80056-126">Go to **Projects** \> **My Work** \> **Approvals**.</span></span>
2. <span data-ttu-id="80056-127">На страницата със списъка **Одобрения** променете изгледа на **Заявки за оттегляне за одобрение**.</span><span class="sxs-lookup"><span data-stu-id="80056-127">On the **Approvals** list page, change the view to **Recall requests for approval**.</span></span> <span data-ttu-id="80056-128">Показва се списък на подадените заявки за оттегляне.</span><span class="sxs-lookup"><span data-stu-id="80056-128">A list of submitted recall requests is shown.</span></span>
3. <span data-ttu-id="80056-129">Изберете един или повече записи и след това изберете **Одобрение** или **Отхвърляне**.</span><span class="sxs-lookup"><span data-stu-id="80056-129">Select one or more entries, and then select either **Approve** or **Reject**.</span></span>
4. <span data-ttu-id="80056-130">Ако сте избрали **Одобрение**, получавате предупредително съобщение, което обяснява въздействието на одобрението.</span><span class="sxs-lookup"><span data-stu-id="80056-130">If you selected **Approve**, you receive a warning message that explains the impact of the approval.</span></span> <span data-ttu-id="80056-131">Изберете **OK**, за да потвърдите операцията.</span><span class="sxs-lookup"><span data-stu-id="80056-131">Select **OK** to confirm the operation.</span></span> <span data-ttu-id="80056-132">Заявката за оттегляне е одобрена.</span><span class="sxs-lookup"><span data-stu-id="80056-132">The recall request is approved.</span></span>

    <span data-ttu-id="80056-133">–или–</span><span class="sxs-lookup"><span data-stu-id="80056-133">–or–</span></span>

    <span data-ttu-id="80056-134">Ако сте избрали **Отхвърляне**, заявката за оттегляне се отхвърля.</span><span class="sxs-lookup"><span data-stu-id="80056-134">If you selected **Reject**, the recall request is rejected.</span></span>

> [!NOTE]
> <span data-ttu-id="80056-135">Както когато се заяви оттегляне, когато се одобри оттегляне, системата проверява за всяка дейност на фактуриране в записите за време или разходи.</span><span class="sxs-lookup"><span data-stu-id="80056-135">As when a recall is requested, when a recall is approved, the system checks for any invoicing activity on the time or expense entries.</span></span> <span data-ttu-id="80056-136">Ако даден запис вече е бил фактуриран или е в чернова на фактура, одобряващият ще получи съобщение за грешка, че времето или разходите не могат да бъдат одобрени за оттегляне, защото той вече е фактуриран.</span><span class="sxs-lookup"><span data-stu-id="80056-136">If an entry was already invoiced, or if it's on a draft invoice, the approver will receive an error message that states that the time or expense can't be approved for recall, because it was already invoiced.</span></span>

## <a name="impact-of-a-recall-request"></a><span data-ttu-id="80056-137">Въздействие на заявката за оттегляне</span><span class="sxs-lookup"><span data-stu-id="80056-137">Impact of a recall request</span></span>

<span data-ttu-id="80056-138">Когато се оттегли одобрение, въздействието е оперативно и финансово.</span><span class="sxs-lookup"><span data-stu-id="80056-138">When an approval is recalled, there is both operational impact and financial impact.</span></span>

### <a name="operational-impact"></a><span data-ttu-id="80056-139">Оперативно въздействие</span><span class="sxs-lookup"><span data-stu-id="80056-139">Operational impact</span></span>

<span data-ttu-id="80056-140">Ако заявката за оттегляне е одобрена, записът за одобрение се маркира като **Отхвърлено**.</span><span class="sxs-lookup"><span data-stu-id="80056-140">If a recall request is approved, the approval record is marked as **Rejected**.</span></span> <span data-ttu-id="80056-141">Състоянието на записа се променя на **Върнато** или **Отхвърлено** в зависимост от това дали е запис за време или запис на разходи.</span><span class="sxs-lookup"><span data-stu-id="80056-141">The status of the entry is changed to either **Returned** or **Rejected**, depending on whether it's a time entry or an expense entry.</span></span>

<span data-ttu-id="80056-142">Членът на екипа на проекта може да прегледа записите, да ги редактира и след това да ги подаде отново или да ги изтрие изцяло.</span><span class="sxs-lookup"><span data-stu-id="80056-142">The project team member can view entries, edit and then resubmit entries, or delete entries entirely.</span></span>

<span data-ttu-id="80056-143">Ако заявката за оттегляне бъде отхвърлена, състоянието на записа остава **Одобрено** и записът не може да бъде редактиран от члена на екипа на проекта или от одобряващия за проекта.</span><span class="sxs-lookup"><span data-stu-id="80056-143">If a recall request is rejected, the status of the entry remains **Approved**, and the entry can't be edited by the project team member or the approver for the project.</span></span>

### <a name="financial-impact"></a><span data-ttu-id="80056-144">Финансово въздействие</span><span class="sxs-lookup"><span data-stu-id="80056-144">Financial impact</span></span>

<span data-ttu-id="80056-145">Ако заявката за оттегляне е одобрена, съответните действителни данни за разходите и продажбите се актуализират по следния начин:</span><span class="sxs-lookup"><span data-stu-id="80056-145">If a recall request is approved, the corresponding actuals for cost and sales are updated in the following manner:</span></span>

- <span data-ttu-id="80056-146">Полето **Състояние на корекцията** се актуализира на **Коригирано**.</span><span class="sxs-lookup"><span data-stu-id="80056-146">The **Adjustment Status** field is updated to **Adjusted**.</span></span>
- <span data-ttu-id="80056-147">Полето **Състояние на фактуриране** се актуализира на **Отменено**.</span><span class="sxs-lookup"><span data-stu-id="80056-147">The **Billing Status** field is updated to **Canceled**.</span></span>

<span data-ttu-id="80056-148">След това се създават записи за сторниране в таблицата „Действителни данни“.</span><span class="sxs-lookup"><span data-stu-id="80056-148">Next, reversal entries are created in the Actuals table.</span></span> <span data-ttu-id="80056-149">За да създадете записи за сторниране, системата копира отгоре стойностите на полето от първоначалните действителни данни.</span><span class="sxs-lookup"><span data-stu-id="80056-149">To create reversal entries, the system copies over the field values from the original actuals.</span></span> <span data-ttu-id="80056-150">Единствените стойности, които не се копират, са количествените стойности.</span><span class="sxs-lookup"><span data-stu-id="80056-150">The only values that aren't copied over are the quantity values.</span></span> <span data-ttu-id="80056-151">Вместо това тези стойности се сторнират.</span><span class="sxs-lookup"><span data-stu-id="80056-151">These values are reversed instead.</span></span> <span data-ttu-id="80056-152">Сторнирани действителни данни се създават за действителни данни **Разходи** и **Нефактурирани продажби**.</span><span class="sxs-lookup"><span data-stu-id="80056-152">Reversed actuals are created for both **Cost** and **Unbilled Sales** actuals.</span></span> <span data-ttu-id="80056-153">Полето **Състояние на корекцията** на сторнирани действителни данни се задава на **Некоректируемо** и полето **Състояние на фактуриране** се задава на **Отменено**.</span><span class="sxs-lookup"><span data-stu-id="80056-153">The **Adjustment Status** field on the reversed actuals is set to **Unadjustable**, and the **Billing status** field is set to **Canceled**.</span></span> <span data-ttu-id="80056-154">Поради тези промени записаните разходи и натрупаните приходи по проекта вече няма да отчитат сумите, които тези действителни данни представляват.</span><span class="sxs-lookup"><span data-stu-id="80056-154">Because of these changes, the recorded spending and the revenue backlog on the project will no longer account for the amounts that these actuals represent.</span></span>

<span data-ttu-id="80056-155">Ако заявката за оттегляне бъде отхвърлена, няма финансово въздействие върху проекта.</span><span class="sxs-lookup"><span data-stu-id="80056-155">If a recall request is rejected, there is no financial impact on the project.</span></span>

## <a name="changes-to-time-entry-records"></a><span data-ttu-id="80056-156">Промени в записи за време</span><span class="sxs-lookup"><span data-stu-id="80056-156">Changes to time entry records</span></span>

<span data-ttu-id="80056-157">Следната илюстрация показва промените, които възникват за одобрените записи за време, когато се отменят.</span><span class="sxs-lookup"><span data-stu-id="80056-157">The following illustration shows the changes that occur for approved time entries when they are recalled.</span></span>

![Преходи в състояние на записи за време](media/TimeEntryStateTransitions.png)

## <a name="changes-to-expense-entry-records"></a><span data-ttu-id="80056-159">Промени в записи за разходи</span><span class="sxs-lookup"><span data-stu-id="80056-159">Changes to expense entry records</span></span>

<span data-ttu-id="80056-160">Следната илюстрация показва промените, които възникват за одобрените записи за разходи, когато се отменят.</span><span class="sxs-lookup"><span data-stu-id="80056-160">The following illustration shows the changes that occur for approved expense entries when they are recalled.</span></span>

![Преходи в състояние на записи за разходи](media/ExpenseEntryStateTransitions.png)
