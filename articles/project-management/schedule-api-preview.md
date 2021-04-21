---
title: Използвайте API на графика, за да извършвате операции с обекти за планиране
description: Тази тема предоставя информация и проби за използване на API за график.
author: sigitac
manager: Annbe
ms.date: 04/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a50a2c6220bb49de8146d0758019827e120e0526
ms.sourcegitcommit: 8ff9fe396db6dec581c21cd6bb9acc2691c815b0
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/07/2021
ms.locfileid: "5868116"
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
- API за график са в публичен преглед. Използването на тези API в производствена среда не се поддържа от Microsoft.

## <a name="sample-scenario"></a>Примерен сценарий

В този сценарий ще създадете проект, член на екип, четири задачи и две задания за ресурси. След това ще актуализирате една задача, ще актуализирате проекта, ще изтриете една задача, ще изтриете едно задание на ресурс и ще създадете зависимост от задачата.

```C#
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
var task4 = GetTask("4ZZ";, projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment"R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

varassignment1Response = CallPssCreateAction(assignment1, operationSetId);
varassignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

varassignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a>Допълнителни проби

```C#
#region Call actions 

///<summary>
/// Calls the action to create an operationSet
/// </summary>
/// <paramname="projectId">project id for the operations to be included in this operationSet>/param>
/// <paramname="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
privatestring CallCreateOperationSetAction(Guid projectId, string description)
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
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary<
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet Id</param>
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
/// <summary>
/// <paramname="recordId">Id of the record to be deleted</param>
/// <paramname="entityLogicalName">Entity logical name of the record</param>
/// <paramname="operationSetId">OperationSet Id</param>
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
/// <summary>
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1";
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);

    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <paramname="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
privatestring CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject><OperationSetResponse>
    ((string)orgResponse.Results["OperationSetResponse";]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet(";msdyn_project", "msdyn_name");
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
    task["msdyn_effort";] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
        task["new_custom1"] = "Just my test";
        task[";new_age"] = 98;
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
publicclassOperationSetResponse
{
    [DataMember(Name = "operationSetId")]
    public Guid OperationSetId { get; set; }

    [DataMember(Name = "operationSetDetailId")]
    public Guid OperationSetDetailId { get; set; }

    [DataMember(Name = "operationType")]
    publicstring OperationType { get; set; }

    [DataMember(Name = "recordId")]
    publicstring RecordId { get; set; }

    [DataMember(Name = "correlationId")]
    publicstring CorrelationId { get; set; }
}

#endregion
```
