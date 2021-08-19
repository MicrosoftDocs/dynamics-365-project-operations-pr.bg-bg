---
title: Разработване на шаблони за проекти с копирането на проект
description: Тази тема предоставя информация за това как да създадете шаблони за проекти с помощта на персонализираното действие Копиране на проект.
author: stsporen
ms.date: 01/21/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: d12301b4e7baabeb0f045f9a11d4695fc026339af3fa7650db7177c495c71e90
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/06/2021
ms.locfileid: "6989227"
---
# <a name="develop-project-templates-with-copy-project"></a>Разработване на шаблони за проекти с копирането на проект

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Dynamics 365 Project Operations поддържа възможността за копиране на проект и връщане на всички присвоявания към общите ресурси, които представляват ролята. Клиентите могат да използват тази функционалност за изграждане на основни шаблони за проекти.

Когато изберете **Копиране на проект**, състоянието на целевия проект се актуализира. Използвайте **описание на състоянието**, за да определите кога действието за копиране е завършено. Избиране **Копиране на проект** също актуализира началната дата на проекта до текущата начална дата, ако в обекта на целевия проект не е открита целева дата.

## <a name="copy-project-custom-action"></a>Копирайте персонализираното действие на проекта 

### <a name="name"></a>Име 

**msdyn_CopyProjectV2**

### <a name="input-parameters"></a>Входни параметри
Има три входящи параметри:

| Параметър          | Тип   | Стойности                                                   | 
|--------------------|--------|----------------------------------------------------------|
| ProjectCopyOption  | String | **{"removeNamedResources":true}** или **{"clearTeamsAndAssignments":true}** |
| SourceProject      | Препратка към обект | Изходен проект |
| Цел             | Препратка към обект | Целеви проект |


- **{"clearTeamsAndAssignments":true}**: Поведението по подразбиране за проект за мрежата и ще премахне всички задания и членове на екипа.
- **{"removeNamedResources":true}** Поведението по подразбиране за Project Operations и ще върне заданията към общи ресурси.

За повече стойности по подразбиране за действия вижте [Използване на действия на Web API](/powerapps/developer/common-data-service/webapi/use-web-api-actions)

## <a name="specify-fields-to-copy"></a>Посочете полета за копиране 
Когато се извика действието, **Копиране на проект** ще разгледа изгледа на проекта **Копиране на колони на проекта**, за да определите кои полета да копирате при копиране на проекта.


### <a name="example"></a>Пример
Следващият пример показва как да извикате **CopyProject** персонализирано действие с набор от параметри **removeNamedResources**.
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