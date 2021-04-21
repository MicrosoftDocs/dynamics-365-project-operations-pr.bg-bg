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
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="45308-103">Използвайте API на графика, за да извършвате операции с обекти за планиране</span><span class="sxs-lookup"><span data-stu-id="45308-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="45308-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="45308-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="45308-105">Част или цялата функционалност, отбелязана в тази тема, е достъпна като част от версия за преглед.</span><span class="sxs-lookup"><span data-stu-id="45308-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="45308-106">Съдържанието и функционалността подлежат на промяна.</span><span class="sxs-lookup"><span data-stu-id="45308-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="45308-107">Обекти за планиране</span><span class="sxs-lookup"><span data-stu-id="45308-107">Scheduling entities</span></span>

<span data-ttu-id="45308-108">Приложните програмни интерфейси (API) на графика предоставят възможност за извършване на операции по създаване, актуализиране и изтриване с **Обекти за планиране**.</span><span class="sxs-lookup"><span data-stu-id="45308-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="45308-109">Тези обекти се управляват чрез механизма за планиране в Project for the web.</span><span class="sxs-lookup"><span data-stu-id="45308-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="45308-110">Създавайте, актуализирайте и изтривайте операции с **Обекти за планиране** бяха ограничени в по-ранни издания на Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="45308-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="45308-111">Следващата таблица предоставя пълен списък на **Обекти за планиране**.</span><span class="sxs-lookup"><span data-stu-id="45308-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="45308-112">Име на обекта</span><span class="sxs-lookup"><span data-stu-id="45308-112">Entity name</span></span>  | <span data-ttu-id="45308-113">Логическо име на обект</span><span class="sxs-lookup"><span data-stu-id="45308-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="45308-114">Project</span><span class="sxs-lookup"><span data-stu-id="45308-114">Project</span></span> | <span data-ttu-id="45308-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="45308-115">msdyn_project</span></span> |
| <span data-ttu-id="45308-116">Задача по проект</span><span class="sxs-lookup"><span data-stu-id="45308-116">Project Task</span></span>  | <span data-ttu-id="45308-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="45308-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="45308-118">Зависимост на задачи от проект</span><span class="sxs-lookup"><span data-stu-id="45308-118">Project Task Dependency</span></span>  | <span data-ttu-id="45308-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="45308-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="45308-120">Назначаване на ресурс</span><span class="sxs-lookup"><span data-stu-id="45308-120">Resource Assignment</span></span> | <span data-ttu-id="45308-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="45308-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="45308-122">Набор на проекта</span><span class="sxs-lookup"><span data-stu-id="45308-122">Project Bucket</span></span>  | <span data-ttu-id="45308-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="45308-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="45308-124">Член на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="45308-124">Project Team Member</span></span> | <span data-ttu-id="45308-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="45308-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="45308-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="45308-126">OperationSet</span></span>

<span data-ttu-id="45308-127">OperationSet е модел на единица работа, който може да се използва, когато в рамките на една транзакция трябва да бъдат обработени няколко искания, засягащи графика.</span><span class="sxs-lookup"><span data-stu-id="45308-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="45308-128">Планиране на API</span><span class="sxs-lookup"><span data-stu-id="45308-128">Schedule APIs</span></span>

<span data-ttu-id="45308-129">По-долу е даден списък на текущите API на график.</span><span class="sxs-lookup"><span data-stu-id="45308-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="45308-130">**msdyn_CreateProjectV1**: Този API може да се използва за създаване на проект.</span><span class="sxs-lookup"><span data-stu-id="45308-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="45308-131">Проектът и сегментът на проекта по подразбиране се създават незабавно.</span><span class="sxs-lookup"><span data-stu-id="45308-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="45308-132">**msdyn_CreateTeamMemberV1**: Този API може да се използва за създаване на член на екип по проект.</span><span class="sxs-lookup"><span data-stu-id="45308-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="45308-133">Записът на члена на екипа се създава незабавно.</span><span class="sxs-lookup"><span data-stu-id="45308-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="45308-134">**msdyn_CreateOperationSetV1**: Този API може да се използва за планиране на няколко заявки, които трябва да бъдат изпълнени в рамките на транзакция.</span><span class="sxs-lookup"><span data-stu-id="45308-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="45308-135">**msdyn_PSSCreateV1**: Този API може да се използва за създаване на обект.</span><span class="sxs-lookup"><span data-stu-id="45308-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="45308-136">Обектът може да бъде всеки от обектите за планиране, които поддържат операцията за създаване.</span><span class="sxs-lookup"><span data-stu-id="45308-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="45308-137">**msdyn_PSSUpdateV1**: Този API може да се използва за актуализиране на обект.</span><span class="sxs-lookup"><span data-stu-id="45308-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="45308-138">Обектът може да бъде всеки от обектите за планиране, които поддържат операцията за актуализиране.</span><span class="sxs-lookup"><span data-stu-id="45308-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="45308-139">**msdyn_PSSDeleteV1**: Този API може да се използва за изтриване на обект.</span><span class="sxs-lookup"><span data-stu-id="45308-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="45308-140">Обектът може да бъде всеки от обектите за планиране, които поддържат операцията за изтриване.</span><span class="sxs-lookup"><span data-stu-id="45308-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="45308-141">**msdyn_ExecuteOperationSetV1**: Този API се използва за изпълнение на всички операции в рамките на дадения набор от операции.</span><span class="sxs-lookup"><span data-stu-id="45308-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="45308-142">Използване на API за график с OperationSet</span><span class="sxs-lookup"><span data-stu-id="45308-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="45308-143">Защото записи с **CreateProjectV1** и **CreateTeamMemberV1** едновременно се създават незабавно, тези API не могат да се използват в **OperationSet** директно.</span><span class="sxs-lookup"><span data-stu-id="45308-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="45308-144">Можете обаче да използвате API, за да създадете необходимите записи, да създадете **OperationSet** и след това използвайте тези предварително създадени записи в **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="45308-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="45308-145">Поддържани операции</span><span class="sxs-lookup"><span data-stu-id="45308-145">Supported operations</span></span>

| <span data-ttu-id="45308-146">Обект за планиране</span><span class="sxs-lookup"><span data-stu-id="45308-146">Scheduling entity</span></span> | <span data-ttu-id="45308-147">Създай</span><span class="sxs-lookup"><span data-stu-id="45308-147">Create</span></span> | <span data-ttu-id="45308-148">Update</span><span class="sxs-lookup"><span data-stu-id="45308-148">Update</span></span> | <span data-ttu-id="45308-149">Delete</span><span class="sxs-lookup"><span data-stu-id="45308-149">Delete</span></span> | <span data-ttu-id="45308-150">Важни съображения</span><span class="sxs-lookup"><span data-stu-id="45308-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="45308-151">Задача от проект</span><span class="sxs-lookup"><span data-stu-id="45308-151">Project task</span></span> | <span data-ttu-id="45308-152">Да</span><span class="sxs-lookup"><span data-stu-id="45308-152">Yes</span></span> | <span data-ttu-id="45308-153">Да</span><span class="sxs-lookup"><span data-stu-id="45308-153">Yes</span></span> | <span data-ttu-id="45308-154">Да</span><span class="sxs-lookup"><span data-stu-id="45308-154">Yes</span></span> | <span data-ttu-id="45308-155">Нищо</span><span class="sxs-lookup"><span data-stu-id="45308-155">None</span></span> |
| <span data-ttu-id="45308-156">Зависимост на задача от проект</span><span class="sxs-lookup"><span data-stu-id="45308-156">Project task dependency</span></span> | <span data-ttu-id="45308-157">Да</span><span class="sxs-lookup"><span data-stu-id="45308-157">Yes</span></span> | <span data-ttu-id="45308-158">Да</span><span class="sxs-lookup"><span data-stu-id="45308-158">Yes</span></span> | | <span data-ttu-id="45308-159">Записите на зависимостта на проектната задача не се актуализират.</span><span class="sxs-lookup"><span data-stu-id="45308-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="45308-160">Вместо това може да се изтрие стар запис и да се създаде нов.</span><span class="sxs-lookup"><span data-stu-id="45308-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="45308-161">Назначаване на ресурс</span><span class="sxs-lookup"><span data-stu-id="45308-161">Resource assignment</span></span> | <span data-ttu-id="45308-162">Да</span><span class="sxs-lookup"><span data-stu-id="45308-162">Yes</span></span> | <span data-ttu-id="45308-163">Да</span><span class="sxs-lookup"><span data-stu-id="45308-163">Yes</span></span> | | <span data-ttu-id="45308-164">Не се поддържат операции със следните полета: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** и **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="45308-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="45308-165">Записите за възлагане на ресурси не се актуализират.</span><span class="sxs-lookup"><span data-stu-id="45308-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="45308-166">Вместо това може да се изтрие старият запис и да се създаде нов.</span><span class="sxs-lookup"><span data-stu-id="45308-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="45308-167">Набор на проекта</span><span class="sxs-lookup"><span data-stu-id="45308-167">Project bucket</span></span> | <span data-ttu-id="45308-168">N/A</span><span class="sxs-lookup"><span data-stu-id="45308-168">N/A</span></span> | <span data-ttu-id="45308-169">N/A</span><span class="sxs-lookup"><span data-stu-id="45308-169">N/A</span></span> | <span data-ttu-id="45308-170">N/A</span><span class="sxs-lookup"><span data-stu-id="45308-170">N/A</span></span> | <span data-ttu-id="45308-171">Кофата по подразбиране се създава с помощта на **CreateProjectV1** API.</span><span class="sxs-lookup"><span data-stu-id="45308-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="45308-172">Член на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="45308-172">Project team member</span></span> | <span data-ttu-id="45308-173">Да</span><span class="sxs-lookup"><span data-stu-id="45308-173">Yes</span></span> | <span data-ttu-id="45308-174">Да</span><span class="sxs-lookup"><span data-stu-id="45308-174">Yes</span></span> | <span data-ttu-id="45308-175">Да</span><span class="sxs-lookup"><span data-stu-id="45308-175">Yes</span></span> | <span data-ttu-id="45308-176">За операцията за създаване използвайте **CreateTeamMemberV1** API.</span><span class="sxs-lookup"><span data-stu-id="45308-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="45308-177">Project</span><span class="sxs-lookup"><span data-stu-id="45308-177">Project</span></span> | <span data-ttu-id="45308-178">Да</span><span class="sxs-lookup"><span data-stu-id="45308-178">Yes</span></span> | <span data-ttu-id="45308-179">Да</span><span class="sxs-lookup"><span data-stu-id="45308-179">Yes</span></span> | <span data-ttu-id="45308-180">N/A</span><span class="sxs-lookup"><span data-stu-id="45308-180">N/A</span></span> | <span data-ttu-id="45308-181">Не се поддържат операции със следните полета: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** и **Duration**.</span><span class="sxs-lookup"><span data-stu-id="45308-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="45308-182">Тези API могат да бъдат извикани с обекти на обекти, които включват персонализирани полета.</span><span class="sxs-lookup"><span data-stu-id="45308-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="45308-183">Свойството ИД не е задължително.</span><span class="sxs-lookup"><span data-stu-id="45308-183">The ID property is optional.</span></span> <span data-ttu-id="45308-184">Ако е предоставено, системата се опитва да го използва и извежда изключение, ако не може да се използва.</span><span class="sxs-lookup"><span data-stu-id="45308-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="45308-185">Ако не е предоставено, системата ще го генерира.</span><span class="sxs-lookup"><span data-stu-id="45308-185">If it isn't provided, the system will generate it.</span></span>

## <a name="limitations-and-known-issues"></a><span data-ttu-id="45308-186">Известни проблеми и ограничения</span><span class="sxs-lookup"><span data-stu-id="45308-186">Limitations and known issues</span></span>
<span data-ttu-id="45308-187">Следва списък с ограничения и известни проблеми:</span><span class="sxs-lookup"><span data-stu-id="45308-187">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="45308-188">API на графика може да се използва само от **Потребители с лиценз за Microsoft Project.**</span><span class="sxs-lookup"><span data-stu-id="45308-188">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="45308-189">Те не могат да бъдат използвани от:</span><span class="sxs-lookup"><span data-stu-id="45308-189">They can't be used by:</span></span>
    - <span data-ttu-id="45308-190">Потребители на приложение</span><span class="sxs-lookup"><span data-stu-id="45308-190">Application users</span></span>
    - <span data-ttu-id="45308-191">Системни потребители</span><span class="sxs-lookup"><span data-stu-id="45308-191">System users</span></span>
    - <span data-ttu-id="45308-192">Потребители на интеграция</span><span class="sxs-lookup"><span data-stu-id="45308-192">Integration users</span></span>
    - <span data-ttu-id="45308-193">Други потребители, които нямат необходимия лиценз</span><span class="sxs-lookup"><span data-stu-id="45308-193">Other users that don't have the required license</span></span>
- <span data-ttu-id="45308-194">Всеки **OperationSet** може да има максимум 100 операции.</span><span class="sxs-lookup"><span data-stu-id="45308-194">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="45308-195">Всеки потребител може да има максимум 10 отворени **OperationSets**.</span><span class="sxs-lookup"><span data-stu-id="45308-195">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="45308-196">Понастоящем Project Operations поддържа максимум 500 общо задачи по проект.</span><span class="sxs-lookup"><span data-stu-id="45308-196">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="45308-197">Състоянието на неуспех **OperationSet** и регистрационните файлове за неуспех в момента не са достъпни.</span><span class="sxs-lookup"><span data-stu-id="45308-197">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="45308-198">API за график са в публичен преглед.</span><span class="sxs-lookup"><span data-stu-id="45308-198">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="45308-199">Използването на тези API в производствена среда не се поддържа от Microsoft.</span><span class="sxs-lookup"><span data-stu-id="45308-199">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="45308-200">Примерен сценарий</span><span class="sxs-lookup"><span data-stu-id="45308-200">Sample scenario</span></span>

<span data-ttu-id="45308-201">В този сценарий ще създадете проект, член на екип, четири задачи и две задания за ресурси.</span><span class="sxs-lookup"><span data-stu-id="45308-201">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="45308-202">След това ще актуализирате една задача, ще актуализирате проекта, ще изтриете една задача, ще изтриете едно задание на ресурс и ще създадете зависимост от задачата.</span><span class="sxs-lookup"><span data-stu-id="45308-202">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="45308-203">Допълнителни проби</span><span class="sxs-lookup"><span data-stu-id="45308-203">Additional samples</span></span>

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
