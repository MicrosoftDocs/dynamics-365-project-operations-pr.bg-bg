---
title: Управление на ресурсите
description: Тази тема предоставя информация за това как можете да управлявате ресурсите.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/13/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 39893019-123b-4bc6-8a2b-a37bc517dc97
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 6c199cbadd1c78e7e29c0cda0febde4236a13d96
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749372"
---
# <a name="manage-resources"></a><span data-ttu-id="2afd8-103">Управление на ресурсите</span><span class="sxs-lookup"><span data-stu-id="2afd8-103">Manage resources</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="2afd8-104">Dynamics 365 Project Service Automation включва табло за управление на ресурси, което предоставя визуален преглед на търсенето и използването на ресурси в цялата организация.</span><span class="sxs-lookup"><span data-stu-id="2afd8-104">Dynamics 365 Project Service Automation includes a resource manager dashboard that provides a visual overview of resource demand and utilization throughout the organization.</span></span> <span data-ttu-id="2afd8-105">Можете да използвате диаграмите в това табло, за да визуализирате следната информация:</span><span class="sxs-lookup"><span data-stu-id="2afd8-105">You can use the charts on this dashboard to visualize the following information:</span></span>

- <span data-ttu-id="2afd8-106">**Търсене на ресурси** – диаграмата **Заявки за активни ресурси** показва ресурсите, които са били подадени.</span><span class="sxs-lookup"><span data-stu-id="2afd8-106">**Resource demand** – The **Active Resource Request** chart shows resources that have been submitted.</span></span> <span data-ttu-id="2afd8-107">Ресурсите се обобщават по роля или по проект.</span><span class="sxs-lookup"><span data-stu-id="2afd8-107">The resources are aggregated by either role or project.</span></span>
- <span data-ttu-id="2afd8-108">**Търсене на неподадени ресурси** – диаграмата **Търсене на неприсвоени ресурси** показва всички изисквания за ресурси, които не са били подадени.</span><span class="sxs-lookup"><span data-stu-id="2afd8-108">**Unsubmitted resource demand** – The **Unassigned Resource Demand** chart shows all the resource requirements that haven't been submitted.</span></span> <span data-ttu-id="2afd8-109">Тя помага на мениджърите на ресурси да преглеждат търсене, което не е твърдо и може да бъде подадено чрез заявка за ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-109">It helps resource managers view demand that isn't firm and might be submitted through a resource request.</span></span>
- <span data-ttu-id="2afd8-110">**Отработено използване за изминалата седмица** – диаграмата **Използване по роля** показва процента на действителното отработено използване на организацията по роля спрямо целевото отработено използване по роля.</span><span class="sxs-lookup"><span data-stu-id="2afd8-110">**Billable utilization for the past week** – The **Utilization by Role** chart shows the percentage of the organization's actual billable utilization by role against its target billable utilization by role.</span></span>

    > [!NOTE]
    > <span data-ttu-id="2afd8-111">За да направите налична диаграмата **Използване по роля**, създайте задача, която изпълнява работния поток UpdateRoleUtilization.</span><span class="sxs-lookup"><span data-stu-id="2afd8-111">To make the **Utilization by Role** chart available, create a job that runs the UpdateRoleUtilization workflow.</span></span> <span data-ttu-id="2afd8-112">Тази повтаряща се задача се изпълнява на всеки седем дни, за да се изчисли отработеното използване за предходните седем дни.</span><span class="sxs-lookup"><span data-stu-id="2afd8-112">This recurring job runs every seven days to calculate billable utilization for the previous seven days.</span></span> <span data-ttu-id="2afd8-113">Резултатите се обобщават по роля.</span><span class="sxs-lookup"><span data-stu-id="2afd8-113">The results are aggregated by role.</span></span>

## <a name="manage-project-team-members"></a><span data-ttu-id="2afd8-114">Управление на членове на екип по проект</span><span class="sxs-lookup"><span data-stu-id="2afd8-114">Manage project team members</span></span>

<span data-ttu-id="2afd8-115">Мениджърите на проекти могат да използват таблото за управление на ресурси за управление на ресурси по проекти.</span><span class="sxs-lookup"><span data-stu-id="2afd8-115">Project managers can use the resource manager dashboard to manage the resources on projects.</span></span> <span data-ttu-id="2afd8-116">Те могат например да добавят член на екипа директно към проект и да резервират член на екипа за изпълнение на изискванията за ресурси, които са били записани от общ ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-116">For example, they can add a team member directly to a project and book a team member to fulfill the resource requirements that were captured by a generic resource.</span></span>

### <a name="add-a-team-member-directly-to-a-project"></a><span data-ttu-id="2afd8-117">Добавяне на член на екипа директно към проект</span><span class="sxs-lookup"><span data-stu-id="2afd8-117">Add a team member directly to a project</span></span>

<span data-ttu-id="2afd8-118">За да добавите член на екипа директно към проект, на страницата **Проекти**, в раздела **Екип** изберете **Нов**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-118">To add a team member directly to a project, on the **Projects** page, on the **Team** tab, select **New**.</span></span> <span data-ttu-id="2afd8-119">Показва се диалоговият прозорец **Бързо създаване: член на екипа на проекта**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-119">The **Quick Create:Project Team Member** dialog box appears.</span></span> <span data-ttu-id="2afd8-120">В този диалогов прозорец можете да изпълнявате следните задачи:</span><span class="sxs-lookup"><span data-stu-id="2afd8-120">In this dialog box, you can perform these tasks:</span></span>

- <span data-ttu-id="2afd8-121">**Резервиране на именуван ресурс** – в полето **Наличен ресурс** изберете името на ресурса.</span><span class="sxs-lookup"><span data-stu-id="2afd8-121">**Book a named resource** – In the **Bookable Resource** field, select the name of the resource.</span></span> <span data-ttu-id="2afd8-122">След това изберете ролята, задайте периода и изберете метод на разпределение.</span><span class="sxs-lookup"><span data-stu-id="2afd8-122">Then select the role, set the period, and select an allocation method.</span></span> <span data-ttu-id="2afd8-123">Наименуван ресурс, който сте избрали, се добавя към проекта с помощта на избрания метод на разпределение и календара на ресурсите.</span><span class="sxs-lookup"><span data-stu-id="2afd8-123">The named resource that you selected is added to the project by using the selected allocation method and the resources calendar.</span></span>
- <span data-ttu-id="2afd8-124">**Добавяне на общ ресурс** – оставете полето **Наличен ресурс** празно и след това изберете ролята, задайте периода и изберете предпочитания метод на разпределение.</span><span class="sxs-lookup"><span data-stu-id="2afd8-124">**Add a generic resource** – Leave the **Bookable resource** field blank, and then select the role, set the period, and select the preferred allocation method.</span></span> <span data-ttu-id="2afd8-125">Общ ресурс се добавя към екипа като контейнер, за да съхранява шаблона за търсене, който се използва за резервиране на наименувани ресурси в екипа.</span><span class="sxs-lookup"><span data-stu-id="2afd8-125">A generic resource is added to the team as a placeholder to hold the demand pattern that is used to book named resources on the team.</span></span> <span data-ttu-id="2afd8-126">Изискването се извършва в съответствие с календара на проекта.</span><span class="sxs-lookup"><span data-stu-id="2afd8-126">The requirement is made according to the project calendar.</span></span>
- <span data-ttu-id="2afd8-127">**Добавяне на наименуван ресурс към екипа, без да се изразходва капацитет** – в полето **Наличен ресурс** изберете ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-127">**Add a named resource to the team without consuming resource capacity** – In the **Bookable Resource** field, select a resource.</span></span> <span data-ttu-id="2afd8-128">След това изберете периода **Няма** като метод на разпределение.</span><span class="sxs-lookup"><span data-stu-id="2afd8-128">Then select the period, and select **None** as the allocation method.</span></span> <span data-ttu-id="2afd8-129">Ресурсът се добавя към екипа, но капацитетът на ресурса не се изразходва чрез резервация.</span><span class="sxs-lookup"><span data-stu-id="2afd8-129">The resource is added to the team, but the resource's capacity isn't consumed through a booking.</span></span>

### <a name="book-a-team-member-to-fulfill-resource-requirements-for-a-generic-resource"></a><span data-ttu-id="2afd8-130">Резервиране на член на екипа за изпълнение на изискванията за ресурси за общ ресурс</span><span class="sxs-lookup"><span data-stu-id="2afd8-130">Book a team member to fulfill resource requirements for a generic resource</span></span>

<span data-ttu-id="2afd8-131">В PSA можете да резервирате общ ресурс в екип по проект и да укажете ролята, необходимия капацитет и начина на разпределение на този капацитет.</span><span class="sxs-lookup"><span data-stu-id="2afd8-131">In PSA, you can book a generic resource on a project team, and can specify the role, the required capacity, and how that capacity is distributed.</span></span> <span data-ttu-id="2afd8-132">В изискването за ресурс можете да укажете атрибути, които са свързани с общия ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-132">On the resource requirement, you can specify attributes that are associated with the generic resource.</span></span> <span data-ttu-id="2afd8-133">Тези атрибути включват изискваните умения, предпочитаната организационна единица и предпочитаните ресурси.</span><span class="sxs-lookup"><span data-stu-id="2afd8-133">These attributes include required skills, the preferred organizational unit, and preferred resources.</span></span>

<span data-ttu-id="2afd8-134">Следвайте тези стъпки, за да укажете необходимите умения за общ ресурс за разработчик.</span><span class="sxs-lookup"><span data-stu-id="2afd8-134">Follow these steps to specify required skills on a generic resource for a developer.</span></span>

1. <span data-ttu-id="2afd8-135">На страницата **Проекти** в раздела **Екип** изберете **Нов** за резервиране на общ ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-135">On the **Projects** page, on the **Team** tab, select **New** to book a generic resource.</span></span>

    ![Общ ресурс, резервиран за екипа](media/Resource-Management-image9.png)

2. <span data-ttu-id="2afd8-137">В изгледа **Всички членове на екипа**, в колоната **Изискване за ресурс**, изберете връзката, за да добавите необходимите умения за общия ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-137">In the **All Team Members** view, in the **Resource Requirement** column, select the link to add required skills for the generic resource.</span></span>

    ![Връзка към изисквания](media/Resource-Management-image10.png)

3. <span data-ttu-id="2afd8-139">На страницата **Изискване за ресурс**, която се показва в мрежата **Умения**, изберете многоточието (**...**) и след това изберете **Добавяне на нова характеристика на изискване**, за да добавите необходимите умения за вашия разработчик.</span><span class="sxs-lookup"><span data-stu-id="2afd8-139">On the **Resource Requirement** page that appears, in the **Skills** grid, select the ellipsis (**...**) and then select **Add New Requirement Characteristic** to add the required skills for your developer.</span></span>

    ![Команда „Добавяне на нова характеристика на изискване“](media/Resource-Management-image11.png)

4. <span data-ttu-id="2afd8-141">В диалоговия прозорец **Бързо създаване: характеристика на изискване**, който се показва, в полето **Характеристика** изберете необходимото умение.</span><span class="sxs-lookup"><span data-stu-id="2afd8-141">In the **Quick Create: Requirement Characteristic** dialog box that appears, in the **Characteristic** field, select the required skill.</span></span> <span data-ttu-id="2afd8-142">След това в полето **Стойност на оценка** изберете нивото на опитност за това умение.</span><span class="sxs-lookup"><span data-stu-id="2afd8-142">Then, in the **Rating value** field, select the proficiency level for that skill.</span></span> <span data-ttu-id="2afd8-143">И накрая, в полето **Изискване за ресурс** задайте изискването на изходни ресурси от организационни единици или дори наименувани ресурси.</span><span class="sxs-lookup"><span data-stu-id="2afd8-143">Finally, in the **Resource Requirement** field, set the requirement to source resources from organizational units or even named resources.</span></span> <span data-ttu-id="2afd8-144">Когато сте готови, изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-144">When you've finished, select **Save**.</span></span>

    ![Диалогов прозорец „Бързо създаване: характеристика на изискване“](media/Resource-Management-image12.png)

5. <span data-ttu-id="2afd8-146">На страницата **Изисквания за ресурс** изберете **Резервиране**, за да изпълните изискването за ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-146">On the **Resource Requirement** page, select **Book** to fulfill the resource requirement.</span></span>

    ![Бутон „Резервиране“ на страницата „Изискване за ресурс“](media/Resource-Management-image13.png)

    <span data-ttu-id="2afd8-148">Можете също да изберете общия ресурс в мрежата **Всички членове на екипа** и след това да изберете **Резервиране**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-148">You can also select the generic resource in the **All Team Members** grid and then select **Book**.</span></span>

    ![Бутон „Резервиране“ над мрежата „Всички членове на екипа“](media/Resource-Management-image14.png)

    > [!NOTE]
    > <span data-ttu-id="2afd8-150">В този пример има 40 задължителни часа, но няма действителни резервирани часове, тъй като общите ресурси нямат резервации.</span><span class="sxs-lookup"><span data-stu-id="2afd8-150">In this example, there are 40 required hours but no actual booked hours, because generic resources don't have bookings.</span></span> <span data-ttu-id="2afd8-151">Освен това няма присвоени часове, тъй като общият ресурс е добавен директно към екипа.</span><span class="sxs-lookup"><span data-stu-id="2afd8-151">Additionally, there are no assigned hours, because the generic resource was added directly to the team.</span></span> <span data-ttu-id="2afd8-152">Той не е добавен с помощта на присвояване на задача.</span><span class="sxs-lookup"><span data-stu-id="2afd8-152">It wasn't added by using task assignment.</span></span>

    <span data-ttu-id="2afd8-153">На страницата **Асистент за планиране** можете да филтрирате наличните ресурси по изискванията, които са указани в изискването за ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-153">On the **Scheduling Assistant** page, you can filter available resources by the requirements that are specified on the resource requirement.</span></span> <span data-ttu-id="2afd8-154">Ресурсите се сортират според параметрите за сортиране, указани в таблото на графика.</span><span class="sxs-lookup"><span data-stu-id="2afd8-154">Resources are sorted according to the sorting parameters that are specified on the Schedule Board.</span></span>

    ![Страница „Асистент за планиране“](media/Resource-Management-image15.png)

    <span data-ttu-id="2afd8-156">Ето някои филтри, които често се използват:</span><span class="sxs-lookup"><span data-stu-id="2afd8-156">Here are some filters that are often used:</span></span>

    - <span data-ttu-id="2afd8-157">**Характеристики заедно с рейтинг** – филтриране по умения, сертификати и други качества на ресурсите в допълнение към оценките за опитност.</span><span class="sxs-lookup"><span data-stu-id="2afd8-157">**Characteristics along with a rating** – Filter by skills, certifications, and other resource qualities, in addition to ratings of proficiency.</span></span>
    - <span data-ttu-id="2afd8-158">**Роли** – филтриране по роли по подразбиране, които са присвоени на налични ресурси.</span><span class="sxs-lookup"><span data-stu-id="2afd8-158">**Roles** – Filter by the default roles that are assigned to bookable resources.</span></span>
    - <span data-ttu-id="2afd8-159">**Организационни единици** – филтриране на наличните ресурси по организационните единици, към които са присвоени.</span><span class="sxs-lookup"><span data-stu-id="2afd8-159">**Organizational units** – Filter bookable resources by the organizational units that they are assigned to.</span></span>

6. <span data-ttu-id="2afd8-160">Ако не сте доволни от резултатите от първоначалното търсене по изискване, можете да промените критериите за филтриране.</span><span class="sxs-lookup"><span data-stu-id="2afd8-160">If you aren't satisfied with the results of the initial requirement search, you can change the filter criteria.</span></span> <span data-ttu-id="2afd8-161">Разгънете прозореца **Изглед на филтър** отляво и след това изберете **Търсене**, за да намерите допълнителни ресурси.</span><span class="sxs-lookup"><span data-stu-id="2afd8-161">Expand the **Filter View** pane on the left, and then select **Search** to find additional resources.</span></span>

    ![Прозорец „Изглед на филтър“](media/Resource-Management-image16.png)

7. <span data-ttu-id="2afd8-163">За да промените начина на сортиране на резултатите, изберете **Сортиране**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-163">To change how the results are sorted, select **Sort**.</span></span>

    ![Команда „Сортиране“](media/Resource-Management-image17.png)

8. <span data-ttu-id="2afd8-165">Изберете ресурси според търсенето, което е указано в изискването, както е посочено в горната част на мрежата.</span><span class="sxs-lookup"><span data-stu-id="2afd8-165">Select resources according to the demand that is specified on the requirement, as indicated at the top of the grid.</span></span> <span data-ttu-id="2afd8-166">Можете да изчистите селекцията от клетки в мрежата и да оставите капацитета на този ресурс отворен.</span><span class="sxs-lookup"><span data-stu-id="2afd8-166">You can clear the selection of cells in the grid and leave that resource capacity open.</span></span> <span data-ttu-id="2afd8-167">Само един ресурс в даден момент може да бъде избран като резервиран.</span><span class="sxs-lookup"><span data-stu-id="2afd8-167">Only one resource at a time can be selected as booked.</span></span>

9. <span data-ttu-id="2afd8-168">Изберете **Резервиране**, за да резервирате избрания ресурс, и оставете таблото на графика отворено, така че да можете да изберете допълнителни ресурси.</span><span class="sxs-lookup"><span data-stu-id="2afd8-168">Select **Book** to book the selected resource and leave the Schedule Board open, so that you can select additional resources.</span></span> <span data-ttu-id="2afd8-169">Или изберете **Резервиране и изход**, за да резервирате избрания ресурс и да затворите таблото на графика.</span><span class="sxs-lookup"><span data-stu-id="2afd8-169">Alternatively, select **Book & Exit** to book the selected resource and close the Schedule Board.</span></span>

    ![Ресурс за резервиране](media/Resource-Management-image19.png)

    <span data-ttu-id="2afd8-171">Получавате известие за резервираните часове.</span><span class="sxs-lookup"><span data-stu-id="2afd8-171">You receive a notification about booked hours.</span></span> <span data-ttu-id="2afd8-172">Индикаторите на търсенето показват колко от изискването за резервация е изпълнено и колко остава.</span><span class="sxs-lookup"><span data-stu-id="2afd8-172">The demand indicators show how much the booking requirement is satisfied and how much remains.</span></span> <span data-ttu-id="2afd8-173">Можете също да видите каква част от капацитета на избрания ресурс е изразходена.</span><span class="sxs-lookup"><span data-stu-id="2afd8-173">You can also see how much of the selected resource's capacity is consumed.</span></span> <span data-ttu-id="2afd8-174">Изберете **Разгъване**, за да видите повече подробности за резервациите на ресурси.</span><span class="sxs-lookup"><span data-stu-id="2afd8-174">Select **Expand** to view more details about resource bookings.</span></span>

9. <span data-ttu-id="2afd8-175">Върнете се към изгледа **Всички членове на екипа**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-175">Return to the **All Team Members** view.</span></span> <span data-ttu-id="2afd8-176">В мрежата забележете, че общият ресурс е заменен с наименуван ресурс и 40 часа са посочени като резервирани за този ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-176">In the grid, notice that the generic resource has been replaced by the named resource, and 40 hours are listed as booked for that resource.</span></span>

    ![Актуализирана мрежа „Всички членове на екипа“](media/Resource-Management-image20.png)

    > [!NOTE]
    > <span data-ttu-id="2afd8-178">Не са показани присвоени часове, защото те са резервирани директно в екипа.</span><span class="sxs-lookup"><span data-stu-id="2afd8-178">No assigned hours are shown, because they were booked directly on the team.</span></span> <span data-ttu-id="2afd8-179">Те не са резервирани с помощта на присвояване на задача.</span><span class="sxs-lookup"><span data-stu-id="2afd8-179">They weren't booked by using task assignment.</span></span>

## <a name="assign-generic-resources-to-tasks-and-generate-resource-requirements"></a><span data-ttu-id="2afd8-180">Присвояване на общи ресурси на задачи и генериране на изисквания за ресурси</span><span class="sxs-lookup"><span data-stu-id="2afd8-180">Assign generic resources to tasks and generate resource requirements</span></span>

<span data-ttu-id="2afd8-181">В PSA можете да създавате задачи и след това да присвоявате общи ресурси на тях.</span><span class="sxs-lookup"><span data-stu-id="2afd8-181">In PSA, you can create tasks and then assign generic resources to them.</span></span> <span data-ttu-id="2afd8-182">По този начин търсенето на ресурси може да бъде представено от контейнери, докато изчислявате графика и финансовите средства.</span><span class="sxs-lookup"><span data-stu-id="2afd8-182">In this way, resource demand can be represented by placeholders while you estimate your schedule and financial numbers.</span></span> <span data-ttu-id="2afd8-183">След това можете да генерирате изисквания за ресурси за общите ресурси и да ги изпълните.</span><span class="sxs-lookup"><span data-stu-id="2afd8-183">You can then generate resource requirements for the generic resources and fulfill them.</span></span>

1. <span data-ttu-id="2afd8-184">На страницата **Проекти**, в раздела **График** изберете **Добавяне**, за да създадете задача.</span><span class="sxs-lookup"><span data-stu-id="2afd8-184">On the **Projects** page, on the **Schedule** tab, select **Add** to create a task.</span></span>

    ![Създадена нова задача](media/Resource-Management-image21.png)

2. <span data-ttu-id="2afd8-186">В полето **Ресурси** изберете символа **Избор на ресурси**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-186">In the **Resources** field, select the **Resource Picker** symbol.</span></span> <span data-ttu-id="2afd8-187">Изборът на ресурси се появява и показва съществуващите членове на екипа за проекта.</span><span class="sxs-lookup"><span data-stu-id="2afd8-187">The Resource Picker appears and shows existing team members for the project.</span></span>

    ![Избор на ресурси](media/Resource-Management-image22.png)

3. <span data-ttu-id="2afd8-189">Въведете името на новия общ ресурс и след това изберете **Създаване**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-189">Enter the name of the new generic resource, and then select **Create**.</span></span>

    ![Въведено име на нов общ ресурс](media/Resource-Management-image23.png)

4. <span data-ttu-id="2afd8-191">В диалоговия прозорец **Бързо създаване: член на екипа на проект**, който се показва, в полето **Роля** изберете ролята за общия ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-191">In the **Quick Create: Project Team Member** dialog box that appears, in the **Role** field, select the role for the generic resource.</span></span> <span data-ttu-id="2afd8-192">В полето **Ресурсна единица** изберете организационната единица за общия ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-192">In the **Resourcing Unit** field, select the organizational unit for the generic resource.</span></span> <span data-ttu-id="2afd8-193">След това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-193">Then select **Save**.</span></span>

    ![Диалогов прозорец „Бързо създаване: член на екипа на проект“](media/Resource-Management-image24.png)

    <span data-ttu-id="2afd8-195">Общият член на екипа вече е присвоен на задачата.</span><span class="sxs-lookup"><span data-stu-id="2afd8-195">The generic team member is now assigned to the task.</span></span>

    ![Общият член на екипа е присвоен на задачата](media/Resource-Management-image25.png)

    <span data-ttu-id="2afd8-197">В раздела **Екип** ще видите новия общ член на екипа.</span><span class="sxs-lookup"><span data-stu-id="2afd8-197">On the **Team** tab, you will see the new generic team member.</span></span> <span data-ttu-id="2afd8-198">Забележете, че той има само присвоени часове.</span><span class="sxs-lookup"><span data-stu-id="2afd8-198">Notice that it has only assigned hours.</span></span> <span data-ttu-id="2afd8-199">Тези часове са сбор от всички задачи, които са присвоени на общия член на екипа.</span><span class="sxs-lookup"><span data-stu-id="2afd8-199">These hours are the sum of all tasks that are assigned to the generic team member.</span></span> <span data-ttu-id="2afd8-200">Общият член на екипа все още няма необходимите часове или изискване за ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-200">The generic team member doesn't yet have required hours or a resource requirement.</span></span>

    ![Общ член на екипа в раздела „Екип“](media/Resource-Management-image26.png)

5. <span data-ttu-id="2afd8-202">Сега можете да присвоите общия член на екипа на други задачи с помощта на функцията за избор на ресурси.</span><span class="sxs-lookup"><span data-stu-id="2afd8-202">You can now assign the generic team member to other tasks by using the Resource Picker.</span></span>

    ![Общ член на екипа във функцията за избор на ресурси](media/Resource-Management-image27.png)

    <span data-ttu-id="2afd8-204">Когато приключите с присвояването на общия ресурс на задачи, можете да генерирате изискване за ресурс за общия ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-204">When you've finished assigning the generic resource to tasks, you can generate a resource requirement for the generic resource.</span></span>

5. <span data-ttu-id="2afd8-205">В раздела **Екип** изберете общия ресурс и след това изберете **Генериране на изискване**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-205">On the **Team** tab, select the generic resource, and then select **Generate Requirement**.</span></span>

    ![Команда „Генериране на изискване“](media/Resource-Management-image28.png)

    <span data-ttu-id="2afd8-207">Когато се генерира изискването, общият член на екипа ще има необходимите часове и връзка за изискването за ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-207">When the requirement is generated, the generic team member will have required hours and a link for the resource requirement.</span></span>

    ![Връзка към изискване за ресурс](media/Resource-Management-image29.png)

    <span data-ttu-id="2afd8-209">След като резервирате наименуван ресурс, общият ресурс се премахва от екипа и се заменя с наименуван ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-209">After you book a named resource, the generic resource is removed from the team and replaced by the named resource.</span></span>

    ![Общ ресурс, заменен с наименуван ресурс](media/Resource-Management-image30.png)

    <span data-ttu-id="2afd8-211">В раздела **График** присвояванията на общи ресурси се премахват и се заменят с наименувания ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-211">On the **Schedule** tab, the generic resource assignments are removed and replaced by the named resource.</span></span>

    ![Присвоявания на общи ресурси, заменени от наименувания ресурс в раздела „График“](media/Resource-Management-image31.png)

    > [!NOTE]
    > <span data-ttu-id="2afd8-213">Това поведение възниква само когато наименуван ресурс е изцяло резервиран за изискването за общ ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-213">This behavior occurs only when a named resource is fully booked for the generic resource requirement.</span></span> <span data-ttu-id="2afd8-214">Когато наименуван ресурс частично заменя изискването за общ ресурс или множество наименувани ресурси заменят изискването за общ ресурс, общият ресурс остава присвоен на задачата.</span><span class="sxs-lookup"><span data-stu-id="2afd8-214">When either a named resource partially replaces the generic resource requirement or multiple named resources replace the generic resource requirement, the generic resource remains assigned to the task.</span></span>

    <span data-ttu-id="2afd8-215">В илюстрацията по-долу е планирана 80-часова задача за срок от пет дни (16 часа на ден за пет дни) и е присвоена на общия ресурс, който е наречен **Функционален**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-215">In the following illustration, an 80-hour task has been planned for a five-day duration (16 hours per day over five days) and assigned to the generic resource that is named **Functional**.</span></span>

    ![80-часова, петдневна задача, присвоена на общия ресурс „Функционален“](media/Resource-Management-image32.png)

    <span data-ttu-id="2afd8-217">Когато генерирате изискването, то е за 80 часа в продължение на пет дни.</span><span class="sxs-lookup"><span data-stu-id="2afd8-217">When you generate the requirement, it's for 80 hours over five days.</span></span>

    ![Изискване, генерирано за 80 часа в продължение на пет дни](media/Resource-Management-image33.png)

    <span data-ttu-id="2afd8-219">Тъй като наличните ресурси работят само осем часа на ден, са необходими два ресурса за изпълнение на изискването.</span><span class="sxs-lookup"><span data-stu-id="2afd8-219">Because available resources work only eight hours per day, two resources are needed to fulfill the requirement.</span></span>

    ![Втори ресурс](media/Resource-Management-image35.png)

    <span data-ttu-id="2afd8-221">В раздела **Екип** сега можете да видите, че общият ресурс няма изисквани часове, но присвоените часове все още се показват заедно с двата наименувани ресурса, които съставят изпълнението.</span><span class="sxs-lookup"><span data-stu-id="2afd8-221">On the **Team** tab, you can now see that the generic resource has no required hours, but the assigned hours still appear together with the two named resources that make up the fulfillment.</span></span>

    ![Двата наименувани ресурса в раздела „Екип“](media/Resource-Management-image36.png)

    <span data-ttu-id="2afd8-223">В раздела **График** общият ресурс остава присвоен на задачата.</span><span class="sxs-lookup"><span data-stu-id="2afd8-223">On the **Schedule** tab, the generic resource remains assigned to the task.</span></span>

    ![Общи ресурси в раздела „График“](media/Resource-Management-image37.png)

<span data-ttu-id="2afd8-225">PSA не присвоява и двата ресурса на задачата, защото това поведение ще доведе до по-малко предсказуем график.</span><span class="sxs-lookup"><span data-stu-id="2afd8-225">PSA doesn't assign both resources to the task, because that behavior would produce a less predictable schedule.</span></span> <span data-ttu-id="2afd8-226">В този прост пример е лесно да разделяте часовете поравно между двата ресурса.</span><span class="sxs-lookup"><span data-stu-id="2afd8-226">In this simple example, it's easy to divide the hours equally between two resources.</span></span> <span data-ttu-id="2afd8-227">В по-сложни сценарии обаче, които включват множество задачи и ресурси, PSA ще трябва да направи предположения как трябва да разпределя резервациите, които са получени за множество ресурси в множество задачи.</span><span class="sxs-lookup"><span data-stu-id="2afd8-227">However, in more complex scenarios that involve multiple tasks and multiple resources, PSA would have to make assumptions about how it should allocate the bookings that are received for multiple resources across multiple tasks.</span></span>

<span data-ttu-id="2afd8-228">Затова в тези сценарии мениджърът на проекти е отговорен за анализиране на множеството резервации и присвояването им според нуждите.</span><span class="sxs-lookup"><span data-stu-id="2afd8-228">Therefore, in these scenarios, the project manager is responsible for parsing the multiple bookings and assigning them as needed.</span></span> <span data-ttu-id="2afd8-229">За да разпредели резервациите, мениджърът на проекти присвоява задачите от общите ресурси на наименуваните ресурси и след това използва изгледа **Съгласуване**, за да се увери, че разпределението работи с резервациите.</span><span class="sxs-lookup"><span data-stu-id="2afd8-229">To allocate the bookings, the project manager assigns the tasks from the generic resources to the named resources and then uses the **Reconciliation** view to make sure that the allocation works with the bookings.</span></span>

### <a name="edit-a-resource-requirement"></a><span data-ttu-id="2afd8-230">Редактиране на изискване за ресурс</span><span class="sxs-lookup"><span data-stu-id="2afd8-230">Edit a resource requirement</span></span>

<span data-ttu-id="2afd8-231">След като е създадено изискване за ресурс, мениджърът на проекти или мениджърът на ресурси може да искат да редактират подробностите, за да прецизират критериите за търсене, когато се използва таблото на графика.</span><span class="sxs-lookup"><span data-stu-id="2afd8-231">After a resource requirement has been created, a project manager or resource manager might want to edit the details to refine the search criteria when the Schedule Board is used.</span></span> <span data-ttu-id="2afd8-232">За да редактирате изискването за ресурс, изпълнете следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="2afd8-232">To edit the resource requirement, follow these steps.</span></span>

1. <span data-ttu-id="2afd8-233">На страницата **Проекти** в раздела **Екип** изберете връзката към което и да е изискване за общ ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-233">On the **Projects** page, on the **Team** tab, select the link to any requirement on a generic resource.</span></span>
2. <span data-ttu-id="2afd8-234">На страницата **Изискване за ресурс**, която се показва, можете да актуализирате няколко атрибута.</span><span class="sxs-lookup"><span data-stu-id="2afd8-234">On the **Resource Requirement** page that appears, you can update several attributes.</span></span> <span data-ttu-id="2afd8-235">Ето някои примери:</span><span class="sxs-lookup"><span data-stu-id="2afd8-235">Here are some examples:</span></span>

    - <span data-ttu-id="2afd8-236">Име</span><span class="sxs-lookup"><span data-stu-id="2afd8-236">Name</span></span>
    - <span data-ttu-id="2afd8-237">Дата „От“</span><span class="sxs-lookup"><span data-stu-id="2afd8-237">From Date</span></span>
    - <span data-ttu-id="2afd8-238">Дата „До“</span><span class="sxs-lookup"><span data-stu-id="2afd8-238">To Date</span></span>
    - <span data-ttu-id="2afd8-239">Продължителност</span><span class="sxs-lookup"><span data-stu-id="2afd8-239">Duration</span></span>
    - <span data-ttu-id="2afd8-240">Тип ресурс</span><span class="sxs-lookup"><span data-stu-id="2afd8-240">Resource Type</span></span>

<span data-ttu-id="2afd8-241">На страницата **Изисквания за ресурс** мениджърът на проекти или мениджърът на ресурси могат да дефинират също и следната информация:</span><span class="sxs-lookup"><span data-stu-id="2afd8-241">On the **Resource Requirement** page, the project manager or resource manager can also define the following information:</span></span>

- <span data-ttu-id="2afd8-242">Умения</span><span class="sxs-lookup"><span data-stu-id="2afd8-242">Skills</span></span>
- <span data-ttu-id="2afd8-243">Роли</span><span class="sxs-lookup"><span data-stu-id="2afd8-243">Roles</span></span>
- <span data-ttu-id="2afd8-244">Предпочитания за ресурси</span><span class="sxs-lookup"><span data-stu-id="2afd8-244">Resource preferences</span></span>
- <span data-ttu-id="2afd8-245">Предпочитана организационна единица</span><span class="sxs-lookup"><span data-stu-id="2afd8-245">Preferred organizational unit</span></span>

### <a name="update-resource-bookings-after-they-are-booked-on-a-project"></a><span data-ttu-id="2afd8-246">Актуализиране на резервации на ресурси, след като са резервирани по проект</span><span class="sxs-lookup"><span data-stu-id="2afd8-246">Update resource bookings after they are booked on a project</span></span>

<span data-ttu-id="2afd8-247">След като добавите общ или наименуван ресурс към екип по проект, можете да промените резервациите на ресурса.</span><span class="sxs-lookup"><span data-stu-id="2afd8-247">After you've added a generic or named resource to a project team, you can change the resource's bookings.</span></span>

1. <span data-ttu-id="2afd8-248">На страницата **Проекти**, в раздела **Екип** изберете нов член на екипа и след това изберете **Поддържане на резервации**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-248">On the **Projects** page, on the **Team** tab, select a team member, and then select **Maintain Bookings**.</span></span>

    ![Отворено табло на графика за избрания член на екипа](media/Resource-Management-image40.png)

    <span data-ttu-id="2afd8-250">Таблото на графика се появява и показва резервациите на члена на екипа по проекта.</span><span class="sxs-lookup"><span data-stu-id="2afd8-250">The Schedule Board appears and shows the project team member's bookings.</span></span> <span data-ttu-id="2afd8-251">Разгънете записа на члена на екипа, за да видите часовете, които са били резервирани спрямо този проект и други проекти, които изразходват капацитета на члена на екипа.</span><span class="sxs-lookup"><span data-stu-id="2afd8-251">Expand the team member's record to view the hours that have been booked against this project and other projects that are consuming the team member's capacity.</span></span>

2. <span data-ttu-id="2afd8-252">Изберете и плъзнете резервацията, за да я разгънете или свиете.</span><span class="sxs-lookup"><span data-stu-id="2afd8-252">Select and drag the booking to extend or shorten it.</span></span> <span data-ttu-id="2afd8-253">Показва се диалогов прозорец **Създаване на резервация на ресурс** и ви позволява да коригирате резервацията.</span><span class="sxs-lookup"><span data-stu-id="2afd8-253">A **Create Resource Booking** dialog box appears that lets you adjust the booking.</span></span>

    ![Диалогов прозорец „Създаване на резервация на ресурс“](media/Resource-Management-image41.png)

3. <span data-ttu-id="2afd8-255">Щракнете с десния бутон върху резервацията.</span><span class="sxs-lookup"><span data-stu-id="2afd8-255">Right-click the booking.</span></span> <span data-ttu-id="2afd8-256">След това можете да използвате контекстното меню, за да извършите следните действия:</span><span class="sxs-lookup"><span data-stu-id="2afd8-256">You can then use the shortcut menu to complete the following actions:</span></span>

    - <span data-ttu-id="2afd8-257">Промяна на състоянието на резервацията.</span><span class="sxs-lookup"><span data-stu-id="2afd8-257">Change the booking status.</span></span>
    - <span data-ttu-id="2afd8-258">Редактиране на резервацията.</span><span class="sxs-lookup"><span data-stu-id="2afd8-258">Edit the booking.</span></span>
    - <span data-ttu-id="2afd8-259">Заместване на ресурс в екипа на проект.</span><span class="sxs-lookup"><span data-stu-id="2afd8-259">Substitute a resource on the project team.</span></span>

### <a name="change-the-booking-status"></a><span data-ttu-id="2afd8-260">Промяна на състоянието на резервацията</span><span class="sxs-lookup"><span data-stu-id="2afd8-260">Change the booking status</span></span>

<span data-ttu-id="2afd8-261">Можете да промените всяко персонализирано състояние или състояние по подразбиране на резервация.</span><span class="sxs-lookup"><span data-stu-id="2afd8-261">You can change any default or custom booking status.</span></span>

![Команда „Промяна на състоянието“](media/Resource-Management-image42.png)

<span data-ttu-id="2afd8-263">Следните състояния са включени в PSA:</span><span class="sxs-lookup"><span data-stu-id="2afd8-263">The following statuses are included in PSA:</span></span>

- <span data-ttu-id="2afd8-264">**Отменено** – това състояние отменя резервацията на ресурса и освобождава неговия капацитет.</span><span class="sxs-lookup"><span data-stu-id="2afd8-264">**Canceled** – This status cancels a resource's booking and frees up the resource's capacity.</span></span>
- <span data-ttu-id="2afd8-265">**Потвърдена резервация** – това състояние изразходва капацитет на ресурса.</span><span class="sxs-lookup"><span data-stu-id="2afd8-265">**Hard Book** – This status consumes a resource's capacity.</span></span> <span data-ttu-id="2afd8-266">Дадена резервация обикновено има това състояние, когато отваряте **Поддържане на резервации** от мрежата **Всички членове на екипа** на страницата **Проекти**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-266">A booking typically has this status when you open **Maintain Bookings** from the **All Team Members** grid on the **Projects** page.</span></span>
- <span data-ttu-id="2afd8-267">**Непотвърдена резервация** – това състояние добавя ресурс към екип, но не изразходва капацитета на ресурса.</span><span class="sxs-lookup"><span data-stu-id="2afd8-267">**Soft Book** – This status adds a resource to a team but doesn't consume the resource's capacity.</span></span> <span data-ttu-id="2afd8-268">Това показва, че ресурсът е запазен за потенциална работа, но все още има капацитет, ако е необходим за други задания.</span><span class="sxs-lookup"><span data-stu-id="2afd8-268">It indicates that the resource has been reserved for potential work but still has capacity if it's needed on other jobs.</span></span> <span data-ttu-id="2afd8-269">С оглед на цялостната наличност на ресурси непотвърдените резервации имат различно състояние от потвърдените резервации.</span><span class="sxs-lookup"><span data-stu-id="2afd8-269">In the view of overall resource availability, soft bookings have a different status than hard bookings.</span></span>
- <span data-ttu-id="2afd8-270">**Предложено** – това състояние представлява предложение на ресурс от мениджър на ресурси или мениджър на проект.</span><span class="sxs-lookup"><span data-stu-id="2afd8-270">**Proposed** – This status represents a resource manager's or project manager's proposal for a resource.</span></span> <span data-ttu-id="2afd8-271">Предложенията не изразходват капацитета на ресурса и ресурсът не се добавя към екипа на проекта.</span><span class="sxs-lookup"><span data-stu-id="2afd8-271">Proposals don't consume the capacity of a resource, and the resource isn't added to the project team.</span></span> <span data-ttu-id="2afd8-272">За да резервирате твърдо ресурса в екипа, мениджърът на проекта трябва да приеме предложението.</span><span class="sxs-lookup"><span data-stu-id="2afd8-272">To hard-book the resource on the team, the project manager must accept the proposal.</span></span>

### <a name="submit-resource-requests"></a><span data-ttu-id="2afd8-273">Подаване на заявки за ресурси</span><span class="sxs-lookup"><span data-stu-id="2afd8-273">Submit resource requests</span></span>

<span data-ttu-id="2afd8-274">Заявките за ресурси се използват за пренасяне на търсенето (изискване за ресурс), което трябва да бъде изпълнено от мениджър на ресурси.</span><span class="sxs-lookup"><span data-stu-id="2afd8-274">Resource requests are used to carry the demand (resource requirement) that must be fulfilled by a resource manager.</span></span> <span data-ttu-id="2afd8-275">За общ ресурс, който вече е в екипа, можете да подадете заявка за ресурс директно.</span><span class="sxs-lookup"><span data-stu-id="2afd8-275">For a generic resource thta is already on the team, you can submit a resource request directly.</span></span> <span data-ttu-id="2afd8-276">Заявката за ресурс може да бъде изпълнена по два начина:</span><span class="sxs-lookup"><span data-stu-id="2afd8-276">A resource request can be fulfilled in two ways:</span></span>

- <span data-ttu-id="2afd8-277">Мениджърът на ресурси директно изпълнява заявката.</span><span class="sxs-lookup"><span data-stu-id="2afd8-277">The resource manager directly fulfills the request.</span></span> <span data-ttu-id="2afd8-278">В този случай общият ресурс се заменя с потвърдена резервация, която има наименуван ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-278">In this case, the generic resource is replaced by a hard booking that has a named resource.</span></span>
- <span data-ttu-id="2afd8-279">Мениджърът на ресурси предлага ресурс на мениджъра на проекти, а той от своя страна одобрява или отхвърля предлагания ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-279">The resource manager proposes a resource to the project manager, and the project manager approves or rejects the proposed resource.</span></span>

#### <a name="direct-fulfillment-of-resource-requests"></a><span data-ttu-id="2afd8-280">Директно изпълнение на заявките за ресурси</span><span class="sxs-lookup"><span data-stu-id="2afd8-280">Direct fulfillment of resource requests</span></span>

<span data-ttu-id="2afd8-281">Когато се генерира изискване за ресурс, мениджърът на проекти може да подаде заявка за ресурс за общ ресурс, като избере ресурса и след това **Подаване на заявка**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-281">When a resource requirement is generated, a project manager can submit a resource request for a generic resource by selecting the resource and then selecting **Submit Request**.</span></span>

![Бутон „Подаване на заявка“](media/Resource-Management-image45.png)

<span data-ttu-id="2afd8-283">Коментарите за ресурса могат да бъдат предоставени на мениджъра на ресурси, който изпълнява заявката.</span><span class="sxs-lookup"><span data-stu-id="2afd8-283">Comments about the resource can be provided to the resource manager who is fulfilling the request.</span></span> <span data-ttu-id="2afd8-284">След като заявката е подадена, полето **Състояние** за члена на екипа се променя на **Подадено**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-284">After the request is submitted, the **Status** field for the team member is changed to **Submitted**.</span></span>

![Въвеждане на коментари по избор](media/Resource-Management-image46.png)

<span data-ttu-id="2afd8-286">Когато мениджърът на ресурси изпълнява заявката, общият член на екипа се заменя от наименувания ресурс в мрежата **Всички членове на екипа**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-286">When the resource manager fulfills the request, the generic team member is replaced by the named resource in the **All Team Members** grid.</span></span>

![Общ член на екип, заменен от наименувания ресурс в мрежата „Всички членове на екипа“](media/Resource-Management-image47.png)

#### <a name="use-a-resource-proposal-for-resource-requests"></a><span data-ttu-id="2afd8-288">Използване на предложение за ресурс за заявки за ресурси</span><span class="sxs-lookup"><span data-stu-id="2afd8-288">Use a resource proposal for resource requests</span></span>

<span data-ttu-id="2afd8-289">Вместо директно резервиране на ресурс по заявка за ресурс мениджър на ресурси може да предложи ресурс на мениджъра на проекта.</span><span class="sxs-lookup"><span data-stu-id="2afd8-289">Instead of directly booking a resource on a resource request, a resource manager can propose a resource to the project manager.</span></span> <span data-ttu-id="2afd8-290">Мениджър на ресурси може да използва тази опция, когато не е налично точно съвпадение за изискванията.</span><span class="sxs-lookup"><span data-stu-id="2afd8-290">A resource manager might use this option when an exact match for the requirements isn't available.</span></span> <span data-ttu-id="2afd8-291">Когато мениджър на ресурси предлага ресурс, мениджърът на проекти вижда, че полето **Състояние** за общия член на екипа се променя на **Нуждае се от преглед**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-291">When a resource manager proposes a resource, the project manager sees that the **Status** field for the generic team member is changed to **Needs Review**.</span></span>

![Състоянието на общия член на екипа е променено на „Нуждае се от преглед“](media/Resource-Management-image48.png)

<span data-ttu-id="2afd8-293">За да прегледате предлагания ресурс заедно с визуализация на ефекта от резервацията на предложението, щракнете двукратно върху члена на екипа, който има състояние на **Нуждае се от преглед**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-293">To view the proposed resource together with a visualization of the effect of the proposal's booking, double-click the team member that has a status of **Needs Review**.</span></span> <span data-ttu-id="2afd8-294">След това изберете раздела **Предложени ресурси**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-294">Then select the **Proposed Resources** tab.</span></span>

![Раздел „Предложени ресурси“](media/Resource-Management-image49.png)

<span data-ttu-id="2afd8-296">Изберете **Приемане на всички предложения** за приемане на всички предложени ресурси или **Отхвърляне на всички предложения** за отхвърлянето им.</span><span class="sxs-lookup"><span data-stu-id="2afd8-296">Select **Accept All Proposals** to accept all proposed resources or **Reject All Proposals** to reject them.</span></span> <span data-ttu-id="2afd8-297">Ако приемете предложените ресурси, те се резервират твърдо по проекта като членове на екипа и заместват общите ресурси.</span><span class="sxs-lookup"><span data-stu-id="2afd8-297">If you accept the proposed resources, they are hard-booked on the project as team members and replace the generic resources.</span></span>

> [!NOTE]
> <span data-ttu-id="2afd8-298">Трябва или да приемете, или да отхвърлите всички предложени ресурси.</span><span class="sxs-lookup"><span data-stu-id="2afd8-298">You must either accept or reject all proposed resources.</span></span> <span data-ttu-id="2afd8-299">Не можете да ги приемете или отхвърлите частично.</span><span class="sxs-lookup"><span data-stu-id="2afd8-299">You can't partially accept or reject them.</span></span>

### <a name="substitute-a-resource-on-the-project-team"></a><span data-ttu-id="2afd8-300">Заместване на ресурс в екипа на проект</span><span class="sxs-lookup"><span data-stu-id="2afd8-300">Substitute a resource on the project team</span></span>

<span data-ttu-id="2afd8-301">Понякога мениджър на проекти трябва да замести резервиран член на екипа по даден проект.</span><span class="sxs-lookup"><span data-stu-id="2afd8-301">Sometimes, a project manager must substitute a booked team member on a project.</span></span>

1. <span data-ttu-id="2afd8-302">На страницата **Проекти**, в раздела **Екип**, изберете ресурса, който трябва да бъде заместен, и след това изберете **Поддържане на резервации**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-302">On the **Projects** page, on the **Team** tab, select the resource that needs a substitute, and then select **Maintain Bookings**.</span></span>
2. <span data-ttu-id="2afd8-303">Разгънете ресурса, за да прегледате проектите, към които е присвоен.</span><span class="sxs-lookup"><span data-stu-id="2afd8-303">Expand the resource to view the projects that it's assigned to.</span></span>

    ![Ресурсът е разгънат, за да се покажат присвоените проекти](media/Resource-Management-image50.png)

3. <span data-ttu-id="2afd8-305">Щракнете с десния бутон върху проекта и след това изберете **Заместване на ресурс**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-305">Right-click the project, and then select **Substitute Resource**.</span></span>
4. <span data-ttu-id="2afd8-306">Ако знаете ресурса, който искате да замести текущия ресурс, изберете или въведете името и след това изберете **Повторно присвояване**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-306">If you know the resource that you want to substitute for the current resource, select or type the name, and then select **Re-assign**.</span></span>

    ![Указване на заместващ ресурс](media/Resource-Management-image51.png)

    <span data-ttu-id="2afd8-308">Или следвайте тези стъпки, за да потърсите ресурс:</span><span class="sxs-lookup"><span data-stu-id="2afd8-308">Alternatively, follow these steps to search for a resource:</span></span>

    1. <span data-ttu-id="2afd8-309">Изберете **Намиране на заместник**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-309">Select **Find Substitution**.</span></span>

        ![Търсене на заместващ ресурс](media/Resource-Management-image52.png)

        <span data-ttu-id="2afd8-311">Асистент за планиране връща списък с наличните заместници.</span><span class="sxs-lookup"><span data-stu-id="2afd8-311">The Schedule Assistant returns a list of available substitutes.</span></span> <span data-ttu-id="2afd8-312">В асистента за планиране можете допълнително да филтрирате наличните ресурси, за да намерите подходящ заместник.</span><span class="sxs-lookup"><span data-stu-id="2afd8-312">In the Schedule Assistant, you can further filter the available resources to find a suitable substitute.</span></span>

        ![Списък с наличните заместници](media/Resource-Management-image53.png)

    2. <span data-ttu-id="2afd8-314">За да заместите, изберете ресурса, който искате, и след това изберете **Заместник**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-314">To substitute the resource, select the resource that you want, and then select **Substitute**.</span></span>

        ![Избран заместник на ресурс](media/Resource-Management-image54.png)

    <span data-ttu-id="2afd8-316">Резервациите и присвояванията се заместват с новия ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-316">The bookings and assignments are substituted with the new resource.</span></span>

    ![Резервации и присвоявания, заместени с новия ресурс](media/Resource-Management-image55.png)

## <a name="reconcile-team-member-bookings-and-assignments"></a><span data-ttu-id="2afd8-318">Съгласуване на резервации и присвоявания на членове на екипа</span><span class="sxs-lookup"><span data-stu-id="2afd8-318">Reconcile team member bookings and assignments</span></span>

<span data-ttu-id="2afd8-319">За членовете на екипа резервациите и присвояванията са свободно свързани.</span><span class="sxs-lookup"><span data-stu-id="2afd8-319">For team members, bookings and assignments are loosely coupled.</span></span> <span data-ttu-id="2afd8-320">С други думи, ресурсите могат да имат присвоявания, но не и резервации, или могат да имат резервации, но да нямат присвояванията.</span><span class="sxs-lookup"><span data-stu-id="2afd8-320">In other words, resources can have assignments but no bookings, or they can have bookings but no assignments.</span></span> <span data-ttu-id="2afd8-321">В идеалния случай резервациите и присвояванията трябва да бъдат изравнени, така че ресурсите да имат заделен капацитет за изпълнение на присвоените задачи.</span><span class="sxs-lookup"><span data-stu-id="2afd8-321">Ideally, bookings and assignments should be aligned, so that resources have committed capacity to perform the task assignments.</span></span> <span data-ttu-id="2afd8-322">Резервациите обаче може да се основават на наличност, а сроковете на задачите може да се променят в течение на проекта.</span><span class="sxs-lookup"><span data-stu-id="2afd8-322">However, the bookings might be based on availability, and task timings might change as the project continues.</span></span> <span data-ttu-id="2afd8-323">Ето защо свободното съчетаване на резервации и присвоявания осигурява гъвкавост.</span><span class="sxs-lookup"><span data-stu-id="2afd8-323">Therefore, the loose coupling of bookings and assignments provides flexibility.</span></span>

<span data-ttu-id="2afd8-324">PSA има раздел **Съгласуване**, който позволява на мениджърите на проекти да съгласуват резервациите на членовете на екипа и техните присвоявания за екипи на проекти.</span><span class="sxs-lookup"><span data-stu-id="2afd8-324">PSA has a **Reconciliation** tab that lets project managers reconcile team members' bookings and their assignments for project teams.</span></span>

![Раздел „Съгласуване“](media/Resource-Management-image56.png)

<span data-ttu-id="2afd8-326">Разделът **Съгласуване** показва резервации и присвоявания до нивото на присвояване на отделни задачи за всеки член на екипа.</span><span class="sxs-lookup"><span data-stu-id="2afd8-326">The **Reconciliation** tab shows bookings and assignments down to the level of the individual task assignment for each team member.</span></span> <span data-ttu-id="2afd8-327">Тя показва часове в клетки, които представляват времеви периоди от месеци до дни.</span><span class="sxs-lookup"><span data-stu-id="2afd8-327">It shows hours in cells that represent time periods from months down to days.</span></span>

<span data-ttu-id="2afd8-328">Разделът показва също обща нетна обща сума за проекта заедно с колона за обща сума.</span><span class="sxs-lookup"><span data-stu-id="2afd8-328">The tab also shows an overall net total for the project, together with a total column.</span></span>

<span data-ttu-id="2afd8-329">За всеки ресурс разделът изчислява разликата между резервациите на члена на екипа и усреднен сбор на присвояванията на задачи на члена на екипа.</span><span class="sxs-lookup"><span data-stu-id="2afd8-329">For each resource, the tab calculates the difference between the team member's bookings and a rollup of the team member's task assignments.</span></span> <span data-ttu-id="2afd8-330">В идеалния случай тази разлика трябва да бъде 0 (нула).</span><span class="sxs-lookup"><span data-stu-id="2afd8-330">Ideally, this difference should be 0 (zero).</span></span> <span data-ttu-id="2afd8-331">С други думи, не трябва да има разлика между резервации и присвоявания.</span><span class="sxs-lookup"><span data-stu-id="2afd8-331">In other words, there should be no difference between bookings and assignments.</span></span> <span data-ttu-id="2afd8-332">Разликите са оцветени и засенчени, за да привличат вниманието към две условия:</span><span class="sxs-lookup"><span data-stu-id="2afd8-332">Differences are colored and shaded to draw attention to two conditions:</span></span>

- <span data-ttu-id="2afd8-333">**Недостиг на резервация** – недостигът на резервация възниква, когато ресурсът има повече присвоявания от резервации.</span><span class="sxs-lookup"><span data-stu-id="2afd8-333">**Booking shortage** – A booking shortage occurs when a resource has more assignments than bookings.</span></span> <span data-ttu-id="2afd8-334">Тъй като този капацитет не е запазен, мениджърът на проекта може да иска да коригира това условие, като удължи резервацията на ресурса, за да покрие дефицита.</span><span class="sxs-lookup"><span data-stu-id="2afd8-334">Because this capacity hasn't been reserved, a project manager might want to correct this condition by extending the resource's bookings to cover the deficit.</span></span>
- <span data-ttu-id="2afd8-335">**Излишък на резервации** – излишък на резервации възниква, когато ресурсът е резервиран за проекта, но не е присвоен на задачи.</span><span class="sxs-lookup"><span data-stu-id="2afd8-335">**Excess bookings** – Excess bookings occur when a resource has been booked to the project but hasn't been assigned to tasks.</span></span> <span data-ttu-id="2afd8-336">Това състояние може да бъде приемливо в случаите, когато ресурсът е бил резервиран за проекта преди да бъде извършено присвояване на задачи.</span><span class="sxs-lookup"><span data-stu-id="2afd8-336">This condition might be acceptable in the cases where the resource was booked to the project before task assignment occurred.</span></span> <span data-ttu-id="2afd8-337">В други случаи обаче ресурсът не е планиран да бъде присвоен на задачи.</span><span class="sxs-lookup"><span data-stu-id="2afd8-337">However, in other cases, the resource isn't planned to be assigned to tasks.</span></span> <span data-ttu-id="2afd8-338">В тези случаи мениджърът на проекта трябва да обмисли анулирането на резервациите на ресурса, така че капацитетът да може да се използва за друг проект.</span><span class="sxs-lookup"><span data-stu-id="2afd8-338">In these cases, the project manager should consider canceling the resource's bookings, so that the capacity can be used for another project.</span></span>

<span data-ttu-id="2afd8-339">В някои случаи, когато преглеждате времето на по-високо ниво от нивото на деня (например нивото на месеца), може да видите нетна разлика нула за даден ресурс (с други думи, резервации = присвоявания).</span><span class="sxs-lookup"><span data-stu-id="2afd8-339">In some cases, when you view time at a higher level than the day level (for example, the month level), you might see a net difference of zero for a resource (in other words, bookings = assignments).</span></span> <span data-ttu-id="2afd8-340">Ако разглеждате времето на ниво седмица обаче, може да видите, че има присвоявания от нула часа и резервации от 40 часа през първата седмица, но присвоявания от 40 часа и резервации от нула часа през втората седмица.</span><span class="sxs-lookup"><span data-stu-id="2afd8-340">However, if you view time at the week level, you might see that there are assignments of zero hours and bookings of 40 hours in the first week, but assignments of 40 hours and bookings of zero hours in the second week.</span></span> <span data-ttu-id="2afd8-341">Като цяло, резервациите и присвояванията са съгласувани, но се различават между отделните седмици.</span><span class="sxs-lookup"><span data-stu-id="2afd8-341">Overall, the bookings and assignments are reconciled, but they differ from one week to the next.</span></span>

<span data-ttu-id="2afd8-342">Когато разглеждате времето на по-високи нива, клетките в раздела **Съгласуване** имат индикатор, който ви информира, че има разлики на по-ниските нива.</span><span class="sxs-lookup"><span data-stu-id="2afd8-342">When you view time at higher levels, cells in the **Reconciliation** tab have an indicator to inform you that there are differences at lower levels.</span></span> <span data-ttu-id="2afd8-343">Чрез двукратно щракване в клетка можете да увеличите мащаба, за да видите разликата.</span><span class="sxs-lookup"><span data-stu-id="2afd8-343">By double-clicking in a cell, you can zoom in to view the difference.</span></span> <span data-ttu-id="2afd8-344">След това можете да щракнете с десния бутон, за да намалите мащаба. Като изберете ресурс и използвате контролата **Следваща разлика** в лентата с инструменти на мрежата, можете да преминете към следващата разлика между резервации и присвоявания за този ресурс.</span><span class="sxs-lookup"><span data-stu-id="2afd8-344">You can then right-click to zoom out. By selecting a resource and then using the **Next difference** control on the grid toolbar, you can go to the next difference between bookings and assignments for that resource.</span></span> <span data-ttu-id="2afd8-345">След това можете да използвате контролата **Предишна разлика**, за да се върнете.</span><span class="sxs-lookup"><span data-stu-id="2afd8-345">You can then use the **Previous difference** control to go back.</span></span> <span data-ttu-id="2afd8-346">Можете също да изключите индикатора за разлика и поведението на навигацията в **Настройки**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-346">You can also turn off the difference indicator and navigation behavior under **Settings**.</span></span>

![Индикатор за разлика](media/Resource-Management-image57.png)

<span data-ttu-id="2afd8-348">Ако имате присвояванията на задачи за ресурс, но нямате резервации на страницата **Проекти**, в раздела **Съгласуване** изберете недостига на резервация и след това изберете **Удължаване на резервацията**.</span><span class="sxs-lookup"><span data-stu-id="2afd8-348">If you have task assignments for a resource but no bookings, on the **Projects** page, on the **Reconciliation** tab, select the booking shortage, and then select **Extend Booking**.</span></span> <span data-ttu-id="2afd8-349">Показва се диалоговият прозорец **Удължаване на резервацията** и показва резервацията, която е необходима за справяне с недостига на ресурса.</span><span class="sxs-lookup"><span data-stu-id="2afd8-349">The **Extend Booking** dialog box appears and shows the booking that is needed to address the resource's shortage.</span></span> <span data-ttu-id="2afd8-350">Освен това показва съществуващите резервации на ресурса във всички проекти или други планируеми обекти.</span><span class="sxs-lookup"><span data-stu-id="2afd8-350">It also shows the resource's existing bookings across all projects or other schedulable entities.</span></span> <span data-ttu-id="2afd8-351">Ако изберете **OK**, за да създадете резервация за ресурса, независимо от наличността на ресурса, може да се стигне до резервиране над капацитета.</span><span class="sxs-lookup"><span data-stu-id="2afd8-351">If you select **OK** to create the booking for the resource, regardless of that resource's availability, you might cause overbooking.</span></span>

![Диалогов прозорец „Удължаване на резервацията“](media/Resource-Management-image58.png)

<span data-ttu-id="2afd8-353">Мениджърът на проекти или мениджърът на ресурси след това може да използва таблото на графика, за да управлява всички ситуации, при които ресурсът е резервиран над капацитета му.</span><span class="sxs-lookup"><span data-stu-id="2afd8-353">The project manager or resource manager can then use the Schedule Board to manage any situations where a resource is overbooked beyond its capacity.</span></span>
