---
title: Планиране на ресурси за проект
description: Как се планират ресурси за проект в Project Service
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: db69348aac96cbfaaa865228c9230cbda4b1e784
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4072026"
---
# <a name="schedule-resources-for-a-project-project-service"></a><span data-ttu-id="96c7b-103">Планиране на ресурси за проект (Project Service)</span><span class="sxs-lookup"><span data-stu-id="96c7b-103">Schedule resources for a project (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="96c7b-104">Можете да проверите наличността на ресурси, за да получите общ преглед на това доколко са ангажирани ресурсите ви, или можете да филтрирате прегледа по умения, екип, местоположение и други опции.</span><span class="sxs-lookup"><span data-stu-id="96c7b-104">You can check resource availability to get an overall view of how booked your resources are, or you can filter the view by skills, team, location, and other options.</span></span>  
  
<span data-ttu-id="96c7b-105">Таблото на графика показва списък с ресурси и тяхната наличност.</span><span class="sxs-lookup"><span data-stu-id="96c7b-105">The schedule board shows list of resources and their availability.</span></span> <span data-ttu-id="96c7b-106">Изберете режим на преглеждане, за да се покаже наличността по **Часове** , **Ден** , **Седмица** или **Месец**.</span><span class="sxs-lookup"><span data-stu-id="96c7b-106">Select a view mode to show availability by **Hours** , **Day** , **Week** , or **Month**.</span></span>  
  
<span data-ttu-id="96c7b-107">Преди да използвате таблото на графика е важно да го настроите.</span><span class="sxs-lookup"><span data-stu-id="96c7b-107">Before you use the schedule board, it’s important to set it up.</span></span> <span data-ttu-id="96c7b-108">За повече информация вижте [Конфигуриране на таблото на графика (Field Service или Project Service Automation)](https://docs.microsoft.com/dynamics365/field-service/configure-schedule-board).</span><span class="sxs-lookup"><span data-stu-id="96c7b-108">For more information, see [Configure the schedule board (Field Service or Project Service Automation)](https://docs.microsoft.com/dynamics365/field-service/configure-schedule-board).</span></span>
  
<span data-ttu-id="96c7b-109">Ако използвате по-стара версия, за наличността на ресурси вижте [Преглед на наличността на ресурси](../psa/view-resource-availability.md).</span><span class="sxs-lookup"><span data-stu-id="96c7b-109">If you are using an older version, for resource availability, see [View resource availability](../psa/view-resource-availability.md).</span></span>  

> [!IMPORTANT]
>  <span data-ttu-id="96c7b-110">За да използвате функционалността за резервиране, геокодиране и услугите за местоположение на таблото на графика, трябва да включите карти.</span><span class="sxs-lookup"><span data-stu-id="96c7b-110">To use the schedule board booking functionality, geocoding, and location services, you need to turn on maps.</span></span>  
> 
> 1. <span data-ttu-id="96c7b-111">От главното меню изберете **Планиране на ресурси** > **Администрация**.</span><span class="sxs-lookup"><span data-stu-id="96c7b-111">On the main menu, select **Resource Scheduling** > **Administration**.</span></span>  
> 2. <span data-ttu-id="96c7b-112">Щракнете върху **Параметри на планиране**.</span><span class="sxs-lookup"><span data-stu-id="96c7b-112">Click **Scheduling parameters**.</span></span>  
> 3. <span data-ttu-id="96c7b-113">Отворете запис и превъртете надолу до секцията **Resource Scheduling Optimization**.</span><span class="sxs-lookup"><span data-stu-id="96c7b-113">Open record and scroll down to the **Resource Scheduling Optimization** section.</span></span>  
> 4. <span data-ttu-id="96c7b-114">В полето **Свързване към карти** изберете **Да**.</span><span class="sxs-lookup"><span data-stu-id="96c7b-114">On the **Connect to Maps** field, choose **Yes**.</span></span>  
> 5. <span data-ttu-id="96c7b-115">Приемете условията и запишете записа.</span><span class="sxs-lookup"><span data-stu-id="96c7b-115">Accept terms and save the record.</span></span>  
> 6. <span data-ttu-id="96c7b-116">В главното меню изберете **Project Service** > **Табло на графика**.</span><span class="sxs-lookup"><span data-stu-id="96c7b-116">On the main menu, select **Project Service** > **Schedule board**.</span></span> <span data-ttu-id="96c7b-117">Оттук има няколко начина за ръчно планиране на изискване за резервация.</span><span class="sxs-lookup"><span data-stu-id="96c7b-117">From here, there are several ways to manually schedule a booking requirement.</span></span> <span data-ttu-id="96c7b-118">Изберете метода, който е удобен за вас.</span><span class="sxs-lookup"><span data-stu-id="96c7b-118">Choose the method that works for you.</span></span>
  
## <a name="find-available-resources"></a><span data-ttu-id="96c7b-119">Намиране на налични ресурси</span><span class="sxs-lookup"><span data-stu-id="96c7b-119">Find available resources</span></span>

1.  <span data-ttu-id="96c7b-120">От списъка **Изискване за резервации** щракнете с десния бутон върху непланирана резервация и изберете едно от следните:</span><span class="sxs-lookup"><span data-stu-id="96c7b-120">From the **Booking Requirement** list, right-click an unscheduled booking and choose one of the following:</span></span>  
  
- <span data-ttu-id="96c7b-121">Изберете **Търсене на наличност - текущи ресурси** за намиране на наличен ресурс от списъка на таблото за графика.</span><span class="sxs-lookup"><span data-stu-id="96c7b-121">Choose **Find availability - Current Resources** to find an available resource from the list on the schedule board.</span></span>  
- <span data-ttu-id="96c7b-122">Изберете **Търсене на наличност - всички ресурси** за намиране на наличен ресурс от ресурсите в системата</span><span class="sxs-lookup"><span data-stu-id="96c7b-122">Choose **Find availability - All Resources** , to find an available resource from resources in the system</span></span>  
   > [!NOTE]
   >  <span data-ttu-id="96c7b-123">Когато направите това, филтрите ще покажат опции за избраното изискване за резервация.</span><span class="sxs-lookup"><span data-stu-id="96c7b-123">When you do this, the filters will show options for the selected booking requirement.</span></span>  
  
2. <span data-ttu-id="96c7b-124">Когато видите наличен слот, щракнете с десния бутон върху времевия слот на таблото за графика и изберете **Резервирай тук**.</span><span class="sxs-lookup"><span data-stu-id="96c7b-124">When you see an available slot, right-click the time slot on the schedule board and choose **Book Here**.</span></span> <span data-ttu-id="96c7b-125">Или плъзнете и пуснете изискването за резервация в наличния времеви интервал.</span><span class="sxs-lookup"><span data-stu-id="96c7b-125">Or, drag and drop the booking requirement to the available time slot.</span></span>  
  

## <a name="book-a-resource-using-the-daily-view-and-find-whos-under-booked"></a><span data-ttu-id="96c7b-126">Резервирайте ресурс с помощта на дневния изглед и разберете кой не е изцяло резервиран</span><span class="sxs-lookup"><span data-stu-id="96c7b-126">Book a resource using the daily view and find who’s under-booked</span></span>
  
1.  <span data-ttu-id="96c7b-127">На таблото за графика изберете **Режим на преглеждане** и изберете **Дни**.</span><span class="sxs-lookup"><span data-stu-id="96c7b-127">On the schedule board, select **View Mode** and select **Days**.</span></span>  
  
    <span data-ttu-id="96c7b-128">Така се показва мрежовиден изглед на броя часове, за които е резервиран ресурса на ден и през кои дни е свободен.</span><span class="sxs-lookup"><span data-stu-id="96c7b-128">This shows a grid view of how many hours a resource is booked per day and which days they are free.</span></span>  
  
2.  <span data-ttu-id="96c7b-129">Щракнете върху името на ресурса, когото желаете да резервирате и след това изберете **Резервирай**.</span><span class="sxs-lookup"><span data-stu-id="96c7b-129">Click the name of the resource you want to book, and then select **Book**.</span></span>  
  
3.  <span data-ttu-id="96c7b-130">В диалоговия прозорец **Резервиране на ресурси (създаване)** изберете проекта, за който искате да резервирате ресурса, както и метода на резервиране и началния и крайния час.</span><span class="sxs-lookup"><span data-stu-id="96c7b-130">On the **Resource booking (create)** dialog box, choose the project that you want to book the resource for along with booking method and start and end times.</span></span>  
  
4.  <span data-ttu-id="96c7b-131">Когато сте готови, изберете **Резервирай**.</span><span class="sxs-lookup"><span data-stu-id="96c7b-131">When you’re done, select **Book**.</span></span>  
  
## <a name="view-to-the-schedule-board"></a><span data-ttu-id="96c7b-132">Преглед на таблото за планиране</span><span class="sxs-lookup"><span data-stu-id="96c7b-132">View to the schedule board</span></span>
  
1.  <span data-ttu-id="96c7b-133">Изберете непланирано изискване за ресурс от списъка в долната част.</span><span class="sxs-lookup"><span data-stu-id="96c7b-133">Select an unscheduled booking requirement from the list at the bottom.</span></span>  
  
2.  <span data-ttu-id="96c7b-134">Плъзнете изискването за резервация към наличен ресурс/времеви интервал на таблото за графика.</span><span class="sxs-lookup"><span data-stu-id="96c7b-134">Drag the booking requirement to an available resource/time slot on the schedule board.</span></span>  
  
3.  <span data-ttu-id="96c7b-135">Когато сте готови, изберете **Резервирай**.</span><span class="sxs-lookup"><span data-stu-id="96c7b-135">When you're done, select **Book**.</span></span>  
  
### <a name="additional-resources"></a><span data-ttu-id="96c7b-136">Допълнителни ресурси</span><span class="sxs-lookup"><span data-stu-id="96c7b-136">Additional resources</span></span>  
 [<span data-ttu-id="96c7b-137">Ръководство за мениджъри на ресурси</span><span class="sxs-lookup"><span data-stu-id="96c7b-137">Resource manager guide</span></span>](../psa/resource-manager-guide.md)
