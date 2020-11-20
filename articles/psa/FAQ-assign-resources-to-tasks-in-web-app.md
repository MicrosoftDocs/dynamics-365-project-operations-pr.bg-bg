---
title: Как да присвоя наличен ресурс към задача в уеб приложението
description: Общ преглед на начините, по които можете да присвоявате налични ресурси.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
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
ms.openlocfilehash: cc1859540ede064c4ab3e2ac128573972912a207
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4125165"
---
# <a name="how-do-i-assign-a-bookable-resource-to-a-task-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="aa996-103">Как да присвоя наличен ресурс към задача в уеб приложението (приложение Project Service, версия 2.x)?</span><span class="sxs-lookup"><span data-stu-id="aa996-103">How do I assign a bookable resource to a task in the web app (Project Service app v2.x)?</span></span>

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="aa996-104">Има два начина да присвоите наличен ресурс към задача в Project Service.</span><span class="sxs-lookup"><span data-stu-id="aa996-104">There are two ways to assign a resource to a task in Project Service.</span></span> <span data-ttu-id="aa996-105">Можете да резервирате ресурс като член на екипа и след това да го присвоите към задача.</span><span class="sxs-lookup"><span data-stu-id="aa996-105">You can book a resource as a team member and then assign it to a task.</span></span> <span data-ttu-id="aa996-106">Или можете да създадете генеричен член на екипа чрез присвояване на роля в задачи, да генерирате екип и след това да изпълните осигуряващите изисквания с именувания ресурс.</span><span class="sxs-lookup"><span data-stu-id="aa996-106">Or, you can create a generic team member through role assignment on tasks, generate a team, and then fulfill the backing requirements with a named resource.</span></span>

<span data-ttu-id="aa996-107">Обърнете внимание, че ако искате да присвоите наличен ресурс към задача, наличният член на екипа на ресурса трябва да има достатъчно достъпни резервации.</span><span class="sxs-lookup"><span data-stu-id="aa996-107">Note that if you’d like to assign a bookable resource to a task, the bookable resource team member must have enough available bookings.</span></span> <span data-ttu-id="aa996-108">Състоянието на резервацията трябва да е „Твърда резервация на тип на разпределение” и с „Разпределено състояние”.</span><span class="sxs-lookup"><span data-stu-id="aa996-108">The status of the booking must be Commit Type Hard Book and Status Committed.</span></span> <span data-ttu-id="aa996-109">Ако няма достатъчно резервации за ресурса, Project Service премахва присвояването и показва следното съобщение за грешка:</span><span class="sxs-lookup"><span data-stu-id="aa996-109">If there aren’t enough bookings for the resource, Project Service removes the assignment and displays the following error message:</span></span>

<span data-ttu-id="aa996-110">*Не може да се присвои ресурс към задача – следните ресурси нямат достатъчно резервирани часове срещу проект*</span><span class="sxs-lookup"><span data-stu-id="aa996-110">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project*</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="aa996-111">Резервиране на ресурс като член на екипа и след това присвояване на ресурса към задача</span><span class="sxs-lookup"><span data-stu-id="aa996-111">Book a resource as a team member and then assign the resource to a task</span></span>

<span data-ttu-id="aa996-112">С помощта на този метод добавяте ресурс към екип на проекта и след това присвоявате задачи към ресурса в графика на проекта.</span><span class="sxs-lookup"><span data-stu-id="aa996-112">With this method you add a resource to the project team and then assign tasks to the resource in the project schedule.</span></span> <span data-ttu-id="aa996-113">Ето как да направите това:</span><span class="sxs-lookup"><span data-stu-id="aa996-113">Here’s how you do this:</span></span>
1.  <span data-ttu-id="aa996-114">В мрежата с членове на екипа добавете нов член на екипа, като изберете **Нов**.</span><span class="sxs-lookup"><span data-stu-id="aa996-114">On the team member grid, add a new team member by selecting **New**.</span></span>
2.  <span data-ttu-id="aa996-115">На екрана за бързо създаване на член на екипа изберете името на наличния ресурс и задайте роля.</span><span class="sxs-lookup"><span data-stu-id="aa996-115">On the Team Member Quick Create screen, select the bookable resource name and set a role.</span></span>
3.  <span data-ttu-id="aa996-116">Изберете дати **От** и **До**.</span><span class="sxs-lookup"><span data-stu-id="aa996-116">Select the **From** and **To** dates.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="aa996-117">![Екранна снимка на добавяне на член на екипа](media/FAQ-Resources-to-Tasks2-1.png "Екранна снимка на добавяне на член на екипа")</span><span class="sxs-lookup"><span data-stu-id="aa996-117">![Screenshot of adding team member](media/FAQ-Resources-to-Tasks2-1.png "Screenshot of adding team member")</span></span>
 
4.  <span data-ttu-id="aa996-118">Изберете един от следните методи на разпределение за резервиране на ресурса:</span><span class="sxs-lookup"><span data-stu-id="aa996-118">Select one of the following allocation methods for booking the resource:</span></span>
    - <span data-ttu-id="aa996-119">**Пълен капацитет** резервира пълния капацитет на ресурса за указаните дати „от” и „до”.</span><span class="sxs-lookup"><span data-stu-id="aa996-119">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="aa996-120">**Процент от капацитета** резервира ресурса за процент от капацитета му за указаните дати „от” и „до”.</span><span class="sxs-lookup"><span data-stu-id="aa996-120">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="aa996-121">**Равномерно разпределение по часове** резервира ресурса за определен брой часове, като ги разпределя поравно за ден през указаните дати „от” и „до”.</span><span class="sxs-lookup"><span data-stu-id="aa996-121">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing it evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="aa996-122">**Предно натоварване на часовете** резервира ресурса за определен брой часове, като натоварва отпред часовете на ден през указаните дати „от” и „до”.</span><span class="sxs-lookup"><span data-stu-id="aa996-122">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>

    <span data-ttu-id="aa996-123">Не избирайте **Няма**, защото това добавя ресурс към екипа, но не създава никакви резервации, които да абсорбират производителността на ресурса.</span><span class="sxs-lookup"><span data-stu-id="aa996-123">Don’t select **None** because it adds the resource to the team but doesn’t create any bookings that absorb the resource's capacity.</span></span>
5.  <span data-ttu-id="aa996-124">Изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="aa996-124">Select **Save**.</span></span>

    <span data-ttu-id="aa996-125">Обърнете внимание, че часовете на резервацията трябва да са достатъчно, за да покриват часовете на усилие и диапазоните от дати в задачите, за които присвоявате този ресурс.</span><span class="sxs-lookup"><span data-stu-id="aa996-125">Note that the hours of the booking must be enough to cover the effort hours and date ranges of the tasks that you assign this resource to.</span></span> <span data-ttu-id="aa996-126">Ако си съответстват, не можете да присвоите ресурса към задача.</span><span class="sxs-lookup"><span data-stu-id="aa996-126">If they aren’t in alignment, you can’t assign the resource to the task.</span></span>

6.  <span data-ttu-id="aa996-127">В съставната структура на работата (WBS) за задачата щракнете върху падащия списък с клетки на ресурс.</span><span class="sxs-lookup"><span data-stu-id="aa996-127">On the work breakdown structure (WBS) for the task, click the resource cell dropdown.</span></span> <span data-ttu-id="aa996-128">След това:</span><span class="sxs-lookup"><span data-stu-id="aa996-128">Then:</span></span> 

    1. <span data-ttu-id="aa996-129">Избери **Добавяне**.</span><span class="sxs-lookup"><span data-stu-id="aa996-129">Select **Add**.</span></span>
    2. <span data-ttu-id="aa996-130">Изберете падащото меню под **Ресурси** и изберете члена на екипа, който добавихте по-горе.</span><span class="sxs-lookup"><span data-stu-id="aa996-130">Select the dropdown under **Resources** and select the team member you added above.</span></span>
    3. <span data-ttu-id="aa996-131">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="aa996-131">Select **OK**.</span></span> <span data-ttu-id="aa996-132">Членът на екипа вече е присвоен към задачата.</span><span class="sxs-lookup"><span data-stu-id="aa996-132">The team member is now assigned to the task.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="aa996-133">![Екранна снимка на добавяне на ресурси със ССР](media/FAQ-Resources-to-Tasks2-2.png "Екранна снимка на добавяне на ресурси със ССР")</span><span class="sxs-lookup"><span data-stu-id="aa996-133">![Screenshot of adding resources with WBS](media/FAQ-Resources-to-Tasks2-2.png "Screenshot of adding resources with WBS")</span></span>
 
<span data-ttu-id="aa996-134">В мрежата за член на екипа ще видите сбора от часовете, присвоени на ресурси под „Присвоени часове”.</span><span class="sxs-lookup"><span data-stu-id="aa996-134">On the team member grid, you’ll see the aggregate of the resource’s assigned hours under Assigned Hours.</span></span> <span data-ttu-id="aa996-135">Той ще бъде по-малък или равен на резервираните часове за ресурса.</span><span class="sxs-lookup"><span data-stu-id="aa996-135">It will be less than or equal to the booked hours for the resource.</span></span> 

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="aa996-136">![Екранна снимка на присвоени часове за ресурс](media/FAQ-Resources-to-Tasks2-3.png "Екранна снимка на присвоени часове за ресурс")</span><span class="sxs-lookup"><span data-stu-id="aa996-136">![Screenshot of assigned hours for a resource](media/FAQ-Resources-to-Tasks2-3.png "Screenshot of assigned hours for a resource")</span></span>
 
<span data-ttu-id="aa996-137">Ако задачата, която се опитвате да присвоите към ресурса започва след крайната дата на резервациите на ресурси, ресурсът няма да се показва в падащото меню.</span><span class="sxs-lookup"><span data-stu-id="aa996-137">If the task you’re attempting to assign to the resource starts after the end date of the resources bookings, the resource won’t appear in the dropdown.</span></span>

<span data-ttu-id="aa996-138">Обърнете внимание, че можете да присвоите ресурс към повече от резервираните часове, ако ресурсът има оставаща неприсвоена производителност.</span><span class="sxs-lookup"><span data-stu-id="aa996-138">Note that you can assign a resource to more hours than their booked hours if the resource has some remaining unassigned capacity.</span></span> <span data-ttu-id="aa996-139">В този случай ресурсът ще бъде само частично присвоен за техните резервации.</span><span class="sxs-lookup"><span data-stu-id="aa996-139">In this case the resource will only be partially assigned up to their bookings.</span></span> <span data-ttu-id="aa996-140">Можете да видите тези оставащи неприсвоени часове на задача, като добавите колоната „Часове без персонал” към съставната структура на работата.</span><span class="sxs-lookup"><span data-stu-id="aa996-140">You can see these remaining unassigned task hours by adding the Unstaffed Hours column to the work breakdown structure.</span></span>

<span data-ttu-id="aa996-141">Ако дадени ресурси за присвоени към техните резервирани часове (техните резервирани часове са равни на присвоените им часове), ще видите следното съобщение за грешка, когато опитате да ги присвоите към следващи задачи:</span><span class="sxs-lookup"><span data-stu-id="aa996-141">If resources are assigned to their booked hours (their booked hours equals their assigned hours), you’ll see the following error message when you attempt to assign them further tasks:</span></span>

<span data-ttu-id="aa996-142">*Не може да се присвои ресурс към задача – Следните ресурси нямат достатъчно резервирани часове срещу проект.*</span><span class="sxs-lookup"><span data-stu-id="aa996-142">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project.*</span></span>

<span data-ttu-id="aa996-143">В допълнение членът на екипа на мениджър на проект по подразбиране, който е добавен към екипа, когато създавате проекта, се добавя без никакви резервации и не може да бъде присвоен към задача.</span><span class="sxs-lookup"><span data-stu-id="aa996-143">Additionally, the default project manager team member that is added to the team when you create the project is added without any bookings and can’t be assigned to any task.</span></span> <span data-ttu-id="aa996-144">Той няма да се показва в падащото меню на ресурс за задачи.</span><span class="sxs-lookup"><span data-stu-id="aa996-144">They won’t show up in the resource dropdown for tasks.</span></span>

<span data-ttu-id="aa996-145">Ако искате да присвоите този ресурс, ще трябва да го премахнете от екипа и след това да го добавите повторно с метод на разпределение, различен от „Няма”.</span><span class="sxs-lookup"><span data-stu-id="aa996-145">If you want to assign this resource, you need to remove them from the team and then re-add them with an allocation method other than None.</span></span> <span data-ttu-id="aa996-146">Причината, поради която се добавя към екипа при създаването на проекта, е, че проектът има поне един одобряващ на проект по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="aa996-146">The reason they’re added to the team when the project is created is so that a project has at least one project approver by default.</span></span>

## <a name="create-a-generic-team-member-through-role-assignment-on-tasks"></a><span data-ttu-id="aa996-147">Създаване на генеричен член на екипа чрез присвояване на роля към задача</span><span class="sxs-lookup"><span data-stu-id="aa996-147">Create a generic team member through role assignment on tasks</span></span>

<span data-ttu-id="aa996-148">Този метод гарантира, че ресурсите имат достатъчно резервации за задачи.</span><span class="sxs-lookup"><span data-stu-id="aa996-148">This method assures that resources have enough bookings for tasks.</span></span> <span data-ttu-id="aa996-149">Първо трябва да създадете контейнер или генеричен ресурс, който описва характеристиките на наименувания ресурс, който в крайна сметка искате да работи по задачата, като генерирате екип след присвояването на роли към задачи.</span><span class="sxs-lookup"><span data-stu-id="aa996-149">First, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks by generating a team after assigning roles to tasks.</span></span> <span data-ttu-id="aa996-150">Ето как да направите това:</span><span class="sxs-lookup"><span data-stu-id="aa996-150">Here’s how you do this:</span></span>

1. <span data-ttu-id="aa996-151">В съставната структура на работата изберете задача.</span><span class="sxs-lookup"><span data-stu-id="aa996-151">On the work breakdown structure, select a task.</span></span>
2. <span data-ttu-id="aa996-152">Изберете иконата на падащото меню **Присвоена роля** в клетката на ресурс.</span><span class="sxs-lookup"><span data-stu-id="aa996-152">Select the **Assigned Role** dropdown icon in the resource cell.</span></span>
3. <span data-ttu-id="aa996-153">Изберете падащото меню **Роля** и изберете ролята за генеричния ресурс.</span><span class="sxs-lookup"><span data-stu-id="aa996-153">Select the **Role** dropdown and select the role for the generic resource.</span></span>
4. <span data-ttu-id="aa996-154">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="aa996-154">Select **OK**.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="aa996-155">![Екранна снимка на използване на ССР за добавяне на ресурси](media/FAQ-Resources-to-Tasks2-4.png "Екранна снимка на използване на ССР за добавяне на ресурси")</span><span class="sxs-lookup"><span data-stu-id="aa996-155">![Screenshot of using WBS to add resource](media/FAQ-Resources-to-Tasks2-4.png "Screenshot of using WBS to add resource")</span></span>
 
<span data-ttu-id="aa996-156">След като приключите с присвояването на роли към задача в ССР, изберете **Генериране на екип на проект**.</span><span class="sxs-lookup"><span data-stu-id="aa996-156">Once you’ve completed assigning roles to the tasks in the WBS, select **Generate Project Team**.</span></span> <span data-ttu-id="aa996-157">Project Service създава минимален брой генерични членове на екипа според ролите, ресурсните организационни единици и календара на проекта чрез обобщаване на присвояванията на задачи.</span><span class="sxs-lookup"><span data-stu-id="aa996-157">Project Service creates the minimum number of generic team members based on the roles, resourcing organization units, and project calendar by aggregating the task assignments.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="aa996-158">![Екранна снимка на генериране на екип на проект](media/FAQ-Resources-to-Tasks2-5.png "Екранна снимка на генериране на екип на проект")</span><span class="sxs-lookup"><span data-stu-id="aa996-158">![Screenshot of generating project team](media/FAQ-Resources-to-Tasks2-5.png "Screenshot of generating project team")</span></span>
 
<span data-ttu-id="aa996-159">В мрежата за член на екипа ще видите ресурси от типа на генеричен ресурс с роля и име на позиция.</span><span class="sxs-lookup"><span data-stu-id="aa996-159">On the Team Member grid, you’ll see resources of the Generic Resource type with the role and position name.</span></span> <span data-ttu-id="aa996-160">Ако два ресурса са необходими за дадена роля да изпълни работата, функцията „Генериране на екип” създава два члена на екипа и използва име на позиция, за да ги отдели.</span><span class="sxs-lookup"><span data-stu-id="aa996-160">If two resources are needed for a role to complete the work, the Generate Team feature creates two team members and uses position name to set them apart.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="aa996-161">![Екранна снимка на добавяне на два общи ресурса](media/FAQ-Resources-to-Tasks2-6.png "Екранна снимка на добавяне на два общи ресурса")</span><span class="sxs-lookup"><span data-stu-id="aa996-161">![Screenshot of adding two generic resources](media/FAQ-Resources-to-Tasks2-6.png "Screenshot of adding two generic resources")</span></span>
 
<span data-ttu-id="aa996-162">Можете да отворите изискване за резервен ресурс за генеричния член на екипа, като изберете връзката под „Изискване за ресурс”.</span><span class="sxs-lookup"><span data-stu-id="aa996-162">You can open the backing resource requirement for the generic team member by selecting the link under Resource Requirement.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="aa996-163">![Екранна снимка на отваряне на изискване за резервен ресурс](media/FAQ-Resources-to-Tasks2-7.png "Екранна снимка на отваряне на изискване за резервен ресурс")</span><span class="sxs-lookup"><span data-stu-id="aa996-163">![Screenshot of opening backing resource requirement](media/FAQ-Resources-to-Tasks2-7.png "Screenshot of opening backing resource requirement")</span></span>

<span data-ttu-id="aa996-164">Изберете **Резервиране** за генеричния ресурс, след което можете да използвате това табло за график, за да намерите и резервирате реален ресурс.</span><span class="sxs-lookup"><span data-stu-id="aa996-164">Select **Book** for the generic resource, and then you can use the schedule board to find and book a real resource.</span></span> <span data-ttu-id="aa996-165">Можете също да подадете изискването за изпълнение от мениджър ресурс, като изберете **Подаване на заявка**.</span><span class="sxs-lookup"><span data-stu-id="aa996-165">You can also submit the requirement for fulfillment by a resource manager by selecting **Submit Request**.</span></span>

<span data-ttu-id="aa996-166">Когато генеричен ресурс е изпълнен с наименуван ресурс, генеричният ресурс се премахва от екипа и присвояванията на задачи за генеричния ресурс се присвояват на наименувания ресурс, който изпълнява изискването на ресурса на генеричния ресурс.</span><span class="sxs-lookup"><span data-stu-id="aa996-166">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>
 

