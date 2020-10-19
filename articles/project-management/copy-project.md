---
title: Копиране на проект
description: Тази тема предоставя информация за копиране на проекти в Dynamics 365 Project Operations.
author: ruhercul
manager: AnnBe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: e35dc725e7938e9f59f7151dd1b37500fabf77a4
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907879"
---
# <a name="copy-a-project"></a><span data-ttu-id="6c7fb-103">Копиране на проект</span><span class="sxs-lookup"><span data-stu-id="6c7fb-103">Copy a project</span></span>

<span data-ttu-id="6c7fb-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="6c7fb-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="6c7fb-105">С Dynamics 365 Project Operations можете бързо да създавате нови проекти, като използвате **Копиране на проект** действие върху формуляра **Проекти**.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-105">With Dynamics 365 Project Operations, you can quickly build new projects by using the **Copy Project** action on the **Projects** from.</span></span> <span data-ttu-id="6c7fb-106">За да копирате проект, изберете проект и след това изберете **Копиране**.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-106">To copy a project, select a project, and then select **Copy**.</span></span> <span data-ttu-id="6c7fb-107">Действието ще копира:</span><span class="sxs-lookup"><span data-stu-id="6c7fb-107">The action will copy:</span></span>

- <span data-ttu-id="6c7fb-108">Свойства на проекта</span><span class="sxs-lookup"><span data-stu-id="6c7fb-108">Project properties</span></span>
- <span data-ttu-id="6c7fb-109">Съставна структура на работата</span><span class="sxs-lookup"><span data-stu-id="6c7fb-109">The Work breakdown structure</span></span>
- <span data-ttu-id="6c7fb-110">Членове на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="6c7fb-110">Project team members</span></span>
- <span data-ttu-id="6c7fb-111">Оценки на проекта</span><span class="sxs-lookup"><span data-stu-id="6c7fb-111">Project estimates</span></span>
- <span data-ttu-id="6c7fb-112">Прогнози за разход по проект</span><span class="sxs-lookup"><span data-stu-id="6c7fb-112">Project expense estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="6c7fb-113">Свойства на проекта</span><span class="sxs-lookup"><span data-stu-id="6c7fb-113">Project properties</span></span>

<span data-ttu-id="6c7fb-114">Когато проектът се копира, стойностите в следните полета се копират:</span><span class="sxs-lookup"><span data-stu-id="6c7fb-114">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="6c7fb-115">Име</span><span class="sxs-lookup"><span data-stu-id="6c7fb-115">Name</span></span>
- <span data-ttu-id="6c7fb-116">Описание</span><span class="sxs-lookup"><span data-stu-id="6c7fb-116">Description</span></span>
- <span data-ttu-id="6c7fb-117">Клиент</span><span class="sxs-lookup"><span data-stu-id="6c7fb-117">Customer</span></span>
- <span data-ttu-id="6c7fb-118">Шаблон на календар</span><span class="sxs-lookup"><span data-stu-id="6c7fb-118">Calendar Template</span></span>
- <span data-ttu-id="6c7fb-119">Валута</span><span class="sxs-lookup"><span data-stu-id="6c7fb-119">Currency</span></span>
- <span data-ttu-id="6c7fb-120">Единица, сключваща договора</span><span class="sxs-lookup"><span data-stu-id="6c7fb-120">Contracting Unit</span></span>
- <span data-ttu-id="6c7fb-121">Мениджър проекти</span><span class="sxs-lookup"><span data-stu-id="6c7fb-121">Project Manager</span></span>
- <span data-ttu-id="6c7fb-122">Състояние</span><span class="sxs-lookup"><span data-stu-id="6c7fb-122">Status</span></span>
- <span data-ttu-id="6c7fb-123">Общо състояние на проекта</span><span class="sxs-lookup"><span data-stu-id="6c7fb-123">Overall Project Status</span></span>
- <span data-ttu-id="6c7fb-124">Коментари</span><span class="sxs-lookup"><span data-stu-id="6c7fb-124">Comments</span></span>
- <span data-ttu-id="6c7fb-125">Оценки</span><span class="sxs-lookup"><span data-stu-id="6c7fb-125">Estimates</span></span>
- <span data-ttu-id="6c7fb-126">Очаквана начална дата</span><span class="sxs-lookup"><span data-stu-id="6c7fb-126">Estimated Start Date</span></span>
- <span data-ttu-id="6c7fb-127">Дата на приключване</span><span class="sxs-lookup"><span data-stu-id="6c7fb-127">Finish Date</span></span>
- <span data-ttu-id="6c7fb-128">Усилие (Часове)</span><span class="sxs-lookup"><span data-stu-id="6c7fb-128">Effort (Hours)</span></span>
- <span data-ttu-id="6c7fb-129">Прогнозен разход за труд</span><span class="sxs-lookup"><span data-stu-id="6c7fb-129">Estimated Labor Cost</span></span>
- <span data-ttu-id="6c7fb-130">Прогнозна цена на разхода</span><span class="sxs-lookup"><span data-stu-id="6c7fb-130">Estimated Expense Cost</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="6c7fb-131">Съставна структура на работата</span><span class="sxs-lookup"><span data-stu-id="6c7fb-131">Work breakdown structure</span></span>

<span data-ttu-id="6c7fb-132">Когато проектът се копира, се копира цялата съставна структура на работата, заредена с ресурси.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-132">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="6c7fb-133">Наименувани ресурси се заменят с генерични ресурси.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-133">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="6c7fb-134">Ако посочените ресурси нямат същото работно време като общия ресурс, графикът ще бъде преизчислен и продължителността на задачите може да се промени.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-134">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="6c7fb-135">Членове на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="6c7fb-135">Project team members</span></span>

<span data-ttu-id="6c7fb-136">Когато проектният екип се копира от изходния проект, се копират общите ресурси.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-136">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="6c7fb-137">Присвояванията на общи ресурси се поддържат също както в изходния проект.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-137">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="6c7fb-138">Имените ресурси ще бъдат преобразувани в общи членове на екипа.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-138">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="6c7fb-139">Оценки</span><span class="sxs-lookup"><span data-stu-id="6c7fb-139">Estimates</span></span>

<span data-ttu-id="6c7fb-140">Когато проектът се копира, редовете за оценка на ресурсите и разходите се копират от проекта източник.</span><span class="sxs-lookup"><span data-stu-id="6c7fb-140">When the project is copied, both resource and expense estimate lines are copied from the source project.</span></span>