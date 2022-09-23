---
title: Използвайте API за график на проекти, за да извършвате операции с обекти за планиране
description: Тази статия предоставя информация и проби за използване на API за график на проекта.
author: sigitac
ms.date: 01/13/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 159d395efff98f2af780e5ed1e5ab3d6483cba89
ms.sourcegitcommit: b1c26ea57be721c5b0b1a33f2de0380ad102648f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/20/2022
ms.locfileid: "9541111"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>Използвайте API за график на проекти, за да извършвате операции с обекти за планиране

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_


**Обекти за планиране**

API за график на проекти предоставят възможност за извършване на операции по създаване, актуализиране и изтриване с **Обекти за планиране**. Тези обекти се управляват чрез механизма за планиране в Project for the web. Създавайте, актуализирайте и изтривайте операции с **Обекти за планиране** бяха ограничени в по-ранни издания на Dynamics 365 Project Operations.

Следващата таблица предоставя пълен списък на обектите от графика на проекта.

| **Име на обекта**         | **Логическо име на обект**     |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Задача по проект            | msdyn_projecttask           |
| Зависимост на задачи от проект | msdyn_projecttaskdependency |
| Назначаване на ресурс     | msdyn_resourceassignment    |
| Набор на проекта          | msdyn_projectbucket         |
| Член на екипа на проект     | msdyn_projectteam           |
| Контролни списъци на проекта      | msdyn_projectchecklist      |
| Етикет на проект           | msdyn_projectlabel          |
| Задача на проекта за етикетиране   | msdyn_projecttasktolabel    |
| Спринт на проект          | msdyn_projectsprint         |

**OperationSet**

OperationSet е модел на единица работа, който може да се използва, когато в рамките на една транзакция трябва да бъдат обработени няколко искания, засягащи графика.

**API на график на проект**

По-долу е даден списък на текущите API на график на проекта.

| **АПИ**                                 | Описание                                                                                                                       |
|-----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| **msdyn_CreateProjectV1**               | Този API се използва за създаване на проект. Проектът и кофата по подразбиране се създават незабавно.                         |
| **msdyn_CreateTeamMemberV1**            | Този API се използва за създаване на член на екипа на проекта. Записът на члена на екипа се създава незабавно.                                  |
| **msdyn_CreateOperationSetV1**          | Този API се използва за планиране на няколко заявки, които трябва да се извършват в рамките на транзакция.                                        |
| **msdyn_PssCreateV1**                   | Този API се използва за създаване на предприятие. Обектът може да бъде всеки от обектите за планиране на проекта, които поддържат операцията за създаване. |
| **msdyn_PssUpdateV1**                   | Този API се използва за актуализиране на предприятие. Предприятието може да бъде всяко от структурите за планиране на проекти, които поддържат операцията по актуализиране.  |
| **msdyn_PssDeleteV1**                   | Този API се използва за изтриване на предприятие. Обектът може да бъде всеки от обектите за планиране на проекта, които поддържат операцията за изтриване. |
| **msdyn_ExecuteOperationSetV1**         | Този API се използва за изпълнение на всички операции в рамките на дадения набор от операции.                                                 |
| **msdyn_PssUpdateResourceAssignmentV1** | Този API се използва за актуализиране на планиран работен контур за присвояване на ресурси.                                                        |



**Използване на API за график на проекти с OperationSet**

Защото записи с **CreateProjectV1** и **CreateTeamMemberV1** едновременно се създават незабавно, тези API не могат да се използват в **OperationSet** директно. Можете обаче да използвате API, за да създадете необходимите записи, да създадете **OperationSet** и след това използвайте тези предварително създадени записи в **OperationSet**.

**Поддържани операции**

| **Обект за планиране**   | **Създай** | **Актуализиране** | **Delete** | **Важни съображения**                                                                                                                                                                                                                                                                                                                            |
|-------------------------|------------|------------|------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Задача от проект            | Да        | Да        | Да        | Полетата "Напредък **,** усилия" и **"Усилия"** **могат** да бъдат редактирани в Project for the Web, но те не могат да бъдат редактирани в Project Operations.                                                                                                                                                                                             |
| Зависимост на задача от проект | Да        | No         | Да        | Записите на зависимостта на проектната задача не се актуализират. Вместо това може да бъде изтрит стар запис и може да се създаде нов запис.                                                                                                                                                                                                                                 |
| Назначаване на ресурс     | Да        | Да\*      | Да        | Не се поддържат операции със следните полета: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** и **PlannedWork**. Записите за възлагане на ресурси не се актуализират. Вместо това старият запис може да бъде изтрит и може да се създаде нов запис. Предоставен е отделен API за актуализиране на контурите за присвояване на ресурси. |
| Набор на проекта          | Да        | Да        | Да        | Кофата по подразбиране се създава с помощта на API CreateProjectV1 **.** Поддръжка за създаване и изтриване на кофи за проекти беше добавена в Update Release 16.                                                                                                                                                                                                   |
| Член на екипа на проект     | Да        | Да        | Да        | За операцията за създаване използвайте **CreateTeamMemberV1** API.                                                                                                                                                                                                                                                                                           |
| Project                 | Да        | Да        |            | Не се поддържат операции със следните полета: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** и **Duration**.                                                                                       |
| Контролни списъци на проекта      | Да        | Да        | Да        |                                                                                                                                                                                                                                                                                                                                                         |
| Етикет на проект           | No         | Да        | No         | Имената на етикетите могат да бъдат променени. Тази функция е достъпна само за Project for the Web                                                                                                                                                                                                                                                                      |
| Задача на проекта за етикетиране   | Да        | No         | Да        | Тази функция е достъпна само за Project for the Web                                                                                                                                                                                                                                                                                                  |
| Спринт на проект          | Да        | Да        | Да        | Стартовото **поле** трябва да има дата по-рано от **полето Finish**. Спринтовете за един и същ проект не могат да се припокриват един с друг. Тази функция е достъпна само за Project for the Web                                                                                                                                                                    |




Свойството ИД не е задължително. Ако е предоставено, системата се опитва да го използва и извежда изключение, ако не може да се използва. Ако не е предоставено, системата ще го генерира.

**Известни проблеми и ограничения**

Следва списък с ограничения и известни проблеми:

-   API за график на проекта могат да се използват само от **потребители с лиценз** за проект на Microsoft. Те не могат да бъдат използвани от:
    -   Потребители на приложение
    -   Системни потребители
    -   Потребители на интеграция
    -   Други потребители, които нямат необходимия лиценз
-   Всеки **OperationSet** може да има максимум 100 операции.
-   Всеки потребител може да има максимум 10 отворени **OperationSets**.
-   Понастоящем Project Operations поддържа максимум 500 общо задачи по проект.
-   Всяка операция за контур за присвояване на ресурси за актуализация се брои като една операция.
-   Всеки списък с актуализирани контури може да съдържа максимум 100 времеви резена.
-   Състоянието на неуспех **OperationSet** и регистрационните файлове за неуспех в момента не са достъпни.
-   Има максимум 400 спринтове на проект.
-   [Ограничения и граници на проекти и задачи](/project-for-the-web/project-for-the-web-limits-and-boundaries).
-   Етикетите в момента са достъпни само за Project for the Web.

**Грешка при обработването**

-   За да прегледате грешките, генерирани от операционните набори, отидете на **Настройки** \> **График на интеграция** \> **Набори от операции**.
-   За да прегледате грешките, генерирани от услугата за график на проекта, отидете на **Настройки** \> **График на интеграция** \> **Регистрационни файлове за грешки в PSS**.

**Редактиране на контури за присвояване на ресурси**

За разлика от всички други API за планиране на проекти, които актуализират предприятието, API за присвояване на ресурси е единствено отговорен за актуализациите на едно поле, msdyn_plannedwork, на едно предприятие, msydn_resourceassignment.

Даден режим на график е:

-   **Фиксирани единици**
-   календар на проекта е 9-5p е 9-5pst, Mon, Tue, Thurs, петък (БЕЗ РАБОТА СРЯДА)
-   и ресурсен календар е 9-1p PST Mon to Fri

Тази задача е за една седмица, четири часа на ден. Това е така, защото ресурсният календар е от 9-1 PST, или четири часа на ден.

| &nbsp;     | Задача | Начална дата | Крайна дата  | Количество | 6/13/2022 | 6/14/2022 | 6/15/2022 | 6/16/2022 | 6/17/2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| 9-1 работник |  Т1  | 6/13/2022  | 6/17/2022 | 20       | 4         | 4         | 4         | 4         | 4         |

Например, ако искате работникът да работи само три часа всеки ден тази седмица и да позволява един час за други задачи.

#### <a name="updatedcontours-sample-payload"></a>АктуализиранКонтури примерен полезен товар:

```json
[{

"minutes":900.0,

"start":"2022-06-13T00:00:00-07:00",

"end":"2022-06-18T00:00:00-07:00"

}]
```

Това е задачата, след като API за актуализиране на контурния график се изпълнява.

| &nbsp;     | Задача | Начална дата | Крайна дата  | Количество | 6/13/2022 | 6/14/2022 | 6/15/2022 | 6/16/2022 | 6/17/2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| 9-1 работник | Т1   | 6/13/2022  | 6/17/2022 | 15       | 3         | 3         | 3         | 3         | 3         |


**Примерен сценарий**

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

** Допълнителни проби

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
