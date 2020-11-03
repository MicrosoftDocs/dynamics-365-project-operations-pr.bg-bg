---
title: Създаване на нов проект
description: Тази тема предоставя информация за това как да създадете нов проект.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 727d287c571b2a64bf10b2393a87567093a420d2
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071955"
---
# <a name="create-a-new-project"></a><span data-ttu-id="890e8-103">Създаване на нов проект</span><span class="sxs-lookup"><span data-stu-id="890e8-103">Create a new project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="890e8-104">Изпълнете следните стъпки, за да създадете нов проект.</span><span class="sxs-lookup"><span data-stu-id="890e8-104">Complete the following steps to create a new project.</span></span>

1. <span data-ttu-id="890e8-105">На страницата **Управление на проект** изберете **Нов проект** и въведете следните стойности:</span><span class="sxs-lookup"><span data-stu-id="890e8-105">On the **Project management** page, select **New project** , and enter the following values:</span></span>

    - <span data-ttu-id="890e8-106">**Тип на проекта:** Време и материал</span><span class="sxs-lookup"><span data-stu-id="890e8-106">**Project type:** Time and material</span></span>
    - <span data-ttu-id="890e8-107">**Име на проекта:** Фаза за надстройка на XYZ 2</span><span class="sxs-lookup"><span data-stu-id="890e8-107">**Project name:** XYZ Upgrade Phase 2</span></span>
    - <span data-ttu-id="890e8-108">**Проектна група:** TM\_WIP</span><span class="sxs-lookup"><span data-stu-id="890e8-108">**Project group:** TM\_WIP</span></span>
    - <span data-ttu-id="890e8-109">**ИД на договор по проект:** 00000002</span><span class="sxs-lookup"><span data-stu-id="890e8-109">**Project contract ID:** 00000002</span></span>

2. <span data-ttu-id="890e8-110">Изберете **Създаване на проект**.</span><span class="sxs-lookup"><span data-stu-id="890e8-110">Select **Create project**.</span></span>

## <a name="assign-a-resource-to-a-project"></a><span data-ttu-id="890e8-111">Присвояване на ресурс към проект</span><span class="sxs-lookup"><span data-stu-id="890e8-111">Assign a resource to a project</span></span>

1. <span data-ttu-id="890e8-112">На страницата **Работници** в **Работници** списък, изберете записа за работника, за който предишно сте задали компетенции, и отворете работния запис.</span><span class="sxs-lookup"><span data-stu-id="890e8-112">On the **Workers** page, in the **Workers** list, select the record for the worker that you previously set up competencies for, and open the worker record.</span></span>
2. <span data-ttu-id="890e8-113">В панела за действие, в раздела **Проект** в групата **Настройки** изберете **Присвояване на проекти**.</span><span class="sxs-lookup"><span data-stu-id="890e8-113">On the Action Pane, on the **Project** tab, in the **Setup** group, select **Assign projects**.</span></span>
3. <span data-ttu-id="890e8-114">На страницата **Задания за валидиране на ресурси** в раздела **Проекти** в полето **Добавете проекта към избрани проекти** филтрирайте по проекта **Фаза за надстройка на XYZ 2**.</span><span class="sxs-lookup"><span data-stu-id="890e8-114">On the **Resource validation project assignments** page, on the **Projects** tab, in the **Add the project to selected projects** field, filter on the **XYZ Upgrade Phase 2** project.</span></span>
4. <span data-ttu-id="890e8-115">В екрана **Оставащи проекти** изберете проект и след това изберете бутона със стрелка, за да го добавите към екрана **Избрани проекти**.</span><span class="sxs-lookup"><span data-stu-id="890e8-115">In the **Remaining projects** pane, select a project, and then select the arrow button to add it to the **Selected projects** pane.</span></span>

<span data-ttu-id="890e8-116">Можете също така да присвоите категории за ресурс, както ви е необходимо.</span><span class="sxs-lookup"><span data-stu-id="890e8-116">You can also assign categories for a resource as you require.</span></span> <span data-ttu-id="890e8-117">Типът категория е или **Разходи** или **Приходи**.</span><span class="sxs-lookup"><span data-stu-id="890e8-117">The category type is either **Cost** or **Revenue**.</span></span> <span data-ttu-id="890e8-118">Типът категория се определя от вашата организация.</span><span class="sxs-lookup"><span data-stu-id="890e8-118">The category type is determined by your organization.</span></span> <span data-ttu-id="890e8-119">Ако за ресурс не са зададени категории, Finance търси категорията по подразбиране за часовите цени за разходи и приходи.</span><span class="sxs-lookup"><span data-stu-id="890e8-119">If no categories are assigned for a resource, Finance looks up the default category on hour prices for cost and revenue.</span></span>

## <a name="set-up-project-resource-and-role-characteristics"></a><span data-ttu-id="890e8-120">Настройте характеристики на ресурсите и ролите на проекта</span><span class="sxs-lookup"><span data-stu-id="890e8-120">Set up project resource and role characteristics</span></span>

<span data-ttu-id="890e8-121">Мениджърът на проекта може да използва функционалността на ресурсите на проекта, за да създаде ролите, необходими за проекта.</span><span class="sxs-lookup"><span data-stu-id="890e8-121">A project manager can use the project resourcing functionality to create the roles that are required for the project.</span></span> <span data-ttu-id="890e8-122">Ролите могат да се използват, ако потвърдените ресурси са все още неизвестни, когато ресурсите се запазват.</span><span class="sxs-lookup"><span data-stu-id="890e8-122">Roles can be used if confirmed resources are still unknown when resources are being reserved.</span></span> <span data-ttu-id="890e8-123">Ролите могат да бъдат временно запазени като планирани ресурси, така че да можете да продължите етапите на планиране на проекта.</span><span class="sxs-lookup"><span data-stu-id="890e8-123">Roles can be temporarily reserved as planned resources, so that you can continue the project planning stages.</span></span>

<span data-ttu-id="890e8-124">[![Пример за роля](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span><span class="sxs-lookup"><span data-stu-id="890e8-124">[![Example of a role](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span></span> 

<span data-ttu-id="890e8-125">**Сценарий:** Contoso е нает да завърши проект за време и материали, който има одобрена харта на проекта.</span><span class="sxs-lookup"><span data-stu-id="890e8-125">**Scenario:** Contoso was hired to complete a Time and material project that has an approved project charter.</span></span> <span data-ttu-id="890e8-126">Младшият ръководител на проекта все още завършва обхвата на проекта.</span><span class="sxs-lookup"><span data-stu-id="890e8-126">The junior project manager is still completing the scope of the project.</span></span> <span data-ttu-id="890e8-127">Понастоящем диспечерът на ресурси идентифицира конкретни ресурси, които ще бъдат запазени за работа по новия проект.</span><span class="sxs-lookup"><span data-stu-id="890e8-127">The resource manager is currently identifying specific resources that will be reserved to work on the new project.</span></span> <span data-ttu-id="890e8-128">Поради критичния характер на проекта, спонсорът на проекта поиска старши ръководител на проекта като една от ролите.</span><span class="sxs-lookup"><span data-stu-id="890e8-128">Because of the critical nature of the project, the project sponsor requested Senior project manager as one of the roles.</span></span> <span data-ttu-id="890e8-129">Мениджърът на ресурсите трябва да придобие новия ресурс и да дефинира ролята в системата в случай, че младшият мениджър на проекта изисква информация за ресурса по време на планирането на проекта.</span><span class="sxs-lookup"><span data-stu-id="890e8-129">The resource manager must acquire the new resource and define the role in the system in case the junior project manager requires the resource information during project planning.</span></span>

<span data-ttu-id="890e8-130">Следващите стъпки показват как мениджърът на ресурси може да настрои ролята на старши мениджър на проекти и да свърже характеристиките на ресурса с нея.</span><span class="sxs-lookup"><span data-stu-id="890e8-130">The following steps show how the resource manager can set up the Senior project manager role and associate resource characteristics with it.</span></span> <span data-ttu-id="890e8-131">По-късно ролята може да се използва за търсене на налични ресурси, които съответстват на необходимите ресурсни компетенции.</span><span class="sxs-lookup"><span data-stu-id="890e8-131">Later, the role can be used to search for available resources that match the required resource competencies.</span></span>

1. <span data-ttu-id="890e8-132">На страницата **Настройки на роли** изберете **Създаване** и въведете следните стойности:</span><span class="sxs-lookup"><span data-stu-id="890e8-132">On the **Setup roles** page, select **New** , and enter the following values:</span></span>

    - <span data-ttu-id="890e8-133">**ИД на роля:** Старши ръководител на проекта</span><span class="sxs-lookup"><span data-stu-id="890e8-133">**Role ID:** Senior Project Manager</span></span>
    - <span data-ttu-id="890e8-134">**Описание:** Старши ръководител на проекта</span><span class="sxs-lookup"><span data-stu-id="890e8-134">**Description:** Senior Project Manager</span></span>

2. <span data-ttu-id="890e8-135">Изберете **Създаване**.</span><span class="sxs-lookup"><span data-stu-id="890e8-135">Select **Create**.</span></span>
3. <span data-ttu-id="890e8-136">Изберете роля **Старши ръководител на проекта** и след това изберете **Конфигуриране на характеристики**.</span><span class="sxs-lookup"><span data-stu-id="890e8-136">Select the **Senior Project Manager** role, and then select **Configure characteristics**.</span></span>
4. <span data-ttu-id="890e8-137">В полето **Тип характеристики** изберете **Умение**.</span><span class="sxs-lookup"><span data-stu-id="890e8-137">In the **Characteristics type** field, select **Skill**.</span></span>
5. <span data-ttu-id="890e8-138">В полето **Налични характеристики** въведете умението за търсене.</span><span class="sxs-lookup"><span data-stu-id="890e8-138">In the **Available characteristics** field, enter the skill to search for.</span></span>
6. <span data-ttu-id="890e8-139">В полето **Тип характеристика** изберете **Сертификат**.</span><span class="sxs-lookup"><span data-stu-id="890e8-139">In the **Characteristic type** field, select **Certificate**.</span></span>
7. <span data-ttu-id="890e8-140">В полето **Налични характеристики** въведете тип сертификат за търсене.</span><span class="sxs-lookup"><span data-stu-id="890e8-140">In the **Available characteristics** field, enter the certificate type to search for.</span></span>

## <a name="assign-a-project-resource-to-a-project"></a><span data-ttu-id="890e8-141">Присвояване на ресурс на проект към проект</span><span class="sxs-lookup"><span data-stu-id="890e8-141">Assign a project resource to a project</span></span>

1. <span data-ttu-id="890e8-142">На страницата **Всички проекти** изберете проект **Фаза за надстройка на XYZ 2**.</span><span class="sxs-lookup"><span data-stu-id="890e8-142">On the **All projects** page, select the **XYZ Upgrade Phase 2** project.</span></span>
2. <span data-ttu-id="890e8-143">В раздела **Екип на проекта и планиране** изберете **Добавяне**.</span><span class="sxs-lookup"><span data-stu-id="890e8-143">On the **Project team and scheduling** tab, select **Add**.</span></span>
3. <span data-ttu-id="890e8-144">В полето **Роля** изберете **Член на екипа**.</span><span class="sxs-lookup"><span data-stu-id="890e8-144">In the **Role** field, select **Team member**.</span></span>
4. <span data-ttu-id="890e8-145">Изберете **Резервация от календар**.</span><span class="sxs-lookup"><span data-stu-id="890e8-145">Select **Book from calendar**.</span></span>
5. <span data-ttu-id="890e8-146">На страницата **Наличност на ресурси** изберете **Преглед на настройките**.</span><span class="sxs-lookup"><span data-stu-id="890e8-146">On the **Resource availability** page, select **View settings**.</span></span>
6. <span data-ttu-id="890e8-147">На страницата **Регулирайте настройките на изгледа** въведете следните стойности:</span><span class="sxs-lookup"><span data-stu-id="890e8-147">On the **Adjust view settings** page, enter the following values:</span></span>

    - <span data-ttu-id="890e8-148">**Формат за изглед на диапазон от дати:** Ден</span><span class="sxs-lookup"><span data-stu-id="890e8-148">**Format for date range view:** Day</span></span>
    - <span data-ttu-id="890e8-149">**Показване на описанията за наличност:** Да</span><span class="sxs-lookup"><span data-stu-id="890e8-149">**Display availability descriptions:** Yes</span></span>
    - <span data-ttu-id="890e8-150">**Показване на оставащия капацитет:** Да</span><span class="sxs-lookup"><span data-stu-id="890e8-150">**Display remaining capacity:** Yes</span></span>

7. <span data-ttu-id="890e8-151">В списъка с ресурси изберете ресурс.</span><span class="sxs-lookup"><span data-stu-id="890e8-151">In the list of resources, select a resource.</span></span>
8. <span data-ttu-id="890e8-152">Изберете **Твърда резервация** и **Пълен капацитет**.</span><span class="sxs-lookup"><span data-stu-id="890e8-152">Select **Hard book** and **Full capacity**.</span></span>

## <a name="assign-a-resource-to-a-default-role"></a><span data-ttu-id="890e8-153">Присвояване на ресурс към роля по подразбиране</span><span class="sxs-lookup"><span data-stu-id="890e8-153">Assign a resource to a default role</span></span>

<span data-ttu-id="890e8-154">За да помогнат на мениджърите на проекти или ресурси могат да разгледат допълнително ресурсите, които могат да бъдат запазени за даден проект.</span><span class="sxs-lookup"><span data-stu-id="890e8-154">To help project or resource managers can drill down further on the resources that can be reserved for a project.</span></span> <span data-ttu-id="890e8-155">Можете да свържете роля по подразбиране със съществуващ ресурс или новопридобит ресурс.</span><span class="sxs-lookup"><span data-stu-id="890e8-155">You can associate a default role with an existing resource or a newly acquired resource.</span></span> <span data-ttu-id="890e8-156">Например, когато Даниел беше нает, той имаше опит и умения да заема ролята на бизнес анализатор.</span><span class="sxs-lookup"><span data-stu-id="890e8-156">For example, when Daniel was hired, he had the experience and skills to fill the Business analyst role.</span></span> <span data-ttu-id="890e8-157">Мениджърът на ресурси назначи тази роля като ролята на Даниел по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="890e8-157">The resource manager assigned this role as Daniel's default role.</span></span> <span data-ttu-id="890e8-158">Затова мениджърът на ресурси добави Даниел към група бизнес анализатори, които са на разположение за работа по проекти.</span><span class="sxs-lookup"><span data-stu-id="890e8-158">Therefore, the resource manager added Daniel to a pool of business analysts who are available to work on projects.</span></span>

<span data-ttu-id="890e8-159">По време на резервирането на ресурси мениджърите на проекти могат да филтрират ресурсите за роля, които са достъпни за работа по проекти.</span><span class="sxs-lookup"><span data-stu-id="890e8-159">During resource reservation, project managers can filter the role resources that are available to work on projects.</span></span> <span data-ttu-id="890e8-160">Те могат да използват тази информация като един критерий, когато извършват многокритериален анализ на решения по време на изпълнението на ресурсите.</span><span class="sxs-lookup"><span data-stu-id="890e8-160">They can use this information as one criterion when they perform multi-criteria decision analysis during resource fulfillment.</span></span> <span data-ttu-id="890e8-161">Те могат също да добавят други характеристики на ресурса към филтъра, за да търсят ресурси, които имат специфични умения, образование и опит за даден проект.</span><span class="sxs-lookup"><span data-stu-id="890e8-161">They can also add other resource characteristics to the filter to search for resources that have specific skills, education, and experience for a given project.</span></span>

<span data-ttu-id="890e8-162">**Сценарий:** Одобреният проект започна и ролята на старши ръководител на проекта беше запазена като планиран ресурс по време на етапа на планиране на проекта.</span><span class="sxs-lookup"><span data-stu-id="890e8-162">**Scenario:** An approved project has started, and the Senior project manager role was reserved as a planned resource during the project planning stage.</span></span> <span data-ttu-id="890e8-163">Мениджърът на ресурси вече е придобил ресурс, за да изпълни ролята на старши мениджър на проекти.</span><span class="sxs-lookup"><span data-stu-id="890e8-163">The resource manager has now acquired a resource to fulfill the Senior project manager role.</span></span>

1. <span data-ttu-id="890e8-164">На страницата **Списък с ресурси** изберете **Даниел Голдшмит**.</span><span class="sxs-lookup"><span data-stu-id="890e8-164">On the **Resources list** page, select **Daniel Goldschmidt**.</span></span>
2. <span data-ttu-id="890e8-165">На страницата **Роля на ресурс** изберете **Създаване** и въведете следните стойности:</span><span class="sxs-lookup"><span data-stu-id="890e8-165">On the **Resource role** page, select **New** , and enter the following values:</span></span>

    - <span data-ttu-id="890e8-166">**Ефективно:** Въведете текущата дата.</span><span class="sxs-lookup"><span data-stu-id="890e8-166">**Effective:** Enter the current date.</span></span>
    - <span data-ttu-id="890e8-167">**Изтичане:** Въведете **Никога**.</span><span class="sxs-lookup"><span data-stu-id="890e8-167">**Expiration:** Enter **Never**.</span></span>
    - <span data-ttu-id="890e8-168">**Роля:** Въведете **Старши ръководител на проекта**.</span><span class="sxs-lookup"><span data-stu-id="890e8-168">**Role:** Enter **Senior Project Manager**.</span></span>

3. <span data-ttu-id="890e8-169">Изберете **Записване** и след това затворете страницата.</span><span class="sxs-lookup"><span data-stu-id="890e8-169">Select **Save** , and then close the page.</span></span>
4. <span data-ttu-id="890e8-170">В раздела **Компетенции** , добавете умението **ProjectMgmt** и сертификат **PMP**.</span><span class="sxs-lookup"><span data-stu-id="890e8-170">On the **Competencies** tab, add the **ProjectMgmt** skill and the **PMP** certificate.</span></span>
