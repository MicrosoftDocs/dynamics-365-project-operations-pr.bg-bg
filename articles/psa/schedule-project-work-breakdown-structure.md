---
title: Планиране на проект със съставна структура на работата
description: Как се планира проект със съставна структура на работата в Project Service
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: d77d9f8427f06015d4f4cb9438d7f59ac840b061
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4072002"
---
# <a name="schedule-a-project-with-a-work-breakdown-structure-project-service"></a><span data-ttu-id="41dab-103">Планиране на проект със съставна структура на работата (Project Service)</span><span class="sxs-lookup"><span data-stu-id="41dab-103">Schedule a project with a work breakdown structure (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="41dab-104">Графикът на проекта съобщава каква работа трябва да бъде извършена, кои ресурси ще изпълняват работата, както и времевата рамка, в която тази работа трябва да бъде завършена.</span><span class="sxs-lookup"><span data-stu-id="41dab-104">A project schedule communicates what work needs to be performed, which resources will perform the work, and the timeframe in which that work needs to be completed.</span></span> <span data-ttu-id="41dab-105">Графикът на проекта отразява цялата работа, свързана с предоставянето на проекта навреме.</span><span class="sxs-lookup"><span data-stu-id="41dab-105">The project schedule reflects all the work associated with delivering the project on time.</span></span> <span data-ttu-id="41dab-106">Една от първите стъпки в етапа на иницииране на проекта е да изготвите график на проекта.</span><span class="sxs-lookup"><span data-stu-id="41dab-106">One of the first steps in the initiation phase of the project is to come up with a project schedule.</span></span> <span data-ttu-id="41dab-107">За създаване на график на проект, трябва да създадете съставна структура на работата.</span><span class="sxs-lookup"><span data-stu-id="41dab-107">To establish a project schedule, you need to create a work breakdown structure.</span></span>  
  
 <span data-ttu-id="41dab-108">Създайте структура на проекта със съставна структура на работата, която ви помага за:</span><span class="sxs-lookup"><span data-stu-id="41dab-108">Create a project structure with a work breakdown structure, which helps you:</span></span>  
  
- <span data-ttu-id="41dab-109">Разбивка на работата на управляеми задачи</span><span class="sxs-lookup"><span data-stu-id="41dab-109">Break down work into manageable tasks</span></span>  
  
- <span data-ttu-id="41dab-110">Оценка на времето, необходимо за завършване на задача</span><span class="sxs-lookup"><span data-stu-id="41dab-110">Estimate the time required to complete a task</span></span>  
  
- <span data-ttu-id="41dab-111">Задаване на зависимости на задачи и продължителност на задачата</span><span class="sxs-lookup"><span data-stu-id="41dab-111">Set task dependencies and task duration</span></span>  
  
- <span data-ttu-id="41dab-112">Определяне на ролите, необходими за изпълнение на всяка задача</span><span class="sxs-lookup"><span data-stu-id="41dab-112">Determine the roles required to complete each task</span></span>  
  
  <span data-ttu-id="41dab-113">Графикът на проекта в съставна структура на работата изглежда познато в допълнение с интерактивна диаграма на Гант.</span><span class="sxs-lookup"><span data-stu-id="41dab-113">The project schedule in the work breakdown structure has a familiar look and feel, complete with an interactive Gantt chart.</span></span>  
  
## <a name="create-a-work-breakdown-structure-for-a-project"></a><span data-ttu-id="41dab-114">Създаване на съставна структура на работата за проект</span><span class="sxs-lookup"><span data-stu-id="41dab-114">Create a work breakdown structure for a project</span></span>  
 <span data-ttu-id="41dab-115">Създавайте съставна структура на работата, за да представите последователността от задачи в проект.</span><span class="sxs-lookup"><span data-stu-id="41dab-115">Create a work breakdown structure to represent the sequence of tasks in a project.</span></span> <span data-ttu-id="41dab-116">Съставната структура на работата включва задачи, изисквания за всяка задача и информация за приходите и разходите.</span><span class="sxs-lookup"><span data-stu-id="41dab-116">The work breakdown structure includes tasks, requirements for each task, and revenue and cost information.</span></span> <span data-ttu-id="41dab-117">В своята съставна структура на работата можете да добавите:</span><span class="sxs-lookup"><span data-stu-id="41dab-117">In your work breakdown structure, you can add:</span></span>  
  
-   <span data-ttu-id="41dab-118">Последователността на задачите в йерархия</span><span class="sxs-lookup"><span data-stu-id="41dab-118">The sequence of tasks in a hierarchy</span></span>  
  
-   <span data-ttu-id="41dab-119">Други задачи, ако има такива, които трябва да бъдат завършени, преди задачата да може да се стартира</span><span class="sxs-lookup"><span data-stu-id="41dab-119">Other tasks, if any, that must be completed before a task can be started</span></span>  
  
-   <span data-ttu-id="41dab-120">Началната дата, крайната дата и продължителността на задача</span><span class="sxs-lookup"><span data-stu-id="41dab-120">The starting date, ending date, and duration of a task</span></span>  
  
-   <span data-ttu-id="41dab-121">Брой часове, необходими за задача</span><span class="sxs-lookup"><span data-stu-id="41dab-121">The number of hours required for a task</span></span>  
  
-   <span data-ttu-id="41dab-122">Всички необходими умения и квалификации на работниците</span><span class="sxs-lookup"><span data-stu-id="41dab-122">Any required worker skills and education</span></span>  
  
-   <span data-ttu-id="41dab-123">Работниците, които са присвоени към дадена задача</span><span class="sxs-lookup"><span data-stu-id="41dab-123">The workers who are assigned to a task</span></span>  
  
-   <span data-ttu-id="41dab-124">Прогнозни приходи и разходи</span><span class="sxs-lookup"><span data-stu-id="41dab-124">Estimated revenue and costs</span></span>  
  
## <a name="task-types"></a><span data-ttu-id="41dab-125">Типове задачи</span><span class="sxs-lookup"><span data-stu-id="41dab-125">Task types</span></span>  
<span data-ttu-id="41dab-126">Можете да използвате следните типове задачи, когато създавате своята съставна структура на работата:</span><span class="sxs-lookup"><span data-stu-id="41dab-126">You’ll use the following types of tasks when creating your work breakdown structure:</span></span>  

| | | 
|---------------------------------------|-----------------------------------------------------------------| 
| <span data-ttu-id="41dab-127">**Основен възел на проект**.</span><span class="sxs-lookup"><span data-stu-id="41dab-127">**Project root node**</span></span> | <span data-ttu-id="41dab-128">Обобщаващата задача от най-високо ниво за проекта.</span><span class="sxs-lookup"><span data-stu-id="41dab-128">The top-level summary task for the project.</span></span> <span data-ttu-id="41dab-129">Всички останали задачи по проекта се създават под него.</span><span class="sxs-lookup"><span data-stu-id="41dab-129">All other project tasks are created under it.</span></span> <span data-ttu-id="41dab-130">Името на основната задача е името на проекта.</span><span class="sxs-lookup"><span data-stu-id="41dab-130">The name of the root task is the project name.</span></span> <span data-ttu-id="41dab-131">Усилията, датите и продължителността на основния възел се базират на стойностите в йерархията под него.</span><span class="sxs-lookup"><span data-stu-id="41dab-131">The effort, dates, and duration of the root node are based on the values on the hierarchy below it.</span></span> <span data-ttu-id="41dab-132">Не можете да редактирате свойства на основния възел или да изтриете основен възел.</span><span class="sxs-lookup"><span data-stu-id="41dab-132">You can’t edit root node properties or delete the root node.</span></span> | 
| <span data-ttu-id="41dab-133">**Обобщаващи задачи или задачи в контейнер**</span><span class="sxs-lookup"><span data-stu-id="41dab-133">**Summary or container tasks**</span></span> | <span data-ttu-id="41dab-134">Обобщаващата задача е задача, под която има подзадачи.</span><span class="sxs-lookup"><span data-stu-id="41dab-134">A summary task is a task that has sub-tasks under it.</span></span> <span data-ttu-id="41dab-135">Обобщаващата задача няма собствено усилия или разходи за работата.</span><span class="sxs-lookup"><span data-stu-id="41dab-135">A summary task doesn’t have any work effort or cost of its own.</span></span> <span data-ttu-id="41dab-136">Нейните усилия и разходи за работата са усреднен сбор на нейните подзадачи.</span><span class="sxs-lookup"><span data-stu-id="41dab-136">Its work effort and cost are a rollup of its sub-tasks.</span></span> <span data-ttu-id="41dab-137">Можете да промените името на обобщаваща задача, но не можете да променяте усилията, датите или продължителността, защото те се изчислява автоматично.</span><span class="sxs-lookup"><span data-stu-id="41dab-137">You can change the name of a summary task, but you can’t change the effort, dates, or duration, because those are automatically calculated.</span></span> <span data-ttu-id="41dab-138">С изтриването на обобщаваща задача се изтриват задачата и всички от нейни подзадачи.</span><span class="sxs-lookup"><span data-stu-id="41dab-138">Deleting a summary task deletes the task and all of its sub-tasks.</span></span>|  
| <span data-ttu-id="41dab-139">**Задачи на краен възел**</span><span class="sxs-lookup"><span data-stu-id="41dab-139">**Leaf node tasks**</span></span> | <span data-ttu-id="41dab-140">Задачата на краен възел представлява най-подробната работа по проекта.</span><span class="sxs-lookup"><span data-stu-id="41dab-140">A leaf node task represents the most detailed work on the project.</span></span> <span data-ttu-id="41dab-141">Тя има прогнозни усилия, планиран брой ресурси, планирани начална и крайна дати и продължителност.</span><span class="sxs-lookup"><span data-stu-id="41dab-141">It has an estimated effort, a planned number of resources, planned start and end dates, and a duration.</span></span>|

  
## <a name="task-hierarchy"></a><span data-ttu-id="41dab-142">Йерархия на задачи</span><span class="sxs-lookup"><span data-stu-id="41dab-142">Task hierarchy</span></span>  
 <span data-ttu-id="41dab-143">Имате следните опции при създаване на йерархия на задачи:</span><span class="sxs-lookup"><span data-stu-id="41dab-143">You have the following options when creating a task hierarchy:</span></span>  
  
- <span data-ttu-id="41dab-144">**Добавяне на задача**.</span><span class="sxs-lookup"><span data-stu-id="41dab-144">**Add task**.</span></span>   <span data-ttu-id="41dab-145">Можете да добавите задача на позиция, която изберете, в йерархията на задачите.</span><span class="sxs-lookup"><span data-stu-id="41dab-145">You can add a task at a position you choose in the task hierarchy.</span></span> <span data-ttu-id="41dab-146">Ако не изберете позиция, вашата нова задача се появява в края.</span><span class="sxs-lookup"><span data-stu-id="41dab-146">If you don’t select a position, your new task appears at the end.</span></span>  
  
- <span data-ttu-id="41dab-147">**Задача с отстъп**.</span><span class="sxs-lookup"><span data-stu-id="41dab-147">**Indent task**.</span></span>   <span data-ttu-id="41dab-148">Въведете задача с отстъп, за да я направите дъщерна на задачата, непосредствено над нея.</span><span class="sxs-lookup"><span data-stu-id="41dab-148">Indent a task to make it a child of the task directly above it.</span></span>  
  
- <span data-ttu-id="41dab-149">**Задача с обратен отстъп**.</span><span class="sxs-lookup"><span data-stu-id="41dab-149">**Outdent task**.</span></span>   <span data-ttu-id="41dab-150">Въведете задача с обратен отстъп, за да прекратите състоянието й на подзадача на първоначалната й родителска задача.</span><span class="sxs-lookup"><span data-stu-id="41dab-150">Outdent a task to make it so it’s no longer a sub-task of its original parent task.</span></span>  
  
- <span data-ttu-id="41dab-151">**Преместване нагоре и преместване надолу**.</span><span class="sxs-lookup"><span data-stu-id="41dab-151">**Move up and Move down**.</span></span>   <span data-ttu-id="41dab-152">Премествайте задачите нагоре и надолу в йерархията на родителските им задачи.</span><span class="sxs-lookup"><span data-stu-id="41dab-152">Move tasks up and down in the hierarchy of its parent task.</span></span> <span data-ttu-id="41dab-153">Преместване на задача нагоре или надолу няма ефект върху нейните усилия, разходи, дати или продължителност.</span><span class="sxs-lookup"><span data-stu-id="41dab-153">Moving a task up or down has no effect on its effort, cost, dates, or duration.</span></span>  
  
## <a name="task-attributes"></a><span data-ttu-id="41dab-154">Атрибути на задача</span><span class="sxs-lookup"><span data-stu-id="41dab-154">Task attributes</span></span>  
 <span data-ttu-id="41dab-155">Името на задача описва работата, която трябва да бъде извършена.</span><span class="sxs-lookup"><span data-stu-id="41dab-155">A task’s name describes the work that needs to be completed.</span></span> <span data-ttu-id="41dab-156">Използвате различни атрибути на задача, за да опишете графика и изискванията за персонал за задачата.</span><span class="sxs-lookup"><span data-stu-id="41dab-156">You use various task attributes to describe the schedule and staffing requirements for the task.</span></span>  
  
### <a name="schedule-attributes"></a><span data-ttu-id="41dab-157">Атрибути на графика</span><span class="sxs-lookup"><span data-stu-id="41dab-157">Schedule attributes</span></span>

 - <span data-ttu-id="41dab-158">Присвоете стойности км **Часове на усилие** , **Брой ресурси** , **Начална дата** , **Крайна дата** и **Продължителност** за определяне на график за изпълнение на задачата.</span><span class="sxs-lookup"><span data-stu-id="41dab-158">Assign values to **Effort hours** , **Number of resources** , **Start date** , **End date** , and **Duration** to determine the schedule for the task.</span></span> 
 - <span data-ttu-id="41dab-159">**Усилия** е прогноза за часовете, необходими за завършване на задачата.</span><span class="sxs-lookup"><span data-stu-id="41dab-159">**Effort** is an estimate of the hours it takes to complete the task.</span></span>
 - <span data-ttu-id="41dab-160">**Брой ресурси** е прогноза, която ръководителят на проекта поставя в задачата, за да помогне за изготвянето на най-добрия възможен график.</span><span class="sxs-lookup"><span data-stu-id="41dab-160">**Number of resources** is an estimate that the project manager puts in the task to help come up with the best possible schedule.</span></span> 
 - <span data-ttu-id="41dab-161">**Продължителност** (в дни) показва броя на работните дни, необходими за завършването на задачата.</span><span class="sxs-lookup"><span data-stu-id="41dab-161">**Duration** (in days) indicates the number of work days it will take to complete the task.</span></span>  
  
### <a name="staffing-attributes"></a><span data-ttu-id="41dab-162">Атрибути за персонал</span><span class="sxs-lookup"><span data-stu-id="41dab-162">Staffing attributes</span></span>

 - <span data-ttu-id="41dab-163">**Роля** , **Организационна единица на ресурс** , **Брой ресурси** и **Ресурси** описват изискванията за персонал за изпълнение на задачата.</span><span class="sxs-lookup"><span data-stu-id="41dab-163">**Role** , **Resource organizational unit** , **Number of resources** , and **Resources** describe the staffing requirements for the task.</span></span> 
 - <span data-ttu-id="41dab-164">**Роля** описва вида на ресурса, необходим за изпълнение на задачата.</span><span class="sxs-lookup"><span data-stu-id="41dab-164">**Role** describes the type of resource needed to perform the task.</span></span> 
 - <span data-ttu-id="41dab-165">**Организационна единица на ресурс** показва организационната единица, от която трябва да се ангажират ресурси за тази задача; това влияе и върху прогнозата за разходи и продажби на задачата, тъй като това се отчита при определяне на единичната продажна цена за ресурса.</span><span class="sxs-lookup"><span data-stu-id="41dab-165">**Resource organizational unit** indicates the organizational unit from which resources should be staffed for that task; this also impacts the cost and sales estimate of the task, since this is accounted for when determining the unit sales price for the resource.</span></span> 
 - <span data-ttu-id="41dab-166">**Ресурси** съдържа общ ресурс или именован ресурс, когато бъде намерен такъв.</span><span class="sxs-lookup"><span data-stu-id="41dab-166">**Resources** holds a generic resource or a named resource when one is found.</span></span>  
  
## <a name="task-dependencies"></a><span data-ttu-id="41dab-167">Зависимости на задачите</span><span class="sxs-lookup"><span data-stu-id="41dab-167">Task dependencies</span></span>  
 <span data-ttu-id="41dab-168">Можете да създадете предшестващи релации между една или повече задачи в съставната структура на работата.</span><span class="sxs-lookup"><span data-stu-id="41dab-168">You can create predecessor relationships between one or more tasks in the work breakdown structure.</span></span> <span data-ttu-id="41dab-169">Можете да зададете една или повече стойности за полето за предшестваща задача за задачите, за да укажете задачите, от които ще зависи.</span><span class="sxs-lookup"><span data-stu-id="41dab-169">You can set one or more values for the predecessor field on tasks to indicate the tasks that it will be dependent on.</span></span> <span data-ttu-id="41dab-170">Когато присвоите стойност на предшестваща задача към задача, задачата може да започне само когато са завършени всички предшестващи задачи.</span><span class="sxs-lookup"><span data-stu-id="41dab-170">When you assign a predecessor value to a task, the task can only start when all the predecessor tasks have completed.</span></span> <span data-ttu-id="41dab-171">Определяне на тази зависимост за дадена задача ще доведе до преизчисляване на планираната начална дата на задачата като последната крайна дата за всички нейни предшестващи задачи.</span><span class="sxs-lookup"><span data-stu-id="41dab-171">Setting this dependency on a task will result in the recalculation of the planned start date of the task as the latest end of all of its predecessors.</span></span> <span data-ttu-id="41dab-172">Свързаните с предшестващите задачи въздействия в даден график не са ограничени от режима на задачи, определен за задачата.</span><span class="sxs-lookup"><span data-stu-id="41dab-172">Predecessor-related impacts on a schedule are not limited by the task mode defined on the task.</span></span>  
  
## <a name="task-mode"></a><span data-ttu-id="41dab-173">Режим на задачи</span><span class="sxs-lookup"><span data-stu-id="41dab-173">Task mode</span></span>  
 <span data-ttu-id="41dab-174">Режимът на задачи е един от най важните фактори, които определят планирането на задачи на краен възел.</span><span class="sxs-lookup"><span data-stu-id="41dab-174">Task mode is one of the important factors that determine scheduling leaf node tasks.</span></span> <span data-ttu-id="41dab-175">Има два режима на задача за всяка задача: режим на автоматично планиране и режим на ръчно планиране.</span><span class="sxs-lookup"><span data-stu-id="41dab-175">There are two task modes for every task: auto scheduling mode and manual scheduling mode.</span></span>  
  
-   <span data-ttu-id="41dab-176">**Автоматично планиране**.</span><span class="sxs-lookup"><span data-stu-id="41dab-176">**Auto scheduling**.</span></span>   <span data-ttu-id="41dab-177">Когато зададете режима на задачите на „Автоматично планиране“, системата за планиране на задачи използва правилата за планиране на следните атрибути на задачата, за да определи графика за изпълнение на задачата:</span><span class="sxs-lookup"><span data-stu-id="41dab-177">When you set the task mode to Automatically Scheduled, the task scheduling engine uses the scheduling rules on the following task attributes to determine the schedule for the task:</span></span>  
  
    -   <span data-ttu-id="41dab-178">Предшественици</span><span class="sxs-lookup"><span data-stu-id="41dab-178">Predecessors</span></span>  
  
    -   <span data-ttu-id="41dab-179">Усилие</span><span class="sxs-lookup"><span data-stu-id="41dab-179">Effort</span></span>  
  
    -   <span data-ttu-id="41dab-180">Брой на ресурсите</span><span class="sxs-lookup"><span data-stu-id="41dab-180">Number of resources</span></span>  
  
    -   <span data-ttu-id="41dab-181">Начална и крайна дати</span><span class="sxs-lookup"><span data-stu-id="41dab-181">Start and end dates</span></span>  
  
-   <span data-ttu-id="41dab-182">**Правила за планиране**.</span><span class="sxs-lookup"><span data-stu-id="41dab-182">**Scheduling rules**.</span></span>   <span data-ttu-id="41dab-183">Началната дата на задача на краен възел, която няма предшественици, се въвежда като начална дата в графика на проекта.</span><span class="sxs-lookup"><span data-stu-id="41dab-183">The start date of a leaf node task that does not have predecessors defaults to the project’s scheduling start date.</span></span> <span data-ttu-id="41dab-184">Продължителността на задачата на краен възел винаги се изчислява като броя на работните дни между началната и крайната дати.</span><span class="sxs-lookup"><span data-stu-id="41dab-184">The duration of a leaf node task is always calculated as the number of working days between its start and end dates.</span></span> <span data-ttu-id="41dab-185">Когато дадена задача е автоматично планирана, системата за планиране следва правилата по-долу:</span><span class="sxs-lookup"><span data-stu-id="41dab-185">When a task is automatically scheduled, the scheduling engine follows the rules below:</span></span>  
  
    -   <span data-ttu-id="41dab-186">Началната и крайната дати на задача трябва винаги да са работни дни съгласно календара за планиране на проекта</span><span class="sxs-lookup"><span data-stu-id="41dab-186">Start and end dates of a task must always be working days according to the project’s scheduling calendar</span></span>  
  
    -   <span data-ttu-id="41dab-187">Началната дата на задача, която има предшественици, се въвежда според последната крайна дата на предшествениците си</span><span class="sxs-lookup"><span data-stu-id="41dab-187">The start date of a task that has predecessors defaults to the latest end date of its predecessors</span></span>  
  
    -   <span data-ttu-id="41dab-188">Усилие = Брой хора \* продължителност \* часове в един стандартен работен ден от календара на проекта</span><span class="sxs-lookup"><span data-stu-id="41dab-188">Effort = Number of people \* Duration \* hours in a standard work day of the project calendar</span></span>  
  
-   <span data-ttu-id="41dab-189">**Ръчно планиране**.</span><span class="sxs-lookup"><span data-stu-id="41dab-189">**Manual scheduling**.</span></span>   <span data-ttu-id="41dab-190">В някои случаи може да искате да се отклоните от тези правила.</span><span class="sxs-lookup"><span data-stu-id="41dab-190">In some cases, you might want to deviate from these rules.</span></span> <span data-ttu-id="41dab-191">В тези случаи можете да зададете режима на задачите а съответната задача на ръчно планиране.</span><span class="sxs-lookup"><span data-stu-id="41dab-191">In these cases, you can set the task mode for the task to be manually scheduled.</span></span> <span data-ttu-id="41dab-192">Това спира системата за планиране от изчисляване на стойностите за други атрибути на планиране.</span><span class="sxs-lookup"><span data-stu-id="41dab-192">This stops the scheduling engine from calculating the values for other scheduling attributes.</span></span> <span data-ttu-id="41dab-193">Определянето на предшествениците на задачите винаги въздейства върху началната дата на зависимата задача.</span><span class="sxs-lookup"><span data-stu-id="41dab-193">Setting predecessors on tasks always impacts the dependent task’s start date.</span></span>  
  
## <a name="create-a-work-breakdown-structure"></a><span data-ttu-id="41dab-194">Създаване на съставна структура на работата</span><span class="sxs-lookup"><span data-stu-id="41dab-194">Create a work breakdown structure</span></span>  
  
1.  <span data-ttu-id="41dab-195">Отидете на **Project Service > Проекти**.</span><span class="sxs-lookup"><span data-stu-id="41dab-195">Go to **Project Service > Projects**.</span></span>  
  
2.  <span data-ttu-id="41dab-196">Щракнете върху проекта, върху който искате да работите.</span><span class="sxs-lookup"><span data-stu-id="41dab-196">Click the project you want to work on.</span></span>  
  
3.  <span data-ttu-id="41dab-197">В лентата в горната част на екрана изберете стрелката за падащо меню до името на проекта и след това щракнете върху „Съставна структура на работата“.</span><span class="sxs-lookup"><span data-stu-id="41dab-197">In the bar across the top of the screen, select the down arrow next to the project name, and then click Work breakdown structure.</span></span>  
  
4.  <span data-ttu-id="41dab-198">За да добавите задача, щракнете върху **Добавяне на задача**.</span><span class="sxs-lookup"><span data-stu-id="41dab-198">To add a task, click **Add Task**.</span></span> <span data-ttu-id="41dab-199">Попълнете полетата за задачата и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="41dab-199">Fill in the fields for the task, and then click **Save**.</span></span>  
  
5.  <span data-ttu-id="41dab-200">Продължете да добавяте задачи, докато съставната структура на работата не бъде запълнена.</span><span class="sxs-lookup"><span data-stu-id="41dab-200">Continue adding tasks until your work breakdown structure is complete.</span></span> <span data-ttu-id="41dab-201">Докато създавате съставната структура на работата, можете да направите следното, за да организирате задачите си:</span><span class="sxs-lookup"><span data-stu-id="41dab-201">While creating your work breakdown structure, you can do the following to organize your tasks:</span></span>  
  
    -   <span data-ttu-id="41dab-202">Изберете задача и щракнете върху **Отстъп** , за да я преместите под друг задача, или щракнете върху „Обратен отстъп“, за да я преместите с едно ниво нагоре.</span><span class="sxs-lookup"><span data-stu-id="41dab-202">Select a task and click **Indent** to move it under another task or click Outdent to move it out a level.</span></span>  
  
    -   <span data-ttu-id="41dab-203">Изберете задача и щракнете върху **Премести нагоре** или **Премести надолу** , за да я преместите нагоре или надолу в списъка.</span><span class="sxs-lookup"><span data-stu-id="41dab-203">Select a task and click **Move Up** or **Move Down** to move it up or down in the list.</span></span>  
  
    -   <span data-ttu-id="41dab-204">Щракнете върху **Скриване на Гант** , за да скриете диаграмата на Гант, и щракнете върху **Показване на Гант** , за да я покажете отново.</span><span class="sxs-lookup"><span data-stu-id="41dab-204">Click **Hide Gantt** to hide the Gantt chart, and click **Show Gantt** to display it again.</span></span>  
  
    -   <span data-ttu-id="41dab-205">Изберете друг период от време за диаграмата на Гант във **Времева скала**.</span><span class="sxs-lookup"><span data-stu-id="41dab-205">Select a different period of time for the Gantt chart in **Time Scale**.</span></span>  
  
6.  <span data-ttu-id="41dab-206">За да добавите ролите, които сте определили в съставната структура на работата за членовете на екипа по проекта, щракнете върху **Генериране на екип по проекта**.</span><span class="sxs-lookup"><span data-stu-id="41dab-206">To add the roles you specified in your work breakdown structure to your project’s team members, click **Generate Project Team**.</span></span>  
  
7.  <span data-ttu-id="41dab-207">Щракнете върху **Запиши** в долния десен ъгъл на екрана, когато сте готови с промените.</span><span class="sxs-lookup"><span data-stu-id="41dab-207">Click **Save** at the bottom right corner of the screen when you’re done making changes.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="41dab-208">Вижте също</span><span class="sxs-lookup"><span data-stu-id="41dab-208">See Also</span></span>  
 [<span data-ttu-id="41dab-209">Ръководство за мениджъри на проекти</span><span class="sxs-lookup"><span data-stu-id="41dab-209">Project manager guide</span></span>](../psa/project-manager-guide.md)
