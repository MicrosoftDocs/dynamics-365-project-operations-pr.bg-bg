---
title: Създаване на шаблон за работно време
description: Как се създава шаблон за работно време в Project Service
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 1a519487-25f1-4e9d-b739-1c1becf1d649
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5e7ef4af5f22419cccd8f29ea2a0a0a21a75875a
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749312"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="5f431-103">Създаване на шаблон за работно време (Project Service)</span><span class="sxs-lookup"><span data-stu-id="5f431-103">Create a work hours template (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="5f431-104">Преди да можете да създавате графици за проекти, трябва да настроите календар за проекта, който определя броя на работни часове за приспособяване на ден в графика и всички неработни дни.</span><span class="sxs-lookup"><span data-stu-id="5f431-104">Before you can create project schedules, you need to set up a project calendar that defines the number of working hours to accommodate per day in the schedule and any business closures.</span></span> <span data-ttu-id="5f431-105">Можете да направите това с шаблон за работно време, който съдържа подробности за работното време на ден, почивните дни, както и всякакви други неработни дни.</span><span class="sxs-lookup"><span data-stu-id="5f431-105">You do this with a work hours template, which contains details about work hours per day, days off, and any other business closures.</span></span>  
  
 <span data-ttu-id="5f431-106">Когато създавате проект, свържете шаблон за работно време към календара на проекта, за да приложите графика проекта.</span><span class="sxs-lookup"><span data-stu-id="5f431-106">When you’re creating a project, you associate a work template to the project calendar to apply the schedule for the project.</span></span>  
  
 <span data-ttu-id="5f431-107">Има два начина, по които можете да създадете шаблон за работно време:</span><span class="sxs-lookup"><span data-stu-id="5f431-107">There are two ways you can create a work hours template:</span></span>  
  
-   <span data-ttu-id="5f431-108">Създаване на шаблон за работно време въз основа на календара на ресурса.</span><span class="sxs-lookup"><span data-stu-id="5f431-108">Create a work hours template based on a resource’s calendar.</span></span>  
  
-   <span data-ttu-id="5f431-109">Създаване на нов шаблон за работно време.</span><span class="sxs-lookup"><span data-stu-id="5f431-109">Create a new work hours template.</span></span>  
  
#### <a name="to-create-a-work-hours-template-based-on-a-resources-calendar"></a><span data-ttu-id="5f431-110">За да създадете шаблон за работно време въз основа на календара на ресурса</span><span class="sxs-lookup"><span data-stu-id="5f431-110">To create a work hours template based on a resource’s calendar</span></span>  
  
1.  <span data-ttu-id="5f431-111">Отидете на **Project Service > Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="5f431-111">Go to **Project Service > Resources**.</span></span>  
  
2.  <span data-ttu-id="5f431-112">Изберете ресурса, върху който искате да базирате работното време.</span><span class="sxs-lookup"><span data-stu-id="5f431-112">Select the resource you want to base your work hours on.</span></span>  
  
3.  <span data-ttu-id="5f431-113">Щракнете върху **Записване на календар като**, въведете име за шаблона за работно време и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="5f431-113">Click **Save Calendar As**, enter a name for the work hours template, and then click **Save**.</span></span>  
  
4.  <span data-ttu-id="5f431-114">Когато сте готови с промяната на опциите, щракнете върху **Запиши и затвори**.</span><span class="sxs-lookup"><span data-stu-id="5f431-114">When you’re done changing options, click **Save and Close**.</span></span>  
  
5.  <span data-ttu-id="5f431-115">Щракнете върху бутона **Запиши** в долния десен ъгъл на екрана.</span><span class="sxs-lookup"><span data-stu-id="5f431-115">Click the **Save** button at the bottom right corner of the screen.</span></span>  
  
#### <a name="to-create-a-new-work-hours-template"></a><span data-ttu-id="5f431-116">За да създадете нов шаблон за работно време</span><span class="sxs-lookup"><span data-stu-id="5f431-116">To create a new work hours template</span></span>  
  
1.  <span data-ttu-id="5f431-117">Отидете на **Project Service > Шаблони за работно време**.</span><span class="sxs-lookup"><span data-stu-id="5f431-117">Go to **Project Service > Work Hours Templates**.</span></span>  
  
2.  <span data-ttu-id="5f431-118">Щракнете върху **Нов**.</span><span class="sxs-lookup"><span data-stu-id="5f431-118">Click **New**.</span></span>  
  
3.  <span data-ttu-id="5f431-119">Въведете име за шаблона за работно време.</span><span class="sxs-lookup"><span data-stu-id="5f431-119">Enter a name for the work hours template.</span></span>  
  
4.  <span data-ttu-id="5f431-120">Изберете ресурс, върху който да се базира работното време, и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="5f431-120">Select a resource to base the work hours on, and then click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="5f431-121">Вижте също</span><span class="sxs-lookup"><span data-stu-id="5f431-121">See Also</span></span>  
 [<span data-ttu-id="5f431-122">Задаване на ресурси</span><span class="sxs-lookup"><span data-stu-id="5f431-122">Set up resources</span></span>](../project-service/set-up-resources.md)
