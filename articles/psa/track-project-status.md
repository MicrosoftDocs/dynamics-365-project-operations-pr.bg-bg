---
title: Проследяване на състоянието на проект
description: Как се проследява състоянието на проект в Project Service
author: ruhercul
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
ms.openlocfilehash: 70d07c98bd9432712e939445dbf867b96642f5ba
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071906"
---
# <a name="track-a-projects-status-project-service"></a><span data-ttu-id="f1817-103">Проследяване на състоянието на проект (Project Service)</span><span class="sxs-lookup"><span data-stu-id="f1817-103">Track a project’s status (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="f1817-104">Използвайте възможностите на [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)], за да следите напредъка на проект на клиента.</span><span class="sxs-lookup"><span data-stu-id="f1817-104">Use the [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] to track the progress of a client’s project.</span></span>  

<span data-ttu-id="f1817-105">С напредването на ангажимент етапите на проекта се актуализират, за да отразят етапа на ангажимента:</span><span class="sxs-lookup"><span data-stu-id="f1817-105">As the engagement progresses, the project stages update to reflect the stage of the engagement:</span></span>  


|              |                                                                                                                                                                                                                                                                                                  |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   <span data-ttu-id="f1817-106">**Нов**</span><span class="sxs-lookup"><span data-stu-id="f1817-106">**New**</span></span>    | <span data-ttu-id="f1817-107">Когато създавате проект, етапът е настроен на **Нов**.</span><span class="sxs-lookup"><span data-stu-id="f1817-107">When you create a project, the stage is set to **New**.</span></span> <span data-ttu-id="f1817-108">Ако сте създали проекта от шаблон, на този етап проектът може да има график, оценки и данни за екипа.</span><span class="sxs-lookup"><span data-stu-id="f1817-108">If you created the project from a template, at this stage the project may have a schedule, estimates, and team data.</span></span> <span data-ttu-id="f1817-109">В противен случай той ще бъде скица на проекта и трябва да въведете ръчно останалата част от компонентите на проекта.</span><span class="sxs-lookup"><span data-stu-id="f1817-109">Otherwise, it will be the outline of the project and you need to manually enter the rest of the project components.</span></span> |
|  <span data-ttu-id="f1817-110">**Оферта**</span><span class="sxs-lookup"><span data-stu-id="f1817-110">**Quote**</span></span>   |      <span data-ttu-id="f1817-111">Когато свържете проект към оферта или да го създадете от оферта, етапът на проект е настроен на **Оферта** и прогнозните начална и крайна дати също се актуализират.</span><span class="sxs-lookup"><span data-stu-id="f1817-111">When you associate a project to a quote or create it from a quote, the project stage is set to **Quote** , and the estimated start and end datesare updated as well.</span></span> <span data-ttu-id="f1817-112">Когато проектът е в етапа на оферта, подробностите за офертата се показват в раздела **Продажби** на страницата **Проект**.</span><span class="sxs-lookup"><span data-stu-id="f1817-112">When the project is in the quote stage, details on the quote display on the **Sales** tab on the **Project** page.</span></span>      |
|   <span data-ttu-id="f1817-113">**План**</span><span class="sxs-lookup"><span data-stu-id="f1817-113">**Plan**</span></span>   |                                     <span data-ttu-id="f1817-114">Когато спечелите оферта, свързана с даден проект, и когато ангажимент напредне до етапа на договор, етапът на проекта се актуализира на **План**.</span><span class="sxs-lookup"><span data-stu-id="f1817-114">When you win a quote associated with a project, and when the engagement progresses to the contract stage, the project stage updates to **Plan**.</span></span> <span data-ttu-id="f1817-115">Подробностите за договора се показват в раздела **Продажби** на страницата **Проект**.</span><span class="sxs-lookup"><span data-stu-id="f1817-115">Contract details display on the **Sales** tab on the **Project** page.</span></span>                                      |
| <span data-ttu-id="f1817-116">**Завършен**</span><span class="sxs-lookup"><span data-stu-id="f1817-116">**Complete**</span></span> |                    <span data-ttu-id="f1817-117">Когато приключи работата по проекта, можете да смените етапа на **Завършен**.</span><span class="sxs-lookup"><span data-stu-id="f1817-117">When the project work is complete, you can flip the stage to **Complete**.</span></span> <span data-ttu-id="f1817-118">Когато на етапът на проекта е зададен като завършен, се разбира, че работата е свършена на 100%, но проектът се запазва отворен, за да се запишат евентуални незавършено записи за време или разходи.</span><span class="sxs-lookup"><span data-stu-id="f1817-118">When the project stage is set to complete, it’s understood that the work is 100% complete but the project is kept open for any pending time or expense entries to be recorded.</span></span>                     |
|  <span data-ttu-id="f1817-119">**Затвори**</span><span class="sxs-lookup"><span data-stu-id="f1817-119">**Close**</span></span>   |           <span data-ttu-id="f1817-120">Когато всички транзакции са били регистрирани по проекта и не очаквате да се регистрират повече можете да зададете ръчно етапа на **Затворен**.</span><span class="sxs-lookup"><span data-stu-id="f1817-120">When all transactions have been recorded on the project and you don't expect any more to be logged, you can manually set the stage to **Close**.</span></span> <span data-ttu-id="f1817-121">Когато проектът е настроен на **Затворен** , не можете да регистрирате повече транзакции по проекта и проектът ще е само за четене.</span><span class="sxs-lookup"><span data-stu-id="f1817-121">When the project is set to **Close** , you can’t log any more transactions on the project and the project will be read only.</span></span>           |

## <a name="to-track-a-projects-status"></a><span data-ttu-id="f1817-122">За проследяване на състоянието на проект</span><span class="sxs-lookup"><span data-stu-id="f1817-122">To track a project’s status</span></span>  

1.  <span data-ttu-id="f1817-123">Отидете на **Project Service > Проекти**.</span><span class="sxs-lookup"><span data-stu-id="f1817-123">Go to **Project Service > Projects**.</span></span>  

2.  <span data-ttu-id="f1817-124">Щракнете върху проекта, върху който искате да работите.</span><span class="sxs-lookup"><span data-stu-id="f1817-124">Click the project you want to work on.</span></span>  

3.  <span data-ttu-id="f1817-125">В лентата в горната част на екрана изберете стрелката за падащо меню до името на проекта и след това щракнете върху **Проследяване на проект**.</span><span class="sxs-lookup"><span data-stu-id="f1817-125">In the bar across the top of the screen, select the down arrow next to the project name, and then click **Project Tracking**.</span></span>  

4.  <span data-ttu-id="f1817-126">Изберете **Проследяване на усилията** или **Проследяване на разходите** в падащия списък над списъка със задачи.</span><span class="sxs-lookup"><span data-stu-id="f1817-126">Select **Effort Tracking** or **Cost Tracking** in the drop-down list above the task list.</span></span>  

5.  <span data-ttu-id="f1817-127">Щракнете двукратно върху задача, за да я редактирате.</span><span class="sxs-lookup"><span data-stu-id="f1817-127">Double-click any task to edit it.</span></span> <span data-ttu-id="f1817-128">Можете също да преместите или преоразмерите стълбовете в диаграмата на Гант, за да промените времето и напредъка за дадена задача.</span><span class="sxs-lookup"><span data-stu-id="f1817-128">You can also move or resize the bars in the Gantt chart to change the time and progress for a task.</span></span>  

### <a name="see-also"></a><span data-ttu-id="f1817-129">Вижте също</span><span class="sxs-lookup"><span data-stu-id="f1817-129">See Also</span></span>  
 [<span data-ttu-id="f1817-130">Ръководство за мениджъри на проекти</span><span class="sxs-lookup"><span data-stu-id="f1817-130">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
