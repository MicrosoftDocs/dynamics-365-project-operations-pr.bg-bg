---
title: Разработване на шаблони за проекти с копирането на проект
description: Тази тема предоставя информация за това как да създадете шаблони за проекти с помощта на персонализираното действие Копиране на проект.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 0100c29873be6346614e958ef6ea0c77da2c9590
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131600"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="ac78b-103">Разработване на шаблони за проекти с копирането на проект</span><span class="sxs-lookup"><span data-stu-id="ac78b-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="ac78b-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="ac78b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ac78b-105">Dynamics 365 Project Operations поддържа възможността за копиране на проект и връщане на всички задания обратно към общите ресурси, които представляват ролята.</span><span class="sxs-lookup"><span data-stu-id="ac78b-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="ac78b-106">Клиентите могат да използват тази функционалност за изграждане на основни шаблони за проекти.</span><span class="sxs-lookup"><span data-stu-id="ac78b-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="ac78b-107">Когато изберете **Копиране на проект**, състоянието на целевия проект се актуализира.</span><span class="sxs-lookup"><span data-stu-id="ac78b-107">When you select **Copy Project**, the status of the target project is updated.</span></span> <span data-ttu-id="ac78b-108">Използвайте **описание на състоянието**, за да определите кога действието за копиране е завършено.</span><span class="sxs-lookup"><span data-stu-id="ac78b-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="ac78b-109">Избиране **Копиране на проект** също актуализира началната дата на проекта до текущата начална дата, ако в обекта на целевия проект не е открита целева дата.</span><span class="sxs-lookup"><span data-stu-id="ac78b-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="ac78b-110">Копирайте персонализираното действие на проекта</span><span class="sxs-lookup"><span data-stu-id="ac78b-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="ac78b-111">Име</span><span class="sxs-lookup"><span data-stu-id="ac78b-111">Name</span></span> 

<span data-ttu-id="ac78b-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="ac78b-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="ac78b-113">Входни параметри</span><span class="sxs-lookup"><span data-stu-id="ac78b-113">Input parameters</span></span>
<span data-ttu-id="ac78b-114">Има три входящи параметри:</span><span class="sxs-lookup"><span data-stu-id="ac78b-114">There are three input parameters:</span></span>

| <span data-ttu-id="ac78b-115">Параметър</span><span class="sxs-lookup"><span data-stu-id="ac78b-115">Parameter</span></span>          | <span data-ttu-id="ac78b-116">Тип</span><span class="sxs-lookup"><span data-stu-id="ac78b-116">Type</span></span>   | <span data-ttu-id="ac78b-117">Стойности</span><span class="sxs-lookup"><span data-stu-id="ac78b-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="ac78b-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="ac78b-118">ProjectCopyOption</span></span>  | <span data-ttu-id="ac78b-119">String</span><span class="sxs-lookup"><span data-stu-id="ac78b-119">String</span></span> | <span data-ttu-id="ac78b-120">**{"removeNamedResources":true}** или **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="ac78b-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="ac78b-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="ac78b-121">SourceProject</span></span>      | <span data-ttu-id="ac78b-122">Препратка към обект</span><span class="sxs-lookup"><span data-stu-id="ac78b-122">Entity Reference</span></span> | <span data-ttu-id="ac78b-123">Изходен проект</span><span class="sxs-lookup"><span data-stu-id="ac78b-123">Source Project</span></span> |
| <span data-ttu-id="ac78b-124">Цел</span><span class="sxs-lookup"><span data-stu-id="ac78b-124">Target</span></span>             | <span data-ttu-id="ac78b-125">Препратка към обект</span><span class="sxs-lookup"><span data-stu-id="ac78b-125">Entity Reference</span></span> | <span data-ttu-id="ac78b-126">Целеви проект</span><span class="sxs-lookup"><span data-stu-id="ac78b-126">Target Project</span></span> |


- <span data-ttu-id="ac78b-127">**{"clearTeamsAndAssignments":true}**: Поведението по подразбиране за проект за мрежата и ще премахне всички задания и членове на екипа.</span><span class="sxs-lookup"><span data-stu-id="ac78b-127">**{"clearTeamsAndAssignments":true}**: Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="ac78b-128">**{"removeNamedResources":true}** Поведението по подразбиране за проектни операции и ще върне заданията към общи ресурси.</span><span class="sxs-lookup"><span data-stu-id="ac78b-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="ac78b-129">За повече стойности по подразбиране за действия вижте [Използване на действия на Web API](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="ac78b-129">For more defaults on actions, see [Use Web API actions](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="ac78b-130">Посочете полета за копиране</span><span class="sxs-lookup"><span data-stu-id="ac78b-130">Specify fields to copy</span></span> 
<span data-ttu-id="ac78b-131">Когато се извика действието, **Копиране на проект** ще разгледа изгледа на проекта **Копиране на колони на проекта**, за да определите кои полета да копирате при копиране на проекта.</span><span class="sxs-lookup"><span data-stu-id="ac78b-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>
