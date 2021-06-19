---
title: Копиране на проект
description: Тази тема предоставя информация за копирането на проекти в Dynamics 365 Project Operations.
author: ruhercul
ms.date: 05/21/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: c3055ab5b8c07faa2bc9167956d283e2a66029dd
ms.sourcegitcommit: 173f2b1f4e063c440a5f78d76d456c62aadbd89e
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/24/2021
ms.locfileid: "6091241"
---
# <a name="copy-a-project"></a><span data-ttu-id="62593-103">Копиране на проект</span><span class="sxs-lookup"><span data-stu-id="62593-103">Copy a project</span></span>

<span data-ttu-id="62593-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="62593-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="62593-105">С помощта на Dynamics 365 Project Operations можете бързо да изграждате нови проекти, като изберете **Копиране на проект** във формуляра **Проекти**.</span><span class="sxs-lookup"><span data-stu-id="62593-105">With Dynamics 365 Project Operations, you can quickly build new projects by selecting **Copy Project** on the **Projects** form.</span></span> <span data-ttu-id="62593-106">За да копирате проект, отворете проекта, който искате да копирате, и след това изберете **Копиране на проект**.</span><span class="sxs-lookup"><span data-stu-id="62593-106">To copy a project, open the project you want to copy, and then select **Copy project**.</span></span> <span data-ttu-id="62593-107">Действието ще копира следното:</span><span class="sxs-lookup"><span data-stu-id="62593-107">The action will copy the following:</span></span>

- <span data-ttu-id="62593-108">Свойства на проекта</span><span class="sxs-lookup"><span data-stu-id="62593-108">Project properties</span></span> 
- <span data-ttu-id="62593-109">Съставна структура на работата</span><span class="sxs-lookup"><span data-stu-id="62593-109">Work breakdown structure</span></span>
- <span data-ttu-id="62593-110">Членове на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="62593-110">Project team members</span></span>
- <span data-ttu-id="62593-111">Оценки на проекта</span><span class="sxs-lookup"><span data-stu-id="62593-111">Project estimates</span></span>
- <span data-ttu-id="62593-112">Прогнози за разход по проект</span><span class="sxs-lookup"><span data-stu-id="62593-112">Project expense estimates</span></span>
- <span data-ttu-id="62593-113">Оценки на материали на проект</span><span class="sxs-lookup"><span data-stu-id="62593-113">Project material estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="62593-114">Свойства на проекта</span><span class="sxs-lookup"><span data-stu-id="62593-114">Project properties</span></span>

<span data-ttu-id="62593-115">Когато проектът се копира, стойностите в следните полета се копират:</span><span class="sxs-lookup"><span data-stu-id="62593-115">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="62593-116">Име</span><span class="sxs-lookup"><span data-stu-id="62593-116">Name</span></span>
- <span data-ttu-id="62593-117">Описание</span><span class="sxs-lookup"><span data-stu-id="62593-117">Description</span></span>
- <span data-ttu-id="62593-118">Клиент</span><span class="sxs-lookup"><span data-stu-id="62593-118">Customer</span></span>
- <span data-ttu-id="62593-119">Шаблон на календар</span><span class="sxs-lookup"><span data-stu-id="62593-119">Calendar Template</span></span>
- <span data-ttu-id="62593-120">Валута</span><span class="sxs-lookup"><span data-stu-id="62593-120">Currency</span></span>
- <span data-ttu-id="62593-121">Единица, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="62593-121">Contracting Unit</span></span>
- <span data-ttu-id="62593-122">Мениджър проекти</span><span class="sxs-lookup"><span data-stu-id="62593-122">Project Manager</span></span>
- <span data-ttu-id="62593-123">Състояние</span><span class="sxs-lookup"><span data-stu-id="62593-123">Status</span></span>
- <span data-ttu-id="62593-124">Общо състояние на проекта</span><span class="sxs-lookup"><span data-stu-id="62593-124">Overall Project Status</span></span>
- <span data-ttu-id="62593-125">Коментари</span><span class="sxs-lookup"><span data-stu-id="62593-125">Comments</span></span>
- <span data-ttu-id="62593-126">Оценки</span><span class="sxs-lookup"><span data-stu-id="62593-126">Estimates</span></span>
- <span data-ttu-id="62593-127">Очаквана начална дата: Това е датата, на която проектът е създаден от копието.</span><span class="sxs-lookup"><span data-stu-id="62593-127">Estimated Start Date: This is the date that the project is created from the copy.</span></span>
- <span data-ttu-id="62593-128">Очаквана дата на приключване: Тази дата се коригира въз основа на началната дата на новия проект, направен от копието.</span><span class="sxs-lookup"><span data-stu-id="62593-128">Estimated Finish Date: This date is adjusted based on the start date of the new project that was made from the copy.</span></span>
- <span data-ttu-id="62593-129">Усилие (Часове)</span><span class="sxs-lookup"><span data-stu-id="62593-129">Effort (Hours)</span></span>
- <span data-ttu-id="62593-130">Прогнозен разход за труд</span><span class="sxs-lookup"><span data-stu-id="62593-130">Estimated Labor Cost</span></span>
- <span data-ttu-id="62593-131">Прогнозна цена на разхода</span><span class="sxs-lookup"><span data-stu-id="62593-131">Estimated Expense Cost</span></span>
- <span data-ttu-id="62593-132">Очакван разход на материал</span><span class="sxs-lookup"><span data-stu-id="62593-132">Estimated Material Cost</span></span>

> [!NOTE]
> <span data-ttu-id="62593-133">Копирането на проект е продължителна операция.</span><span class="sxs-lookup"><span data-stu-id="62593-133">Copy project is a long running operation.</span></span> <span data-ttu-id="62593-134">Записите на проекти, съответните им атрибути и много свързани обекти също се копират.</span><span class="sxs-lookup"><span data-stu-id="62593-134">Project records, their relevant attributes, and many related entities are also copied.</span></span> <span data-ttu-id="62593-135">Поради продължителния характер на операцията, след стартирането на копирането, целевата страница на проекта се заключва за редактиране, докато операцията по копиране не завърши.</span><span class="sxs-lookup"><span data-stu-id="62593-135">Because of the long running nature of the operation, after the copy starts, the target project page is locked for editing until the copy operation is complete.</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="62593-136">Съставна структура на работата</span><span class="sxs-lookup"><span data-stu-id="62593-136">Work breakdown structure</span></span>

<span data-ttu-id="62593-137">Когато проектът се копира, се копира цялата съставна структура на работата, заредена с ресурси.</span><span class="sxs-lookup"><span data-stu-id="62593-137">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="62593-138">Наименувани ресурси се заменят с генерични ресурси.</span><span class="sxs-lookup"><span data-stu-id="62593-138">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="62593-139">Ако посочените ресурси нямат същото работно време като общия ресурс, графикът ще бъде преизчислен и продължителността на задачите може да се промени.</span><span class="sxs-lookup"><span data-stu-id="62593-139">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="62593-140">Членове на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="62593-140">Project team members</span></span>

<span data-ttu-id="62593-141">Когато проектният екип се копира от изходния проект, се копират общите ресурси.</span><span class="sxs-lookup"><span data-stu-id="62593-141">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="62593-142">Присвояванията на общи ресурси се поддържат също както в изходния проект.</span><span class="sxs-lookup"><span data-stu-id="62593-142">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="62593-143">Имените ресурси ще бъдат преобразувани в общи членове на екипа.</span><span class="sxs-lookup"><span data-stu-id="62593-143">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="62593-144">Оценки</span><span class="sxs-lookup"><span data-stu-id="62593-144">Estimates</span></span>

<span data-ttu-id="62593-145">Когато проектът се копира, редове за оценка на ресурси, разходи и материали се копират от изходния проект.</span><span class="sxs-lookup"><span data-stu-id="62593-145">When the project is copied, resource, expense and material estimate lines are copied from the source project.</span></span> 

<span data-ttu-id="62593-146">За информация как програмно да влезете в Copy Project, вижте [Разработвайте шаблони за проекти с Copy Project](dev-copy-project.md).</span><span class="sxs-lookup"><span data-stu-id="62593-146">For information on how to programmatically access Copy Project, see [Develop project templates with Copy Project](dev-copy-project.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
