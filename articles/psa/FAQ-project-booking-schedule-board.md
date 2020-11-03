---
title: Създаване на резервация за проект от таблото на графика
description: Тази тема предоставя информация за това как да създадете резервация за проект от таблото на графика.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
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
ms.openlocfilehash: 57fbc71681015fca73cdda4bc7d392f6be4289f3
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071837"
---
# <a name="create-a-project-booking-from-the-schedule-board"></a><span data-ttu-id="366b5-103">Създаване на резервация за проект от таблото на графика</span><span class="sxs-lookup"><span data-stu-id="366b5-103">Create a project booking from the Schedule board</span></span>

<span data-ttu-id="366b5-104">Можете да резервирате ресурс в проект или директно от раздела **Екип** на проекта, или чрез генериране на изискване за ресурс от присвояване на общ член на екипа и след това изпълнение на генерираното изискване с член на екипа на проекта.</span><span class="sxs-lookup"><span data-stu-id="366b5-104">You can book a resource onto a project directly from the **Team** tab of the project or by generating a resource requirement from a generic team member assignment and then fulfilling the generated requirement with a project team member.</span></span>

<span data-ttu-id="366b5-105">Можете също да резервирате ресурс в проект директно от таблото на графика.</span><span class="sxs-lookup"><span data-stu-id="366b5-105">You can also book a resource onto a project directly from the Schedule board.</span></span> <span data-ttu-id="366b5-106">Има три начина да направите това:</span><span class="sxs-lookup"><span data-stu-id="366b5-106">There are three ways to do this:</span></span>

- <span data-ttu-id="366b5-107">**Резервиране от генерирано изискване за ресурс** : можете да генерирате изискване за ресурс, след като създадете общ ресурс и присвоите задачи в рамките на проект.</span><span class="sxs-lookup"><span data-stu-id="366b5-107">**Book from a generated resource requirement:** You can generate a resource requirement after you create a generic resource and assign tasks within a project.</span></span>

- <span data-ttu-id="366b5-108">**Резервиране от основното изискване:** основните изисквания се показват в таблото на графика в раздела **Проект**.</span><span class="sxs-lookup"><span data-stu-id="366b5-108">**Book from the primary requirement:** The primary requirements show up on the Schedule board on the **Project** tab.</span></span> 

- <span data-ttu-id="366b5-109">**Резервиране от ново изискване за ресурс:** можете да създадете изискване за ресурс от нулата и да го свържете с проект.</span><span class="sxs-lookup"><span data-stu-id="366b5-109">**Book from a new resource requirement:** You can create a resource requirement from scratch and associate it with a project.</span></span> <span data-ttu-id="366b5-110">На таблото на графика изискването за ресурс се показва в раздела **Отворени изисквания**.</span><span class="sxs-lookup"><span data-stu-id="366b5-110">On the Schedule board, the resource requirement shows up on the **Open Requirements** tab.</span></span>

## <a name="book-from-a-generated-resource-requirement"></a><span data-ttu-id="366b5-111">Резервиране от генерирано изискване за ресурс</span><span class="sxs-lookup"><span data-stu-id="366b5-111">Book from a generated resource requirement</span></span>

<span data-ttu-id="366b5-112">Можете да създадете общ ресурс и да му присвоите една или повече задачи в рамките на проект.</span><span class="sxs-lookup"><span data-stu-id="366b5-112">You can create a generic resource and assign it one or more tasks within a project.</span></span> <span data-ttu-id="366b5-113">След това можете да генерирате изискване за ресурс от общия член на екипа.</span><span class="sxs-lookup"><span data-stu-id="366b5-113">Then you can generate a resource requirement from the generic team member.</span></span> 

1.  <span data-ttu-id="366b5-114">На таблото на графика този ресурс се показва в раздела **Отворени изисквания**. Възможно е да трябва да използвате филтрите за колони в мрежата, ако имате множество отворени изисквания.</span><span class="sxs-lookup"><span data-stu-id="366b5-114">On the Schedule board, this resource will show up on the **Open Requirements** tab. You might need to use column filters on the grid if you have many open requirements.</span></span> 

    <span data-ttu-id="366b5-115">![Раздел „Отворени изисквания“ на таблото на графика](media/FAQ-Project-Booking-Schedule-Board-1.png "Екранна снимка на таблицата за резервации и присвоявания")</span><span class="sxs-lookup"><span data-stu-id="366b5-115">![Open Requirements tab on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-1.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="366b5-116">Изберете изискване.</span><span class="sxs-lookup"><span data-stu-id="366b5-116">Select the requirement.</span></span> <span data-ttu-id="366b5-117">Разделът **Търсене на наличност** ще се покаже в горната част на избрания ред.</span><span class="sxs-lookup"><span data-stu-id="366b5-117">The **Find Availability** tab will appear at the top of the selected row.</span></span>
 
3. <span data-ttu-id="366b5-118">Когато изберете раздела, режимът на асистента за планиране на таблото на графика се отваря и след това филтрира наличните ресурси, които отговарят на изискването за ресурс.</span><span class="sxs-lookup"><span data-stu-id="366b5-118">When you select the tab, the Schedule Assistant mode of the Schedule board opens and then filters the available resources that meet the resource requirement.</span></span> <span data-ttu-id="366b5-119">След това можете да резервирате ресурс.</span><span class="sxs-lookup"><span data-stu-id="366b5-119">After that, you can book a resource.</span></span>

4. <span data-ttu-id="366b5-120">Можете също да плъзнете и пуснете избрания ред от долната част на таблото на графика в клетка на ресурс в мрежата отгоре.</span><span class="sxs-lookup"><span data-stu-id="366b5-120">You can also drag and drop the selected row from the bottom of the Schedule board to a resource cell in the grid above.</span></span> <span data-ttu-id="366b5-121">Когато го пуснете, то отваря панела **Създаване на резервация за ресурс** вдясно.</span><span class="sxs-lookup"><span data-stu-id="366b5-121">When you drop it, it opens the **Create Resource Booking** panel on the right.</span></span>

    <span data-ttu-id="366b5-122">Избирането на **Резервация** резервира ресурса върху екипа на проекта.</span><span class="sxs-lookup"><span data-stu-id="366b5-122">Selecting **Book** books the resource onto the project team.</span></span>

![Панел „Създаване на резервация на ресурс“](media/FAQ-Project-Booking-Schedule-Board-6.png "")
 

## <a name="book-from-the-primary-requirement"></a><span data-ttu-id="366b5-124">Резервиране от основното изискване</span><span class="sxs-lookup"><span data-stu-id="366b5-124">Book from the Primary Requirement</span></span>

<span data-ttu-id="366b5-125">Създаването на проект в Project Service автоматично създава изискване за ресурс, наречено „Основно изискване”.</span><span class="sxs-lookup"><span data-stu-id="366b5-125">Creating a project in Project Service automatically creates a resource requirement called the Primary Requirement.</span></span> <span data-ttu-id="366b5-126">Това е празно изискване, което се използва за бързо резервиране на ресурс чрез таблото на графика без генериране на изискване или създаване на такова отначало.</span><span class="sxs-lookup"><span data-stu-id="366b5-126">This is an empty requirement that is used to quickly book a resource with the Schedule board without generating a requirement or creating one from scratch.</span></span> <span data-ttu-id="366b5-127">Тъй като изискването е празно, ще трябва да укажете дати, както и метод за разпределение и часове, ако има такива.</span><span class="sxs-lookup"><span data-stu-id="366b5-127">Because the requirement is empty, you’ll need to specify dates as well as the allocation method and hours, if applicable.</span></span> 

1. <span data-ttu-id="366b5-128">За да резервирате ресурс с основното изискване, на таблото на графика изберете раздела **Проект**. Възможно е да трябва да използвате филтъра за колони в колоната **Проект** , ако имате много проекти.</span><span class="sxs-lookup"><span data-stu-id="366b5-128">To book a resource with the Primary Requirement, on the Schedule board, select the **Project** tab. You might need to use the column filter on the **Project** column if you have many projects.</span></span>

   <span data-ttu-id="366b5-129">![Филтри на колони в таблото на графика](media/FAQ-Project-Booking-Schedule-Board-2.png "Екранна снимка на таблицата за резервации и присвоявания")</span><span class="sxs-lookup"><span data-stu-id="366b5-129">![Column filters on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-2.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="366b5-130">Изберете изискването, което има само името на проекта като свое име и времетраене нула (0).</span><span class="sxs-lookup"><span data-stu-id="366b5-130">Select the requirement that only has the project name as its name and has a duration of zero (0).</span></span>

3. <span data-ttu-id="366b5-131">Изберете раздела **Намиране на наличност** , който се показва на реда.</span><span class="sxs-lookup"><span data-stu-id="366b5-131">Select the **Find Availability** tab that appears on the row.</span></span> <span data-ttu-id="366b5-132">Това поставя таблото на графика в режим на асистент за планиране и показва наличните ресурси, които могат да бъдат резервирани по проекта.</span><span class="sxs-lookup"><span data-stu-id="366b5-132">This puts the Schedule board in Schedule Assistant mode and shows the available resources that can be booked onto the project.</span></span>

4. <span data-ttu-id="366b5-133">Тъй като **Основно изискване** е празно изискване с времетраене нула (0), ще трябва да зададете времетраенето в панела **Създаване на резервация за ресурс** , когато избирате и резервирате ресурс.</span><span class="sxs-lookup"><span data-stu-id="366b5-133">Because a **Primary Requirement** is an empty requirement with zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when selecting and booking a resource.</span></span>

5. <span data-ttu-id="366b5-134">Можете също да изберете **Основно изискване на проект** в долната част на таблото на графика и да го плъзнете и пуснете в ресурс, за да го резервирате.</span><span class="sxs-lookup"><span data-stu-id="366b5-134">You can also select the **Project Primary Requirement** at the bottom of the Schedule board and drag and drop it on a resource to book it.</span></span>
 
    <span data-ttu-id="366b5-135">Тъй като **Основно изискване** е празно изискване с времетраене нула (0), ще трябва да зададете времетраенето в панела **Създаване на резервация за ресурс** , когато избирате и резервирате ресурс.</span><span class="sxs-lookup"><span data-stu-id="366b5-135">Because the **Primary Requirement** is an empty requirement that has zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when you select and book a resource.</span></span>
 
    <span data-ttu-id="366b5-136">Когато резервирате ресурс чрез **Основно изискване** в таблото на графика, го добавяте към екипа на проекта без присвоявания.</span><span class="sxs-lookup"><span data-stu-id="366b5-136">When you book a resource through the **Primary Requirement** on the Schedule board, you add it to the project team without any assignments.</span></span>
 
## <a name="book-from-a-new-resource-requirement"></a><span data-ttu-id="366b5-137">Резервиране от ново изискване за ресурс</span><span class="sxs-lookup"><span data-stu-id="366b5-137">Book from a new resource requirement</span></span>
<span data-ttu-id="366b5-138">Изпълнете следните стъпки за резервиране от ново изискване за ресурс.</span><span class="sxs-lookup"><span data-stu-id="366b5-138">Complete the following steps to book from a new resource requirement.</span></span> 

1. <span data-ttu-id="366b5-139">Отидете на **Изисквания за ресурси** и изберете **Ново** , за да създадете ново изискване за ресурс.</span><span class="sxs-lookup"><span data-stu-id="366b5-139">Go to **Resource Requirements** , and then select **New** to create a new resource requirement.</span></span>

2. <span data-ttu-id="366b5-140">В раздела **Проект** изберете проект, за да свържете изискването към проекта.</span><span class="sxs-lookup"><span data-stu-id="366b5-140">On the **Project** tab, select a project to associate the requirement to the project.</span></span>
 
    <span data-ttu-id="366b5-141">В таблото на графика това ново изискване се показва като **Отворено изискване** , което можете да изпълните.</span><span class="sxs-lookup"><span data-stu-id="366b5-141">On the Schedule board, this new requirement shows as an **Open Requirement** that you can fulfill.</span></span>

3. <span data-ttu-id="366b5-142">Резервирайте ресурса, за да го добавите към екипа на проекта.</span><span class="sxs-lookup"><span data-stu-id="366b5-142">Book the resource to add it to the project team.</span></span>

4. <span data-ttu-id="366b5-143">След като ресурсът е резервиран, трябва да присвоите задачите ръчно.</span><span class="sxs-lookup"><span data-stu-id="366b5-143">Now that the resource is booked, you must assign tasks manually.</span></span>

