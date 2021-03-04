---
title: Създаване на шаблон на проект
description: Как се създава шаблон на проект в Project Service
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
ms.openlocfilehash: efc404131208e1c971cb091cf174c1f4707552f0
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149350"
---
# <a name="create-a-project-template-project-service"></a><span data-ttu-id="6bb1f-103">Създаване на шаблон на проект (Project Service)</span><span class="sxs-lookup"><span data-stu-id="6bb1f-103">Create a project template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="6bb1f-104">Шаблоните за проекти ви спестяват време , ако компанията ви редовно наддава за подобни типове проекти.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-104">Project templates save you time if your company regularly bids on similar types of projects.</span></span> <span data-ttu-id="6bb1f-105">Те предоставят стандартен набор от роли и очаквани часове за тип проект.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-105">They provide a standard set of roles and estimated hours for a type of project.</span></span> <span data-ttu-id="6bb1f-106">Управителите на акаунти и управителите на проекти могат да създават проекти според шаблон на проект или могат да копирате шаблона и да го направят свой.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-106">Account managers and project managers can create projects based on a project template, or they can copy the template and make one of their own.</span></span>  
  
## <a name="components-of-project-template"></a><span data-ttu-id="6bb1f-107">Компоненти на шаблона на проект</span><span class="sxs-lookup"><span data-stu-id="6bb1f-107">Components of project template</span></span>
 <span data-ttu-id="6bb1f-108">Шаблонът на проект се състои от три компонента:</span><span class="sxs-lookup"><span data-stu-id="6bb1f-108">A project template consists of three components:</span></span>  
  
- <span data-ttu-id="6bb1f-109">**Съставна структура на работата**: Съставна структура на работата в шаблон на проект притежава същия набор от елементи както проекта.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-109">**Work breakdown structure**: A work breakdown structure in a project template has the same set of elements as in the project.</span></span> <span data-ttu-id="6bb1f-110">Можете да създадете йерархия на задачата, свържете роля към задача, определите атрибути на график, зададете зависимости и прегледате всички данни в диаграма на Гант.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-110">You can create a task hierarchy, associate roles to task, define schedule attributes, set dependencies and view all the data in the Gantt.</span></span> <span data-ttu-id="6bb1f-111">Съставна структура на работата в шаблоните за проекти поддържа и модели на задачи за всяка задача.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-111">The work breakdown structure in project templates also support task modes for each task.</span></span> <span data-ttu-id="6bb1f-112">Няма разлика между шаблон на проект и проект, когато създавате работен график.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-112">There is no difference between a project template and a project when creating work schedule.</span></span>  
  
- <span data-ttu-id="6bb1f-113">**Прогнози за проект**: Прогнозите за проект в шаблоните работят по същия начин както в проектите, освен ценовите листи, при които цените на разходи и продажби са тези, определени в параметрите [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="6bb1f-113">**Project estimates**: Project estimates in templates work the same way as they do in projects, except the price lists for defaulting the cost and sales prices are always the default cost and sales price lists defined in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] parameters.</span></span> <span data-ttu-id="6bb1f-114">Останалата част от функционалността е същата като в проект.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-114">The rest of the functionality is the same as in a project.</span></span>  
  
- <span data-ttu-id="6bb1f-115">**Формиране на екип за проект**: Когато формирате екип за проект за шаблон на проект, не можете да резервирате именуван ресурс в шаблон.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-115">**Project team formation**: When forming a project team for a project template, you can’t book a named resource in a template.</span></span> <span data-ttu-id="6bb1f-116">Можете да използвате **Генериране на екип за проект** в съставна структура на работата, за да генерирате набор от генерични ресурси.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-116">You can use **Generate Project Team** in the work breakdown structure to generate a set of generic resources.</span></span> <span data-ttu-id="6bb1f-117">Можете също да зададете необходимите умения и владеене за генерични ресурси.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-117">You can also specify required skills and proficiencies for generic resources.</span></span> <span data-ttu-id="6bb1f-118">Не можете да замените генеричен ресурс с наличен ресурс в шаблони на проект.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-118">You can’t substitute a generic resource with a bookable resource in project templates.</span></span>  
  
## <a name="create-a-project-from-a-template"></a><span data-ttu-id="6bb1f-119">Създаване на проект от шаблон</span><span class="sxs-lookup"><span data-stu-id="6bb1f-119">Create a project from a template</span></span>  
 <span data-ttu-id="6bb1f-120">Можете да създадете проект от шаблон по тези начини:</span><span class="sxs-lookup"><span data-stu-id="6bb1f-120">You can create a project from a template in these following ways:</span></span>  
  
-   <span data-ttu-id="6bb1f-121">При създаване на проект от офертата можете да изберете шаблон на проект във формуляра за бързо създаване на проект.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-121">When creating a project from the quote, you can choose a project template in the project quick create form.</span></span>  
  
-   <span data-ttu-id="6bb1f-122">При създаване на проект чрез щракване върху **Нов проект** формулярът на проекта се показва, преди да запишете записа.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-122">When creating a project by clicking **New Project**, the project form displays before you save the record.</span></span> <span data-ttu-id="6bb1f-123">От тук можете да щракнете върху полето **Избор на шаблон**, за да изберете от списък с предварително дефинирани шаблони на проекти във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-123">From here, you can click **Pick a template** field to choose from the list of pre-defined project templates in your organization.</span></span>  
  
-   <span data-ttu-id="6bb1f-124">Щракнете върху **Създаване на проект от шаблон** на страницата **Шаблон на проект**, за да създадете проект от шаблона.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-124">Click **Create project from a template** on the **Project Template** page to create a project from the template.</span></span>  
  
## <a name="copying-components-of-a-template-to-a-project"></a><span data-ttu-id="6bb1f-125">Копиране на компоненти от шаблон в проект</span><span class="sxs-lookup"><span data-stu-id="6bb1f-125">Copying components of a template to a project</span></span>  
 <span data-ttu-id="6bb1f-126">Когато копирате компоненти от шаблон в проект, има няколко неща, които трябва да знаете.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-126">When you copy components of a template into a project, there are a few things you should know about.</span></span>  
  
 <span data-ttu-id="6bb1f-127">**Копиране на съставна структура на работата**: Когато копирате съставна структура на работата от шаблон на проект, ако проектът има различен календар на проект от шаблона, работните часове от календара на проекта ще бъдат приложени към графика със задачи.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-127">**Copying a work breakdown structure**: When you copy the work breakdown structure from a project template, if the project has a different project calendar than the template, the work hours from the project’s calendar will be applied to the schedule of tasks.</span></span> <span data-ttu-id="6bb1f-128">Това настройва графика на вторичния календар на проект.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-128">This adjusts the schedule to the backing project calendar.</span></span> <span data-ttu-id="6bb1f-129">По подобен начин първата задача от съставна структура на работата заема началната дата на проекта, така че останалата част от графика за йерархия на задачите се актуализира на базата на времетраенето и зависимостите, посочени в съставната структура на работата на шаблона.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-129">Similarly, the first task on the work breakdown structure takes the project’s start date, so the rest of the task hierarchy schedule is updated based on the duration and dependencies specified in the template’s work breakdown structure.</span></span>  
  
 <span data-ttu-id="6bb1f-130">**Копиране на прогнози за проект**: Когато копирате през редове за прогнози на проекта, ценовите листи се актуализират въз основа на притежаващата проекта единица за ценовата листа на разходите и клиента за ценовата листа на продажбите.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-130">**Copying project estimates**: When you copy across project estimate lines, price lists are updated based on the owning unit of the project for the cost price list and customer for the sales price list.</span></span> <span data-ttu-id="6bb1f-131">Разходите на единица и продажните цени се определят от тези ценови листи по проекти, които са свързани към обект на продажба.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-131">The unit cost and sales prices are determined from these price lists on projects that are associated to a sales entity.</span></span>  
  
 <span data-ttu-id="6bb1f-132">**Копиране на екип на проект**: Когато копирате екипа на проект от шаблона на проекта, генеричните ресурси се копират, заедно с уменията и владеенето, дефинирани в шаблона.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-132">**Copying a project team**: When you copy the project team from the template to a project, the generic resources are copied across, along with the skills and proficiencies defined in the template.</span></span> <span data-ttu-id="6bb1f-133">Възлаганията на генерични ресурси се поддържат също както в шаблона на проект.</span><span class="sxs-lookup"><span data-stu-id="6bb1f-133">Generic resource assignments are also maintained as in the project template.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="6bb1f-134">Вижте също</span><span class="sxs-lookup"><span data-stu-id="6bb1f-134">See Also</span></span>  
 [<span data-ttu-id="6bb1f-135">Ръководство за мениджъри на проекти</span><span class="sxs-lookup"><span data-stu-id="6bb1f-135">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
