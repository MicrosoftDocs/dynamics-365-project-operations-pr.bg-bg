---
title: Разработване на шаблони за проекти с копирането на проект
description: Тази статия предоставя информация за това как да създадете шаблони за проекти с помощта на персонализираното действие "Копиране на проект".
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

msdyn\_ CopyProjectV3

### <a name="input-parameters"></a>Входни параметри

Има три входящи параметри:

- **ReplaceNamedResources** или **ClearTeamsAndРазпределения** – Задайте само една от опциите. Не поставяй и двете.

    - **\{"ReplaceNamedResources":true\}** – Поведението по подразбиране за Операции по проекта. Всички наименувани ресурси се заменят с генерични ресурси.
    - **\{"ClearTeamsAndAssignments":true\}** – Поведението по подразбиране за Project за уеб. Всички задачи и членове на екипа се премахват.

- **SourceProject** – Препратката към обект на проекта източник, от който да копирате. Този параметър не може да е нищожна.
- **Цел** – Препратката към обекта на целевия проект, в която да копирате. Този параметър не може да е нищожна.

Следната таблица предоставя обобщение на трите параметъра.

| параметър                | Вид             | Value                 |
|--------------------------|------------------|-----------------------|
| ЗамениНаименованияРесурси    | Boolean          | **Вярно** или **невярно** |
| ClearTeamsИзадачи | Boolean          | **Вярно** или **невярно** |
| SourceProject            | Препратка към обект | Проектът източник    |
| Цел                   | Препратка към обект | Целевият проект    |

За повече по подразбиране за действия вижте [Използване на действия](/powerapps/developer/common-data-service/webapi/use-web-api-actions) на Web API.

### <a name="validations"></a>Потвърждаване

Правят се следните валидации.

1. Null проверява и извлича източника и целевите проекти, за да потвърди съществуването и на двата проекта в организацията.
2. Системата валидира, че целевият проект е валиден за копиране, като проверява следните условия:

    - В проекта няма предишна дейност (включително избор на **раздела Задачи**), а проектът е новосъздаен.
    - Няма предишно копие, в този проект не е поискано импортиране и проектът няма **състояние "Неуспешно** ".

3. Операцията не се извиква чрез HTTP.

## <a name="specify-fields-to-copy"></a>Посочете полета за копиране

Когато се извика действието, **Копиране на проект** ще разгледа изгледа на проекта **Копиране на колони на проекта**, за да определите кои полета да копирате при копиране на проекта.

### <a name="example"></a>Пример

Следният пример показва как да се обадите **на действие CopyProjectV3** по избор с **набора от параметри на removeNamedResources**.

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
