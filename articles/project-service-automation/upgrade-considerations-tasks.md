---
title: Съображения за надстройване за съставната структура на работата
description: Тази тема предоставя информация за надстройване на съставната структура на работата от Project Service Automation 2.x до 3.x.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 Project Service Automation 2.x
author: ruhercul
ms.assetid: 9e43d5b5-ca5d-41f5-9012-c48f8e3080f9
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 9aa35dd8784bfa55737b0836e653afd0442b80c2
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749321"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a><span data-ttu-id="93284-103">Съображения за надстройване за съставната структура на работата</span><span class="sxs-lookup"><span data-stu-id="93284-103">Upgrade considerations for the work breakdown structure</span></span>
<span data-ttu-id="93284-104">Тази тема предоставя информация за надстройване на съставната структура на работата от Project Service Automation 2.x до 3.x.</span><span class="sxs-lookup"><span data-stu-id="93284-104">This topic provides information about upgrading the work breakdown structure from Project Service Automation 2.x to 3.x.</span></span> <span data-ttu-id="93284-105">Тази тема определя изправното състояние на проект в Project Service Automation (PSA), което е необходимо за успешно надстройване.</span><span class="sxs-lookup"><span data-stu-id="93284-105">This topic defines the healthy state of a project in Project Service Automation (PSA) that is required for a successful upgrade.</span></span> <span data-ttu-id="93284-106">Има и информация за често срещаните условия за блокиране, които ще доведат до неуспешно надстройване.</span><span class="sxs-lookup"><span data-stu-id="93284-106">There is also information about the common blocking conditions that will cause upgrade to fail.</span></span> <span data-ttu-id="93284-107">За повече информация относно определянето на задачи по проекти и техните функции в график на проекти вижте [Графици на проекти](project-creating.md).</span><span class="sxs-lookup"><span data-stu-id="93284-107">For more information about defining project tasks and their functions within a project schedule, see [Project schedules](project-creating.md).</span></span>

## <a name="key-entities"></a><span data-ttu-id="93284-108">Основни обекти</span><span class="sxs-lookup"><span data-stu-id="93284-108">Key entities</span></span>
<span data-ttu-id="93284-109">За точна съставна структура на работата, която вече е натоварена с ресурси, се изискват следните обекти:</span><span class="sxs-lookup"><span data-stu-id="93284-109">For an accurate work breakdown structure that is already loaded with resources, the following entities are required:</span></span>

- [<span data-ttu-id="93284-110">Проект</span><span class="sxs-lookup"><span data-stu-id="93284-110">Project</span></span>](../developer/entities/msdyn_project.md)
- [<span data-ttu-id="93284-111">Екип на проект</span><span class="sxs-lookup"><span data-stu-id="93284-111">Project Team</span></span>](../developer/entities/msdyn_projectteam.md)
- [<span data-ttu-id="93284-112">Задача от проект</span><span class="sxs-lookup"><span data-stu-id="93284-112">Project Task</span></span>](../developer/entities/msdyn_projecttask.md)
- [<span data-ttu-id="93284-113">Присвоявания на ресурси</span><span class="sxs-lookup"><span data-stu-id="93284-113">Resource Assignments</span></span>](../developer/entities/msdyn_resourceassignment.md)
- [<span data-ttu-id="93284-114">Зависимост на задачи от проект</span><span class="sxs-lookup"><span data-stu-id="93284-114">Project Task Dependency</span></span>](../developer/entities/msdyn_projecttaskdependency.md)
- [<span data-ttu-id="93284-115">Налични ресурси</span><span class="sxs-lookup"><span data-stu-id="93284-115">Bookable Resources</span></span>](../developer/entities/bookableresource.md)

<span data-ttu-id="93284-116">За да дефинирате съставна структура на работата, натоварена с ресурси, трябва да изпълните следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="93284-116">To define a resource loaded work breakdown structure, you must complete the following steps:</span></span>

1. <span data-ttu-id="93284-117">Създайте нов проект.</span><span class="sxs-lookup"><span data-stu-id="93284-117">Create a new project.</span></span> <span data-ttu-id="93284-118">За повече информация как да създадете нов проект вижте [msdyn_project](../developer/entities/msdyn_project.md).</span><span class="sxs-lookup"><span data-stu-id="93284-118">For more information about how to create a new project, see [msdyn_project](../developer/entities/msdyn_project.md).</span></span>
2. <span data-ttu-id="93284-119">Създайте една или повече задачи.</span><span class="sxs-lookup"><span data-stu-id="93284-119">Create one or more tasks.</span></span> <span data-ttu-id="93284-120">За повече информация как да създадете задача вижте [msdyn_projecttask](../developer/entities/msdyn_projecttask.md).</span><span class="sxs-lookup"><span data-stu-id="93284-120">For more information about how to create a task, see [msdyn_projecttask](../developer/entities/msdyn_projecttask.md).</span></span>
3. <span data-ttu-id="93284-121">Дефинирайте зависимостите на задачата.</span><span class="sxs-lookup"><span data-stu-id="93284-121">Define the task dependencies.</span></span> <span data-ttu-id="93284-122">За повече информация вижте [Зависимост на задачи от проект](../developer/entities/msdyn_projecttaskdependency.md),</span><span class="sxs-lookup"><span data-stu-id="93284-122">For more information, see [Project Task Dependency](../developer/entities/msdyn_projecttaskdependency.md).</span></span>
4. <span data-ttu-id="93284-123">Присвоете членове на екипа на проекта към проекта.</span><span class="sxs-lookup"><span data-stu-id="93284-123">Assign project team members to the project.</span></span> <span data-ttu-id="93284-124">За повече информация вижте [msdyn_projectteam](../developer/entities/msdyn_projectteam.md).</span><span class="sxs-lookup"><span data-stu-id="93284-124">For more information, see [msdyn_projectteam](../developer/entities/msdyn_projectteam.md).</span></span>
5. <span data-ttu-id="93284-125">Присвоете членове на екипа на проекта към задачите.</span><span class="sxs-lookup"><span data-stu-id="93284-125">Assign project team members to the tasks.</span></span> <span data-ttu-id="93284-126">За повече информация вижте [msdyn_resourceassignment](../developer/entities/msdyn_resourceassignment.md).</span><span class="sxs-lookup"><span data-stu-id="93284-126">For more information, see [msdyn_resourceassignment](../developer/entities/msdyn_resourceassignment.md).</span></span>

## <a name="project-team-relationships"></a><span data-ttu-id="93284-127">Релации на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="93284-127">Project team relationships</span></span>

<span data-ttu-id="93284-128">За да осигурите успешна надстройка, следните релации трябва да се поддържат правилно:</span><span class="sxs-lookup"><span data-stu-id="93284-128">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>
- <span data-ttu-id="93284-129">Всички членове на екипа на проект трябва да бъдат свързани с наличен ресурс.</span><span class="sxs-lookup"><span data-stu-id="93284-129">All project team members must be associated with a bookable resource.</span></span>
- <span data-ttu-id="93284-130">Всички членове на екипа на проект трябва да бъдат свързани с един и същ проект.</span><span class="sxs-lookup"><span data-stu-id="93284-130">All project team members must be associated with the same project.</span></span> 

## <a name="project-task-relationships"></a><span data-ttu-id="93284-131">Релации на задачите на проект</span><span class="sxs-lookup"><span data-stu-id="93284-131">Project task relationships</span></span>
<span data-ttu-id="93284-132">За да осигурите успешна надстройка, следните релации трябва да се поддържат правилно:</span><span class="sxs-lookup"><span data-stu-id="93284-132">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="93284-133">Всички свързани задачи трябва да бъдат свързани с един и същ проект.</span><span class="sxs-lookup"><span data-stu-id="93284-133">Any related tasks must be associated with the same project.</span></span>
- <span data-ttu-id="93284-134">Всяка линейна задача трябва да има родителска задача.</span><span class="sxs-lookup"><span data-stu-id="93284-134">Every line task must have a parent task.</span></span>
- <span data-ttu-id="93284-135">Всяка задача трябва да има родителски проект.</span><span class="sxs-lookup"><span data-stu-id="93284-135">Every task must have a parent project.</span></span>

### <a name="valid-conditions"></a><span data-ttu-id="93284-136">Валидни условия</span><span class="sxs-lookup"><span data-stu-id="93284-136">Valid conditions</span></span>

- <span data-ttu-id="93284-137">Цялата продължителност на задачата трябва да бъде по-голяма или равна на (> =) един час и по-малка от 1 800 000 минути (1250 дни).\*</span><span class="sxs-lookup"><span data-stu-id="93284-137">All task durations must be greater than or equal to (>=) one hour and less than 1,800,000 minutes (1,250 days).\*</span></span>
- <span data-ttu-id="93284-138">Всички задачи трябва да имат начална дата не по-рано от 2000/01/01.\*</span><span class="sxs-lookup"><span data-stu-id="93284-138">All tasks must have a start date no earlier than 2000/01/01.\*</span></span>
- <span data-ttu-id="93284-139">Всички задачи трябва да имат начална дата не по-късно от 17 години от настоящия ден.\*</span><span class="sxs-lookup"><span data-stu-id="93284-139">All tasks must have a start date no later than 17 years from the present day.\*</span></span>
- <span data-ttu-id="93284-140">Всички задачи трябва да имат начална дата, по-ранна или същата като датата на завършване.</span><span class="sxs-lookup"><span data-stu-id="93284-140">All tasks must have a start date earlier or equal to their finish date.</span></span>
- <span data-ttu-id="93284-141">Всички типове транзакции по класификации (разходи, материали, данъци и време) трябва да имат стойности за **Единица по подразбиране** и **Група единици**.</span><span class="sxs-lookup"><span data-stu-id="93284-141">All transaction types on classifications (Expense, Material, Tax, and Time) must have values for **Default Unit** and **Unit Group**.</span></span>
- <span data-ttu-id="93284-142">Форматите за дата с букви трябва да се избягват.</span><span class="sxs-lookup"><span data-stu-id="93284-142">Date formats with letters should be avoided.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="93284-143">Потенциални стъпки за смекчаване</span><span class="sxs-lookup"><span data-stu-id="93284-143">Potential mitigation steps</span></span>
- <span data-ttu-id="93284-144">Използвайте разширено търсене, за да идентифицирате задачи от проекти, които не съдържат ИД на проект.</span><span class="sxs-lookup"><span data-stu-id="93284-144">Use Advanced Find to identify Project tasks that do not contain a Project ID.</span></span>
- <span data-ttu-id="93284-145">Използвайте разширено търсене, за да идентифицирате задачи от проекти, в които планираното времетраене е по-голямо от > 1 800 000.</span><span class="sxs-lookup"><span data-stu-id="93284-145">Use Advanced Find to identify Project tasks where the scheduled duration is greater than > 1,800,000.</span></span>
- <span data-ttu-id="93284-146">Преди да направите каквито и да било промени на данните, трябва да проучите всички персонализации, свързани с обекта, които може да са довели до лошото състояние на данните.</span><span class="sxs-lookup"><span data-stu-id="93284-146">Prior to making any data changes, you should investigate any customizations associated with the entity that may have led to getting the data into a bad state.</span></span> <span data-ttu-id="93284-147">Тези персонализации трябва да бъдат разгледани, преди да се пристъпи към някакви актуализации, свързани с данните.</span><span class="sxs-lookup"><span data-stu-id="93284-147">These customizations should be addressed before proceeding with any data-related updates.</span></span>
- <span data-ttu-id="93284-148">За откритите „осиротели” задачи помислете за изтриване на тези задачи, ако не са необходими или ако трябва да бъдат свързани с правилния родителски проект.</span><span class="sxs-lookup"><span data-stu-id="93284-148">For the identified tasks that have been orphaned, consider deleting these tasks if they are not needed or if they should be associated with the correct parent project.</span></span>
- <span data-ttu-id="93284-149">За всички задачи, при които времетраенето е по-голямо от 1250 дни, помислете за добавяне на няколко задачи, които да представят общото времетраене, ако е възможно.</span><span class="sxs-lookup"><span data-stu-id="93284-149">For any tasks where the duration is greater than 1,250 days, consider adding multiple tasks to represent the total duration, if feasible.</span></span>

> [!NOTE]
> <span data-ttu-id="93284-150">Елементите, отбелязани със звездичка (\*), имат ограничения, които се дължат на факта, че управлението на взаимоотношенията с клиенти (CRM) поддържа само 7320 повтарящи се разширения.</span><span class="sxs-lookup"><span data-stu-id="93284-150">Items noted with an asterisk (\*) have limits that are due to the fact that customer relationship management (CRM) supports only 7,320 recurrence expansions.</span></span> <span data-ttu-id="93284-151">Трябва да останете под този лимит.</span><span class="sxs-lookup"><span data-stu-id="93284-151">You must stay below this limit.</span></span>

## <a name="resource-assignment-relationships"></a><span data-ttu-id="93284-152">Релации на присвояване на ресурси</span><span class="sxs-lookup"><span data-stu-id="93284-152">Resource Assignment relationships</span></span>
<span data-ttu-id="93284-153">За да осигурите успешна надстройка, следните релации трябва да се поддържат правилно:</span><span class="sxs-lookup"><span data-stu-id="93284-153">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="93284-154">Всички присвоявания на ресурси в съставната структура на работата трябва да са свързани с един и същ проект.</span><span class="sxs-lookup"><span data-stu-id="93284-154">All Resource Assignments in a work breakdown structure must be related to the same project.</span></span>
- <span data-ttu-id="93284-155">Всички присвоявания на ресурси в съставната структура на работата трябва да са свързани с членовете на екипа в един и същ проект.</span><span class="sxs-lookup"><span data-stu-id="93284-155">All Resource Assignments in a work breakdown structure must be associated to project team members in the same project.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="93284-156">Потенциални стъпки за смекчаване</span><span class="sxs-lookup"><span data-stu-id="93284-156">Potential mitigation steps</span></span>
- <span data-ttu-id="93284-157">Определете всички задачи, които попадат извън условията, описани по-горе.</span><span class="sxs-lookup"><span data-stu-id="93284-157">Identify all tasks that fall outside the conditions described above.</span></span>  
- <span data-ttu-id="93284-158">Всички присвоявания на ресурси, които вече не са валидни, трябва да бъдат изтрити.</span><span class="sxs-lookup"><span data-stu-id="93284-158">Any Resource Assignments that are no longer valid should be deleted.</span></span>

## <a name="project-task-dependency-relationships"></a><span data-ttu-id="93284-159">Релации на зависимости на задачи на проекти</span><span class="sxs-lookup"><span data-stu-id="93284-159">Project task dependency relationships</span></span>
<span data-ttu-id="93284-160">За да осигурите успешна надстройка, следните релации трябва да се поддържат правилно:</span><span class="sxs-lookup"><span data-stu-id="93284-160">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="93284-161">Всички зависимости на задача на проект трябва да са свързани с един и същ проект.</span><span class="sxs-lookup"><span data-stu-id="93284-161">All project task dependencies must be related to the same project.</span></span>
- <span data-ttu-id="93284-162">Една задача не може да има една и съща зависимост, към която има препратка повече от веднъж.</span><span class="sxs-lookup"><span data-stu-id="93284-162">A task can't have the same dependency referenced more than once.</span></span>
