---
title: Създаване на шаблон за работно време
description: Как се създава шаблон за работно време в Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 54d7385a2bb161c7dd02d882090790debaef3bdb
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148765"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="0693e-103">Създаване на шаблон за работно време (Project Service)</span><span class="sxs-lookup"><span data-stu-id="0693e-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="0693e-104">Преди да можете да създавате графици за проекти, трябва да настроите календар за проекта, който определя броя на работни часове за приспособяване на ден в графика и всички неработни дни.</span><span class="sxs-lookup"><span data-stu-id="0693e-104">Before you can create project schedules, you need to set up a project calendar that defines the number of working hours to accommodate per day in the schedule and any business closures.</span></span> <span data-ttu-id="0693e-105">Можете да направите това с шаблон за работно време, който съдържа подробности за работното време на ден, почивните дни, както и всякакви други неработни дни.</span><span class="sxs-lookup"><span data-stu-id="0693e-105">You do this with a work hours template, which contains details about work hours per day, days off, and any other business closures.</span></span>  
  
 <span data-ttu-id="0693e-106">Когато създавате проект, свържете шаблон за работно време към календара на проекта, за да приложите графика проекта.</span><span class="sxs-lookup"><span data-stu-id="0693e-106">When you’re creating a project, you associate a work template to the project calendar to apply the schedule for the project.</span></span>  
  
 <span data-ttu-id="0693e-107">Има два начина, по които можете да създадете шаблон за работно време:</span><span class="sxs-lookup"><span data-stu-id="0693e-107">There are two ways you can create a work hours template:</span></span>  
  
-   <span data-ttu-id="0693e-108">Създаване на шаблон за работно време въз основа на календара на ресурса.</span><span class="sxs-lookup"><span data-stu-id="0693e-108">Create a work hours template based on a resource’s calendar.</span></span>  
  
-   <span data-ttu-id="0693e-109">Създаване на нов шаблон за работно време.</span><span class="sxs-lookup"><span data-stu-id="0693e-109">Create a new work hours template.</span></span>  
  
#### <a name="to-create-a-work-hours-template-based-on-a-resources-calendar"></a><span data-ttu-id="0693e-110">За да създадете шаблон за работно време въз основа на календара на ресурса</span><span class="sxs-lookup"><span data-stu-id="0693e-110">To create a work hours template based on a resource’s calendar</span></span>  
  
1.  <span data-ttu-id="0693e-111">Отидете на **Project Service > Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="0693e-111">Go to **Project Service > Resources**.</span></span>  
  
2.  <span data-ttu-id="0693e-112">Изберете ресурса, върху който искате да базирате работното време.</span><span class="sxs-lookup"><span data-stu-id="0693e-112">Select the resource you want to base your work hours on.</span></span>  
  
3.  <span data-ttu-id="0693e-113">Щракнете върху **Записване на календар като**, въведете име за шаблона за работно време и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="0693e-113">Click **Save Calendar As**, enter a name for the work hours template, and then click **Save**.</span></span>  
  
4.  <span data-ttu-id="0693e-114">Когато сте готови с промяната на опциите, щракнете върху **Запиши и затвори**.</span><span class="sxs-lookup"><span data-stu-id="0693e-114">When you’re done changing options, click **Save and Close**.</span></span>  
  
5.  <span data-ttu-id="0693e-115">Щракнете върху бутона **Запиши** в долния десен ъгъл на екрана.</span><span class="sxs-lookup"><span data-stu-id="0693e-115">Click the **Save** button at the bottom right corner of the screen.</span></span>  
  
#### <a name="to-create-a-new-work-hours-template"></a><span data-ttu-id="0693e-116">За да създадете нов шаблон за работно време</span><span class="sxs-lookup"><span data-stu-id="0693e-116">To create a new work hours template</span></span>  
  
1.  <span data-ttu-id="0693e-117">Отидете на **Project Service > Шаблони за работно време**.</span><span class="sxs-lookup"><span data-stu-id="0693e-117">Go to **Project Service > Work Hours Templates**.</span></span>  
  
2.  <span data-ttu-id="0693e-118">Щракнете върху **Нов**.</span><span class="sxs-lookup"><span data-stu-id="0693e-118">Click **New**.</span></span>  
  
3.  <span data-ttu-id="0693e-119">Въведете име за шаблона за работно време.</span><span class="sxs-lookup"><span data-stu-id="0693e-119">Enter a name for the work hours template.</span></span>  
  
4.  <span data-ttu-id="0693e-120">Изберете ресурс, върху който да се базира работното време, и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="0693e-120">Select a resource to base the work hours on, and then click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="0693e-121">Вижте също</span><span class="sxs-lookup"><span data-stu-id="0693e-121">See Also</span></span>  
 [<span data-ttu-id="0693e-122">Задаване на ресурси</span><span class="sxs-lookup"><span data-stu-id="0693e-122">Set up resources</span></span>](../psa/set-up-resources.md)
