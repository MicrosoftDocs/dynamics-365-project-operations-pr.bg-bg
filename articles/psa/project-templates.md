---
title: Шаблони на проекти
description: Тази тема предоставя информация как да използвате шаблоните за проекти за бърза настройка на проекти.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: bedcbc76d932a81e0c78bb58ce6a161446a26dde
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998263"
---
# <a name="project-templates"></a><span data-ttu-id="255da-103">Шаблони на проекти</span><span class="sxs-lookup"><span data-stu-id="255da-103">Project templates</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="255da-104">Шаблонът на проект е предварително дефинирана рамка, която ви помага бързо и лесно да стартирате проект.</span><span class="sxs-lookup"><span data-stu-id="255da-104">A project template is a predefined framework that helps you quickly and easily start a project.</span></span> <span data-ttu-id="255da-105">Можете да използвате предварително зададен шаблон, за да създадете нов проект с едно щракване.</span><span class="sxs-lookup"><span data-stu-id="255da-105">You can use a predefined template to create a new project with a single click.</span></span> <span data-ttu-id="255da-106">Що се отнася до проектите, трябва да дефинирате предварителните изисквания за шаблоните на проекти.</span><span class="sxs-lookup"><span data-stu-id="255da-106">As for projects, you must define the prerequisites for project templates.</span></span> <span data-ttu-id="255da-107">Трябва да дефинирате календар на проект за всеки шаблон на проект, а ролите и ценовите листи трябва да са предварително дефинирани в организацията, така че компонентите на шаблона да имат полезни данни.</span><span class="sxs-lookup"><span data-stu-id="255da-107">You must define a project calendar for each project template, and roles and price lists must be predefined in the organization, so that the components of the template have useful data.</span></span>

<span data-ttu-id="255da-108">Шаблонът на проект се състои от три компонента: график, прогнозни оценки на проект и членове на екипа на проект.</span><span class="sxs-lookup"><span data-stu-id="255da-108">A project template consists of three components: a schedule, project estimates, and project team members.</span></span>

## <a name="schedule"></a><span data-ttu-id="255da-109">График</span><span class="sxs-lookup"><span data-stu-id="255da-109">Schedule</span></span>

<span data-ttu-id="255da-110">График в шаблон на проект има същия набор от елементи като график в проект.</span><span class="sxs-lookup"><span data-stu-id="255da-110">A schedule in a project template has the same set of elements as a schedule in a project.</span></span> <span data-ttu-id="255da-111">Можете да създавате йерархия на задачите, да свързвате роли със задачи, да дефинирате атрибути на графика и да задавате зависимости.</span><span class="sxs-lookup"><span data-stu-id="255da-111">You can create a task hierarchy, associate roles with tasks, define schedule attributes, and set dependencies.</span></span> <span data-ttu-id="255da-112">График в шаблон на проект поддържа също режими на задача за всяка задача.</span><span class="sxs-lookup"><span data-stu-id="255da-112">A schedule in a project template also supports task modes for each task.</span></span> <span data-ttu-id="255da-113">Затова той поддържа инструмента за планиране.</span><span class="sxs-lookup"><span data-stu-id="255da-113">Therefore, it supports the scheduling engine.</span></span> <span data-ttu-id="255da-114">Трябва да свържете календар на проект с проекта.</span><span class="sxs-lookup"><span data-stu-id="255da-114">You must associate a project calendar with the project.</span></span> <span data-ttu-id="255da-115">Когато създавате работен график, няма разлика между шаблон на проект и проект.</span><span class="sxs-lookup"><span data-stu-id="255da-115">When you create a work schedule, there is no difference between a project template and a project.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="255da-116">Прогнозни оценки на проекта</span><span class="sxs-lookup"><span data-stu-id="255da-116">Project estimates</span></span>

<span data-ttu-id="255da-117">Прогнозните оценки на проект в шаблон на проект работят по същия начин като прогнозните оценки на проект в проект.</span><span class="sxs-lookup"><span data-stu-id="255da-117">Project estimates in a project template work the same way as project estimates in a project.</span></span> <span data-ttu-id="255da-118">Разходите и продажните цени обаче се извличат от ценовите листи за разходи и продажби по подразбиране, които са дефинирани в параметрите.</span><span class="sxs-lookup"><span data-stu-id="255da-118">However, the cost and sales prices are pulled from the default cost and sales price lists that are defined in the parameters.</span></span>

## <a name="creating-a-project-from-a-template"></a><span data-ttu-id="255da-119">Създаване на проект от шаблон</span><span class="sxs-lookup"><span data-stu-id="255da-119">Creating a project from a template</span></span>
 
<span data-ttu-id="255da-120">Има няколко начина за създаване на проект от шаблон:</span><span class="sxs-lookup"><span data-stu-id="255da-120">There are several ways to create a project from a project template:</span></span>

- <span data-ttu-id="255da-121">Когато създавате проект от оферта, можете да изберете шаблон на проект в диалоговия прозорец **Бързо създаване: проект**.</span><span class="sxs-lookup"><span data-stu-id="255da-121">When you create a project from a quote, you can select a project template in the **Quick Create: Project** dialog box.</span></span>

> ![Диалогов прозорец „Бързо създаване: проект“](media/project-11.png)

- <span data-ttu-id="255da-123">Когато създавате проект чрез избиране на **Нов проект**, страницата **Проект** се появява преди записът да бъде записан.</span><span class="sxs-lookup"><span data-stu-id="255da-123">When you create a project by selecting **New Project**, the **Project** page appears before the record is saved.</span></span> <span data-ttu-id="255da-124">В полето **Избор на шаблон** изберете един от предварително зададените шаблони на проекти в организацията.</span><span class="sxs-lookup"><span data-stu-id="255da-124">In the **Pick a Template** field, select one of the predefined project templates in the organization.</span></span>
- <span data-ttu-id="255da-125">Използвайте **Създаване на проект от шаблон** на страницата **Обект на шаблон**.</span><span class="sxs-lookup"><span data-stu-id="255da-125">Use **Create Project from a Template** on the **Template Entity** page.</span></span>

## <a name="copying-components-of-template-to-project"></a><span data-ttu-id="255da-126">Копиране на компоненти от шаблон в проект</span><span class="sxs-lookup"><span data-stu-id="255da-126">Copying components of template to project</span></span>

<span data-ttu-id="255da-127">Когато копирате компонентите на шаблон на проект в проект, могат да възникнат няколко замествания в зависимост от настройките в проекта.</span><span class="sxs-lookup"><span data-stu-id="255da-127">When you copy the components of a project template to a project, a few overrides can occur, depending on the settings in the project.</span></span>

### <a name="copying-the-schedule"></a><span data-ttu-id="255da-128">Копиране на графика</span><span class="sxs-lookup"><span data-stu-id="255da-128">Copying the schedule</span></span>

<span data-ttu-id="255da-129">Когато копирате графика от шаблон на проект, ако проектът има различен календар на проект от шаблона, работните часове от календара на проекта се прилагат към графика на задачите.</span><span class="sxs-lookup"><span data-stu-id="255da-129">When you copy the schedule from a project template, if the project has a different project calendar than the template, work hours from the project's calendar are applied to the task schedule.</span></span> <span data-ttu-id="255da-130">По този начин графикът се съобразява с поддържащия календар на проекта.</span><span class="sxs-lookup"><span data-stu-id="255da-130">In this way, the schedule is adjusted to match the backing project calendar.</span></span> <span data-ttu-id="255da-131">По подобен начин първата задача от графика заема началната дата на проекта, а графикът на останалата част от йерархията се актуализира на базата на продължителността и зависимостите, посочени в шаблона.</span><span class="sxs-lookup"><span data-stu-id="255da-131">Similarly, the first task on the schedule takes the project's start date, and the schedule of the rest of the hierarchy is updated based on the duration and dependencies that are specified in the template.</span></span> 

### <a name="copying-project-estimates"></a><span data-ttu-id="255da-132">Копиране на прогнозни оценки на проекта</span><span class="sxs-lookup"><span data-stu-id="255da-132">Copying project estimates</span></span> 

<span data-ttu-id="255da-133">Когато копирате в редовете за прогнозни оценки на проекта, ценовите листи се актуализират.</span><span class="sxs-lookup"><span data-stu-id="255da-133">When you copy across project estimate lines, the price lists are updated.</span></span> <span data-ttu-id="255da-134">За ценовата листа за разходи тези актуализации се базират на притежаващата единица на проекта.</span><span class="sxs-lookup"><span data-stu-id="255da-134">For the cost price list, these updates are based on the owning unit of the project.</span></span> <span data-ttu-id="255da-135">За ценовата листа за продажби те се базират на клиента.</span><span class="sxs-lookup"><span data-stu-id="255da-135">For the sales price list, they are based on the customer.</span></span> <span data-ttu-id="255da-136">За проекти, които са свързани с обект на продажби, разходите на единица и продажните цени се определят въз основа на тези ценови листи.</span><span class="sxs-lookup"><span data-stu-id="255da-136">For projects that are associated with a sales entity, the unit cost and sales prices are determined based on these price lists.</span></span>

### <a name="copying-a-project-team"></a><span data-ttu-id="255da-137">Копиране на екип на проект</span><span class="sxs-lookup"><span data-stu-id="255da-137">Copying a project team</span></span>

<span data-ttu-id="255da-138">Когато екип на проект се копира от шаблон на проект в проект, общите ресурси се копират заедно с уменията и опитностите, дефинирани в шаблона.</span><span class="sxs-lookup"><span data-stu-id="255da-138">When a project team is copied from a project template to a project, the generic resources are copied, together with the skills and proficiencies that are defined in the template.</span></span> <span data-ttu-id="255da-139">Присвояванията на общи ресурси се поддържат също както в шаблона на проект.</span><span class="sxs-lookup"><span data-stu-id="255da-139">Generic resource assignments are also maintained as they were in the project template.</span></span> <span data-ttu-id="255da-140">Наименувани ресурси не се поддържат в шаблоните на проекти.</span><span class="sxs-lookup"><span data-stu-id="255da-140">Named resources aren't supported in project templates.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]