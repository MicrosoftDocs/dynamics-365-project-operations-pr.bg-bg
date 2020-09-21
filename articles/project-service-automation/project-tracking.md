---
title: Напредък и консумация на разход на проекти
description: Тази тема предоставя информация за това как да проследявате напредъка на проекта и консумацията на разходите.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 0d742164-5469-421d-8917-63160a81f651
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8aa5814938129f30885d8161a7c86197ab013364
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749343"
---
# <a name="project-progress-and-cost-consumption"></a><span data-ttu-id="72a04-103">Напредък и консумация на разход на проекти</span><span class="sxs-lookup"><span data-stu-id="72a04-103">Project progress and cost consumption</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="72a04-104">Необходимостта от проследяване на напредъка спрямо графика варира в зависимост от отрасъла.</span><span class="sxs-lookup"><span data-stu-id="72a04-104">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="72a04-105">Някои отрасли проследяват на детайлно ниво, докато други отрасли проследяват на по-високо ниво.</span><span class="sxs-lookup"><span data-stu-id="72a04-105">Some industries track at a granular level, whereas other industries track at a higher level.</span></span> <span data-ttu-id="72a04-106">Тази тема показва как да планирате графика, за да отговорите на изискванията на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="72a04-106">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="72a04-107">Изглед за проследяване на усилие</span><span class="sxs-lookup"><span data-stu-id="72a04-107">Effort tracking view</span></span>

<span data-ttu-id="72a04-108">Изгледът **Проследяване на усилията** проследява напредъка на задачите в графика.</span><span class="sxs-lookup"><span data-stu-id="72a04-108">The **Effort tracking** view tracks the progress of tasks in the schedule.</span></span> <span data-ttu-id="72a04-109">Той сравнява действителните часове на усилия, изразходвани за дадена задача, спрямо планираните часове на усилия за тази задача.</span><span class="sxs-lookup"><span data-stu-id="72a04-109">It compares the actual effort hours that have been spent on a task to the planned effort hours for that task.</span></span> <span data-ttu-id="72a04-110">PSA използва следните формули, за да изчисли показателите за проследяване:</span><span class="sxs-lookup"><span data-stu-id="72a04-110">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="72a04-111">Процент на напредъка = действителни усилия, изразходвани до момента ÷ планирани усилия за задачата</span><span class="sxs-lookup"><span data-stu-id="72a04-111">Progress percentage = Actual effort spent to date ÷ Planned effort for the task</span></span> 
- <span data-ttu-id="72a04-112">Оценка до завършване (ОДЗ) = планирани усилия – действителни усилия, изразходвани до момента</span><span class="sxs-lookup"><span data-stu-id="72a04-112">Estimate to complete (ETC) = Planned effort – Actual effort spent to date</span></span> 
- <span data-ttu-id="72a04-113">Оценка при завършване (ОПЗ) = оставащи усилия + действителни усилия, изразходвани до момента</span><span class="sxs-lookup"><span data-stu-id="72a04-113">Estimate at complete (EAC) = Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="72a04-114">Прогнозна разлика в усилията = планирани усилия – ОПЗ</span><span class="sxs-lookup"><span data-stu-id="72a04-114">Projected effort variance = Planned effort – EAC</span></span>

<span data-ttu-id="72a04-115">PSA показва прогнозна разлика в усилията за задачата.</span><span class="sxs-lookup"><span data-stu-id="72a04-115">PSA shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="72a04-116">Ако ОПЗ е повече от планираното усилие, задачата се предвижда да отнеме повече време, отколкото е планирано първоначално.</span><span class="sxs-lookup"><span data-stu-id="72a04-116">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned.</span></span> <span data-ttu-id="72a04-117">Затова изостава от графика.</span><span class="sxs-lookup"><span data-stu-id="72a04-117">Therefore, it's behind schedule.</span></span> <span data-ttu-id="72a04-118">Ако ОПЗ е по-малко от планираното усилие, задачата се предвижда да отнеме по-малко време, отколкото е планирано първоначално.</span><span class="sxs-lookup"><span data-stu-id="72a04-118">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned.</span></span> <span data-ttu-id="72a04-119">Затова изпреварва графика.</span><span class="sxs-lookup"><span data-stu-id="72a04-119">Therefore, it's ahead of schedule.</span></span>

## <a name="re-projecting-effort"></a><span data-ttu-id="72a04-120">Повторно прогнозиране на усилията</span><span class="sxs-lookup"><span data-stu-id="72a04-120">Re-projecting effort</span></span>

<span data-ttu-id="72a04-121">Обичайно за ръководител на проект е да преразглежда на първоначалните прогнозни оценки за задача.</span><span class="sxs-lookup"><span data-stu-id="72a04-121">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="72a04-122">Повторните прогнози на проекта са разбирането на прогнозните оценки на ръководителя на проекта, като се има предвид текущото състояние на проекта.</span><span class="sxs-lookup"><span data-stu-id="72a04-122">Project re-projections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="72a04-123">Ние обаче не препоръчваме на мениджърите на проекти да променят базовите числа, защото базовата линия на проекта представлява установеният източник на достоверни данни за графика на проекта и прогнозните разходи и всички заинтересовани лица по проекта са я приели.</span><span class="sxs-lookup"><span data-stu-id="72a04-123">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="72a04-124">Има два начина, по които ръководител на проект може да прогнозира повторно усилия по задачи:</span><span class="sxs-lookup"><span data-stu-id="72a04-124">There are two ways that a project manager can re-project effort on tasks:</span></span>

- <span data-ttu-id="72a04-125">Заместване на ОДЗ по подразбиране с нова прогнозна оценка на действителните оставащите усилия по задачата.</span><span class="sxs-lookup"><span data-stu-id="72a04-125">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="72a04-126">Заместване на процента на напредъка по подразбиране с нова прогнозна оценка на действителния напредък по задачата.</span><span class="sxs-lookup"><span data-stu-id="72a04-126">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="72a04-127">Всеки от тези подходи води до преизчисляване на ОДЗ, ОПЗ и процента на напредък по задачата и прогнозираната разлика в усилията по дадена задача.</span><span class="sxs-lookup"><span data-stu-id="72a04-127">Each of these approaches cause a recalculation of the task's ETC, EAC, and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="72a04-128">ОДЗ, ОПЗ и процентът на напредъка по обобщаващи задачи също се преизчисляват и създават нова прогноза за разлика в усилията.</span><span class="sxs-lookup"><span data-stu-id="72a04-128">The EAC, ETC, and progress percentage on the summary tasks are also recalculated, and produce a new projection of effort variance.</span></span>

## <a name="re-projection-of-effort-on-summary-tasks"></a><span data-ttu-id="72a04-129">Повторно прогнозиране на усилията за обобщени задачи</span><span class="sxs-lookup"><span data-stu-id="72a04-129">Re-projection of effort on summary tasks</span></span>

<span data-ttu-id="72a04-130">Усилията за обобщени задачи или задачи на контейнери могат да бъдат повторно прогнозирани.</span><span class="sxs-lookup"><span data-stu-id="72a04-130">Effort on summary tasks or container tasks can be re-projected.</span></span> <span data-ttu-id="72a04-131">Независимо от това дали потребителят повторно прогнозира чрез използване на оставащите усилия или процента на напредъка за обобщените задачи, започва следният набор от изчисления:</span><span class="sxs-lookup"><span data-stu-id="72a04-131">Regardless of whether the user re-projects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="72a04-132">Изчисляват се ОПЗ, ОДЗ и процентът на напредъка по задачата.</span><span class="sxs-lookup"><span data-stu-id="72a04-132">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="72a04-133">Новата ОПЗ е разпределена до дъщерни задачи в същото съотношение, както оригиналната ОПЗ е била в задачата.</span><span class="sxs-lookup"><span data-stu-id="72a04-133">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="72a04-134">Изчислява се новата ОПЗ за всяка от индивидуалните задачи надолу до задачите в крайния възел.</span><span class="sxs-lookup"><span data-stu-id="72a04-134">The new EAC on each of the individualt tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="72a04-135">ОДЗ и процентът на напредъка на засегнатите дъщерни задачи надолу до крайните възли се преизчисляват въз основа на стойността на ОПЗ.</span><span class="sxs-lookup"><span data-stu-id="72a04-135">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="72a04-136">Това води до нова прогноза за разликата в усилията на задачата.</span><span class="sxs-lookup"><span data-stu-id="72a04-136">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="72a04-137">Изчисляват се ОПЗ на обобщените задачи чак до основния възел.</span><span class="sxs-lookup"><span data-stu-id="72a04-137">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="72a04-138">Изглед „Проследяване на разходи“</span><span class="sxs-lookup"><span data-stu-id="72a04-138">Cost tracking view</span></span> 

<span data-ttu-id="72a04-139">Изгледът **Проследяване на разходи** сравнява действителните разходи, изразходвани за задача, с планираните разходи за дадена задача.</span><span class="sxs-lookup"><span data-stu-id="72a04-139">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost on a task.</span></span> 

> [!NOTE]
> <span data-ttu-id="72a04-140">Този изглед показва само разходи за труд и не включва разходи от прогнозните разходи.</span><span class="sxs-lookup"><span data-stu-id="72a04-140">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> 

<span data-ttu-id="72a04-141">PSA използва следните формули, за да изчисли показателите за проследяване:</span><span class="sxs-lookup"><span data-stu-id="72a04-141">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="72a04-142">Процент на консумираните разходи = действителни данни за разходи, направени до момента ÷ планирани разходи за задачата</span><span class="sxs-lookup"><span data-stu-id="72a04-142">Percentage of cost consumed = Actual cost spent to date ÷ Planned cost for the task</span></span>
- <span data-ttu-id="72a04-143">Разходи до завършване (РДЗ) = планирани разходи – действителни данни за разходи, направени до момента</span><span class="sxs-lookup"><span data-stu-id="72a04-143">Cost to complete (CTC) = Planned cost – Actual cost spent to date</span></span>
- <span data-ttu-id="72a04-144">ОПЗ = РДЗ + действителни данни за разходи, направени до момента</span><span class="sxs-lookup"><span data-stu-id="72a04-144">EAC = CTC + Actual cost spent to date</span></span>
- <span data-ttu-id="72a04-145">Прогнозна разлика в разходите = планиран разход – ОПЗ</span><span class="sxs-lookup"><span data-stu-id="72a04-145">Projected cost variance = Planned cost – EAC</span></span>

<span data-ttu-id="72a04-146">В задачата е показана прогноза за разликата в разходите.</span><span class="sxs-lookup"><span data-stu-id="72a04-146">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="72a04-147">Ако ОПЗ е повече от планирания разход, задачата се предвижда да струва повече, отколкото е планирано първоначално.</span><span class="sxs-lookup"><span data-stu-id="72a04-147">If the EAC is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="72a04-148">Ето защо това е тенденция над бюджета.</span><span class="sxs-lookup"><span data-stu-id="72a04-148">Therefore, it's trending over budget.</span></span> <span data-ttu-id="72a04-149">Ако ОПЗ е по-малко от планирания разход, задачата се предвижда да струва по-малко, отколкото е планирано първоначално.</span><span class="sxs-lookup"><span data-stu-id="72a04-149">If the EAC is less than the planned cost, the task is projected to cost less than was originally planned.</span></span> <span data-ttu-id="72a04-150">Ето защо това е тенденция под бюджета.</span><span class="sxs-lookup"><span data-stu-id="72a04-150">Therefore, it's trending under budget.</span></span>

## <a name="project-managers-re-projection-of-cost"></a><span data-ttu-id="72a04-151">Повторно прогнозиране на разходите на мениджъра на проекта</span><span class="sxs-lookup"><span data-stu-id="72a04-151">Project manager’s re-projection of cost</span></span>

<span data-ttu-id="72a04-152">Когато усилията се прогнозират отново, РДЗ, ОПЗ, процентът на консумираните разходи и прогнозираната разлика в разходите се преизчисляват в изгледа **Проследяване на разходите**.</span><span class="sxs-lookup"><span data-stu-id="72a04-152">When effort is re-projected, the CTC, EAC, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="72a04-153">Обобщение на състоянието на проекта</span><span class="sxs-lookup"><span data-stu-id="72a04-153">Project status summary</span></span>

<span data-ttu-id="72a04-154">Проследяването на данни в изгледите **Проследяване на усилията** и **Проследяване на разходите** показва напредъка и консумацията на разходите на нивото на основния възел на проекта, обобщените задачи и задачите при крайния възел.</span><span class="sxs-lookup"><span data-stu-id="72a04-154">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="72a04-155">Секцията **Състояние** на страницата **Обект на проекта** показва обобщение на състоянието на проектно ниво.</span><span class="sxs-lookup"><span data-stu-id="72a04-155">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="72a04-156">Полета за обобщение на състоянието</span><span class="sxs-lookup"><span data-stu-id="72a04-156">Status summary fields</span></span>

<span data-ttu-id="72a04-157">Полето **Цялостно състояние на проекта** е редактируемо поле, което показва цялостното състояние на проекта.</span><span class="sxs-lookup"><span data-stu-id="72a04-157">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="72a04-158">То използва цветово кодиране, като зелено, жълто и червено, за да покаже нарастващ риск.</span><span class="sxs-lookup"><span data-stu-id="72a04-158">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="72a04-159">Полето **Коментари** позволява на мениджъра на проекти да въведете конкретни коментари за състоянието.</span><span class="sxs-lookup"><span data-stu-id="72a04-159">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="72a04-160">Полето **Състоянието е актуализирано на** не може да се редактира и стойността е времево клеймо, който показва кога актуализирано за последно състоянието.</span><span class="sxs-lookup"><span data-stu-id="72a04-160">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="72a04-161">Полетата **Ефективност на графика** и **Ефективност на разходите** се задават от датата на проследяване.</span><span class="sxs-lookup"><span data-stu-id="72a04-161">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="72a04-162">Когато графикът и разликата в разходите за основния възел в изгледа **Проследяване на усилията** са положителни, можете да зададете тези полета на **Изпреварване**.</span><span class="sxs-lookup"><span data-stu-id="72a04-162">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="72a04-163">Когато графикът и разликата в разходите за основния възел са отрицателни, можете да ги зададете на **Изоставане**.</span><span class="sxs-lookup"><span data-stu-id="72a04-163">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>
