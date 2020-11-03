---
title: Присвояване на ресурс към задача
description: Тази тема предоставя информация за това как да присвоявате ресурси към задачи.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 9/27/2019
ms.topic: article
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
ms.openlocfilehash: 77f13d1e96b76dfea241fbf7a67d5676582f0235
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4072009"
---
# <a name="assign-a-resource-to-a-task"></a><span data-ttu-id="f5e37-103">Присвояване на ресурс към задача</span><span class="sxs-lookup"><span data-stu-id="f5e37-103">Assign a resource to a task</span></span>

<span data-ttu-id="f5e37-104">Има три начина да присвоите ресурс към задача в Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f5e37-104">There are three ways to assign a resource to a task in Microsoft Dynamics 365 Project Service Automation.</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="f5e37-105">Резервиране на ресурс като член на екипа и след това присвояване на ресурса към задача</span><span class="sxs-lookup"><span data-stu-id="f5e37-105">Book a resource as a team member, and then assign the resource to a task</span></span>

<span data-ttu-id="f5e37-106">Можете да добавите ресурс към екипа на проекта и след това да присвоите ресурса към задача в графика на проекта.</span><span class="sxs-lookup"><span data-stu-id="f5e37-106">You can add a resource to the project team, and then assign the resource to tasks in the project schedule.</span></span>

1. <span data-ttu-id="f5e37-107">В раздела **Член на екипа** добавете нов член на екипа, като изберете **Нов**.</span><span class="sxs-lookup"><span data-stu-id="f5e37-107">On the **Team Member** tab, add a new team member by selecting **New**.</span></span> 

2. <span data-ttu-id="f5e37-108">Отваря се панелът **Бързо създаване на член на екипа** , където можете да изберете име на наличен ресурс и да зададете роля.</span><span class="sxs-lookup"><span data-stu-id="f5e37-108">The **Team Member Quick Create** panel opens, where you can select the bookable resource name and set a role.</span></span> 

    <span data-ttu-id="f5e37-109">Изберете един от следните методи на разпределение за резервиране на ресурса:</span><span class="sxs-lookup"><span data-stu-id="f5e37-109">Select one of the following allocation methods for the resource’s booking:</span></span>

    - <span data-ttu-id="f5e37-110">**Пълен капацитет** резервира пълния капацитет на ресурса за указаните дати „от” и „до”.</span><span class="sxs-lookup"><span data-stu-id="f5e37-110">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="f5e37-111">**Процент от капацитета** резервира ресурса за процент от капацитета му за указаните дати „от” и „до”.</span><span class="sxs-lookup"><span data-stu-id="f5e37-111">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="f5e37-112">**Равномерно разпределение по часове** резервира ресурса за указан брой часове, като ги разпределя поравно на ден за указаните дати „от” и „до”.</span><span class="sxs-lookup"><span data-stu-id="f5e37-112">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing them evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="f5e37-113">**Предно натоварване на часовете** резервира ресурса за определен брой часове, като натоварва отпред часовете на ден през указаните дати „от” и „до”.</span><span class="sxs-lookup"><span data-stu-id="f5e37-113">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>
    - <span data-ttu-id="f5e37-114">**Няма** добавя ресурса към екипа, но не създава никакви резервации, които да абсорбират производителността му.</span><span class="sxs-lookup"><span data-stu-id="f5e37-114">**None** adds the resource to the team but doesn’t create any bookings that absorb their capacity.</span></span>

3. <span data-ttu-id="f5e37-115">В мрежата **График** за задача изберете иконата **Ресурс** в клетката за ресурс, след което под **Члена на екипа** изберете члена на екипа, който току-що добавихте.</span><span class="sxs-lookup"><span data-stu-id="f5e37-115">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell, and then under **Team Members** , select the team member you just added.</span></span> 

> [!NOTE]
> <span data-ttu-id="f5e37-116">В раздела **Член на екипа** и в раздела **Съгласуване** ресурсът показва резервирани и присвоени часове.</span><span class="sxs-lookup"><span data-stu-id="f5e37-116">On the **Team Member** and **Reconciliation** tabs, the resource shows booked and assigned hours.</span></span> <span data-ttu-id="f5e37-117">Те би трябвало да са еднакви, но не е задължително, защото резервациите и присвояванията не са тясно обвързани.</span><span class="sxs-lookup"><span data-stu-id="f5e37-117">The hours should be the same, but it isn't required as bookings and assignments are not tightly coupled.</span></span> <span data-ttu-id="f5e37-118">Разделът **Съгласуване** ви предоставя подробности, когато са различни, например когато присвоите на ресурс повече часове, отколкото сте резервирали.</span><span class="sxs-lookup"><span data-stu-id="f5e37-118">The **Reconciliation** tab gives you details when they are different, such as when you assign a resource more hours than you have booked.</span></span> <span data-ttu-id="f5e37-119">Ако е необходимо, можете да коригирате информацията, като удължите резервациите на ресурса или промените присвояването.</span><span class="sxs-lookup"><span data-stu-id="f5e37-119">If needed, you can correct the information by extending the resource's bookings or changing the assignment.</span></span>

## <a name="create-a-generic-team-member-through-task-assignment"></a><span data-ttu-id="f5e37-120">Създаване на общ член на екипа чрез присвояване на задачи</span><span class="sxs-lookup"><span data-stu-id="f5e37-120">Create a generic team member through task assignment</span></span>

<span data-ttu-id="f5e37-121">Когато създавате общ член на екип чрез присвояване на задачи, създавате контейнер или общ ресурс, който описва характеристиките на наименувания ресурс, който в крайна сметка искате да работи по задачата.</span><span class="sxs-lookup"><span data-stu-id="f5e37-121">When you create a generic team member through task assignment, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks.</span></span> <span data-ttu-id="f5e37-122">След това създавате изискване (или подавате заявка с помощта на това изискване), което се използва за търсене и резервиране на наименувания ресурс.</span><span class="sxs-lookup"><span data-stu-id="f5e37-122">You then generate a requirement (or submit a request using the requirement) that is used to search for and book the named resource.</span></span>

1. <span data-ttu-id="f5e37-123">В мрежата **График** за дадена задача изберете иконата **Ресурс** в клетката на ресурса.</span><span class="sxs-lookup"><span data-stu-id="f5e37-123">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="f5e37-124">Въведете име, което да служи като име на ресурс на контейнера.</span><span class="sxs-lookup"><span data-stu-id="f5e37-124">Type a name to serve as the placeholder resource’s name.</span></span> <span data-ttu-id="f5e37-125">Например програмен мениджър.</span><span class="sxs-lookup"><span data-stu-id="f5e37-125">For example, Program Manager.</span></span>

3. <span data-ttu-id="f5e37-126">Изберете **Създаване** и в полето **Бързо създаване на член на екипа на проекта** задайте ролята за общия ресурс.</span><span class="sxs-lookup"><span data-stu-id="f5e37-126">Select **Create** , and in the **Quick Create Project Team Member** field, set the role for the generic resource.</span></span>

4. <span data-ttu-id="f5e37-127">Можете да продължите да присвоявате задачи към този ресурс на контейнер, като изберете ресурса в **Селектор на ресурси** за задачата.</span><span class="sxs-lookup"><span data-stu-id="f5e37-127">You can continue to assign tasks to this placeholder resource by selecting the resource on the **Resource Selector** for the task.</span></span> <span data-ttu-id="f5e37-128">Те са изброени под **Членове на екипа**.</span><span class="sxs-lookup"><span data-stu-id="f5e37-128">They’re listed under **Team Members**.</span></span>

5. <span data-ttu-id="f5e37-129">Когато приключите с присвояването на общ ресурс, изберете общия ресурс в раздела **Екип** и след това изберете **Създаване на изискване** , за да създадете изискване за ресурс за общия ресурс.</span><span class="sxs-lookup"><span data-stu-id="f5e37-129">When you’re done assigning the generic resource, select the generic resource on the **Team** tab, and then select **Generate Requirement** to create a resource requirement for the generic resource.</span></span>

6. <span data-ttu-id="f5e37-130">Изберете **Резервиране** за генеричен ресурс.</span><span class="sxs-lookup"><span data-stu-id="f5e37-130">Select **Book** for the generic resource.</span></span> <span data-ttu-id="f5e37-131">След това можете да използвате таблото на графика, за да намерите и резервирате реален ресурс.</span><span class="sxs-lookup"><span data-stu-id="f5e37-131">You can then use the Schedule board to find and book a real resource.</span></span> <span data-ttu-id="f5e37-132">Можете също да подадете изискването за изпълнение от мениджър на ресурс.</span><span class="sxs-lookup"><span data-stu-id="f5e37-132">You can also submit the requirement for fulfillment by a resource manager.</span></span>

7. <span data-ttu-id="f5e37-133">Когато генеричен ресурс е изпълнен с наименуван ресурс, генеричният ресурс се премахва от екипа и присвояванията на задачи за генеричния ресурс се присвояват на наименувания ресурс, който изпълнява изискването на ресурса на генеричния ресурс.</span><span class="sxs-lookup"><span data-stu-id="f5e37-133">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>

## <a name="assign-a-named-resource-from-the-list-of-all-bookable-resources"></a><span data-ttu-id="f5e37-134">Присвояване на наименуван ресурс от списъка с всички налични ресурси</span><span class="sxs-lookup"><span data-stu-id="f5e37-134">Assign a named resource from the list of all bookable resources</span></span>

<span data-ttu-id="f5e37-135">Можете да използвате полето за търсене в **Селектор на ресурси** , за да търсите всички налични ресурси и да ги присвоявате към задача.</span><span class="sxs-lookup"><span data-stu-id="f5e37-135">You can use the search box in the **Resource Selector** to search all bookable resources and assign them to a task.</span></span>

<span data-ttu-id="f5e37-136">Ресурсите, присвоени по този начин, се добавят към екипа без никакви резервации.</span><span class="sxs-lookup"><span data-stu-id="f5e37-136">Resources assigned this way are added to the team without any bookings.</span></span> <span data-ttu-id="f5e37-137">Това е подобно на добавянето на член на екипа и избирането на „Няма“ като метод на разпределение.</span><span class="sxs-lookup"><span data-stu-id="f5e37-137">This is similar to adding a team member and selecting None as the allocation method.</span></span> <span data-ttu-id="f5e37-138">Ресурсът се показва в разделите **Екип** и **Съгласуване** като ресурси само с присвоявания и дефицит на резервиране.</span><span class="sxs-lookup"><span data-stu-id="f5e37-138">The resource is displayed in the **Team** and **Reconciliation** tabs as resources with only assignments and a booking deficit.</span></span> <span data-ttu-id="f5e37-139">Резервирайте ги, ако искате да използвате тяхната наличност.</span><span class="sxs-lookup"><span data-stu-id="f5e37-139">Book them if you want to use their availability.</span></span>

1. <span data-ttu-id="f5e37-140">В мрежата **График** за дадена задача изберете иконата **Ресурс** в клетката на ресурса.</span><span class="sxs-lookup"><span data-stu-id="f5e37-140">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="f5e37-141">Започнете да въвеждате име.</span><span class="sxs-lookup"><span data-stu-id="f5e37-141">Start typing a name.</span></span> <span data-ttu-id="f5e37-142">Резултатите от търсенето за името се показват в **Селектор на ресурси** под **Други ресурси**.</span><span class="sxs-lookup"><span data-stu-id="f5e37-142">The search results for the name are displayed in the **Resource Selector** under **Other Resources**.</span></span>

3. <span data-ttu-id="f5e37-143">Изберете ресурса, който искате да присвоите на задачата.</span><span class="sxs-lookup"><span data-stu-id="f5e37-143">Select the resource that you want to assign to the task.</span></span>

