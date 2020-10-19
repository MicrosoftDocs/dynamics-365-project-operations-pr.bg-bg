---
title: Поддръжка на членовете на екипа
description: Тази тема предоставя информация за резервиране на наименувани ресурси за екипи на проекти и присвояването им към задачи.
author: ruhercul
manager: AnnBe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: f5b36628e90896c9fe6570de71c95eab83a44ebd
ms.sourcegitcommit: 396e0fea2f1598a5313cb0128eca4fe0bb5aade9
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961817"
---
# <a name="maintain-team-members"></a><span data-ttu-id="2f56f-103">Поддръжка на членовете на екипа</span><span class="sxs-lookup"><span data-stu-id="2f56f-103">Maintain team members</span></span>

<span data-ttu-id="2f56f-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="2f56f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="2f56f-105">Можете да добавите наименуван ресурс към екипа на проекта си, като го резервирате директно в екипа.</span><span class="sxs-lookup"><span data-stu-id="2f56f-105">You can add a named resource to your project team by booking them directly to the team.</span></span>

1. <span data-ttu-id="2f56f-106">В Dynamics 365 Project Operations отидете на **Проекти** и изберете да отворите проекта, за който резервирате.</span><span class="sxs-lookup"><span data-stu-id="2f56f-106">In Dynamics 365 Project Operations, go to **Projects**, and select the open the project that you're booking for.</span></span>
2. <span data-ttu-id="2f56f-107">На страницата **Проект**, в раздела **Екип**, изберете **Създаване**.</span><span class="sxs-lookup"><span data-stu-id="2f56f-107">On the **Project** page, on the **Team** tab, select **New**.</span></span> 
3. <span data-ttu-id="2f56f-108">В диалоговия прозорец **Бързо създаване на член на екипа на проекта** изберете наличния ресурс.</span><span class="sxs-lookup"><span data-stu-id="2f56f-108">In the **Quick Create Project Team Member** dialog box, select the bookable resource.</span></span> <span data-ttu-id="2f56f-109">Полето **Роля** ще се попълни с ролята на ресурса по подразбиране, ако има присвоена такава.</span><span class="sxs-lookup"><span data-stu-id="2f56f-109">The **Role** field will populate with the resource's default role if they have one assigned.</span></span> <span data-ttu-id="2f56f-110">Можете да промените ролята.</span><span class="sxs-lookup"><span data-stu-id="2f56f-110">You can change the role.</span></span> 
4. <span data-ttu-id="2f56f-111">Изберете датите от и до, между които ресурсът ще е необходим, и изберете метода на разпределение на капацитета на ресурса.</span><span class="sxs-lookup"><span data-stu-id="2f56f-111">Select the from and to dates that the resource will be needed, and select the allocation method of the resource's capacity.</span></span> 
5. <span data-ttu-id="2f56f-112">В полето **Одобряващ на проект** изберете **Да**, ако искате членът на екипа да бъде одобряващ на проект.</span><span class="sxs-lookup"><span data-stu-id="2f56f-112">In the **Project Approver** field, select **Yes** if you want the team member to be a project approver.</span></span> <span data-ttu-id="2f56f-113">Членът на екипа може да одобри подадените записи за време и разходи за този проект.</span><span class="sxs-lookup"><span data-stu-id="2f56f-113">The team member can approve submitted time and expense entries for this project.</span></span> 
6. <span data-ttu-id="2f56f-114">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="2f56f-114">Select **Save**.</span></span>

<span data-ttu-id="2f56f-115">Сега можете да присвоите резервирания ресурс на задачи по проекта.</span><span class="sxs-lookup"><span data-stu-id="2f56f-115">You can now assign the booked resource to tasks on the project.</span></span> <span data-ttu-id="2f56f-116">На страницата **Проект** в раздела **График** присвоете задачи на новия ресурс.</span><span class="sxs-lookup"><span data-stu-id="2f56f-116">On the **Project** page, on the **Schedule** tab, assign tasks to the new resource.</span></span> <span data-ttu-id="2f56f-117">Функцията за избор на ресурси, която се стартира от **Ресурси** в мрежата на задачата ще покаже членовете на екипа, които можете да изберете.</span><span class="sxs-lookup"><span data-stu-id="2f56f-117">The resource picker that is launched from the **Resources** field in the task grid will show the team members that you can select.</span></span>


<span data-ttu-id="2f56f-118">В Project Operations резервирането на ресурси и задачите на задачи не са тясно свързани.</span><span class="sxs-lookup"><span data-stu-id="2f56f-118">In Project Operations, resource bookings and task assignments aren't tightly coupled.</span></span> <span data-ttu-id="2f56f-119">Когато използвате функцията за избор на ресурси в графика, можете да присвоите задачи на членове на екипа за повече часове, отколкото техните резервации покриват в проекта.</span><span class="sxs-lookup"><span data-stu-id="2f56f-119">When you use the resource picker in the schedule, you can assign tasks to team members for more hours than their bookings cover on the project.</span></span>

<span data-ttu-id="2f56f-120">Разликите между резервациите и заданията на членовете на екипа са показани на раздели **Екип** и **Съгласуване на ресурсите**.</span><span class="sxs-lookup"><span data-stu-id="2f56f-120">The differences between team member bookings and assignments are shown on the **Team** and **Resource Reconciliation** tabs.</span></span> <span data-ttu-id="2f56f-121">Можете също така да съгласувате разликите между резервации и задания за ресурси на по-подробно ниво.</span><span class="sxs-lookup"><span data-stu-id="2f56f-121">You can also reconcile the differences between bookings and assignments for resources at a more detailed level.</span></span>

<span data-ttu-id="2f56f-122">Използвайте функцията за избор на ресурси в раздела **График** за търсене и избор на налични ресурси, които вече не са част от екипа на проекта.</span><span class="sxs-lookup"><span data-stu-id="2f56f-122">Use the resource picker on the **Schedule** tab to search for and select bookable resources that are not already part of the project team.</span></span> <span data-ttu-id="2f56f-123">Тези ресурси се показват в инструмента за избор на ресурси като **Други ресурси**.</span><span class="sxs-lookup"><span data-stu-id="2f56f-123">These resources are shown in the resource picker as **Other Resources**.</span></span>

<span data-ttu-id="2f56f-124">Когато направите селекция, ресурсът се добавя към екипа на проекта и се присвоява на задачата, но не се генерират резервации.</span><span class="sxs-lookup"><span data-stu-id="2f56f-124">When you make a selection, the resource is added to the project team and assigned to the task, but no bookings are generated.</span></span>

<span data-ttu-id="2f56f-125">Можете да използвате възможността за удължаване на резервации в раздела **Съгласуване** или **Табло на графика**, за да резервирате капацитета на ресурса за проекта.</span><span class="sxs-lookup"><span data-stu-id="2f56f-125">You can use the **Reconciliation** tab’s extend booking capability or the **Schedule Board** to book the resource’s capacity to the project.</span></span>

<span data-ttu-id="2f56f-126">След като член на екип бъде резервиран по вашия проект, можете да използвате **поддръжката на резервации** или **таблото на графика** директно, за да управлявате неговите резервации.</span><span class="sxs-lookup"><span data-stu-id="2f56f-126">After a team member is booked on your project, you can use **Maintain bookings** or the **Schedule Board** directly to manage their bookings.</span></span>
