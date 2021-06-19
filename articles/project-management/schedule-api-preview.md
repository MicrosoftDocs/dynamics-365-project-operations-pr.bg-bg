---
title: Използвайте API на графика, за да извършвате операции с обекти за планиране
description: Тази тема предоставя информация и проби за използване на API за график.
author: sigitac
ms.date: 04/27/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4a032dc7bcbdf23fce3c3b2ca63c51d473bd8e26
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116784"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a>Използвайте API на графика, за да извършвате операции с обекти за планиране

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

> [!IMPORTANT] 
> Част или цялата функционалност, отбелязана в тази тема, е достъпна като част от версия за преглед. Съдържанието и функционалността подлежат на промяна. 

## <a name="scheduling-entities"></a>Обекти за планиране

Приложните програмни интерфейси (API) на графика предоставят възможност за извършване на операции по създаване, актуализиране и изтриване с **Обекти за планиране**. Тези обекти се управляват чрез механизма за планиране в Project for the web. Създавайте, актуализирайте и изтривайте операции с **Обекти за планиране** бяха ограничени в по-ранни издания на Dynamics 365 Project Operations.

Следващата таблица предоставя пълен списък на **Обекти за планиране**.

| Име на обекта  | Логическо име на обект |
| --- | --- |
| Project | msdyn_project |
| Задача по проект  | msdyn_projecttask  |
| Зависимост на задачи от проект  | msdyn_projecttaskdependency  |
| Назначаване на ресурс | msdyn_resourceassignment |
| Набор на проекта  | msdyn_projectbucket |
| Член на екипа на проект | msdyn_projectteam |

## <a name="operationset"></a>OperationSet

OperationSet е модел на единица работа, който може да се използва, когато в рамките на една транзакция трябва да бъдат обработени няколко искания, засягащи графика.

## <a name="schedule-apis"></a>Планиране на API

По-долу е даден списък на текущите API на график.

- **msdyn_CreateProjectV1**: Този API може да се използва за създаване на проект. Проектът и сегментът на проекта по подразбиране се създават незабавно.
- **msdyn_CreateTeamMemberV1**: Този API може да се използва за създаване на член на екип по проект. Записът на члена на екипа се създава незабавно.
- **msdyn_CreateOperationSetV1**: Този API може да се използва за планиране на няколко заявки, които трябва да бъдат изпълнени в рамките на транзакция.
- **msdyn_PSSCreateV1**: Този API може да се използва за създаване на обект. Обектът може да бъде всеки от обектите за планиране, които поддържат операцията за създаване.
- **msdyn_PSSUpdateV1**: Този API може да се използва за актуализиране на обект. Обектът може да бъде всеки от обектите за планиране, които поддържат операцията за актуализиране.
- **msdyn_PSSDeleteV1**: Този API може да се използва за изтриване на обект. Обектът може да бъде всеки от обектите за планиране, които поддържат операцията за изтриване.
- **msdyn_ExecuteOperationSetV1**: Този API се използва за изпълнение на всички операции в рамките на дадения набор от операции.

## <a name="using-schedule-apis-with-operationset"></a>Използване на API за график с OperationSet

Защото записи с **CreateProjectV1** и **CreateTeamMemberV1** едновременно се създават незабавно, тези API не могат да се използват в **OperationSet** директно. Можете обаче да използвате API, за да създадете необходимите записи, да създадете **OperationSet** и след това използвайте тези предварително създадени записи в **OperationSet**.

## <a name="supported-operations"></a>Поддържани операции

| Обект за планиране | Създай | Update | Delete | Важни съображения |
| --- | --- | --- | --- | --- |
Задача от проект | Да | Да | Да | Нищо |
| Зависимост на задача от проект | Да | Да | | Записите на зависимостта на проектната задача не се актуализират. Вместо това може да се изтрие стар запис и да се създаде нов. |
| Назначаване на ресурс | Да | Да | | Не се поддържат операции със следните полета: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** и **PlannedWork**. Записите за възлагане на ресурси не се актуализират. Вместо това може да се изтрие старият запис и да се създаде нов. |
| Набор на проекта | N/A | N/A | N/A | Кофата по подразбиране се създава с помощта на **CreateProjectV1** API. |
| Член на екипа на проект | Да | Да | Да | За операцията за създаване използвайте **CreateTeamMemberV1** API. |
| Project | Да | Да | N/A | Не се поддържат операции със следните полета: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** и **Duration**. |

Тези API могат да бъдат извикани с обекти на обекти, които включват персонализирани полета.

Свойството ИД не е задължително. Ако е предоставено, системата се опитва да го използва и извежда изключение, ако не може да се използва. Ако не е предоставено, системата ще го генерира.

## <a name="restricted-fields"></a>Ограничени полета

Следващите таблици определят полетата, за които е забранено да **Създават** и **Редактират**.

### <a name="project-task"></a>Задача от проект

| **Логическо име**                       | **Може да създава** | **Може да редактира**     |
|----------------------------------------|----------------|------------------|
| msdyn_actualcost                       | не             | не               |
| msdyn_actualcost_base                  | не             | не               |
| msdyn_actualend                        | не             | не               |
| msdyn_actualsales                      | не             | не               |
| msdyn_actualsales_base                 | не             | не               |
| msdyn_actualstart                      | не             | не               |
| msdyn_costatcompleteestimate           | не             | не               |
| msdyn_costatcompleteestimate_base      | не             | не               |
| msdyn_costconsumptionpercentage        | не             | не               |
| msdyn_effortcompleted                  | не             | не               |
| msdyn_effortestimateatcomplete         | не             | не               |
| msdyn_iscritical                       | не             | не               |
| msdyn_iscriticalname                   | не             | не               |
| msdyn_ismanual                         | не             | не               |
| msdyn_ismanualname                     | не             | не               |
| msdyn_ismilestone                      | не             | не               |
| msdyn_ismilestonename                  | не             | не               |
| msdyn_LinkStatus                       | не             | не               |
| msdyn_linkstatusname                   | не             | не               |
| msdyn_msprojectclientid                | не             | не               |
| msdyn_plannedcost                      | не             | не               |
| msdyn_plannedcost_base                 | не             | не               |
| msdyn_plannedsales                     | не             | не               |
| msdyn_plannedsales_base                | не             | не               |
| msdyn_pluginprocessingdata             | не             | не               |
| msdyn_progress                         | не             | не (да за P4W) |
| msdyn_remainingcost                    | не             | не               |
| msdyn_remainingcost_base               | не             | не               |
| msdyn_remainingsales                   | не             | не               |
| msdyn_remainingsales_base              | не             | не               |
| msdyn_requestedhours                   | не             | не               |
| msdyn_resourcecategory                 | не             | не               |
| msdyn_resourcecategoryname             | не             | не               |
| msdyn_resourceorganizationalunitid     | не             | не               |
| msdyn_resourceorganizationalunitidname | не             | не               |
| msdyn_salesconsumptionpercentage       | не             | не               |
| msdyn_salesestimateatcomplete          | не             | не               |
| msdyn_salesestimateatcomplete_base     | не             | не               |
| msdyn_salesvariance                    | не             | не               |
| msdyn_salesvariance_base               | не             | не               |
| msdyn_scheduleddurationminutes         | не             | не               |
| msdyn_scheduledend                     | не             | не               |
| msdyn_scheduledstart                   | не             | не               |
| msdyn_schedulevariance                 | не             | не               |
| msdyn_skipupdateestimateline           | не             | не               |
| msdyn_skipupdateestimatelinename       | не             | не               |
| msdyn_summary                          | не             | не               |
| msdyn_varianceofcost                   | не             | не               |
| msdyn_varianceofcost_base              | не             | не               |

### <a name="project-task-dependency"></a>Зависимост на задача от проект

| **Логическо име**              | **Може да създава** | **Може да редактира** |
|-------------------------------|----------------|--------------|
| msdyn_linktype                | не             | не           |
| msdyn_linktypename            | не             | не           |
| msdyn_predecessortask         | да            | не           |
| msdyn_predecessortaskname     | да            | не           |
| msdyn_project                 | да            | не           |
| msdyn_projectname             | да            | не           |
| msdyn_projecttaskdependencyid | да            | не           |
| msdyn_successortask           | да            | не           |
| msdyn_successortaskname       | да            | не           |

### <a name="resource-assignment"></a>Назначаване на ресурс

| **Логическо име**             | **Може да създава** | **Може да редактира** |
|------------------------------|----------------|--------------|
| msdyn_bookableresourceid     | да            | не           |
| msdyn_bookableresourceidname | да            | не           |
| msdyn_bookingstatusid        | не             | не           |
| msdyn_bookingstatusidname    | не             | не           |
| msdyn_committype             | не             | не           |
| msdyn_committypename         | не             | не           |
| msdyn_effort                 | не             | не           |
| msdyn_effortcompleted        | не             | не           |
| msdyn_effortremaining        | не             | не           |
| msdyn_finish                 | не             | не           |
| msdyn_plannedcost            | не             | не           |
| msdyn_plannedcost_base       | не             | не           |
| msdyn_plannedcostcontour     | не             | не           |
| msdyn_plannedsales           | не             | не           |
| msdyn_plannedsales_base      | не             | не           |
| msdyn_plannedsalescontour    | не             | не           |
| msdyn_plannedwork            | не             | не           |
| msdyn_projectid              | да            | не           |
| msdyn_projectidname          | не             | не           |
| msdyn_projectteamid          | не             | не           |
| msdyn_projectteamidname      | не             | не           |
| msdyn_start                  | не             | не           |
| msdyn_taskid                 | не             | не           |
| msdyn_taskidname             | не             | не           |
| msdyn_userresourceid         | не             | не           |

### <a name="project-team-member"></a>Член на екипа на проект

| **Логическо име**                                 | **Може да създава** | **Може да редактира** |
|--------------------------------------------------|----------------|--------------|
| msdyn_calendarid                                 | не             | не           |
| msdyn_creategenericteammemberwithrequirementname | не             | не           |
| msdyn_deletestatus                               | не             | не           |
| msdyn_deletestatusname                           | не             | не           |
| msdyn_effort                                     | не             | не           |
| msdyn_effortcompleted                            | не             | не           |
| msdyn_effortremaining                            | не             | не           |
| msdyn_finish                                     | не             | не           |
| msdyn_hardbookedhours                            | не             | не           |
| msdyn_hours                                      | не             | не           |
| msdyn_markedfordeletiontimer                     | не             | не           |
| msdyn_markedfordeletiontimestamp                 | не             | не           |
| msdyn_msprojectclientid                          | не             | не           |
| msdyn_percentage                                 | не             | не           |
| msdyn_requiredhours                              | не             | не           |
| msdyn_softbookedhours                            | не             | не           |
| msdyn_start                                      | не             | не           |

### <a name="project"></a>Project

| **Логическо име**                       | **Може да създава** | **Може да редактира** |
|----------------------------------------|----------------|--------------|
| msdyn_actualexpensecost                | не             | не           |
| msdyn_actualexpensecost_base           | не             | не           |
| msdyn_actuallaborcost                  | не             | не           |
| msdyn_actuallaborcost_base             | не             | не           |
| msdyn_actualsales                      | не             | не           |
| msdyn_actualsales_base                 | не             | не           |
| msdyn_contractlineproject              | да            | не           |
| msdyn_contractorganizationalunitid     | да            | не           |
| msdyn_contractorganizationalunitidname | да            | не           |
| msdyn_costconsumption                  | не             | не           |
| msdyn_costestimateatcomplete           | не             | не           |
| msdyn_costestimateatcomplete_base      | не             | не           |
| msdyn_costvariance                     | не             | не           |
| msdyn_costvariance_base                | не             | не           |
| msdyn_duration                         | не             | не           |
| msdyn_effort                           | не             | не           |
| msdyn_effortcompleted                  | не             | не           |
| msdyn_effortestimateatcompleteeac      | не             | не           |
| msdyn_effortremaining                  | не             | не           |
| msdyn_finish                           | да            | да          |
| msdyn_globalrevisiontoken              | не             | не           |
| msdyn_islinkedtomsprojectclient        | не             | не           |
| msdyn_islinkedtomsprojectclientname    | не             | не           |
| msdyn_linkeddocumenturl                | не             | не           |
| msdyn_msprojectdocument                | не             | не           |
| msdyn_msprojectdocumentname            | не             | не           |
| msdyn_plannedexpensecost               | не             | не           |
| msdyn_plannedexpensecost_base          | не             | не           |
| msdyn_plannedlaborcost                 | не             | не           |
| msdyn_plannedlaborcost_base            | не             | не           |
| msdyn_plannedsales                     | не             | не           |
| msdyn_plannedsales_base                | не             | не           |
| msdyn_progress                         | не             | не           |
| msdyn_remainingcost                    | не             | не           |
| msdyn_remainingcost_base               | не             | не           |
| msdyn_remainingsales                   | не             | не           |
| msdyn_remainingsales_base              | не             | не           |
| msdyn_replaylogheader                  | не             | не           |
| msdyn_salesconsumption                 | не             | не           |
| msdyn_salesestimateatcompleteeac       | не             | не           |
| msdyn_salesestimateatcompleteeac_base  | не             | не           |
| msdyn_salesvariance                    | не             | не           |
| msdyn_salesvariance_base               | не             | не           |
| msdyn_scheduleperformance              | не             | не           |
| msdyn_scheduleperformancename          | не             | не           |
| msdyn_schedulevariance                 | не             | не           |
| msdyn_taskearlieststart                | не             | не           |
| msdyn_teamsize                         | не             | не           |
| msdyn_teamsize_date                    | не             | не           |
| msdyn_teamsize_state                   | не             | не           |
| msdyn_totalactualcost                  | не             | не           |
| msdyn_totalactualcost_base             | не             | не           |
| msdyn_totalplannedcost                 | не             | не           |
| msdyn_totalplannedcost_base            | не             | не           |


## <a name="limitations-and-known-issues"></a>Известни проблеми и ограничения
Следва списък с ограничения и известни проблеми:

- API на графика може да се използва само от **Потребители с лиценз за Microsoft Project.** Те не могат да бъдат използвани от:
    - Потребители на приложение
    - Системни потребители
    - Потребители на интеграция
    - Други потребители, които нямат необходимия лиценз
- Всеки **OperationSet** може да има максимум 100 операции.
- Всеки потребител може да има максимум 10 отворени **OperationSets**.
- Понастоящем Project Operations поддържа максимум 500 общо задачи по проект.
- Състоянието на неуспех **OperationSet** и регистрационните файлове за неуспех в момента не са достъпни.
- [Граници и ограничения на проекти и задачи](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a>Грешка при обработването

   - За да прегледате грешките, генерирани от операционните набори, отидете на **Настройки** \> **График на интеграция** \> **Набори от операции**.
   - За да прегледате грешките, генерирани от услугата за планиране на проекти, отидете на **Настройки** \> **График на интеграция** \> **Регистрационни файлове за грешки в PSS**.

## <a name="sample-scenario"></a>Примерен сценарий

В този сценарий ще създадете проект, член на екип, четири задачи и две задания за ресурси. След това ще актуализирате една задача, ще актуализирате проекта, ще изтриете една задача, ще изтриете едно задание на ресурс и ще създадете зависимост от задачата.

```csharp
Entity project = CreateProject();
project.Id = CallCreateProjectAction(project);
var projectReference = project.ToEntityReference();

var teamMember = new Entity("msdyn_projectteam", Guid.NewGuid());
teamMember["msdyn_name"] = $"TM {DateTime.Now.ToShortTimeString()}";
teamMember["msdyn_project"] = projectReference;
var createTeamMemberResponse = CallCreateTeamMemberAction(teamMember);

var description = $"My demo {DateTime.Now.ToShortTimeString()}";
var operationSetId = CallCreateOperationSetAction(project.Id, description);

var task1 = GetTask("1WW", projectReference);
var task2 = GetTask("2XX", projectReference, task1.ToEntityReference());
var task3 = GetTask("3YY", projectReference);
var task4 = GetTask("4ZZ", projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment("R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

var assignment1Response = CallPssCreateAction(assignment1, operationSetId);
var assignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

var assignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a>Допълнителни проби

```csharp
#region Call actions --- Sample code ----

/// <summary>
/// Calls the action to create an operationSet
/// </summary>
/// <param name="projectId">project id for the operations to be included in this operationSet</param>
/// <param name="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
private string CallCreateOperationSetAction(Guid projectId, string description)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_CreateOperationSetV1");
    operationSetRequest["ProjectId"] = projectId.ToString();
    operationSetRequest["Description"] = description;
    OrganizationResponse response = organizationService.Execute(operationSetRequest);
    return response["OperationSetId"].ToString();
}

/// <summary>
/// Calls the action to create an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>

private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssUpdateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssUpdateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="recordId">Id of the record to be deleted</param>
/// <param name="entityLogicalName">Entity logical name of the record</param>
/// <param name="operationSetId">OperationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssDeleteAction(string recordId, string entityLogicalName, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssDeleteV1");
    operationSetRequest["RecordId"] = recordId;
    operationSetRequest["EntityLogicalName"] = entityLogicalName;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to execute requests in an operationSet
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallExecuteOperationSetAction(string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_ExecuteOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// This can be used to abandon an operationSet that is no longer needed
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
protected OperationSetResponse CallAbandonOperationSetAction(Guid operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_AbandonOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId.ToString();
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}


/// <summary>
/// Calls the action to create a new project
/// </summary>
/// <param name="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1");
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);
    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <param name="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
private string CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject<OperationSetResponse>((string)orgResponse.Results["OperationSetResponse"]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet("msdyn_project", "msdyn_name");
    var getDefaultBucket = new QueryExpression("msdyn_projectbucket")
    {
        ColumnSet = columnsToFetch,
        Criteria =
        {
            Conditions =
            {
                new ConditionExpression("msdyn_project", ConditionOperator.Equal, projectReference.Id),
                new ConditionExpression("msdyn_name", ConditionOperator.Equal, "Bucket 1")
            }
        }
    };

    return organizationService.RetrieveMultiple(getDefaultBucket);
}

private Entity GetBucket(EntityReference projectReference)
{
    var bucketCollection = GetDefaultBucket(projectReference);
    if (bucketCollection.Entities.Count > 0)
    {
        return bucketCollection[0].ToEntity<Entity>();
    }

    throw new Exception($"Please open project with id {projectReference.Id} in the Dynamics UI and navigate to the Tasks tab");
}

private Entity CreateProject()
{
    var project = new Entity("msdyn_project", Guid.NewGuid());
    project["msdyn_subject"] = $"Proj {DateTime.Now.ToShortTimeString()}";

    return project;
}



private Entity GetTask(string name, EntityReference projectReference, EntityReference parentReference = null)
{
    var task = new Entity("msdyn_projecttask", Guid.NewGuid());
    task["msdyn_project"] = projectReference;
    task["msdyn_subject"] = name;
    task["msdyn_effort"] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
    task["new_custom1"] = "Just my test";
    task["new_age"] = 98;
    task["new_amount"] = 591.34m;
    task["new_isready"] = new OptionSetValue(100000000);
    */

    if (parentReference == null)
    {
        task["msdyn_outlinelevel"] = 1;
    }
    else
    {
        task["msdyn_parenttask"] = parentReference;
    }

    return task;
}

private Entity GetResourceAssignment(string name, Entity teamMember, Entity task, Entity project)
{
    var assignment = new Entity("msdyn_resourceassignment", Guid.NewGuid());
    assignment["msdyn_projectteamid"] = teamMember.ToEntityReference();
    assignment["msdyn_taskid"] = task.ToEntityReference();
    assignment["msdyn_projectid"] = project.ToEntityReference();
    assignment["msdyn_name"] = name;
    assignment["msdyn_start"] = DateTime.Now;
    assignment["msdyn_finish"] = DateTime.Now;

    return assignment;
}

protected Entity GetTaskDependency(Entity project, Entity predecessor, Entity successor)
{
    var taskDependency = new Entity("msdyn_projecttaskdependency", Guid.NewGuid());
    taskDependency["msdyn_project"] = project.ToEntityReference();
    taskDependency["msdyn_predecessortask"] = predecessor.ToEntityReference();
    taskDependency["msdyn_successortask"] = successor.ToEntityReference();
    taskDependency["msdyn_linktype"] = new OptionSetValue(192350000);

    return taskDependency;
}

#endregion


#region OperationSetResponse DataContract --- Sample code ----

[DataContract]
public class OperationSetResponse
{
[DataMember(Name = "operationSetId")]
public Guid OperationSetId { get; set; }

[DataMember(Name = "operationSetDetailId")]
public Guid OperationSetDetailId { get; set; }

[DataMember(Name = "operationType")]
public string OperationType { get; set; }

[DataMember(Name = "recordId")]
public string RecordId { get; set; }

[DataMember(Name = "correlationId")]
public string CorrelationId { get; set; }
}

#endregion
```
