---
title: Промени в управлението на ресурси (Project Service Automation 3.x)
description: Тази тема предоставя информация за промените в областта за управление „Ресурси“.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 03/18/2019
ms.topic: article
ms.service: business-applications
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 5176d2c6b7b00d47d4aeb12f54bdb84d4b87304c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4072011"
---
# <a name="resource-management-changes-project-service-automation-3x"></a><span data-ttu-id="4b6c2-103">Промени в управлението на ресурси (Project Service Automation 3.x)</span><span class="sxs-lookup"><span data-stu-id="4b6c2-103">Resource management changes (Project Service Automation 3.x)</span></span>

<span data-ttu-id="4b6c2-104">Разделите в тази тема предоставят информация за промените, които са направени в областта за управление „Ресурси“ на Dynamics 365 Project Service Automation версия 3.x.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-104">The sections of this topic provide information about the changes that have been made to the Resource management area of Dynamics 365 Project Service Automation version 3.x.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="4b6c2-105">Прогнозни оценки на проекта</span><span class="sxs-lookup"><span data-stu-id="4b6c2-105">Project estimates</span></span>

<span data-ttu-id="4b6c2-106">Вместо да се базират на обекта **msdyn\_projecttask** ( **Задача по проект** ), прогнозните оценки на проекта се базират на обекта **msdyn\_resourceassignment** ( **Присвояване на ресурс** ).</span><span class="sxs-lookup"><span data-stu-id="4b6c2-106">Instead of being based on the **msdyn\_projecttask** entity ( **Project Task** ), project estimates are based on the **msdyn\_resourceassignment** entity ( **Resource Assignment** ).</span></span> <span data-ttu-id="4b6c2-107">Присвояването на ресурси стана „източник на достоверни данни“ за планиране на задачи и ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-107">Resource assignments have become the "source of truth" for task scheduling and pricing.</span></span>

## <a name="line-tasks"></a><span data-ttu-id="4b6c2-108">Линейни задачи</span><span class="sxs-lookup"><span data-stu-id="4b6c2-108">Line tasks</span></span>

<span data-ttu-id="4b6c2-109">В PSA 3.x линейните задачи са остарели (отхвърлени).</span><span class="sxs-lookup"><span data-stu-id="4b6c2-109">In PSA 3.x, line tasks are obsolete (deprecated).</span></span> <span data-ttu-id="4b6c2-110">Присвояванията сега сочат към цялата задача вместо към линейните задачи.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-110">Assignments now point to the whole task instead of the line tasks.</span></span>

<span data-ttu-id="4b6c2-111">Следващият пример показва как задача, която се нарича „Тестова задача“, се присвоява на членовете на екипа А и В в по-стари версии на PSA и PSA 3.x.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-111">The following example shows how a task that is named "Test task" is assigned to team members A and B in earlier versions of PSA and in PSA 3.x.</span></span>

- <span data-ttu-id="4b6c2-112">**Преди PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="4b6c2-112">**Before PSA 3.x:**</span></span>

    - <span data-ttu-id="4b6c2-113">Тестова задача</span><span class="sxs-lookup"><span data-stu-id="4b6c2-113">Test task</span></span>

        - <span data-ttu-id="4b6c2-114">Тестова задача – линейна задача 1</span><span class="sxs-lookup"><span data-stu-id="4b6c2-114">Test task – Line task 1</span></span>

            - <span data-ttu-id="4b6c2-115">Присвояване на A</span><span class="sxs-lookup"><span data-stu-id="4b6c2-115">Assignment to A</span></span>

        - <span data-ttu-id="4b6c2-116">Тестова задача – линейна задача 2</span><span class="sxs-lookup"><span data-stu-id="4b6c2-116">Test task – Line task 2</span></span>

            - <span data-ttu-id="4b6c2-117">Присвояване на В</span><span class="sxs-lookup"><span data-stu-id="4b6c2-117">Assignment to B</span></span>

- <span data-ttu-id="4b6c2-118">**PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="4b6c2-118">**PSA 3.x:**</span></span>

    - <span data-ttu-id="4b6c2-119">Тестова задача</span><span class="sxs-lookup"><span data-stu-id="4b6c2-119">Test task</span></span>

        - <span data-ttu-id="4b6c2-120">Присвояване на A</span><span class="sxs-lookup"><span data-stu-id="4b6c2-120">Assignment to A</span></span>
        - <span data-ttu-id="4b6c2-121">Присвояване на В</span><span class="sxs-lookup"><span data-stu-id="4b6c2-121">Assignment to B</span></span>

## <a name="unassigned-assignment"></a><span data-ttu-id="4b6c2-122">Неприсвоено присвояване</span><span class="sxs-lookup"><span data-stu-id="4b6c2-122">Unassigned assignment</span></span>

<span data-ttu-id="4b6c2-123">В PSA 3.x, неприсвоено присвояване е такова, което е присвоено на член на екипа **NULL** и ресурс **NULL**.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-123">In PSA 3.x, an unassigned assignment is an assignment that is assigned to a **NULL** team member and a **NULL** resource.</span></span> <span data-ttu-id="4b6c2-124">Неприсвоени присвоявания могат да възникнат в няколко сценария:</span><span class="sxs-lookup"><span data-stu-id="4b6c2-124">Unassigned assignments can occur in a couple of scenarios:</span></span>

- <span data-ttu-id="4b6c2-125">Ако е създадена задача, но все още не е присвоена на който и да е член на екипа, винаги се създава неприсвоено присвояване.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-125">If a task has been created, but it hasn't yet been assigned to any team member, an unassigned assignment is always created.</span></span> 
- <span data-ttu-id="4b6c2-126">Ако всички, на които е присвоена дадена задача, бъдат премахнати, за тази задача се създава отново неприсвоено присвояване.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-126">If all assignees on a task are removed, an unassigned assignment is re-created for that task.</span></span>

## <a name="scheduling-fields-on-the-project-task-entity"></a><span data-ttu-id="4b6c2-127">Полета за планиране в обекта „Задача по проект“</span><span class="sxs-lookup"><span data-stu-id="4b6c2-127">Scheduling fields on the Project Task entity</span></span>

<span data-ttu-id="4b6c2-128">Полетата в обекта **msdyn\_projecttask** са отхвърлени или преместени в обекта **msdyn\_resourceassignment** , или вече получават препратки от обекта **msdyn\_projectteam** ( **Член на екипа по проект** ).</span><span class="sxs-lookup"><span data-stu-id="4b6c2-128">The fields on the **msdyn\_projecttask** entity have been deprecated or moved to the **msdyn\_resourceassignment** entity, or they are now referenced from the **msdyn\_projectteam** entity ( **Project Team Member** ).</span></span>

| <span data-ttu-id="4b6c2-129">Отхвърлено поле в msdyn\_projecttask (задача по проект)</span><span class="sxs-lookup"><span data-stu-id="4b6c2-129">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="4b6c2-130">Ново поле msdyn\_resourceassignment (присвояване на ресурси)</span><span class="sxs-lookup"><span data-stu-id="4b6c2-130">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> | <span data-ttu-id="4b6c2-131">Коментар</span><span class="sxs-lookup"><span data-stu-id="4b6c2-131">Comment</span></span> |
|---|---|---|
| <span data-ttu-id="4b6c2-132">msdyn\_assignedresources</span><span class="sxs-lookup"><span data-stu-id="4b6c2-132">msdyn\_assignedresources</span></span> | <span data-ttu-id="4b6c2-133">Няма</span><span class="sxs-lookup"><span data-stu-id="4b6c2-133">None</span></span> | |
| <span data-ttu-id="4b6c2-134">msdyn\_assignedteammembers</span><span class="sxs-lookup"><span data-stu-id="4b6c2-134">msdyn\_assignedteammembers</span></span> | <span data-ttu-id="4b6c2-135">Няма</span><span class="sxs-lookup"><span data-stu-id="4b6c2-135">None</span></span> | |
| <span data-ttu-id="4b6c2-136">msdyn\_numberofresources</span><span class="sxs-lookup"><span data-stu-id="4b6c2-136">msdyn\_numberofresources</span></span> | <span data-ttu-id="4b6c2-137">Няма</span><span class="sxs-lookup"><span data-stu-id="4b6c2-137">None</span></span> | |
| <span data-ttu-id="4b6c2-138">msdyn\_scheduledhours</span><span class="sxs-lookup"><span data-stu-id="4b6c2-138">msdyn\_scheduledhours</span></span> | <span data-ttu-id="4b6c2-139">Няма</span><span class="sxs-lookup"><span data-stu-id="4b6c2-139">None</span></span> | |
| <span data-ttu-id="4b6c2-140">msdyn\_effortcontour</span><span class="sxs-lookup"><span data-stu-id="4b6c2-140">msdyn\_effortcontour</span></span> | <span data-ttu-id="4b6c2-141">msdyn\_plannedwork</span><span class="sxs-lookup"><span data-stu-id="4b6c2-141">msdyn\_plannedwork</span></span> | <span data-ttu-id="4b6c2-142">Форматът на структурата на данни на обекта на JavaScript (JSON), който се съхранява в полето, е променен.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-142">The format of the JavaScript Object Notation (JSON) data structure that is stored in the field has been changed.</span></span> |

## <a name="schedule-contour"></a><span data-ttu-id="4b6c2-143">Контур на график</span><span class="sxs-lookup"><span data-stu-id="4b6c2-143">Schedule contour</span></span>

<span data-ttu-id="4b6c2-144">Контурът на графика се съхранява в полето **Planned Work** ( **msdyn\_plannedwork** ) на всеки обект **Присвояване на ресурс** ( **msdyn\_resourceassignment** ).</span><span class="sxs-lookup"><span data-stu-id="4b6c2-144">The schedule contour is stored in the **Planned Work** field ( **msdyn\_plannedwork** ) of each **Resource Assignment** entity ( **msdyn\_resourceassignment** ).</span></span>

### <a name="structure"></a><span data-ttu-id="4b6c2-145">Структура</span><span class="sxs-lookup"><span data-stu-id="4b6c2-145">Structure</span></span>

<span data-ttu-id="4b6c2-146">Новата структура на контура на графика се състои от гъвкави времеви срезове, дефинирани за всеки ден от графика.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-146">The new structure of the schedule contour consists of flexible time slices that are defined for each day of the schedule.</span></span> <span data-ttu-id="4b6c2-147">Всеки времеви срез има следните свойства:</span><span class="sxs-lookup"><span data-stu-id="4b6c2-147">Each time slice has the following properties:</span></span>

- <span data-ttu-id="4b6c2-148">**Начало** – началото на работното време за деня според календара на проекта.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-148">**Start** – The start of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="4b6c2-149">**Край** – краят на работното време за деня според календара на проекта.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-149">**End** – The end of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="4b6c2-150">**Часове** – броят на часовете, които са присвоени за деня.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-150">**Hours** – The number of hours that are assigned on the day.</span></span>

<span data-ttu-id="4b6c2-151">**Пример**</span><span class="sxs-lookup"><span data-stu-id="4b6c2-151">**Example**</span></span>

<span data-ttu-id="4b6c2-152">Този пример използва календар на проекта, където работният ден е от 9:00 до 17:00 в UTC-8 часова зона.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-152">This example uses a project calendar where the workday is from 9 AM to 5 PM in the UTC-8 time zone.</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

### <a name="auto-scheduling-and-manual-scheduling"></a><span data-ttu-id="4b6c2-153">Автоматично планиране и ръчно планиране</span><span class="sxs-lookup"><span data-stu-id="4b6c2-153">Auto-scheduling and manual scheduling</span></span>

<span data-ttu-id="4b6c2-154">Ако дадена задача е автоматично планирана, часовете се натоварват отпред и продължителността на задачата може да бъде намалена.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-154">If a task is auto-scheduled, the hours are front-loaded, and the task duration might be reduced.</span></span>

<span data-ttu-id="4b6c2-155">**Пример**</span><span class="sxs-lookup"><span data-stu-id="4b6c2-155">**Example**</span></span>

<span data-ttu-id="4b6c2-156">Следващата задача се планира автоматично за 18 часа в продължение на три дни (от 3 декември 2018 г. до 5 декември 2018 г.).</span><span class="sxs-lookup"><span data-stu-id="4b6c2-156">The following task is auto-scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

<span data-ttu-id="4b6c2-157">Ако дадена задача е планирана ръчно, часовете се разпределят поравно към всички дати.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-157">If a task is manually scheduled, the hours are evenly distributed to all the dates.</span></span>

<span data-ttu-id="4b6c2-158">**Пример**</span><span class="sxs-lookup"><span data-stu-id="4b6c2-158">**Example**</span></span>

<span data-ttu-id="4b6c2-159">Следващата задача се планира ръчно за 18 часа в продължение на три дни (от 3 декември 2018 г. до 5 декември 2018 г.).</span><span class="sxs-lookup"><span data-stu-id="4b6c2-159">The following task is manually scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":6},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":6},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":6}]
```

### <a name="assignment-unit"></a><span data-ttu-id="4b6c2-160">Единица на присвояване</span><span class="sxs-lookup"><span data-stu-id="4b6c2-160">Assignment unit</span></span>

<span data-ttu-id="4b6c2-161">Единицата на присвояване е отхвърлена в PSA 3.x.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-161">The assignment unit has been deprecated in PSA 3.x.</span></span> <span data-ttu-id="4b6c2-162">Часовете усилия за задачата сега са еднакво разпределени, на ден, между всички присвоени ресурси.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-162">The task effort hours are now equally divided, per day, among all the assigned resources.</span></span>

<span data-ttu-id="4b6c2-163">**Пример**</span><span class="sxs-lookup"><span data-stu-id="4b6c2-163">**Example**</span></span>

<span data-ttu-id="4b6c2-164">В този пример задачата се присвоява на два ресурса и се планира автоматично за 36 часа в продължение на три дни (от 3 декември 2018 г. до 5 декември 2018 г.).</span><span class="sxs-lookup"><span data-stu-id="4b6c2-164">In this example, the task is is assigned to two resources and is auto-scheduled for 36 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

- <span data-ttu-id="4b6c2-165">Присвояване 1:</span><span class="sxs-lookup"><span data-stu-id="4b6c2-165">Assignment 1:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

- <span data-ttu-id="4b6c2-166">Присвояване 2:</span><span class="sxs-lookup"><span data-stu-id="4b6c2-166">Assignment 2:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

## <a name="pricing-dimensions"></a><span data-ttu-id="4b6c2-167">Ценови измерения</span><span class="sxs-lookup"><span data-stu-id="4b6c2-167">Pricing dimensions</span></span>

<span data-ttu-id="4b6c2-168">В PSA 3. x специфични за ресурсите полета за ценови измерения (като **Роля** и **Организационна единица** ) са премахнати от обекта **msdyn\_projecttask**.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-168">In PSA 3.x, resource-specific pricing dimension fields (such as **Role** and **Organizational Unit** ) have been removed from the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="4b6c2-169">Тези полета сега могат да бъдат извлечени от съответния член на екипа на ( **msdyn\_projectteam** ) на присвояването на ресурс ( **msdyn\_resourceassignment** ) при генериране на прогнозни оценки за проекта.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-169">These fields can now be retrieved from the corresponding project team member ( **msdyn\_projectteam** ) of the resource assignment ( **msdyn\_resourceassignment** ) when project estimates are generated.</span></span> <span data-ttu-id="4b6c2-170">Ново поле **msdyn\_organizationalunit** е добавено към обекта **msdyn\_projectteam**.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-170">A new field, **msdyn\_organizationalunit** , has been added to the **msdyn\_projectteam** entity.</span></span>

| <span data-ttu-id="4b6c2-171">Отхвърлено поле в msdyn\_projecttask (задача по проект)</span><span class="sxs-lookup"><span data-stu-id="4b6c2-171">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="4b6c2-172">Поле от msdyn\_projectteam (член на екипа по проект), което се използва вместо</span><span class="sxs-lookup"><span data-stu-id="4b6c2-172">Field from msdyn\_projectteam (Project Team Member) that is used instead</span></span> |
|---|---|
| <span data-ttu-id="4b6c2-173">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="4b6c2-173">msdyn\_resourcecategory</span></span> | <span data-ttu-id="4b6c2-174">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="4b6c2-174">msdyn\_resourcecategory</span></span> |
| <span data-ttu-id="4b6c2-175">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="4b6c2-175">msdyn\_organizationalunit</span></span> | <span data-ttu-id="4b6c2-176">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="4b6c2-176">msdyn\_organizationalunit</span></span> |

## <a name="contours"></a><span data-ttu-id="4b6c2-177">Контури</span><span class="sxs-lookup"><span data-stu-id="4b6c2-177">Contours</span></span>

<span data-ttu-id="4b6c2-178">Полетата на контур за ценообразуване и прогнозна оценка са отхвърлени в обекта **msdyn\_projecttask**.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-178">The pricing and estimation contour fields have been deprecated on the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="4b6c2-179">Те са преместени в обекта **msdyn\_resourceassignment**.</span><span class="sxs-lookup"><span data-stu-id="4b6c2-179">They have been moved to the **msdyn\_resourceassignment** entity.</span></span>

| <span data-ttu-id="4b6c2-180">Отхвърлено поле в msdyn\_projecttask (задача по проект)</span><span class="sxs-lookup"><span data-stu-id="4b6c2-180">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="4b6c2-181">Ново поле msdyn\_resourceassignment (присвояване на ресурси)</span><span class="sxs-lookup"><span data-stu-id="4b6c2-181">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> |
|---|---|
| <span data-ttu-id="4b6c2-182">msdyn\_costestimatecontour</span><span class="sxs-lookup"><span data-stu-id="4b6c2-182">msdyn\_costestimatecontour</span></span> | <span data-ttu-id="4b6c2-183">msdyn\_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="4b6c2-183">msdyn\_plannedcostcontour</span></span> |
| <span data-ttu-id="4b6c2-184">msdyn\_salesestimatecontour</span><span class="sxs-lookup"><span data-stu-id="4b6c2-184">msdyn\_salesestimatecontour</span></span> | <span data-ttu-id="4b6c2-185">msdyn\_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="4b6c2-185">msdyn\_plannedsalescontour</span></span> |

<span data-ttu-id="4b6c2-186">Следващите полета са добавени в обекта **msdyn\_resourceassignment** :</span><span class="sxs-lookup"><span data-stu-id="4b6c2-186">The following fields have been added to the **msdyn\_resourceassignment** entity:</span></span>

* <span data-ttu-id="4b6c2-187">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="4b6c2-187">msdyn\_plannedcost</span></span>
* <span data-ttu-id="4b6c2-188">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="4b6c2-188">msdyn\_plannedsales</span></span>

<span data-ttu-id="4b6c2-189">Следващите полета за планирани, действителни и останали разходи и продажби са непроменени в обекта **msdyn\_projecttask** :</span><span class="sxs-lookup"><span data-stu-id="4b6c2-189">The following fields for planned, actual, and remaining cost and sales are unchanged on the **msdyn\_projecttask** entity:</span></span>

* <span data-ttu-id="4b6c2-190">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="4b6c2-190">msdyn\_plannedcost</span></span>
* <span data-ttu-id="4b6c2-191">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="4b6c2-191">msdyn\_plannedsales</span></span>
* <span data-ttu-id="4b6c2-192">msdyn\_actualcost</span><span class="sxs-lookup"><span data-stu-id="4b6c2-192">msdyn\_actualcost</span></span>
* <span data-ttu-id="4b6c2-193">msdyn\_actualsales</span><span class="sxs-lookup"><span data-stu-id="4b6c2-193">msdyn\_actualsales</span></span>
* <span data-ttu-id="4b6c2-194">msdyn\_remainingcost</span><span class="sxs-lookup"><span data-stu-id="4b6c2-194">msdyn\_remainingcost</span></span>
* <span data-ttu-id="4b6c2-195">msdyn\_remainingsales</span><span class="sxs-lookup"><span data-stu-id="4b6c2-195">msdyn\_remainingsales</span></span>
