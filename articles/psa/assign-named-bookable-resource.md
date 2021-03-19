---
title: Резервиране на наименувани налични ресурси в екип по проект и присвояване на задачи
description: Тази тема предоставя информация за това как да резервирате наименувани ресурси за екипи на проекти и присвояването им към задачи.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 11/28/2018
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
ms.openlocfilehash: 6169f2bdc107e63d666fb32d34f531fd5d472c2f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291426"
---
# <a name="book-named-bookable-resources-to-a-project-team-and-assign-tasks"></a><span data-ttu-id="fc4bd-103">Резервиране на наименувани налични ресурси в екип по проект и присвояване на задачи</span><span class="sxs-lookup"><span data-stu-id="fc4bd-103">Book named bookable resources to a project team and assign tasks</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="fc4bd-104">Можете да добавите наименуван ресурс към екипа на проекта си, като го резервирате директно в екипа.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-104">You can  add a named resource to your project team by booking them directly onto the team.</span></span> <span data-ttu-id="fc4bd-105">За целта изпълнете следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-105">To do this, complete the following steps.</span></span>

1. <span data-ttu-id="fc4bd-106">В Project Service Automation отидете на **Проекти** и изберете да отворите проекта, за който резервирате.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-106">In  Project Service Automation, go to **Projects**, and select the open the project that you are booking for.</span></span>
2. <span data-ttu-id="fc4bd-107">На страницата **Проект**, в раздела **Екип**, щракнете върху **Нов**.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-107">On the **Project** page, on the **Team** tab, click **New**.</span></span> 

![Добавяне на член на екипа от раздел „Екип“](media/RM-how-to-1.png)

3. <span data-ttu-id="fc4bd-109">В диалоговия прозорец **Бързо създаване на член на екипа на проекта** изберете наличния ресурс.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-109">In the **Quick Create Project Team Member** dialog box, select the bookable resource.</span></span> <span data-ttu-id="fc4bd-110">Полето **Роля** ще се попълни с ролята на ресурса по подразбиране, ако има присвоена такава.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-110">The **Role** field will populate with the resource's default role if they have one assigned.</span></span> <span data-ttu-id="fc4bd-111">Можете да промените ролята, ако е необходимо.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-111">You can change the role if needed.</span></span> 
4. <span data-ttu-id="fc4bd-112">Изберете датите от и до, между които ресурсът ще е необходим, и изберете метода на разпределение на капацитета на ресурса.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-112">Select the from and to dates that the resource will be needed and select the allocation method of the resource's capacity.</span></span> 
5. <span data-ttu-id="fc4bd-113">Ако искате членът на екипа да бъде одобряващ на проект, изберете **Да** в полето **Одобряващ на проект**.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-113">If you want the team member to be a project approver, select **Yes** in the **Project Approver** field.</span></span> <span data-ttu-id="fc4bd-114">Това ще означава, че членът на екипа може да одобри подадените записи за време и разходи за този проект.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-114">This will mean that the team member can approve submitted time and expense entries for this project.</span></span> 
6. <span data-ttu-id="fc4bd-115">Щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-115">Click **Save**.</span></span>

![Добавяне на член на екипа във формуляра за бързо създаване](media/RM-how-to-2.png)


<span data-ttu-id="fc4bd-117">Сега можете да присвоите резервирания ресурс на задачи по проекта.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-117">You can now assign the booked resource to tasks on the project.</span></span> <span data-ttu-id="fc4bd-118">На страницата **Проект** щракнете върху раздела **График**, за да присвоите задачи на новия ресурс.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-118">On the **Project** page, click the **Schedule** tab to assign tasks to the new resource.</span></span> <span data-ttu-id="fc4bd-119">Функцията за избор на ресурси, която се стартира от **Ресурси** в мрежата на задачата ще покаже членовете на екипа, които можете да изберете.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-119">The resource picker that is launched from the **Resources** field in the task grid will show the team members that you can select.</span></span>

![Присвояване на член на екип на задача в раздела „График“](media/RM-how-to-3.png)

<span data-ttu-id="fc4bd-121">Във версия 3 за Project Service Automation (PSA) резервациите на ресурси и присвояванията на задачи не са тясно обвързани.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-121">In version 3 for Project Service Automation (PSA), resource bookings and task assignments are not tightly coupled.</span></span> <span data-ttu-id="fc4bd-122">Това означава, че когато използвате функцията за избор на ресурси в графика, можете да присвоите задачи на членове на екипа за повече часове, отколкото техните резервации покриват в проекта.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-122">This means that when you use the resource picker in the schedule, you can assign tasks to team members for more hours than their bookings cover on the project.</span></span>
<span data-ttu-id="fc4bd-123">Можете да видите разликите между резервации и присвоявания за членовете на екипа в раздела **Екип** или в раздела **Съгласуване на ресурси**. Можете също така да съгласувате разликите между резервациите и присвояванията за ресурси на по-детайлно ниво.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-123">You can see the differences between team member bookings and assignments on the **Team** tab or on the **Resource Reconciliation** tab. You can also reconcile the differences between bookings and assignments for resources at a more detailed level.</span></span>

![Раздел „Съгласуване на ресурси“](media/RM-how-to-4.png)

<span data-ttu-id="fc4bd-125">Можете също да използвате функцията за избор на ресурси в раздела **График** за търсене и избор на налични ресурси, които вече не са част от екипа на проекта.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-125">You can also use the resource picker on the **Schedule** tab to search for and select bookable resources that are not already part of the project team.</span></span> <span data-ttu-id="fc4bd-126">Те се показват във функцията за избор на ресурси като **Други ресурси**.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-126">These are shown in the resource picker as **Other Resources**.</span></span>

![Присвояване на ресурс, който не член на екип, на задача](media/RM-how-to-5.png)

<span data-ttu-id="fc4bd-128">Когато направите това, ресурсът се добавя към екипа на проекта и се присвоява на задачата, но не се генерират резервации.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-128">When you do this, the resource is added to the project team and assigned to the task, but no bookings are generated.</span></span>

![Член на екипа с присвоявания и без резервации](media/RM-how-to-6.png)

<span data-ttu-id="fc4bd-130">Можете да използвате възможността за удължаване на резервации в раздела **Съгласуване** или **Табло на графика**, за да резервирате капацитета на ресурса за проекта.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-130">You can use the **Reconciliation** tab’s extend booking capability or the **Schedule Board** to book the resource’s capacity to the project.</span></span>

![Удължаване на резервациите за член на екипа в раздела „Съгласуване на ресурси“](media/RM-how-to-7.png)

<span data-ttu-id="fc4bd-132">След като член на екип бъде резервиран по вашия проект, можете да използвате поддръжката на резервации или таблото на графика директно, за да управлявате неговите резервации.</span><span class="sxs-lookup"><span data-stu-id="fc4bd-132">After a team member is booked on your project, you can use maintain bookings or use the Schedule Board directly to manage their bookings.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]