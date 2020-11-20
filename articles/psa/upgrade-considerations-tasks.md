---
title: Съображения за надстройване за съставната структура на работата
description: Тази тема предоставя информация за надстройване на съставната структура на работата от Project Service Automation 2.x до 3.x.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 0b75fd372732f42a3557aaa5eccec1f24a644941
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121790"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a><span data-ttu-id="25bd5-103">Съображения за надстройване за съставната структура на работата</span><span class="sxs-lookup"><span data-stu-id="25bd5-103">Upgrade considerations for the work breakdown structure</span></span>
<span data-ttu-id="25bd5-104">Тази тема предоставя информация за надстройване на съставната структура на работата от Project Service Automation 2.x до 3.x.</span><span class="sxs-lookup"><span data-stu-id="25bd5-104">This topic provides information about upgrading the work breakdown structure from Project Service Automation 2.x to 3.x.</span></span> <span data-ttu-id="25bd5-105">Тази тема определя изправното състояние на проект в Project Service Automation (PSA), което е необходимо за успешно надстройване.</span><span class="sxs-lookup"><span data-stu-id="25bd5-105">This topic defines the healthy state of a project in Project Service Automation (PSA) that is required for a successful upgrade.</span></span> <span data-ttu-id="25bd5-106">Има и информация за често срещаните условия за блокиране, които ще доведат до неуспешно надстройване.</span><span class="sxs-lookup"><span data-stu-id="25bd5-106">There is also information about the common blocking conditions that will cause upgrade to fail.</span></span> <span data-ttu-id="25bd5-107">За повече информация относно определянето на задачи по проекти и техните функции в график на проекти вижте [Графици на проекти](project-creating.md).</span><span class="sxs-lookup"><span data-stu-id="25bd5-107">For more information about defining project tasks and their functions within a project schedule, see [Project schedules](project-creating.md).</span></span>

## <a name="key-entities"></a><span data-ttu-id="25bd5-108">Основни обекти</span><span class="sxs-lookup"><span data-stu-id="25bd5-108">Key entities</span></span>
<span data-ttu-id="25bd5-109">За точна съставна структура на работата, която вече е натоварена с ресурси, се изискват следните обекти:</span><span class="sxs-lookup"><span data-stu-id="25bd5-109">For an accurate work breakdown structure that is already loaded with resources, the following entities are required:</span></span>

- [<span data-ttu-id="25bd5-110">Проект</span><span class="sxs-lookup"><span data-stu-id="25bd5-110">Project</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [<span data-ttu-id="25bd5-111">Екип на проект</span><span class="sxs-lookup"><span data-stu-id="25bd5-111">Project Team</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [<span data-ttu-id="25bd5-112">Задача от проект</span><span class="sxs-lookup"><span data-stu-id="25bd5-112">Project Task</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [<span data-ttu-id="25bd5-113">Присвоявания на ресурси</span><span class="sxs-lookup"><span data-stu-id="25bd5-113">Resource Assignments</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [<span data-ttu-id="25bd5-114">Зависимост на задачи от проект</span><span class="sxs-lookup"><span data-stu-id="25bd5-114">Project Task Dependency</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [<span data-ttu-id="25bd5-115">Налични ресурси</span><span class="sxs-lookup"><span data-stu-id="25bd5-115">Bookable Resources</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

<span data-ttu-id="25bd5-116">За да дефинирате съставна структура на работата, натоварена с ресурси, трябва да изпълните следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="25bd5-116">To define a resource loaded work breakdown structure, you must complete the following steps:</span></span>

1. <span data-ttu-id="25bd5-117">Създайте нов проект.</span><span class="sxs-lookup"><span data-stu-id="25bd5-117">Create a new project.</span></span> <span data-ttu-id="25bd5-118">За повече информация как да създадете нов проект вижте [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span><span class="sxs-lookup"><span data-stu-id="25bd5-118">For more information about how to create a new project, see [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span></span>
2. <span data-ttu-id="25bd5-119">Създайте една или повече задачи.</span><span class="sxs-lookup"><span data-stu-id="25bd5-119">Create one or more tasks.</span></span> <span data-ttu-id="25bd5-120">За повече информация как да създадете задача вижте [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span><span class="sxs-lookup"><span data-stu-id="25bd5-120">For more information about how to create a task, see [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span></span>
3. <span data-ttu-id="25bd5-121">Дефинирайте зависимостите на задачата.</span><span class="sxs-lookup"><span data-stu-id="25bd5-121">Define the task dependencies.</span></span> <span data-ttu-id="25bd5-122">За повече информация вижте [Зависимост на задачи от проект](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency),</span><span class="sxs-lookup"><span data-stu-id="25bd5-122">For more information, see [Project Task Dependency](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).</span></span>
4. <span data-ttu-id="25bd5-123">Присвоете членове на екипа на проекта към проекта.</span><span class="sxs-lookup"><span data-stu-id="25bd5-123">Assign project team members to the project.</span></span> <span data-ttu-id="25bd5-124">За повече информация вижте [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).</span><span class="sxs-lookup"><span data-stu-id="25bd5-124">For more information, see [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).</span></span>
5. <span data-ttu-id="25bd5-125">Присвоете членове на екипа на проекта към задачите.</span><span class="sxs-lookup"><span data-stu-id="25bd5-125">Assign project team members to the tasks.</span></span> <span data-ttu-id="25bd5-126">За повече информация вижте [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).</span><span class="sxs-lookup"><span data-stu-id="25bd5-126">For more information, see [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).</span></span>

## <a name="project-team-relationships"></a><span data-ttu-id="25bd5-127">Релации на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="25bd5-127">Project team relationships</span></span>

<span data-ttu-id="25bd5-128">За да осигурите успешна надстройка, следните релации трябва да се поддържат правилно:</span><span class="sxs-lookup"><span data-stu-id="25bd5-128">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>
- <span data-ttu-id="25bd5-129">Всички членове на екипа на проект трябва да бъдат свързани с наличен ресурс.</span><span class="sxs-lookup"><span data-stu-id="25bd5-129">All project team members must be associated with a bookable resource.</span></span>
- <span data-ttu-id="25bd5-130">Всички членове на екипа на проект трябва да бъдат свързани с един и същ проект.</span><span class="sxs-lookup"><span data-stu-id="25bd5-130">All project team members must be associated with the same project.</span></span> 

## <a name="project-task-relationships"></a><span data-ttu-id="25bd5-131">Релации на задачите на проект</span><span class="sxs-lookup"><span data-stu-id="25bd5-131">Project task relationships</span></span>
<span data-ttu-id="25bd5-132">За да осигурите успешна надстройка, следните релации трябва да се поддържат правилно:</span><span class="sxs-lookup"><span data-stu-id="25bd5-132">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="25bd5-133">Всички свързани задачи трябва да бъдат свързани с един и същ проект.</span><span class="sxs-lookup"><span data-stu-id="25bd5-133">Any related tasks must be associated with the same project.</span></span>
- <span data-ttu-id="25bd5-134">Всяка линейна задача трябва да има родителска задача.</span><span class="sxs-lookup"><span data-stu-id="25bd5-134">Every line task must have a parent task.</span></span>
- <span data-ttu-id="25bd5-135">Всяка задача трябва да има родителски проект.</span><span class="sxs-lookup"><span data-stu-id="25bd5-135">Every task must have a parent project.</span></span>

### <a name="valid-conditions"></a><span data-ttu-id="25bd5-136">Валидни условия</span><span class="sxs-lookup"><span data-stu-id="25bd5-136">Valid conditions</span></span>

- <span data-ttu-id="25bd5-137">Цялата продължителност на задачата трябва да бъде по-голяма или равна на (> =) един час и по-малка от 1 800 000 минути (1250 дни).\*</span><span class="sxs-lookup"><span data-stu-id="25bd5-137">All task durations must be greater than or equal to (>=) one hour and less than 1,800,000 minutes (1,250 days).\*</span></span>
- <span data-ttu-id="25bd5-138">Всички задачи трябва да имат начална дата не по-рано от 2000/01/01.\*</span><span class="sxs-lookup"><span data-stu-id="25bd5-138">All tasks must have a start date no earlier than 2000/01/01.\*</span></span>
- <span data-ttu-id="25bd5-139">Всички задачи трябва да имат начална дата не по-късно от 17 години от настоящия ден.\*</span><span class="sxs-lookup"><span data-stu-id="25bd5-139">All tasks must have a start date no later than 17 years from the present day.\*</span></span>
- <span data-ttu-id="25bd5-140">Всички задачи трябва да имат начална дата, по-ранна или същата като датата на завършване.</span><span class="sxs-lookup"><span data-stu-id="25bd5-140">All tasks must have a start date earlier or equal to their finish date.</span></span>
- <span data-ttu-id="25bd5-141">Всички типове транзакции по класификации (разходи, материали, данъци и време) трябва да имат стойности за **Единица по подразбиране** и **Група единици**.</span><span class="sxs-lookup"><span data-stu-id="25bd5-141">All transaction types on classifications (Expense, Material, Tax, and Time) must have values for **Default Unit** and **Unit Group**.</span></span>
- <span data-ttu-id="25bd5-142">Форматите за дата с букви трябва да се избягват.</span><span class="sxs-lookup"><span data-stu-id="25bd5-142">Date formats with letters should be avoided.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="25bd5-143">Потенциални стъпки за смекчаване</span><span class="sxs-lookup"><span data-stu-id="25bd5-143">Potential mitigation steps</span></span>
- <span data-ttu-id="25bd5-144">Използвайте разширено търсене, за да идентифицирате задачи от проекти, които не съдържат ИД на проект.</span><span class="sxs-lookup"><span data-stu-id="25bd5-144">Use Advanced Find to identify Project tasks that do not contain a Project ID.</span></span>
- <span data-ttu-id="25bd5-145">Използвайте разширено търсене, за да идентифицирате задачи от проекти, в които планираното времетраене е по-голямо от > 1 800 000.</span><span class="sxs-lookup"><span data-stu-id="25bd5-145">Use Advanced Find to identify Project tasks where the scheduled duration is greater than > 1,800,000.</span></span>
- <span data-ttu-id="25bd5-146">Преди да направите каквито и да било промени на данните, трябва да проучите всички персонализации, свързани с обекта, които може да са довели до лошото състояние на данните.</span><span class="sxs-lookup"><span data-stu-id="25bd5-146">Prior to making any data changes, you should investigate any customizations associated with the entity that may have led to getting the data into a bad state.</span></span> <span data-ttu-id="25bd5-147">Тези персонализации трябва да бъдат разгледани, преди да се пристъпи към някакви актуализации, свързани с данните.</span><span class="sxs-lookup"><span data-stu-id="25bd5-147">These customizations should be addressed before proceeding with any data-related updates.</span></span>
- <span data-ttu-id="25bd5-148">За откритите „осиротели” задачи помислете за изтриване на тези задачи, ако не са необходими или ако трябва да бъдат свързани с правилния родителски проект.</span><span class="sxs-lookup"><span data-stu-id="25bd5-148">For the identified tasks that have been orphaned, consider deleting these tasks if they are not needed or if they should be associated with the correct parent project.</span></span>
- <span data-ttu-id="25bd5-149">За всички задачи, при които времетраенето е по-голямо от 1250 дни, помислете за добавяне на няколко задачи, които да представят общото времетраене, ако е възможно.</span><span class="sxs-lookup"><span data-stu-id="25bd5-149">For any tasks where the duration is greater than 1,250 days, consider adding multiple tasks to represent the total duration, if feasible.</span></span>

> [!NOTE]
> <span data-ttu-id="25bd5-150">Елементите, отбелязани със звездичка (\*), имат ограничения, които се дължат на факта, че управлението на взаимоотношенията с клиенти (CRM) поддържа само 7320 повтарящи се разширения.</span><span class="sxs-lookup"><span data-stu-id="25bd5-150">Items noted with an asterisk (\*) have limits that are due to the fact that customer relationship management (CRM) supports only 7,320 recurrence expansions.</span></span> <span data-ttu-id="25bd5-151">Трябва да останете под този лимит.</span><span class="sxs-lookup"><span data-stu-id="25bd5-151">You must stay below this limit.</span></span>

## <a name="resource-assignment-relationships"></a><span data-ttu-id="25bd5-152">Релации на присвояване на ресурси</span><span class="sxs-lookup"><span data-stu-id="25bd5-152">Resource Assignment relationships</span></span>
<span data-ttu-id="25bd5-153">За да осигурите успешна надстройка, следните релации трябва да се поддържат правилно:</span><span class="sxs-lookup"><span data-stu-id="25bd5-153">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="25bd5-154">Всички присвоявания на ресурси в съставната структура на работата трябва да са свързани с един и същ проект.</span><span class="sxs-lookup"><span data-stu-id="25bd5-154">All Resource Assignments in a work breakdown structure must be related to the same project.</span></span>
- <span data-ttu-id="25bd5-155">Всички присвоявания на ресурси в съставната структура на работата трябва да са свързани с членовете на екипа в един и същ проект.</span><span class="sxs-lookup"><span data-stu-id="25bd5-155">All Resource Assignments in a work breakdown structure must be associated to project team members in the same project.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="25bd5-156">Потенциални стъпки за смекчаване</span><span class="sxs-lookup"><span data-stu-id="25bd5-156">Potential mitigation steps</span></span>
- <span data-ttu-id="25bd5-157">Определете всички задачи, които попадат извън условията, описани по-горе.</span><span class="sxs-lookup"><span data-stu-id="25bd5-157">Identify all tasks that fall outside the conditions described above.</span></span>  
- <span data-ttu-id="25bd5-158">Всички присвоявания на ресурси, които вече не са валидни, трябва да бъдат изтрити.</span><span class="sxs-lookup"><span data-stu-id="25bd5-158">Any Resource Assignments that are no longer valid should be deleted.</span></span>

## <a name="project-task-dependency-relationships"></a><span data-ttu-id="25bd5-159">Релации на зависимости на задачи на проекти</span><span class="sxs-lookup"><span data-stu-id="25bd5-159">Project task dependency relationships</span></span>
<span data-ttu-id="25bd5-160">За да осигурите успешна надстройка, следните релации трябва да се поддържат правилно:</span><span class="sxs-lookup"><span data-stu-id="25bd5-160">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="25bd5-161">Всички зависимости на задача на проект трябва да са свързани с един и същ проект.</span><span class="sxs-lookup"><span data-stu-id="25bd5-161">All project task dependencies must be related to the same project.</span></span>
- <span data-ttu-id="25bd5-162">Една задача не може да има една и съща зависимост, към която има препратка повече от веднъж.</span><span class="sxs-lookup"><span data-stu-id="25bd5-162">A task can't have the same dependency referenced more than once.</span></span>
