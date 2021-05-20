---
title: Разработване на шаблони за проекти с копирането на проект
description: Тази тема предоставя информация за това как да създадете шаблони за проекти с помощта на персонализираното действие Копиране на проект.
author: stsporen
manager: Annbe
ms.date: 01/21/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cc17df0c73b276048f7c4b04bd9dc6644e828dc0
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949801"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="e1085-103">Разработване на шаблони за проекти с копирането на проект</span><span class="sxs-lookup"><span data-stu-id="e1085-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="e1085-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="e1085-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="e1085-105">Dynamics 365 Project Operations поддържа възможността за копиране на проект и връщане на всички присвоявания към общите ресурси, които представляват ролята.</span><span class="sxs-lookup"><span data-stu-id="e1085-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="e1085-106">Клиентите могат да използват тази функционалност за изграждане на основни шаблони за проекти.</span><span class="sxs-lookup"><span data-stu-id="e1085-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="e1085-107">Когато изберете **Копиране на проект**, състоянието на целевия проект се актуализира.</span><span class="sxs-lookup"><span data-stu-id="e1085-107">When you select **Copy Project**, the status of the target project is updated.</span></span> <span data-ttu-id="e1085-108">Използвайте **описание на състоянието**, за да определите кога действието за копиране е завършено.</span><span class="sxs-lookup"><span data-stu-id="e1085-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="e1085-109">Избиране **Копиране на проект** също актуализира началната дата на проекта до текущата начална дата, ако в обекта на целевия проект не е открита целева дата.</span><span class="sxs-lookup"><span data-stu-id="e1085-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="e1085-110">Копирайте персонализираното действие на проекта</span><span class="sxs-lookup"><span data-stu-id="e1085-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="e1085-111">Име</span><span class="sxs-lookup"><span data-stu-id="e1085-111">Name</span></span> 

<span data-ttu-id="e1085-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="e1085-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="e1085-113">Входни параметри</span><span class="sxs-lookup"><span data-stu-id="e1085-113">Input parameters</span></span>
<span data-ttu-id="e1085-114">Има три входящи параметри:</span><span class="sxs-lookup"><span data-stu-id="e1085-114">There are three input parameters:</span></span>

| <span data-ttu-id="e1085-115">Параметър</span><span class="sxs-lookup"><span data-stu-id="e1085-115">Parameter</span></span>          | <span data-ttu-id="e1085-116">Тип</span><span class="sxs-lookup"><span data-stu-id="e1085-116">Type</span></span>   | <span data-ttu-id="e1085-117">Стойности</span><span class="sxs-lookup"><span data-stu-id="e1085-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="e1085-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="e1085-118">ProjectCopyOption</span></span>  | <span data-ttu-id="e1085-119">String</span><span class="sxs-lookup"><span data-stu-id="e1085-119">String</span></span> | <span data-ttu-id="e1085-120">**{"removeNamedResources":true}** или **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="e1085-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="e1085-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="e1085-121">SourceProject</span></span>      | <span data-ttu-id="e1085-122">Препратка към обект</span><span class="sxs-lookup"><span data-stu-id="e1085-122">Entity Reference</span></span> | <span data-ttu-id="e1085-123">Изходен проект</span><span class="sxs-lookup"><span data-stu-id="e1085-123">Source Project</span></span> |
| <span data-ttu-id="e1085-124">Цел</span><span class="sxs-lookup"><span data-stu-id="e1085-124">Target</span></span>             | <span data-ttu-id="e1085-125">Препратка към обект</span><span class="sxs-lookup"><span data-stu-id="e1085-125">Entity Reference</span></span> | <span data-ttu-id="e1085-126">Целеви проект</span><span class="sxs-lookup"><span data-stu-id="e1085-126">Target Project</span></span> |


- <span data-ttu-id="e1085-127">**{"clearTeamsAndAssignments":true}**: Поведението по подразбиране за проект за мрежата и ще премахне всички задания и членове на екипа.</span><span class="sxs-lookup"><span data-stu-id="e1085-127">**{"clearTeamsAndAssignments":true}**: Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="e1085-128">**{"removeNamedResources":true}** Поведението по подразбиране за Project Operations и ще върне заданията към общи ресурси.</span><span class="sxs-lookup"><span data-stu-id="e1085-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="e1085-129">За повече стойности по подразбиране за действия вижте [Използване на действия на Web API](/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="e1085-129">For more defaults on actions, see [Use Web API actions](/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="e1085-130">Посочете полета за копиране</span><span class="sxs-lookup"><span data-stu-id="e1085-130">Specify fields to copy</span></span> 
<span data-ttu-id="e1085-131">Когато се извика действието, **Копиране на проект** ще разгледа изгледа на проекта **Копиране на колони на проекта**, за да определите кои полета да копирате при копиране на проекта.</span><span class="sxs-lookup"><span data-stu-id="e1085-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>


### <a name="example"></a><span data-ttu-id="e1085-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e1085-132">Example</span></span>
<span data-ttu-id="e1085-133">Следващият пример показва как да извикате **CopyProject** персонализирано действие с набор от параметри **removeNamedResources**.</span><span class="sxs-lookup"><span data-stu-id="e1085-133">The following example shows how to call the **CopyProject** custom action with the **removeNamedResources** parameter set.</span></span>
```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

    [DataContract]
    public class ProjectCopyOption
    {
        /// <summary>
        /// Clear teams and assignments.
        /// </summary>
        [DataMember(Name = "clearTeamsAndAssignments")]
        public bool ClearTeamsAndAssignments { get; set; }

        /// <summary>
        /// Replace named resource with generic resource.
        /// </summary>
        [DataMember(Name = "removeNamedResources")]
        public bool ReplaceNamedResources { get; set; }
    }

    public class CopyProjectSample
    {
        private IOrganizationService organizationService;

        public CopyProjectSample(IOrganizationService organizationService)
        {
            this.organizationService = organizationService;
        }

        public void SampleRun()
        {
            // Example source project GUID
            Guid sourceProjectId = new Guid("11111111-1111-1111-1111-111111111111");
            var sourceProject = new Entity("msdyn_project", sourceProjectId);

            Entity targetProject = new Entity("msdyn_project");
            targetProject["msdyn_subject"] = "Example Project";
            targetProject.Id = organizationService.Create(targetProject);

            ProjectCopyOption copyOption = new ProjectCopyOption();
            copyOption.ReplaceNamedResources = true;

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, ProjectCopyOption projectCopyOption)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV2");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;
            req["ProjectCopyOption"] = JsonConvert.SerializeObject(projectCopyOption);
            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```


[!INCLUDE[footer-include](../includes/footer-banner.md)]