---
title: Управление на часови зони
description: Когато се създаде проект, неговата часова зона се основава на часовата зона, дефинирана в приложения шаблон за работен час.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 27f58f0dacc3404119a719547ad374629c740740
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071758"
---
# <a name="manage-time-zones"></a><span data-ttu-id="43f77-103">Управление на часови зони</span><span class="sxs-lookup"><span data-stu-id="43f77-103">Manage time zones</span></span>

<span data-ttu-id="43f77-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="43f77-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


## <a name="projects"></a><span data-ttu-id="43f77-105">Проекти</span><span class="sxs-lookup"><span data-stu-id="43f77-105">Projects</span></span>

<span data-ttu-id="43f77-106">Когато се създаде проект, неговата часова зона се основава на часовата зона, дефинирана в приложения шаблон за работен час.</span><span class="sxs-lookup"><span data-stu-id="43f77-106">When a project is created, the time zone is based on the time zone defined in the applied work hour template.</span></span> <span data-ttu-id="43f77-107">В **Проект** датите винаги са свързани с часовата зона на потребителя, който е влязъл във всеки раздел, с изключение на раздела **Задача** . Когато преглеждате структурата на разбивка на работата, датите винаги ще се показват в часовата зона на проекта.</span><span class="sxs-lookup"><span data-stu-id="43f77-107">On the **Project** for, the dates are always relative to the time zone of the user that is logged in on each tab, except the **Task** tab. When you view the work breakdown structure, the dates will always be displayed in the project’s time zone.</span></span>

## <a name="tasks"></a><span data-ttu-id="43f77-108">Задачи</span><span class="sxs-lookup"><span data-stu-id="43f77-108">Tasks</span></span>

<span data-ttu-id="43f77-109">Когато се създаде задача, началното, крайното време и часовете / ден се контролират от работното време на проекта.</span><span class="sxs-lookup"><span data-stu-id="43f77-109">When a task is created, the start time, end time, and hours/day is controlled by the working hours of the project.</span></span> <span data-ttu-id="43f77-110">Например, ако задача е създадена с проект, чиято часова зона е -8 PST и има следното работно време: от 9:00 до 17:00 от понеделник до петък, всяка задача, създадена без задание, ще спазва началния час и краен час на календара на проекта.</span><span class="sxs-lookup"><span data-stu-id="43f77-110">For example, if a task is created with a project whose time zone is -8 PST and has the following working hours: 9:00 AM to 5:00 PM Monday to Friday, any task created without an assignment will respect the start time and end time of the project calendar.</span></span>

## <a name="manage-resources-with-time-zones"></a><span data-ttu-id="43f77-111">Управление на ресурси с часови зони</span><span class="sxs-lookup"><span data-stu-id="43f77-111">Manage resources with time zones</span></span>

<span data-ttu-id="43f77-112">За точни и предсказуеми резултати при използване **Удължете резервацията** , има две основни предпоставки, които трябва да бъдат изпълнени:</span><span class="sxs-lookup"><span data-stu-id="43f77-112">For accurate and predictable results when using **Extend Booking** , there are two key prerequisites that must be met:</span></span>  

- <span data-ttu-id="43f77-113">Потребителят трябва да конфигурира часовата зона на устройството си, за да съответства на часовата зона, определена в системата **Настройки за персонализация**.</span><span class="sxs-lookup"><span data-stu-id="43f77-113">The user must configure their device's time zone to match the time zone defined in the system's **Personalization Settings**.</span></span>
 
  ![Настройки на часовата зона в Windows 10](media/reconcile-assignments-03.png)

  ![Настройки на часовата зона в настройките за персонализиране](media/reconcile-assignments-04.png)
 
- <span data-ttu-id="43f77-116">Наличният ресурс трябва да има работно време от поне една минута, което се припокрива с контурите, използвани за определяне на заявеното удължаване.</span><span class="sxs-lookup"><span data-stu-id="43f77-116">The bookable resource must have at least one minute of working time that overlaps with the contours that are used to define the requested extension.</span></span> <span data-ttu-id="43f77-117">Например следните ресурси с работно време, което пада между 9:00 и 19:00.</span><span class="sxs-lookup"><span data-stu-id="43f77-117">For example, the following resources with working hours that fall between 9:00 AM and 7:00 PM.</span></span> 

  ![Сравнение на контурите на ресурсите](media/reconcile-assignments-05.png)

<span data-ttu-id="43f77-119">Таблицата по-долу показва:</span><span class="sxs-lookup"><span data-stu-id="43f77-119">The following table shows:</span></span>

- <span data-ttu-id="43f77-120">Шаблон за календар на проект</span><span class="sxs-lookup"><span data-stu-id="43f77-120">A project calendar template</span></span>
- <span data-ttu-id="43f77-121">Ресурс А: Този ресурс има същия календар и е в същата часова зона като проекта.</span><span class="sxs-lookup"><span data-stu-id="43f77-121">Resource A: This resource has the same calendar and is in the same time zone as the project.</span></span> <span data-ttu-id="43f77-122">Началният час на резервациите ще бъде 9:00 ч.</span><span class="sxs-lookup"><span data-stu-id="43f77-122">The start time of the bookings will be 9:00 AM.</span></span>
- <span data-ttu-id="43f77-123">Ресурс Б: Този ресурс се намира в различна часова зона от проекта и започва в 7:00 ч. В тяхната часова зона.</span><span class="sxs-lookup"><span data-stu-id="43f77-123">Resource B: This resource is located in a different time zone than the project and starts at 7:00 AM in their time zone.</span></span> <span data-ttu-id="43f77-124">Резервациите обаче ще започнат в 9:00 ч., тъй като това е най-ранният начален час на контура за присвояване.</span><span class="sxs-lookup"><span data-stu-id="43f77-124">However, the bookings will begin at 9:00 AM as that is the earliest start time of the assignment contour.</span></span>
- <span data-ttu-id="43f77-125">Ресурси C и D: Ресурсите се намират в различни часови зони, различни и един от друг, и от проекта, и резервациите им започват не по-рано от съответните налични начални часове.</span><span class="sxs-lookup"><span data-stu-id="43f77-125">Resources C and D: The resources are located in different time zones, both different from each other and the project, and their bookings start no earlier than their respective available start times.</span></span>

|<span data-ttu-id="43f77-126">Обект</span><span class="sxs-lookup"><span data-stu-id="43f77-126">Entity</span></span>  |<span data-ttu-id="43f77-127">Календар</span><span class="sxs-lookup"><span data-stu-id="43f77-127">Calendar</span></span>  |
|-|-|
|<span data-ttu-id="43f77-128">Шаблон за календар на проект</span><span class="sxs-lookup"><span data-stu-id="43f77-128">Project calendar template</span></span>   | ![календар на проект](media/reconcile-assignments-06.png) |
|<span data-ttu-id="43f77-130">Ресурс А</span><span class="sxs-lookup"><span data-stu-id="43f77-130">Resource A</span></span>  | ![Календар на ресурс А](media/reconcile-assignments-06.png) |
|<span data-ttu-id="43f77-132">Ресурс Б</span><span class="sxs-lookup"><span data-stu-id="43f77-132">Resource B</span></span>  |  ![Календар на ресурс Б](media/reconcile-assignments-07.png) |
|<span data-ttu-id="43f77-134">Ресурс В</span><span class="sxs-lookup"><span data-stu-id="43f77-134">Resource C</span></span>  |  ![Календар на ресурс В](media/reconcile-assignments-08.png) |
|<span data-ttu-id="43f77-136">Ресурс Г</span><span class="sxs-lookup"><span data-stu-id="43f77-136">Resource D</span></span>  | ![Календар на ресурс Г](media/reconcile-assignments-09.png)  |
 
<span data-ttu-id="43f77-138">Когато навигирате до изгледа **Съгласуване** , се показват назначенията на ресурси и свързаните с това недостиг на резервации.</span><span class="sxs-lookup"><span data-stu-id="43f77-138">When you navigate to the **Reconciliation** view, the resource assignments and the associated booking shortages are displayed.</span></span>

![Изглед за съгласуване преди удължаване](media/reconcile-assignments-10.png)

<span data-ttu-id="43f77-140">След като се използва функционалността за удължено резервиране за всеки ресурс, резервациите се удължават успешно за всеки ресурс, тъй като работното време на всеки ресурс се припокрива с контурите на недостига.</span><span class="sxs-lookup"><span data-stu-id="43f77-140">After the extend booking functionality has been used for each resource, bookings are successfully extended for each resource because each resource’s working hours overlapped with the contours of the shortage.</span></span>

![Изглед за съгласуване след удължаване на резервацията](media/reconcile-assignments-11.png) 

<span data-ttu-id="43f77-142">Забележете, че по-внимателният поглед върху детайлите на резервациите показва разлики в началния час на резервациите.</span><span class="sxs-lookup"><span data-stu-id="43f77-142">Notice that a closer look at the details of the bookings shows differences in the start time of the bookings.</span></span> <span data-ttu-id="43f77-143">Резервациите започват не по-рано от началното време на контура на заданието и не по-рано от наличното начално време на ресурса.</span><span class="sxs-lookup"><span data-stu-id="43f77-143">The bookings start no earlier than the start time of the assignment contour and no earlier than the available start time of the resource.</span></span>

![Нови резервации на ресурсите в таблото на графика](media/reconcile-assignments-12.png)
