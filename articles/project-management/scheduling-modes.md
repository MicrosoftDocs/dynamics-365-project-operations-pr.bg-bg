---
title: Методи на планиране
description: Тази тема предоставя информация за режимите на планиране.
author: ruhercul
manager: AnnBe
ms.date: 05/04/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fe54944999617b248ff925148a78601dd4be7aca
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981422"
---
# <a name="scheduling-modes"></a><span data-ttu-id="57fcf-103">Методи на планиране</span><span class="sxs-lookup"><span data-stu-id="57fcf-103">Scheduling modes</span></span>

<span data-ttu-id="57fcf-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="57fcf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="57fcf-105">Dynamics 365 Project Operations предоставя способността на организациите да определят как управляват промените в ключови променливи в задачите в съставната структура на работата.</span><span class="sxs-lookup"><span data-stu-id="57fcf-105">Dynamics 365 Project Operations provides the ability for organizations to define how they manage changes to key variables in tasks within the work breakdown structure.</span></span> <span data-ttu-id="57fcf-106">Въз основа на специфичните нужди на организацията, мениджърите на проекти могат да правят промени в режима на планиране, когато се създава проект.</span><span class="sxs-lookup"><span data-stu-id="57fcf-106">Based on the specific needs of the organization, Project Managers can make changes to the scheduling mode when a project is created.</span></span>

<span data-ttu-id="57fcf-107">Има три режима за планиране, налични в Project Operations:</span><span class="sxs-lookup"><span data-stu-id="57fcf-107">There are three scheduling modes available in Project Operations:</span></span>

  - <span data-ttu-id="57fcf-108">Фиксирана продължителност (това е режимът по подразбиране)</span><span class="sxs-lookup"><span data-stu-id="57fcf-108">Fixed duration (this is the default mode)</span></span>
  - <span data-ttu-id="57fcf-109">Фиксирана работа</span><span class="sxs-lookup"><span data-stu-id="57fcf-109">Fixed work</span></span>
  - <span data-ttu-id="57fcf-110">Фиксирани единици</span><span class="sxs-lookup"><span data-stu-id="57fcf-110">Fixed units</span></span>

<span data-ttu-id="57fcf-111">Стойностите, повлияни от дефиницията на конкретен режим на планиране, се определят по следната формула:</span><span class="sxs-lookup"><span data-stu-id="57fcf-111">The values impacted by the definition of a specific scheduling mode are determined by the following formula:</span></span>

  <span data-ttu-id="57fcf-112">Усилие (*Работа*) = Продължителност x единици</span><span class="sxs-lookup"><span data-stu-id="57fcf-112">Effort (*Work*) = Duration x Units</span></span>

<span data-ttu-id="57fcf-113">Когато дефинирате режим на планиране на проект, вие задавате една от тези стойности, които след това не могат да бъдат променени.</span><span class="sxs-lookup"><span data-stu-id="57fcf-113">When you define a project’s scheduling mode, you are setting one of these values, which then can't be changed.</span></span> <span data-ttu-id="57fcf-114">Задържането на тази стойност като константа поставя приоритет върху тази стойност, който уведомява системата да не я променя, когато другите две стойности се променят.</span><span class="sxs-lookup"><span data-stu-id="57fcf-114">Holding this value as a constant places a priority on that value, which notifies the system not to change it when the other two values change.</span></span> <span data-ttu-id="57fcf-115">Следващата таблица предоставя информация за въздействието на избора на определен режим.</span><span class="sxs-lookup"><span data-stu-id="57fcf-115">The following table provides information about the impacts of selecting a specific mode.</span></span>

| <span data-ttu-id="57fcf-116">**В тази задача**</span><span class="sxs-lookup"><span data-stu-id="57fcf-116">**In this task**</span></span>             | <span data-ttu-id="57fcf-117">**Ако ревизирате единици**</span><span class="sxs-lookup"><span data-stu-id="57fcf-117">**If you revise units**</span></span>   | <span data-ttu-id="57fcf-118">**Ако ревизирате времетраене**</span><span class="sxs-lookup"><span data-stu-id="57fcf-118">**If you revise duration**</span></span> | <span data-ttu-id="57fcf-119">**Ако ревизирате усилие**</span><span class="sxs-lookup"><span data-stu-id="57fcf-119">**If you revise effort**</span></span>  |
|----------------------|---------------------------|----------------------------|---------------------------|
| <span data-ttu-id="57fcf-120">Задача с фиксирани единици</span><span class="sxs-lookup"><span data-stu-id="57fcf-120">Fixed units task</span></span>     | <span data-ttu-id="57fcf-121">Продължителността се преизчислява.</span><span class="sxs-lookup"><span data-stu-id="57fcf-121">Duration is recalculated.</span></span> | <span data-ttu-id="57fcf-122">Усилието се преизчислява.</span><span class="sxs-lookup"><span data-stu-id="57fcf-122">Effort is recalculated.</span></span>    | <span data-ttu-id="57fcf-123">Продължителността се преизчислява.</span><span class="sxs-lookup"><span data-stu-id="57fcf-123">Duration is recalculated.</span></span> |
| <span data-ttu-id="57fcf-124">Задача с фиксирано усилие</span><span class="sxs-lookup"><span data-stu-id="57fcf-124">Fixed effort task</span></span>    | <span data-ttu-id="57fcf-125">Продължителността се преизчислява.</span><span class="sxs-lookup"><span data-stu-id="57fcf-125">Duration is recalculated.</span></span> | <span data-ttu-id="57fcf-126">Единиците се преизчисляват.</span><span class="sxs-lookup"><span data-stu-id="57fcf-126">Units are recalculated.</span></span>    | <span data-ttu-id="57fcf-127">Продължителността се преизчислява.</span><span class="sxs-lookup"><span data-stu-id="57fcf-127">Duration is recalculated.</span></span> |
| <span data-ttu-id="57fcf-128">Задача с фиксирано времетраене</span><span class="sxs-lookup"><span data-stu-id="57fcf-128">Fixed duration task</span></span>  | <span data-ttu-id="57fcf-129">Усилието се преизчислява.</span><span class="sxs-lookup"><span data-stu-id="57fcf-129">Effort is recalculated.</span></span>   | <span data-ttu-id="57fcf-130">Усилието се преизчислява.</span><span class="sxs-lookup"><span data-stu-id="57fcf-130">Effort is recalculated.</span></span>    | <span data-ttu-id="57fcf-131">Единиците се преизчисляват.</span><span class="sxs-lookup"><span data-stu-id="57fcf-131">Units are recalculated.</span></span>   |

<span data-ttu-id="57fcf-132">За повече информация относно последиците от даден режим вижте [Променете типа задача за по-точно планиране](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span><span class="sxs-lookup"><span data-stu-id="57fcf-132">For more information about the implications of a given mode, see [Change the task type for more accurate scheduling](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span></span> <span data-ttu-id="57fcf-133">В темата терминът **Работа** се използва вместо **Усилие**.</span><span class="sxs-lookup"><span data-stu-id="57fcf-133">In the topic, the term **Work** is used instead of **Effort**.</span></span>

## <a name="change-the-organizations-scheduling-mode"></a><span data-ttu-id="57fcf-134">Променете режима за планиране на организацията</span><span class="sxs-lookup"><span data-stu-id="57fcf-134">Change the organization’s scheduling mode</span></span>

<span data-ttu-id="57fcf-135">Изпълнете следните стъпки, за да определите режима за планиране на организация.</span><span class="sxs-lookup"><span data-stu-id="57fcf-135">Complete the following steps to define the scheduling mode of an organization.</span></span>

1. <span data-ttu-id="57fcf-136">Отидете на **Настройки** \> **Общи** \> **Параметри** и след това изберете параметъра на проекта.</span><span class="sxs-lookup"><span data-stu-id="57fcf-136">Go to **Settings** \> **General** \> **Parameters**, and then select the project parameter.</span></span> 
2. <span data-ttu-id="57fcf-137">На **Параметри на проекта** страница, изберете режима на график по подразбиране за организацията и след това дефинирайте способността на мениджъра на проекта да замени настройката при създаване на нов проект.</span><span class="sxs-lookup"><span data-stu-id="57fcf-137">On the **Project Parameters** page, select the default scheduling mode for the organization, and then define ability for the Project manager to override the setting when creating a new project.</span></span>

## <a name="change-the-scheduling-mode-setting-on-a-project"></a><span data-ttu-id="57fcf-138">Променете настройката за режим на планиране на проект</span><span class="sxs-lookup"><span data-stu-id="57fcf-138">Change the scheduling mode setting on a project</span></span>

<span data-ttu-id="57fcf-139">Ако организация позволява на мениджъра на проекта да замени режима на график по подразбиране, мениджърът на проекта може да направи тази промяна, когато създаде нов проект.</span><span class="sxs-lookup"><span data-stu-id="57fcf-139">If an organization allows the Project manager to override the default scheduling mode, the Project manager can make that change when they create a new project.</span></span> <span data-ttu-id="57fcf-140">След като проектът бъде запазен, режимът на планиране не може да бъде променен.</span><span class="sxs-lookup"><span data-stu-id="57fcf-140">However, after the project has been saved, the scheduling mode can't be changed.</span></span>

## <a name="copied-projects"></a><span data-ttu-id="57fcf-141">Копирани проекти</span><span class="sxs-lookup"><span data-stu-id="57fcf-141">Copied projects</span></span>

<span data-ttu-id="57fcf-142">Тъй като проектът се създава, когато се предприеме действие за копиране на проект, мениджърът на проекти не може да зададе режим на планиране.</span><span class="sxs-lookup"><span data-stu-id="57fcf-142">Because a project is created when the copy project action is taken, the Project manager can't set the scheduling mode.</span></span> <span data-ttu-id="57fcf-143">Целевият проект винаги ще използва по подразбиране режима, дефиниран на организационно ниво.</span><span class="sxs-lookup"><span data-stu-id="57fcf-143">The destination project will always default to the mode defined at the organizational level.</span></span>

## <a name="copied-tasks"></a><span data-ttu-id="57fcf-144">Копирани задачи</span><span class="sxs-lookup"><span data-stu-id="57fcf-144">Copied tasks</span></span>

<span data-ttu-id="57fcf-145">Когато задача се копира от един проект в друг, тя наследява режима на планиране на целевия проект.</span><span class="sxs-lookup"><span data-stu-id="57fcf-145">When a task is copied from one project to another, the task inherits the scheduling mode of the destination project.</span></span>
