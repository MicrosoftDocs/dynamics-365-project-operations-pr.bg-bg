---
title: Използвайте API на графика, за да извършвате операции с обекти за планиране
description: Тази тема предоставя информация и проби за използване на API за график.
author: sigitac
manager: Annbe
ms.date: 04/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e03f4e6c49a835206b23cade3fabe3fd26693441
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950791"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="4bef2-103">Използвайте API на графика, за да извършвате операции с обекти за планиране</span><span class="sxs-lookup"><span data-stu-id="4bef2-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="4bef2-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="4bef2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="4bef2-105">Част или цялата функционалност, отбелязана в тази тема, е достъпна като част от версия за преглед.</span><span class="sxs-lookup"><span data-stu-id="4bef2-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="4bef2-106">Съдържанието и функционалността подлежат на промяна.</span><span class="sxs-lookup"><span data-stu-id="4bef2-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="4bef2-107">Обекти за планиране</span><span class="sxs-lookup"><span data-stu-id="4bef2-107">Scheduling entities</span></span>

<span data-ttu-id="4bef2-108">Приложните програмни интерфейси (API) на графика предоставят възможност за извършване на операции по създаване, актуализиране и изтриване с **Обекти за планиране**.</span><span class="sxs-lookup"><span data-stu-id="4bef2-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="4bef2-109">Тези обекти се управляват чрез механизма за планиране в Project for the web.</span><span class="sxs-lookup"><span data-stu-id="4bef2-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="4bef2-110">Създавайте, актуализирайте и изтривайте операции с **Обекти за планиране** бяха ограничени в по-ранни издания на Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="4bef2-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="4bef2-111">Следващата таблица предоставя пълен списък на **Обекти за планиране**.</span><span class="sxs-lookup"><span data-stu-id="4bef2-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="4bef2-112">Име на обекта</span><span class="sxs-lookup"><span data-stu-id="4bef2-112">Entity name</span></span>  | <span data-ttu-id="4bef2-113">Логическо име на обект</span><span class="sxs-lookup"><span data-stu-id="4bef2-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="4bef2-114">Project</span><span class="sxs-lookup"><span data-stu-id="4bef2-114">Project</span></span> | <span data-ttu-id="4bef2-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="4bef2-115">msdyn_project</span></span> |
| <span data-ttu-id="4bef2-116">Задача по проект</span><span class="sxs-lookup"><span data-stu-id="4bef2-116">Project Task</span></span>  | <span data-ttu-id="4bef2-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="4bef2-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="4bef2-118">Зависимост на задачи от проект</span><span class="sxs-lookup"><span data-stu-id="4bef2-118">Project Task Dependency</span></span>  | <span data-ttu-id="4bef2-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="4bef2-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="4bef2-120">Назначаване на ресурс</span><span class="sxs-lookup"><span data-stu-id="4bef2-120">Resource Assignment</span></span> | <span data-ttu-id="4bef2-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="4bef2-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="4bef2-122">Набор на проекта</span><span class="sxs-lookup"><span data-stu-id="4bef2-122">Project Bucket</span></span>  | <span data-ttu-id="4bef2-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="4bef2-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="4bef2-124">Член на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="4bef2-124">Project Team Member</span></span> | <span data-ttu-id="4bef2-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="4bef2-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="4bef2-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="4bef2-126">OperationSet</span></span>

<span data-ttu-id="4bef2-127">OperationSet е модел на единица работа, който може да се използва, когато в рамките на една транзакция трябва да бъдат обработени няколко искания, засягащи графика.</span><span class="sxs-lookup"><span data-stu-id="4bef2-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="4bef2-128">Планиране на API</span><span class="sxs-lookup"><span data-stu-id="4bef2-128">Schedule APIs</span></span>

<span data-ttu-id="4bef2-129">По-долу е даден списък на текущите API на график.</span><span class="sxs-lookup"><span data-stu-id="4bef2-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="4bef2-130">**msdyn_CreateProjectV1**: Този API може да се използва за създаване на проект.</span><span class="sxs-lookup"><span data-stu-id="4bef2-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="4bef2-131">Проектът и сегментът на проекта по подразбиране се създават незабавно.</span><span class="sxs-lookup"><span data-stu-id="4bef2-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="4bef2-132">**msdyn_CreateTeamMemberV1**: Този API може да се използва за създаване на член на екип по проект.</span><span class="sxs-lookup"><span data-stu-id="4bef2-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="4bef2-133">Записът на члена на екипа се създава незабавно.</span><span class="sxs-lookup"><span data-stu-id="4bef2-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="4bef2-134">**msdyn_CreateOperationSetV1**: Този API може да се използва за планиране на няколко заявки, които трябва да бъдат изпълнени в рамките на транзакция.</span><span class="sxs-lookup"><span data-stu-id="4bef2-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="4bef2-135">**msdyn_PSSCreateV1**: Този API може да се използва за създаване на обект.</span><span class="sxs-lookup"><span data-stu-id="4bef2-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="4bef2-136">Обектът може да бъде всеки от обектите за планиране, които поддържат операцията за създаване.</span><span class="sxs-lookup"><span data-stu-id="4bef2-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="4bef2-137">**msdyn_PSSUpdateV1**: Този API може да се използва за актуализиране на обект.</span><span class="sxs-lookup"><span data-stu-id="4bef2-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="4bef2-138">Обектът може да бъде всеки от обектите за планиране, които поддържат операцията за актуализиране.</span><span class="sxs-lookup"><span data-stu-id="4bef2-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="4bef2-139">**msdyn_PSSDeleteV1**: Този API може да се използва за изтриване на обект.</span><span class="sxs-lookup"><span data-stu-id="4bef2-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="4bef2-140">Обектът може да бъде всеки от обектите за планиране, които поддържат операцията за изтриване.</span><span class="sxs-lookup"><span data-stu-id="4bef2-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="4bef2-141">**msdyn_ExecuteOperationSetV1**: Този API се използва за изпълнение на всички операции в рамките на дадения набор от операции.</span><span class="sxs-lookup"><span data-stu-id="4bef2-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="4bef2-142">Използване на API за график с OperationSet</span><span class="sxs-lookup"><span data-stu-id="4bef2-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="4bef2-143">Защото записи с **CreateProjectV1** и **CreateTeamMemberV1** едновременно се създават незабавно, тези API не могат да се използват в **OperationSet** директно.</span><span class="sxs-lookup"><span data-stu-id="4bef2-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="4bef2-144">Можете обаче да използвате API, за да създадете необходимите записи, да създадете **OperationSet** и след това използвайте тези предварително създадени записи в **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="4bef2-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="4bef2-145">Поддържани операции</span><span class="sxs-lookup"><span data-stu-id="4bef2-145">Supported operations</span></span>

| <span data-ttu-id="4bef2-146">Обект за планиране</span><span class="sxs-lookup"><span data-stu-id="4bef2-146">Scheduling entity</span></span> | <span data-ttu-id="4bef2-147">Създай</span><span class="sxs-lookup"><span data-stu-id="4bef2-147">Create</span></span> | <span data-ttu-id="4bef2-148">Update</span><span class="sxs-lookup"><span data-stu-id="4bef2-148">Update</span></span> | <span data-ttu-id="4bef2-149">Delete</span><span class="sxs-lookup"><span data-stu-id="4bef2-149">Delete</span></span> | <span data-ttu-id="4bef2-150">Важни съображения</span><span class="sxs-lookup"><span data-stu-id="4bef2-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="4bef2-151">Задача от проект</span><span class="sxs-lookup"><span data-stu-id="4bef2-151">Project task</span></span> | <span data-ttu-id="4bef2-152">Да</span><span class="sxs-lookup"><span data-stu-id="4bef2-152">Yes</span></span> | <span data-ttu-id="4bef2-153">Да</span><span class="sxs-lookup"><span data-stu-id="4bef2-153">Yes</span></span> | <span data-ttu-id="4bef2-154">Да</span><span class="sxs-lookup"><span data-stu-id="4bef2-154">Yes</span></span> | <span data-ttu-id="4bef2-155">Нищо</span><span class="sxs-lookup"><span data-stu-id="4bef2-155">None</span></span> |
| <span data-ttu-id="4bef2-156">Зависимост на задача от проект</span><span class="sxs-lookup"><span data-stu-id="4bef2-156">Project task dependency</span></span> | <span data-ttu-id="4bef2-157">Да</span><span class="sxs-lookup"><span data-stu-id="4bef2-157">Yes</span></span> | <span data-ttu-id="4bef2-158">Да</span><span class="sxs-lookup"><span data-stu-id="4bef2-158">Yes</span></span> | | <span data-ttu-id="4bef2-159">Записите на зависимостта на проектната задача не се актуализират.</span><span class="sxs-lookup"><span data-stu-id="4bef2-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="4bef2-160">Вместо това може да се изтрие стар запис и да се създаде нов.</span><span class="sxs-lookup"><span data-stu-id="4bef2-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="4bef2-161">Назначаване на ресурс</span><span class="sxs-lookup"><span data-stu-id="4bef2-161">Resource assignment</span></span> | <span data-ttu-id="4bef2-162">Да</span><span class="sxs-lookup"><span data-stu-id="4bef2-162">Yes</span></span> | <span data-ttu-id="4bef2-163">Да</span><span class="sxs-lookup"><span data-stu-id="4bef2-163">Yes</span></span> | | <span data-ttu-id="4bef2-164">Не се поддържат операции със следните полета: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** и **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="4bef2-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="4bef2-165">Записите за възлагане на ресурси не се актуализират.</span><span class="sxs-lookup"><span data-stu-id="4bef2-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="4bef2-166">Вместо това може да се изтрие старият запис и да се създаде нов.</span><span class="sxs-lookup"><span data-stu-id="4bef2-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="4bef2-167">Набор на проекта</span><span class="sxs-lookup"><span data-stu-id="4bef2-167">Project bucket</span></span> | <span data-ttu-id="4bef2-168">N/A</span><span class="sxs-lookup"><span data-stu-id="4bef2-168">N/A</span></span> | <span data-ttu-id="4bef2-169">N/A</span><span class="sxs-lookup"><span data-stu-id="4bef2-169">N/A</span></span> | <span data-ttu-id="4bef2-170">N/A</span><span class="sxs-lookup"><span data-stu-id="4bef2-170">N/A</span></span> | <span data-ttu-id="4bef2-171">Кофата по подразбиране се създава с помощта на **CreateProjectV1** API.</span><span class="sxs-lookup"><span data-stu-id="4bef2-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="4bef2-172">Член на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="4bef2-172">Project team member</span></span> | <span data-ttu-id="4bef2-173">Да</span><span class="sxs-lookup"><span data-stu-id="4bef2-173">Yes</span></span> | <span data-ttu-id="4bef2-174">Да</span><span class="sxs-lookup"><span data-stu-id="4bef2-174">Yes</span></span> | <span data-ttu-id="4bef2-175">Да</span><span class="sxs-lookup"><span data-stu-id="4bef2-175">Yes</span></span> | <span data-ttu-id="4bef2-176">За операцията за създаване използвайте **CreateTeamMemberV1** API.</span><span class="sxs-lookup"><span data-stu-id="4bef2-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="4bef2-177">Project</span><span class="sxs-lookup"><span data-stu-id="4bef2-177">Project</span></span> | <span data-ttu-id="4bef2-178">Да</span><span class="sxs-lookup"><span data-stu-id="4bef2-178">Yes</span></span> | <span data-ttu-id="4bef2-179">Да</span><span class="sxs-lookup"><span data-stu-id="4bef2-179">Yes</span></span> | <span data-ttu-id="4bef2-180">N/A</span><span class="sxs-lookup"><span data-stu-id="4bef2-180">N/A</span></span> | <span data-ttu-id="4bef2-181">Не се поддържат операции със следните полета: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** и **Duration**.</span><span class="sxs-lookup"><span data-stu-id="4bef2-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="4bef2-182">Тези API могат да бъдат извикани с обекти на обекти, които включват персонализирани полета.</span><span class="sxs-lookup"><span data-stu-id="4bef2-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="4bef2-183">Свойството ИД не е задължително.</span><span class="sxs-lookup"><span data-stu-id="4bef2-183">The ID property is optional.</span></span> <span data-ttu-id="4bef2-184">Ако е предоставено, системата се опитва да го използва и извежда изключение, ако не може да се използва.</span><span class="sxs-lookup"><span data-stu-id="4bef2-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="4bef2-185">Ако не е предоставено, системата ще го генерира.</span><span class="sxs-lookup"><span data-stu-id="4bef2-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="4bef2-186">Ограничени полета</span><span class="sxs-lookup"><span data-stu-id="4bef2-186">Restricted fields</span></span>

<span data-ttu-id="4bef2-187">Следващите таблици определят полетата, за които е забранено да **Създават** и **Редактират**.</span><span class="sxs-lookup"><span data-stu-id="4bef2-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="4bef2-188">Задача от проект</span><span class="sxs-lookup"><span data-stu-id="4bef2-188">Project task</span></span>

| <span data-ttu-id="4bef2-189">**Логическо име**</span><span class="sxs-lookup"><span data-stu-id="4bef2-189">**Logical name**</span></span>                       | <span data-ttu-id="4bef2-190">**Може да създава**</span><span class="sxs-lookup"><span data-stu-id="4bef2-190">**Can create**</span></span> | <span data-ttu-id="4bef2-191">**Може да редактира**</span><span class="sxs-lookup"><span data-stu-id="4bef2-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="4bef2-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="4bef2-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="4bef2-193">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-193">no</span></span>             | <span data-ttu-id="4bef2-194">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-194">no</span></span>               |
| <span data-ttu-id="4bef2-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="4bef2-196">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-196">no</span></span>             | <span data-ttu-id="4bef2-197">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-197">no</span></span>               |
| <span data-ttu-id="4bef2-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="4bef2-198">msdyn_actualend</span></span>                        | <span data-ttu-id="4bef2-199">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-199">no</span></span>             | <span data-ttu-id="4bef2-200">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-200">no</span></span>               |
| <span data-ttu-id="4bef2-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="4bef2-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="4bef2-202">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-202">no</span></span>             | <span data-ttu-id="4bef2-203">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-203">no</span></span>               |
| <span data-ttu-id="4bef2-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="4bef2-205">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-205">no</span></span>             | <span data-ttu-id="4bef2-206">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-206">no</span></span>               |
| <span data-ttu-id="4bef2-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="4bef2-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="4bef2-208">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-208">no</span></span>             | <span data-ttu-id="4bef2-209">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-209">no</span></span>               |
| <span data-ttu-id="4bef2-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="4bef2-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="4bef2-211">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-211">no</span></span>             | <span data-ttu-id="4bef2-212">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-212">no</span></span>               |
| <span data-ttu-id="4bef2-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="4bef2-214">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-214">no</span></span>             | <span data-ttu-id="4bef2-215">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-215">no</span></span>               |
| <span data-ttu-id="4bef2-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="4bef2-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="4bef2-217">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-217">no</span></span>             | <span data-ttu-id="4bef2-218">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-218">no</span></span>               |
| <span data-ttu-id="4bef2-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="4bef2-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="4bef2-220">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-220">no</span></span>             | <span data-ttu-id="4bef2-221">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-221">no</span></span>               |
| <span data-ttu-id="4bef2-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="4bef2-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="4bef2-223">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-223">no</span></span>             | <span data-ttu-id="4bef2-224">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-224">no</span></span>               |
| <span data-ttu-id="4bef2-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="4bef2-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="4bef2-226">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-226">no</span></span>             | <span data-ttu-id="4bef2-227">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-227">no</span></span>               |
| <span data-ttu-id="4bef2-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="4bef2-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="4bef2-229">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-229">no</span></span>             | <span data-ttu-id="4bef2-230">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-230">no</span></span>               |
| <span data-ttu-id="4bef2-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="4bef2-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="4bef2-232">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-232">no</span></span>             | <span data-ttu-id="4bef2-233">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-233">no</span></span>               |
| <span data-ttu-id="4bef2-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="4bef2-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="4bef2-235">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-235">no</span></span>             | <span data-ttu-id="4bef2-236">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-236">no</span></span>               |
| <span data-ttu-id="4bef2-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="4bef2-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="4bef2-238">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-238">no</span></span>             | <span data-ttu-id="4bef2-239">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-239">no</span></span>               |
| <span data-ttu-id="4bef2-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="4bef2-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="4bef2-241">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-241">no</span></span>             | <span data-ttu-id="4bef2-242">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-242">no</span></span>               |
| <span data-ttu-id="4bef2-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="4bef2-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="4bef2-244">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-244">no</span></span>             | <span data-ttu-id="4bef2-245">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-245">no</span></span>               |
| <span data-ttu-id="4bef2-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="4bef2-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="4bef2-247">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-247">no</span></span>             | <span data-ttu-id="4bef2-248">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-248">no</span></span>               |
| <span data-ttu-id="4bef2-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="4bef2-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="4bef2-250">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-250">no</span></span>             | <span data-ttu-id="4bef2-251">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-251">no</span></span>               |
| <span data-ttu-id="4bef2-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="4bef2-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="4bef2-253">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-253">no</span></span>             | <span data-ttu-id="4bef2-254">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-254">no</span></span>               |
| <span data-ttu-id="4bef2-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="4bef2-256">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-256">no</span></span>             | <span data-ttu-id="4bef2-257">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-257">no</span></span>               |
| <span data-ttu-id="4bef2-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="4bef2-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="4bef2-259">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-259">no</span></span>             | <span data-ttu-id="4bef2-260">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-260">no</span></span>               |
| <span data-ttu-id="4bef2-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="4bef2-262">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-262">no</span></span>             | <span data-ttu-id="4bef2-263">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-263">no</span></span>               |
| <span data-ttu-id="4bef2-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="4bef2-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="4bef2-265">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-265">no</span></span>             | <span data-ttu-id="4bef2-266">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-266">no</span></span>               |
| <span data-ttu-id="4bef2-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="4bef2-267">msdyn_progress</span></span>                         | <span data-ttu-id="4bef2-268">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-268">no</span></span>             | <span data-ttu-id="4bef2-269">не (да за P4W)</span><span class="sxs-lookup"><span data-stu-id="4bef2-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="4bef2-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="4bef2-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="4bef2-271">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-271">no</span></span>             | <span data-ttu-id="4bef2-272">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-272">no</span></span>               |
| <span data-ttu-id="4bef2-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="4bef2-274">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-274">no</span></span>             | <span data-ttu-id="4bef2-275">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-275">no</span></span>               |
| <span data-ttu-id="4bef2-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="4bef2-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="4bef2-277">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-277">no</span></span>             | <span data-ttu-id="4bef2-278">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-278">no</span></span>               |
| <span data-ttu-id="4bef2-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="4bef2-280">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-280">no</span></span>             | <span data-ttu-id="4bef2-281">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-281">no</span></span>               |
| <span data-ttu-id="4bef2-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="4bef2-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="4bef2-283">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-283">no</span></span>             | <span data-ttu-id="4bef2-284">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-284">no</span></span>               |
| <span data-ttu-id="4bef2-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="4bef2-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="4bef2-286">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-286">no</span></span>             | <span data-ttu-id="4bef2-287">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-287">no</span></span>               |
| <span data-ttu-id="4bef2-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="4bef2-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="4bef2-289">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-289">no</span></span>             | <span data-ttu-id="4bef2-290">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-290">no</span></span>               |
| <span data-ttu-id="4bef2-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="4bef2-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="4bef2-292">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-292">no</span></span>             | <span data-ttu-id="4bef2-293">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-293">no</span></span>               |
| <span data-ttu-id="4bef2-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="4bef2-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="4bef2-295">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-295">no</span></span>             | <span data-ttu-id="4bef2-296">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-296">no</span></span>               |
| <span data-ttu-id="4bef2-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="4bef2-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="4bef2-298">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-298">no</span></span>             | <span data-ttu-id="4bef2-299">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-299">no</span></span>               |
| <span data-ttu-id="4bef2-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="4bef2-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="4bef2-301">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-301">no</span></span>             | <span data-ttu-id="4bef2-302">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-302">no</span></span>               |
| <span data-ttu-id="4bef2-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="4bef2-304">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-304">no</span></span>             | <span data-ttu-id="4bef2-305">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-305">no</span></span>               |
| <span data-ttu-id="4bef2-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="4bef2-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="4bef2-307">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-307">no</span></span>             | <span data-ttu-id="4bef2-308">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-308">no</span></span>               |
| <span data-ttu-id="4bef2-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="4bef2-310">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-310">no</span></span>             | <span data-ttu-id="4bef2-311">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-311">no</span></span>               |
| <span data-ttu-id="4bef2-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="4bef2-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="4bef2-313">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-313">no</span></span>             | <span data-ttu-id="4bef2-314">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-314">no</span></span>               |
| <span data-ttu-id="4bef2-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="4bef2-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="4bef2-316">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-316">no</span></span>             | <span data-ttu-id="4bef2-317">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-317">no</span></span>               |
| <span data-ttu-id="4bef2-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="4bef2-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="4bef2-319">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-319">no</span></span>             | <span data-ttu-id="4bef2-320">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-320">no</span></span>               |
| <span data-ttu-id="4bef2-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="4bef2-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="4bef2-322">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-322">no</span></span>             | <span data-ttu-id="4bef2-323">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-323">no</span></span>               |
| <span data-ttu-id="4bef2-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="4bef2-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="4bef2-325">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-325">no</span></span>             | <span data-ttu-id="4bef2-326">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-326">no</span></span>               |
| <span data-ttu-id="4bef2-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="4bef2-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="4bef2-328">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-328">no</span></span>             | <span data-ttu-id="4bef2-329">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-329">no</span></span>               |
| <span data-ttu-id="4bef2-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="4bef2-330">msdyn_summary</span></span>                          | <span data-ttu-id="4bef2-331">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-331">no</span></span>             | <span data-ttu-id="4bef2-332">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-332">no</span></span>               |
| <span data-ttu-id="4bef2-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="4bef2-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="4bef2-334">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-334">no</span></span>             | <span data-ttu-id="4bef2-335">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-335">no</span></span>               |
| <span data-ttu-id="4bef2-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="4bef2-337">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-337">no</span></span>             | <span data-ttu-id="4bef2-338">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="4bef2-339">Зависимост на задача от проект</span><span class="sxs-lookup"><span data-stu-id="4bef2-339">Project task dependency</span></span>

| <span data-ttu-id="4bef2-340">**Логическо име**</span><span class="sxs-lookup"><span data-stu-id="4bef2-340">**Logical name**</span></span>              | <span data-ttu-id="4bef2-341">**Може да създава**</span><span class="sxs-lookup"><span data-stu-id="4bef2-341">**Can create**</span></span> | <span data-ttu-id="4bef2-342">**Може да редактира**</span><span class="sxs-lookup"><span data-stu-id="4bef2-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="4bef2-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="4bef2-343">msdyn_linktype</span></span>                | <span data-ttu-id="4bef2-344">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-344">no</span></span>             | <span data-ttu-id="4bef2-345">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-345">no</span></span>           |
| <span data-ttu-id="4bef2-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="4bef2-346">msdyn_linktypename</span></span>            | <span data-ttu-id="4bef2-347">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-347">no</span></span>             | <span data-ttu-id="4bef2-348">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-348">no</span></span>           |
| <span data-ttu-id="4bef2-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="4bef2-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="4bef2-350">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-350">yes</span></span>            | <span data-ttu-id="4bef2-351">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-351">no</span></span>           |
| <span data-ttu-id="4bef2-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="4bef2-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="4bef2-353">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-353">yes</span></span>            | <span data-ttu-id="4bef2-354">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-354">no</span></span>           |
| <span data-ttu-id="4bef2-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="4bef2-355">msdyn_project</span></span>                 | <span data-ttu-id="4bef2-356">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-356">yes</span></span>            | <span data-ttu-id="4bef2-357">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-357">no</span></span>           |
| <span data-ttu-id="4bef2-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="4bef2-358">msdyn_projectname</span></span>             | <span data-ttu-id="4bef2-359">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-359">yes</span></span>            | <span data-ttu-id="4bef2-360">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-360">no</span></span>           |
| <span data-ttu-id="4bef2-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="4bef2-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="4bef2-362">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-362">yes</span></span>            | <span data-ttu-id="4bef2-363">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-363">no</span></span>           |
| <span data-ttu-id="4bef2-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="4bef2-364">msdyn_successortask</span></span>           | <span data-ttu-id="4bef2-365">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-365">yes</span></span>            | <span data-ttu-id="4bef2-366">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-366">no</span></span>           |
| <span data-ttu-id="4bef2-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="4bef2-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="4bef2-368">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-368">yes</span></span>            | <span data-ttu-id="4bef2-369">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="4bef2-370">Назначаване на ресурс</span><span class="sxs-lookup"><span data-stu-id="4bef2-370">Resource assignment</span></span>

| <span data-ttu-id="4bef2-371">**Логическо име**</span><span class="sxs-lookup"><span data-stu-id="4bef2-371">**Logical name**</span></span>             | <span data-ttu-id="4bef2-372">**Може да създава**</span><span class="sxs-lookup"><span data-stu-id="4bef2-372">**Can create**</span></span> | <span data-ttu-id="4bef2-373">**Може да редактира**</span><span class="sxs-lookup"><span data-stu-id="4bef2-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="4bef2-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="4bef2-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="4bef2-375">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-375">yes</span></span>            | <span data-ttu-id="4bef2-376">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-376">no</span></span>           |
| <span data-ttu-id="4bef2-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="4bef2-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="4bef2-378">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-378">yes</span></span>            | <span data-ttu-id="4bef2-379">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-379">no</span></span>           |
| <span data-ttu-id="4bef2-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="4bef2-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="4bef2-381">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-381">no</span></span>             | <span data-ttu-id="4bef2-382">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-382">no</span></span>           |
| <span data-ttu-id="4bef2-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="4bef2-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="4bef2-384">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-384">no</span></span>             | <span data-ttu-id="4bef2-385">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-385">no</span></span>           |
| <span data-ttu-id="4bef2-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="4bef2-386">msdyn_committype</span></span>             | <span data-ttu-id="4bef2-387">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-387">no</span></span>             | <span data-ttu-id="4bef2-388">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-388">no</span></span>           |
| <span data-ttu-id="4bef2-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="4bef2-389">msdyn_committypename</span></span>         | <span data-ttu-id="4bef2-390">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-390">no</span></span>             | <span data-ttu-id="4bef2-391">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-391">no</span></span>           |
| <span data-ttu-id="4bef2-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="4bef2-392">msdyn_effort</span></span>                 | <span data-ttu-id="4bef2-393">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-393">no</span></span>             | <span data-ttu-id="4bef2-394">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-394">no</span></span>           |
| <span data-ttu-id="4bef2-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="4bef2-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="4bef2-396">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-396">no</span></span>             | <span data-ttu-id="4bef2-397">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-397">no</span></span>           |
| <span data-ttu-id="4bef2-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="4bef2-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="4bef2-399">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-399">no</span></span>             | <span data-ttu-id="4bef2-400">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-400">no</span></span>           |
| <span data-ttu-id="4bef2-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="4bef2-401">msdyn_finish</span></span>                 | <span data-ttu-id="4bef2-402">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-402">no</span></span>             | <span data-ttu-id="4bef2-403">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-403">no</span></span>           |
| <span data-ttu-id="4bef2-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="4bef2-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="4bef2-405">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-405">no</span></span>             | <span data-ttu-id="4bef2-406">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-406">no</span></span>           |
| <span data-ttu-id="4bef2-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="4bef2-408">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-408">no</span></span>             | <span data-ttu-id="4bef2-409">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-409">no</span></span>           |
| <span data-ttu-id="4bef2-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="4bef2-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="4bef2-411">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-411">no</span></span>             | <span data-ttu-id="4bef2-412">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-412">no</span></span>           |
| <span data-ttu-id="4bef2-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="4bef2-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="4bef2-414">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-414">no</span></span>             | <span data-ttu-id="4bef2-415">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-415">no</span></span>           |
| <span data-ttu-id="4bef2-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="4bef2-417">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-417">no</span></span>             | <span data-ttu-id="4bef2-418">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-418">no</span></span>           |
| <span data-ttu-id="4bef2-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="4bef2-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="4bef2-420">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-420">no</span></span>             | <span data-ttu-id="4bef2-421">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-421">no</span></span>           |
| <span data-ttu-id="4bef2-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="4bef2-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="4bef2-423">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-423">no</span></span>             | <span data-ttu-id="4bef2-424">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-424">no</span></span>           |
| <span data-ttu-id="4bef2-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="4bef2-425">msdyn_projectid</span></span>              | <span data-ttu-id="4bef2-426">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-426">yes</span></span>            | <span data-ttu-id="4bef2-427">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-427">no</span></span>           |
| <span data-ttu-id="4bef2-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="4bef2-428">msdyn_projectidname</span></span>          | <span data-ttu-id="4bef2-429">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-429">no</span></span>             | <span data-ttu-id="4bef2-430">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-430">no</span></span>           |
| <span data-ttu-id="4bef2-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="4bef2-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="4bef2-432">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-432">no</span></span>             | <span data-ttu-id="4bef2-433">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-433">no</span></span>           |
| <span data-ttu-id="4bef2-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="4bef2-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="4bef2-435">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-435">no</span></span>             | <span data-ttu-id="4bef2-436">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-436">no</span></span>           |
| <span data-ttu-id="4bef2-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="4bef2-437">msdyn_start</span></span>                  | <span data-ttu-id="4bef2-438">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-438">no</span></span>             | <span data-ttu-id="4bef2-439">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-439">no</span></span>           |
| <span data-ttu-id="4bef2-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="4bef2-440">msdyn_taskid</span></span>                 | <span data-ttu-id="4bef2-441">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-441">no</span></span>             | <span data-ttu-id="4bef2-442">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-442">no</span></span>           |
| <span data-ttu-id="4bef2-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="4bef2-443">msdyn_taskidname</span></span>             | <span data-ttu-id="4bef2-444">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-444">no</span></span>             | <span data-ttu-id="4bef2-445">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-445">no</span></span>           |
| <span data-ttu-id="4bef2-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="4bef2-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="4bef2-447">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-447">no</span></span>             | <span data-ttu-id="4bef2-448">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="4bef2-449">Член на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="4bef2-449">Project team member</span></span>

| <span data-ttu-id="4bef2-450">**Логическо име**</span><span class="sxs-lookup"><span data-stu-id="4bef2-450">**Logical name**</span></span>                                 | <span data-ttu-id="4bef2-451">**Може да създава**</span><span class="sxs-lookup"><span data-stu-id="4bef2-451">**Can create**</span></span> | <span data-ttu-id="4bef2-452">**Може да редактира**</span><span class="sxs-lookup"><span data-stu-id="4bef2-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="4bef2-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="4bef2-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="4bef2-454">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-454">no</span></span>             | <span data-ttu-id="4bef2-455">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-455">no</span></span>           |
| <span data-ttu-id="4bef2-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="4bef2-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="4bef2-457">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-457">no</span></span>             | <span data-ttu-id="4bef2-458">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-458">no</span></span>           |
| <span data-ttu-id="4bef2-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="4bef2-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="4bef2-460">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-460">no</span></span>             | <span data-ttu-id="4bef2-461">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-461">no</span></span>           |
| <span data-ttu-id="4bef2-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="4bef2-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="4bef2-463">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-463">no</span></span>             | <span data-ttu-id="4bef2-464">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-464">no</span></span>           |
| <span data-ttu-id="4bef2-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="4bef2-465">msdyn_effort</span></span>                                     | <span data-ttu-id="4bef2-466">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-466">no</span></span>             | <span data-ttu-id="4bef2-467">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-467">no</span></span>           |
| <span data-ttu-id="4bef2-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="4bef2-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="4bef2-469">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-469">no</span></span>             | <span data-ttu-id="4bef2-470">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-470">no</span></span>           |
| <span data-ttu-id="4bef2-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="4bef2-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="4bef2-472">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-472">no</span></span>             | <span data-ttu-id="4bef2-473">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-473">no</span></span>           |
| <span data-ttu-id="4bef2-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="4bef2-474">msdyn_finish</span></span>                                     | <span data-ttu-id="4bef2-475">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-475">no</span></span>             | <span data-ttu-id="4bef2-476">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-476">no</span></span>           |
| <span data-ttu-id="4bef2-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="4bef2-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="4bef2-478">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-478">no</span></span>             | <span data-ttu-id="4bef2-479">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-479">no</span></span>           |
| <span data-ttu-id="4bef2-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="4bef2-480">msdyn_hours</span></span>                                      | <span data-ttu-id="4bef2-481">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-481">no</span></span>             | <span data-ttu-id="4bef2-482">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-482">no</span></span>           |
| <span data-ttu-id="4bef2-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="4bef2-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="4bef2-484">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-484">no</span></span>             | <span data-ttu-id="4bef2-485">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-485">no</span></span>           |
| <span data-ttu-id="4bef2-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="4bef2-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="4bef2-487">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-487">no</span></span>             | <span data-ttu-id="4bef2-488">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-488">no</span></span>           |
| <span data-ttu-id="4bef2-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="4bef2-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="4bef2-490">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-490">no</span></span>             | <span data-ttu-id="4bef2-491">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-491">no</span></span>           |
| <span data-ttu-id="4bef2-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="4bef2-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="4bef2-493">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-493">no</span></span>             | <span data-ttu-id="4bef2-494">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-494">no</span></span>           |
| <span data-ttu-id="4bef2-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="4bef2-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="4bef2-496">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-496">no</span></span>             | <span data-ttu-id="4bef2-497">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-497">no</span></span>           |
| <span data-ttu-id="4bef2-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="4bef2-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="4bef2-499">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-499">no</span></span>             | <span data-ttu-id="4bef2-500">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-500">no</span></span>           |
| <span data-ttu-id="4bef2-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="4bef2-501">msdyn_start</span></span>                                      | <span data-ttu-id="4bef2-502">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-502">no</span></span>             | <span data-ttu-id="4bef2-503">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="4bef2-504">Project</span><span class="sxs-lookup"><span data-stu-id="4bef2-504">Project</span></span>

| <span data-ttu-id="4bef2-505">**Логическо име**</span><span class="sxs-lookup"><span data-stu-id="4bef2-505">**Logical name**</span></span>                       | <span data-ttu-id="4bef2-506">**Може да създава**</span><span class="sxs-lookup"><span data-stu-id="4bef2-506">**Can create**</span></span> | <span data-ttu-id="4bef2-507">**Може да редактира**</span><span class="sxs-lookup"><span data-stu-id="4bef2-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="4bef2-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="4bef2-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="4bef2-509">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-509">no</span></span>             | <span data-ttu-id="4bef2-510">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-510">no</span></span>           |
| <span data-ttu-id="4bef2-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="4bef2-512">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-512">no</span></span>             | <span data-ttu-id="4bef2-513">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-513">no</span></span>           |
| <span data-ttu-id="4bef2-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="4bef2-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="4bef2-515">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-515">no</span></span>             | <span data-ttu-id="4bef2-516">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-516">no</span></span>           |
| <span data-ttu-id="4bef2-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="4bef2-518">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-518">no</span></span>             | <span data-ttu-id="4bef2-519">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-519">no</span></span>           |
| <span data-ttu-id="4bef2-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="4bef2-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="4bef2-521">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-521">no</span></span>             | <span data-ttu-id="4bef2-522">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-522">no</span></span>           |
| <span data-ttu-id="4bef2-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="4bef2-524">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-524">no</span></span>             | <span data-ttu-id="4bef2-525">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-525">no</span></span>           |
| <span data-ttu-id="4bef2-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="4bef2-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="4bef2-527">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-527">yes</span></span>            | <span data-ttu-id="4bef2-528">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-528">no</span></span>           |
| <span data-ttu-id="4bef2-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="4bef2-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="4bef2-530">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-530">yes</span></span>            | <span data-ttu-id="4bef2-531">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-531">no</span></span>           |
| <span data-ttu-id="4bef2-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="4bef2-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="4bef2-533">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-533">yes</span></span>            | <span data-ttu-id="4bef2-534">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-534">no</span></span>           |
| <span data-ttu-id="4bef2-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="4bef2-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="4bef2-536">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-536">no</span></span>             | <span data-ttu-id="4bef2-537">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-537">no</span></span>           |
| <span data-ttu-id="4bef2-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="4bef2-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="4bef2-539">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-539">no</span></span>             | <span data-ttu-id="4bef2-540">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-540">no</span></span>           |
| <span data-ttu-id="4bef2-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="4bef2-542">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-542">no</span></span>             | <span data-ttu-id="4bef2-543">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-543">no</span></span>           |
| <span data-ttu-id="4bef2-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="4bef2-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="4bef2-545">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-545">no</span></span>             | <span data-ttu-id="4bef2-546">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-546">no</span></span>           |
| <span data-ttu-id="4bef2-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="4bef2-548">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-548">no</span></span>             | <span data-ttu-id="4bef2-549">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-549">no</span></span>           |
| <span data-ttu-id="4bef2-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="4bef2-550">msdyn_duration</span></span>                         | <span data-ttu-id="4bef2-551">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-551">no</span></span>             | <span data-ttu-id="4bef2-552">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-552">no</span></span>           |
| <span data-ttu-id="4bef2-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="4bef2-553">msdyn_effort</span></span>                           | <span data-ttu-id="4bef2-554">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-554">no</span></span>             | <span data-ttu-id="4bef2-555">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-555">no</span></span>           |
| <span data-ttu-id="4bef2-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="4bef2-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="4bef2-557">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-557">no</span></span>             | <span data-ttu-id="4bef2-558">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-558">no</span></span>           |
| <span data-ttu-id="4bef2-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="4bef2-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="4bef2-560">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-560">no</span></span>             | <span data-ttu-id="4bef2-561">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-561">no</span></span>           |
| <span data-ttu-id="4bef2-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="4bef2-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="4bef2-563">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-563">no</span></span>             | <span data-ttu-id="4bef2-564">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-564">no</span></span>           |
| <span data-ttu-id="4bef2-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="4bef2-565">msdyn_finish</span></span>                           | <span data-ttu-id="4bef2-566">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-566">yes</span></span>            | <span data-ttu-id="4bef2-567">да</span><span class="sxs-lookup"><span data-stu-id="4bef2-567">yes</span></span>          |
| <span data-ttu-id="4bef2-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="4bef2-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="4bef2-569">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-569">no</span></span>             | <span data-ttu-id="4bef2-570">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-570">no</span></span>           |
| <span data-ttu-id="4bef2-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="4bef2-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="4bef2-572">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-572">no</span></span>             | <span data-ttu-id="4bef2-573">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-573">no</span></span>           |
| <span data-ttu-id="4bef2-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="4bef2-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="4bef2-575">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-575">no</span></span>             | <span data-ttu-id="4bef2-576">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-576">no</span></span>           |
| <span data-ttu-id="4bef2-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="4bef2-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="4bef2-578">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-578">no</span></span>             | <span data-ttu-id="4bef2-579">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-579">no</span></span>           |
| <span data-ttu-id="4bef2-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="4bef2-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="4bef2-581">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-581">no</span></span>             | <span data-ttu-id="4bef2-582">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-582">no</span></span>           |
| <span data-ttu-id="4bef2-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="4bef2-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="4bef2-584">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-584">no</span></span>             | <span data-ttu-id="4bef2-585">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-585">no</span></span>           |
| <span data-ttu-id="4bef2-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="4bef2-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="4bef2-587">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-587">no</span></span>             | <span data-ttu-id="4bef2-588">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-588">no</span></span>           |
| <span data-ttu-id="4bef2-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="4bef2-590">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-590">no</span></span>             | <span data-ttu-id="4bef2-591">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-591">no</span></span>           |
| <span data-ttu-id="4bef2-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="4bef2-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="4bef2-593">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-593">no</span></span>             | <span data-ttu-id="4bef2-594">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-594">no</span></span>           |
| <span data-ttu-id="4bef2-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="4bef2-596">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-596">no</span></span>             | <span data-ttu-id="4bef2-597">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-597">no</span></span>           |
| <span data-ttu-id="4bef2-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="4bef2-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="4bef2-599">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-599">no</span></span>             | <span data-ttu-id="4bef2-600">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-600">no</span></span>           |
| <span data-ttu-id="4bef2-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="4bef2-602">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-602">no</span></span>             | <span data-ttu-id="4bef2-603">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-603">no</span></span>           |
| <span data-ttu-id="4bef2-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="4bef2-604">msdyn_progress</span></span>                         | <span data-ttu-id="4bef2-605">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-605">no</span></span>             | <span data-ttu-id="4bef2-606">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-606">no</span></span>           |
| <span data-ttu-id="4bef2-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="4bef2-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="4bef2-608">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-608">no</span></span>             | <span data-ttu-id="4bef2-609">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-609">no</span></span>           |
| <span data-ttu-id="4bef2-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="4bef2-611">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-611">no</span></span>             | <span data-ttu-id="4bef2-612">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-612">no</span></span>           |
| <span data-ttu-id="4bef2-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="4bef2-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="4bef2-614">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-614">no</span></span>             | <span data-ttu-id="4bef2-615">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-615">no</span></span>           |
| <span data-ttu-id="4bef2-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="4bef2-617">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-617">no</span></span>             | <span data-ttu-id="4bef2-618">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-618">no</span></span>           |
| <span data-ttu-id="4bef2-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="4bef2-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="4bef2-620">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-620">no</span></span>             | <span data-ttu-id="4bef2-621">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-621">no</span></span>           |
| <span data-ttu-id="4bef2-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="4bef2-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="4bef2-623">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-623">no</span></span>             | <span data-ttu-id="4bef2-624">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-624">no</span></span>           |
| <span data-ttu-id="4bef2-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="4bef2-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="4bef2-626">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-626">no</span></span>             | <span data-ttu-id="4bef2-627">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-627">no</span></span>           |
| <span data-ttu-id="4bef2-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="4bef2-629">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-629">no</span></span>             | <span data-ttu-id="4bef2-630">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-630">no</span></span>           |
| <span data-ttu-id="4bef2-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="4bef2-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="4bef2-632">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-632">no</span></span>             | <span data-ttu-id="4bef2-633">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-633">no</span></span>           |
| <span data-ttu-id="4bef2-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="4bef2-635">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-635">no</span></span>             | <span data-ttu-id="4bef2-636">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-636">no</span></span>           |
| <span data-ttu-id="4bef2-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="4bef2-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="4bef2-638">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-638">no</span></span>             | <span data-ttu-id="4bef2-639">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-639">no</span></span>           |
| <span data-ttu-id="4bef2-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="4bef2-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="4bef2-641">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-641">no</span></span>             | <span data-ttu-id="4bef2-642">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-642">no</span></span>           |
| <span data-ttu-id="4bef2-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="4bef2-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="4bef2-644">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-644">no</span></span>             | <span data-ttu-id="4bef2-645">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-645">no</span></span>           |
| <span data-ttu-id="4bef2-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="4bef2-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="4bef2-647">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-647">no</span></span>             | <span data-ttu-id="4bef2-648">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-648">no</span></span>           |
| <span data-ttu-id="4bef2-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="4bef2-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="4bef2-650">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-650">no</span></span>             | <span data-ttu-id="4bef2-651">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-651">no</span></span>           |
| <span data-ttu-id="4bef2-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="4bef2-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="4bef2-653">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-653">no</span></span>             | <span data-ttu-id="4bef2-654">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-654">no</span></span>           |
| <span data-ttu-id="4bef2-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="4bef2-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="4bef2-656">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-656">no</span></span>             | <span data-ttu-id="4bef2-657">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-657">no</span></span>           |
| <span data-ttu-id="4bef2-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="4bef2-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="4bef2-659">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-659">no</span></span>             | <span data-ttu-id="4bef2-660">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-660">no</span></span>           |
| <span data-ttu-id="4bef2-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="4bef2-662">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-662">no</span></span>             | <span data-ttu-id="4bef2-663">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-663">no</span></span>           |
| <span data-ttu-id="4bef2-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="4bef2-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="4bef2-665">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-665">no</span></span>             | <span data-ttu-id="4bef2-666">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-666">no</span></span>           |
| <span data-ttu-id="4bef2-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="4bef2-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="4bef2-668">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-668">no</span></span>             | <span data-ttu-id="4bef2-669">не</span><span class="sxs-lookup"><span data-stu-id="4bef2-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="4bef2-670">Известни проблеми и ограничения</span><span class="sxs-lookup"><span data-stu-id="4bef2-670">Limitations and known issues</span></span>
<span data-ttu-id="4bef2-671">Следва списък с ограничения и известни проблеми:</span><span class="sxs-lookup"><span data-stu-id="4bef2-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="4bef2-672">API на графика може да се използва само от **Потребители с лиценз за Microsoft Project.**</span><span class="sxs-lookup"><span data-stu-id="4bef2-672">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="4bef2-673">Те не могат да бъдат използвани от:</span><span class="sxs-lookup"><span data-stu-id="4bef2-673">They can't be used by:</span></span>
    - <span data-ttu-id="4bef2-674">Потребители на приложение</span><span class="sxs-lookup"><span data-stu-id="4bef2-674">Application users</span></span>
    - <span data-ttu-id="4bef2-675">Системни потребители</span><span class="sxs-lookup"><span data-stu-id="4bef2-675">System users</span></span>
    - <span data-ttu-id="4bef2-676">Потребители на интеграция</span><span class="sxs-lookup"><span data-stu-id="4bef2-676">Integration users</span></span>
    - <span data-ttu-id="4bef2-677">Други потребители, които нямат необходимия лиценз</span><span class="sxs-lookup"><span data-stu-id="4bef2-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="4bef2-678">Всеки **OperationSet** може да има максимум 100 операции.</span><span class="sxs-lookup"><span data-stu-id="4bef2-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="4bef2-679">Всеки потребител може да има максимум 10 отворени **OperationSets**.</span><span class="sxs-lookup"><span data-stu-id="4bef2-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="4bef2-680">Понастоящем Project Operations поддържа максимум 500 общо задачи по проект.</span><span class="sxs-lookup"><span data-stu-id="4bef2-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="4bef2-681">Състоянието на неуспех **OperationSet** и регистрационните файлове за неуспех в момента не са достъпни.</span><span class="sxs-lookup"><span data-stu-id="4bef2-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="4bef2-682">API за график са в публичен преглед.</span><span class="sxs-lookup"><span data-stu-id="4bef2-682">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="4bef2-683">Използването на тези API в производствена среда не се поддържа от Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4bef2-683">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>
- [<span data-ttu-id="4bef2-684">Граници и ограничения на проекти и задачи</span><span class="sxs-lookup"><span data-stu-id="4bef2-684">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="4bef2-685">Грешка при обработването</span><span class="sxs-lookup"><span data-stu-id="4bef2-685">Error handling</span></span>

   - <span data-ttu-id="4bef2-686">За да прегледате грешките, генерирани от операционните набори, отидете на **Настройки** \> **График на интеграция** \> **Набори от операции**.</span><span class="sxs-lookup"><span data-stu-id="4bef2-686">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="4bef2-687">За да прегледате грешките, генерирани от услугата за планиране на проекти, отидете на **Настройки** \> **График на интеграция** \> **Регистрационни файлове за грешки в PSS**.</span><span class="sxs-lookup"><span data-stu-id="4bef2-687">To review errors generated from the Project Scheduling Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="4bef2-688">Примерен сценарий</span><span class="sxs-lookup"><span data-stu-id="4bef2-688">Sample scenario</span></span>

<span data-ttu-id="4bef2-689">В този сценарий ще създадете проект, член на екип, четири задачи и две задания за ресурси.</span><span class="sxs-lookup"><span data-stu-id="4bef2-689">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="4bef2-690">След това ще актуализирате една задача, ще актуализирате проекта, ще изтриете една задача, ще изтриете едно задание на ресурс и ще създадете зависимост от задачата.</span><span class="sxs-lookup"><span data-stu-id="4bef2-690">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="4bef2-691">Допълнителни проби</span><span class="sxs-lookup"><span data-stu-id="4bef2-691">Additional samples</span></span>

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
