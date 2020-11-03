---
title: Оценете продажбите на проекта и разходите, когато наличен ресурс запълва множество роли в даден проект
description: Тази тема предоставя информация за това как ценовите измерения могат да се използват в подкрепа на ценообразуването и ценообразуването за ресурс, който запълва множество роли в даден проект.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 8ddc827a4170c5576c0a4350b51e6a119094ac50
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071872"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-mulitple-roles-on-a-project"></a><span data-ttu-id="9c1e2-103">Оценете продажбите на проекта и разходите, когато наличен ресурс запълва множество роли в даден проект</span><span class="sxs-lookup"><span data-stu-id="9c1e2-103">Estimate project sales and costs when a bookable resource fills mulitple roles on a project</span></span> 

<span data-ttu-id="9c1e2-104">Базираните на проекти компании често имат нужда от един ресурс, за да изпълняват множество роли в даден проект.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-104">Project-based companies often have the need for one resource to perform mulitple roles on a project.</span></span> <span data-ttu-id="9c1e2-105">Всяка от тези роли може да бъде оценена по различен начин, което означава, че времето на един и същ ресурс в проекта може да получи различна финансова оценка в зависимост от сметката и разходните ставки за всяка от ролите.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-105">Each of these roles could be priced and costed differently which means the same resource's time on the project could get a different financial estimate depending on the bill and cost rates for each of the roles.</span></span> <span data-ttu-id="9c1e2-106">Project Service Automation позволява настройката на стойностите в записа на члена на екипа за посочения ресурс и позволява различни замествания на всяка от задачите, на които е назначен членът на екипа.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-106">Project Service Automation allows the setup of the values on the team member record for the named resource and allows for different overrides on each of the tasks that the team member is assigned to.</span></span>

<span data-ttu-id="9c1e2-107">Следващият пример обяснява как простото заменяне на тази стойност позволява на ресурса да има множество роли в проект с различни разходи и тарифи.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-107">The following example  explains how the simple override of this value allows a resource to have multiple roles on a project with different cost and bill rates.</span></span>

## <a name="create-tasks"></a><span data-ttu-id="9c1e2-108">Създаване на задачи</span><span class="sxs-lookup"><span data-stu-id="9c1e2-108">Create tasks</span></span>
<span data-ttu-id="9c1e2-109">Създайте две проектни задачи за по 40 часа, задача A и задача B. Изберете задача A като предшественик на задача B.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-109">Create two project tasks for 40 hours each, Task A and Task B. Select Task A as a predecessor to Task B.</span></span>

## <a name="set-up-role-and-organization-unit-for-a-generic-project-team-member"></a><span data-ttu-id="9c1e2-110">Създайте роля и организационна единица за обичаен член на екипа по проекта</span><span class="sxs-lookup"><span data-stu-id="9c1e2-110">Set up Role and Organization Unit for a generic project team member</span></span>

1. <span data-ttu-id="9c1e2-111">На страницата **График** изберете реда **Задача** за Задача А.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-111">On the **Schedule** page, select the **Task** row for Task A.</span></span> 
2. <span data-ttu-id="9c1e2-112">В полето **Ресурси** изберете **Създаване** в падащия списък.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-112">In the **Resources** field, select **Create** in the drop-down list.</span></span>
3. <span data-ttu-id="9c1e2-113">На страницата **Бързо създаване на Член на екипа** посочете атрибутите на обичаен член на екипа, който може да изпълни тази задача.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-113">On the **Team Member Quick Create** page, specify the attributes of the generic team member who can perform this task.</span></span>
4. <span data-ttu-id="9c1e2-114">Изберете подходящата роля и организационна единица и след това изберете **Запиши и затвори**.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-114">Select the appropriate role and organizational unit, and then select **Save and Close**.</span></span> <span data-ttu-id="9c1e2-115">Създава се общ член на екипа, който се възлага на тази задача.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-115">A generic team member is created and assigned to this task.</span></span> 

<span data-ttu-id="9c1e2-116">Повторете тези стъпки за Задача Б и се уверете, че ролята и организационната единица на общия член на екипа, създаден за Задача Б, е различна от Задача А.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-116">Repeat these steps for Task B and make sure that the role and organizational unit on the generic team member created for Task B is different than Task A.</span></span> 

## <a name="set-up-role-and-organization-unit-for-a-project-task"></a><span data-ttu-id="9c1e2-117">Създайте роля и организационна единица за задача по проекта</span><span class="sxs-lookup"><span data-stu-id="9c1e2-117">Set up role and organization unit for a project task</span></span>

1. <span data-ttu-id="9c1e2-118">След като създадете задача A, изберете задачата и след това изберете **Редактиране на задачата**.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-118">After you create Task A, select the task, and then select **Edit task**.</span></span>
2. <span data-ttu-id="9c1e2-119">На страницата **Подробности за задачата** намерете полетата **Роля** и **Организационна единица** , добавете стойностите, които се изискват от ресурс, който би изпълнил тази задача.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-119">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="9c1e2-120">Ако завършвате този сценарий, като използвате демонстрационни данни на Project Service Automation, изберете **Консултиране на потенциален клиент** за ролята и **Fabrikam US** като организационна единица.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-120">If you are completing this scenarios using Project Service Automation demo data, select **Consulting Lead** for the role, and **Fabrikam US** as the organizational unit.</span></span>

3. <span data-ttu-id="9c1e2-121">Изберете Задача Б, след което изберете **Редактиране на задачата**.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-121">Select Task B and then select **Edit task**.</span></span>
4. <span data-ttu-id="9c1e2-122">На страницата **Подробности за задачата** намерете полетата **Роля** и **Организационна единица** , добавете стойностите, които се изискват от ресурс, който би изпълнил тази задача.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-122">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> <span data-ttu-id="9c1e2-123">Уверете се, че стойностите в полетата **Роля** и **Организационна единица** са различни за задача Б от тези за задача А.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-123">Make sure that the values in the **Role** and **Organizational Unit** fields are different for Task B from those for Task A.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="9c1e2-124">Ако завършвате този сценарий, като използвате демонстрационни данни на Project Service Automation, изберете **Мрежов техник** за ролята и **Fabrikam US** като организационна единица.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-124">If you are completing this scenarios using Project Service Automation demo data, select **Network Technician** for the role, and **Fabrikam US** as the organizational unit.</span></span>

5. <span data-ttu-id="9c1e2-125">Запишете и затворете страницата **Подробности за задача**.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-125">Save and close the **Task Details** page.</span></span> 

## <a name="team-member-and-estimates-behaviour"></a><span data-ttu-id="9c1e2-126">Член на екипа и поведение на прогнози</span><span class="sxs-lookup"><span data-stu-id="9c1e2-126">Team member and estimates behaviour</span></span> 

1. <span data-ttu-id="9c1e2-127">На страницата **Подробности за задачата** в **Член на екипа** изберете двамата обичайни членове на екипа и след това изберете **Генериране на изисквания**.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-127">On the **Task Details** page, on the **Team Member** , select the two generic team Members and then select **Generate Requirements**.</span></span> <span data-ttu-id="9c1e2-128">Това ще генерира изисквания за ресурси.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-128">This will generate resource requirements.</span></span> 
2. <span data-ttu-id="9c1e2-129">Изберете реда на члена на екипа за **Консултиране на потенциален клиент** и след това изберете **Резервиране**.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-129">Select the team member row for **Consulting Lead** and then select **Book**.</span></span> <span data-ttu-id="9c1e2-130">Таблото за графици се отваря и резервира ресурс за това изискване.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-130">The schedule board opens and books a resource to that requirement.</span></span>
3. <span data-ttu-id="9c1e2-131">Изберете реда на члена на екипа за **Мрежов техник** и след това изберете **Резервиране**.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-131">Select the team member row for **Network Technician** and the select **Book**.</span></span> <span data-ttu-id="9c1e2-132">Таблото за графици се отваря и резервира същия ресурс за това изискване.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-132">The schedule board opens and books the same resource on that requirement.</span></span>

### <a name="team-member-grid"></a><span data-ttu-id="9c1e2-133">Мрежа на член на екипа</span><span class="sxs-lookup"><span data-stu-id="9c1e2-133">Team Member grid</span></span> 
<span data-ttu-id="9c1e2-134">В мрежата **Член на екипа** забележете, че двата общи записа на членовете на екипа са изтрити и са заменени с един ресурс.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-134">On the **Team Member** grid, notice that the two generic team member records are deleted and have been replaced one resource.</span></span> <span data-ttu-id="9c1e2-135">Има един набор от стойности за този ресурс, който показва набор от стойности по подразбиране за **Роля** и **Организационна единица**.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-135">There is one set of values for that resource that shows a default set of values for **Role** and **Organizational Unit**.</span></span>
<span data-ttu-id="9c1e2-136">Когато разширите реда на този запис на член на екипа, можете да видите различни задания в записа на члена на екипа и за двете задачи.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-136">When you expand the row of that Team Member record, you can see distinct assignments on the team member record for both of those tasks.</span></span> <span data-ttu-id="9c1e2-137">Всеки ред за задание има специфични за задачата стойности за **Роля** и **Организационна единица**.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-137">Each assignment row has task specific values for **Role** and **Organizational Unit**.</span></span> 

### <a name="estimates-grid"></a><span data-ttu-id="9c1e2-138">Мрежа с оценки</span><span class="sxs-lookup"><span data-stu-id="9c1e2-138">Estimates grid</span></span> 
<span data-ttu-id="9c1e2-139">Когато навигирате до мрежата **Оценки** , ще забележите, че и двете задания за един и същи ресурс се оценяват по различен начин.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-139">When you navigate to the **Estimates** grid, you will notice that both assignments for the same resource are priced differently.</span></span>
<span data-ttu-id="9c1e2-140">Заданието за ресурса по Задача A се определя с помощта на стойността на атрибута **Роля** на **Консултиране на потенциален клиент**.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-140">The assignment for the resource on Task A is priced using the **Role** attribute value of **Consulting Lead**.</span></span> <span data-ttu-id="9c1e2-141">Заданието за същия ресурс по Задача Б се определя с помощта на стойността на атрибута **Роля** на **Мрежов техник**.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-141">The assignment for the same resource on Task B is priced using the **Role** attribute value of **Network Technician**.</span></span>





