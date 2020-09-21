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
ms.prod: ''
ms.technology: ''
ms.assetid: 7610aecb-318c-422b-b626-9106b0736b5f
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: e4d53b6235c3b941bce525dca09ee3d647c3d242
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749356"
---
# <a name="track-a-projects-status-project-service"></a><span data-ttu-id="df981-103">Проследяване на състоянието на проект (Project Service)</span><span class="sxs-lookup"><span data-stu-id="df981-103">Track a project’s status (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="df981-104">Използвайте възможностите на [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)], за да следите напредъка на проект на клиента.</span><span class="sxs-lookup"><span data-stu-id="df981-104">Use the [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] to track the progress of a client’s project.</span></span>  

<span data-ttu-id="df981-105">С напредването на ангажимент етапите на проекта се актуализират, за да отразят етапа на ангажимента:</span><span class="sxs-lookup"><span data-stu-id="df981-105">As the engagement progresses, the project stages update to reflect the stage of the engagement:</span></span>  


|              |                                                                                                                                                                                                                                                                                                  |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   <span data-ttu-id="df981-106">**Нов**</span><span class="sxs-lookup"><span data-stu-id="df981-106">**New**</span></span>    | <span data-ttu-id="df981-107">Когато създавате проект, етапът е настроен на **Нов**.</span><span class="sxs-lookup"><span data-stu-id="df981-107">When you create a project, the stage is set to **New**.</span></span> <span data-ttu-id="df981-108">Ако сте създали проекта от шаблон, на този етап проектът може да има график, оценки и данни за екипа.</span><span class="sxs-lookup"><span data-stu-id="df981-108">If you created the project from a template, at this stage the project may have a schedule, estimates, and team data.</span></span> <span data-ttu-id="df981-109">В противен случай той ще бъде скица на проекта и трябва да въведете ръчно останалата част от компонентите на проекта.</span><span class="sxs-lookup"><span data-stu-id="df981-109">Otherwise, it will be the outline of the project and you need to manually enter the rest of the project components.</span></span> |
|  <span data-ttu-id="df981-110">**Оферта**</span><span class="sxs-lookup"><span data-stu-id="df981-110">**Quote**</span></span>   |      <span data-ttu-id="df981-111">Когато свържете проект към оферта или да го създадете от оферта, етапът на проект е настроен на **Оферта** и прогнозните начална и крайна дати също се актуализират.</span><span class="sxs-lookup"><span data-stu-id="df981-111">When you associate a project to a quote or create it from a quote, the project stage is set to **Quote**, and the estimated start and end datesare updated as well.</span></span> <span data-ttu-id="df981-112">Когато проектът е в етапа на оферта, подробностите за офертата се показват в раздела **Продажби** на страницата **Проект**.</span><span class="sxs-lookup"><span data-stu-id="df981-112">When the project is in the quote stage, details on the quote display on the **Sales** tab on the **Project** page.</span></span>      |
|   <span data-ttu-id="df981-113">**План**</span><span class="sxs-lookup"><span data-stu-id="df981-113">**Plan**</span></span>   |                                     <span data-ttu-id="df981-114">Когато спечелите оферта, свързана с даден проект, и когато ангажимент напредне до етапа на договор, етапът на проекта се актуализира на **План**.</span><span class="sxs-lookup"><span data-stu-id="df981-114">When you win a quote associated with a project, and when the engagement progresses to the contract stage, the project stage updates to **Plan**.</span></span> <span data-ttu-id="df981-115">Подробностите за договора се показват в раздела **Продажби**на страницата **Проект**.</span><span class="sxs-lookup"><span data-stu-id="df981-115">Contract details display on the **Sales** tab on the **Project** page.</span></span>                                      |
| <span data-ttu-id="df981-116">**Завършен**</span><span class="sxs-lookup"><span data-stu-id="df981-116">**Complete**</span></span> |                    <span data-ttu-id="df981-117">Когато приключи работата по проекта, можете да смените етапа на **Завършен**.</span><span class="sxs-lookup"><span data-stu-id="df981-117">When the project work is complete, you can flip the stage to **Complete**.</span></span> <span data-ttu-id="df981-118">Когато на етапът на проекта е зададен като завършен, се разбира, че работата е свършена на 100%, но проектът се запазва отворен, за да се запишат евентуални незавършено записи за време или разходи.</span><span class="sxs-lookup"><span data-stu-id="df981-118">When the project stage is set to complete, it’s understood that the work is 100% complete but the project is kept open for any pending time or expense entries to be recorded.</span></span>                     |
|  <span data-ttu-id="df981-119">**Затвори**</span><span class="sxs-lookup"><span data-stu-id="df981-119">**Close**</span></span>   |           <span data-ttu-id="df981-120">Когато всички транзакции са били регистрирани по проекта и не очаквате да се регистрират повече можете да зададете ръчно етапа на **Затворен**.</span><span class="sxs-lookup"><span data-stu-id="df981-120">When all transactions have been recorded on the project and you don't expect any more to be logged, you can manually set the stage to **Close**.</span></span> <span data-ttu-id="df981-121">Когато проектът е настроен на **Затворен**, не можете да регистрирате повече транзакции по проекта и проектът ще е само за четене.</span><span class="sxs-lookup"><span data-stu-id="df981-121">When the project is set to **Close**, you can’t log any more transactions on the project and the project will be read only.</span></span>           |

## <a name="to-track-a-projects-status"></a><span data-ttu-id="df981-122">За проследяване на състоянието на проект</span><span class="sxs-lookup"><span data-stu-id="df981-122">To track a project’s status</span></span>  

1.  <span data-ttu-id="df981-123">Отидете на **Project Service > Проекти**.</span><span class="sxs-lookup"><span data-stu-id="df981-123">Go to **Project Service > Projects**.</span></span>  

2.  <span data-ttu-id="df981-124">Щракнете върху проекта, върху който искате да работите.</span><span class="sxs-lookup"><span data-stu-id="df981-124">Click the project you want to work on.</span></span>  

3.  <span data-ttu-id="df981-125">В лентата в горната част на екрана изберете стрелката за падащо меню до името на проекта и след това щракнете върху **Проследяване на проект**.</span><span class="sxs-lookup"><span data-stu-id="df981-125">In the bar across the top of the screen, select the down arrow next to the project name, and then click **Project Tracking**.</span></span>  

4.  <span data-ttu-id="df981-126">Изберете **Проследяване на усилията** или **Проследяване на разходите** в падащия списък над списъка със задачи.</span><span class="sxs-lookup"><span data-stu-id="df981-126">Select **Effort Tracking** or **Cost Tracking** in the drop-down list above the task list.</span></span>  

5.  <span data-ttu-id="df981-127">Щракнете двукратно върху задача, за да я редактирате.</span><span class="sxs-lookup"><span data-stu-id="df981-127">Double-click any task to edit it.</span></span> <span data-ttu-id="df981-128">Можете също да преместите или преоразмерите стълбовете в диаграмата на Гант, за да промените времето и напредъка за дадена задача.</span><span class="sxs-lookup"><span data-stu-id="df981-128">You can also move or resize the bars in the Gantt chart to change the time and progress for a task.</span></span>  

### <a name="see-also"></a><span data-ttu-id="df981-129">Вижте също</span><span class="sxs-lookup"><span data-stu-id="df981-129">See Also</span></span>  
 [<span data-ttu-id="df981-130">Ръководство за мениджъри на проекти</span><span class="sxs-lookup"><span data-stu-id="df981-130">Project Manager Guide</span></span>](../project-service/project-manager-guide.md)
