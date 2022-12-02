---
title: Разработване на шаблони за проекти с копирането на проект
description: Тази статия предоставя информация за това как да създадете шаблони за проекти с помощта на персонализираното действие Копиране на проект.
author: stsporen
ms.date: 03/10/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 47c1023bbc4c21e3571bffbf3670bf0f7854f81d
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923819"
---
# <a name="develop-project-templates-with-copy-project"></a>Разработване на шаблони за проекти с копирането на проект

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

Dynamics 365 Project Operations поддържа възможността за копиране на проект и връщане на всички присвоявания към общите ресурси, които представляват ролята. Клиентите могат да използват тази функционалност за изграждане на основни шаблони за проекти.

Когато изберете **Копиране на проект**, състоянието на целевия проект се актуализира. Използвайте **описание на състоянието**, за да определите кога действието за копиране е завършено. Избиране **Копиране на проект** също актуализира началната дата на проекта до текущата начална дата, ако в обекта на целевия проект не е открита целева дата.

## <a name="copy-project-custom-action"></a>Копирайте персонализираното действие на проекта

### <a name="name"></a>Име 

msdyn\_CopyProjectV3

### <a name="input-parameters"></a>Входни параметри

Има три входящи параметри:

- **ReplaceNamedResources** или **ClearTeamsAndAssignments** – Задайте само една от опциите. Не задавайте и двете.

    - **\{"ReplaceNamedResources":true\}** – Поведението по подразбиране за Project Operations. Всякакви наименувани ресурси се заменят с генерични ресурси.
    - **\{"ClearTeamsAndAssignments":true\}** – Поведението по подразбиране за Project for the Web. Всички задачи и членове на екипа се премахват.

- **SourceProject** – Обръщението към обекта на изходния проект, от който да копирате. Този параметър не може да бъде нула.
- **Target** – Обръщението към обекта на изходния проект, в който да копирате. Този параметър не може да бъде нула.

В следващата таблица е представено обобщение на трите параметъра.

| параметър                | Тип             | Стойност                 |
|--------------------------|------------------|-----------------------|
| ReplaceNamedResources    | Boolean          | **Вярно** или **невярно** |
| ClearTeamsAndAssignments | Boolean          | **Вярно** или **невярно** |
| SourceProject            | Препратка към обект | Изходният проект    |
| Цел                   | Препратка към обект | Целевият проект    |

За повече стойности по подразбиране за действия вижте [Използване на действия на Web API](/powerapps/developer/common-data-service/webapi/use-web-api-actions).

### <a name="validations"></a>Проверки

Извършват се следните валидации.

1. Null проверява и извлича изходния и целевия проекти, за да потвърди съществуването и на двата проекта в организацията.
2. Системата потвърждава, че целевият проект е валиден за копиране, като проверява следните условия:

    - Няма предишна дейност по проекта (включително избор на **Задачи** раздел) и проектът е новосъздаден.
    - Няма предишно копие, не е заявено импортиране на този проект и проектът няма състояние **Неуспешно**.

3. Операцията не се извиква чрез HTTP.

## <a name="specify-fields-to-copy"></a>Посочете полета за копиране

Когато се извика действието, **Копиране на проект** ще разгледа изгледа на проекта **Копиране на колони на проекта**, за да определите кои полета да копирате при копиране на проекта.

### <a name="example"></a>Пример

Следващият пример показва как да извикате **CopyProjectV3** персонализирано действие с набор от параметри **removeNamedResources**.

```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

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
            targetProject["msdyn_subject"] = "Example Project - Copy";
            targetProject.Id = organizationService.Create(targetProject);

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption, true, false);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, bool replaceNamedResources = true, bool clearTeamsAndAssignments = false)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV3");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;

            if (replaceNamedResources)
            {
                req["ReplaceNamedResources"] = true;
            }
            else
            {
                req["ClearTeamsAndAssignments"] = true;
            }

            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```

[!INCLUDE[footer-include](../includes/footer-banner.md)]
