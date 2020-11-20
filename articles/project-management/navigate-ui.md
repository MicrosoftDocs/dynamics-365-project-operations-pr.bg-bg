---
title: Навигиране в потребителския интерфейс
description: Тази тема предоставя информация за управление на проекти в Dynamics 365 Project operations.
author: ruhercul
manager: AnnBe
ms.date: 10/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: deedfe0c6601fd09e09460034c9a0db936b6566e
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127505"
---
# <a name="navigating-the-user-interface"></a><span data-ttu-id="a8ca8-103">Навигиране в потребителския интерфейс</span><span class="sxs-lookup"><span data-stu-id="a8ca8-103">Navigating the user interface</span></span>

<span data-ttu-id="a8ca8-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="a8ca8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

## <a name="overview"></a><span data-ttu-id="a8ca8-105">Общ преглед</span><span class="sxs-lookup"><span data-stu-id="a8ca8-105">Overview</span></span>

<span data-ttu-id="a8ca8-106">Основната форма на проекта е разделена на няколко раздела.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-106">The main project form is separated into several tabs.</span></span> <span data-ttu-id="a8ca8-107">Всеки раздел представлява различно ниво на детайлност в рамките на проекта.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-107">Each tab represents a different level of detail within the project.</span></span>

- <span data-ttu-id="a8ca8-108">**Обобщение**: Осигурява описание на проекта и обобщава както планираното, така и действителното изпълнение на проекта.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-108">**Summary**: Provides a description of the project and aggregates both the planned and actual project performance.</span></span>

    ![Раздел и полета Обобщение](media/navigation7.png)

- <span data-ttu-id="a8ca8-110">**Задачи**: Предоставя подробности относно структурата на разбивка на работата, представена от изглед на мрежа, изглед на дъска и гант.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-110">**Tasks**: Provides the details regarding the work breakdown structure represented by a grid view, board view, and a gantt.</span></span>

    ![Раздел и полета за задачи](media/navigation8.png)

- <span data-ttu-id="a8ca8-112">**Екип**: Предоставя подробности относно участниците в проекта.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-112">**Team**: Provides details regarding the project participants.</span></span> <span data-ttu-id="a8ca8-113">Възложените усилия на всеки член на екипа също са обобщени в този изглед.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-113">The assigned effort of each team member is also summarized in this view.</span></span>

    ![Раздел и полета за екипи](media/navigation9.png)

- <span data-ttu-id="a8ca8-115">**Присвояване на ресурси**: Предоставя периодично представяне на усилията за всеки ресурс по даден проект.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-115">**Resource assignments**: Provides a time-phased view of the effort for each resource on a project.</span></span>

    ![Раздел и полета за задания на ресурси](media/navigation10.png)

- <span data-ttu-id="a8ca8-117">**Изравняване на ресурсите**: Предоставя периодичен изглед на разликите между заданията на всеки именен ресурс и техните резервации.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-117">**Resource reconciliation**: Provides a time-phased view of the differences between the assignments of each named resource and their bookings.</span></span>

    ![Раздел и полета за съгласуване на ресурси](media/navigation11.png)

- <span data-ttu-id="a8ca8-119">**Оценки**: Предоставя периодичен изглед на разходите и оценките на продажбите на даден проект.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-119">**Estimates**: Provides a time-phased view of the cost and sales estimates of a project.</span></span>

    ![Раздел и полета за прогнозни данни](media/navigation12.png)

- <span data-ttu-id="a8ca8-121">**Проследяване**: Предоставя изглед, който показва напредъка на задачите в структурата на разбивка на работата за усилия, разходи и продажби.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-121">**Tracking**: Provides a view that shows the progress of tasks in the work breakdown structure for effort, cost, and sales.</span></span>

    ![Раздел и полета за проследяване](media/navigation13.png)

- <span data-ttu-id="a8ca8-123">**Продажби**: Осигурява дълбоки връзки към оферти и договори, свързани с проекта.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-123">**Sales**: Provides deep links to quotes and contracts associated with the project.</span></span>

- <span data-ttu-id="a8ca8-124">**Оценки на разходите**: Предоставя мрежа, която определя разходите по проекта въз основа на категориите организационни разходи.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-124">**Expense Estimates**: Provides a grid that defines project expenses based upon organizational expense categories.</span></span>

    ![Раздел и полета за прогнози за разходи](media/navigation14.png)

## <a name="grid-controls"></a><span data-ttu-id="a8ca8-126">Контроли на мрежата</span><span class="sxs-lookup"><span data-stu-id="a8ca8-126">Grid controls</span></span>

<span data-ttu-id="a8ca8-127">Следва кратък преглед на типичните контроли, намерени в различните раздели за планиране на проекти.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-127">The follow is a brief overview of the typical controls found on the various project planning tabs.</span></span>

### <a name="refresh"></a><span data-ttu-id="a8ca8-128">Опресняване</span><span class="sxs-lookup"><span data-stu-id="a8ca8-128">Refresh</span></span>

<span data-ttu-id="a8ca8-129">**Обнови**: Извлича последните данни от сървъра, ако са настъпили промени след зареждането на мрежата.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-129">**Refresh**: Retrieves the latest data from the server if any changes occurred after the grid was loaded.</span></span>

![Бутон за опресняване](media/navigation7.png)

### <a name="group-by"></a><span data-ttu-id="a8ca8-131">Групиране по</span><span class="sxs-lookup"><span data-stu-id="a8ca8-131">Group by</span></span>

<span data-ttu-id="a8ca8-132">**Групиране по**: Актуализира групирането на редовете в мрежата, за да отрази или ресурси, роли или категории въз основа на нуждите на потребителя.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-132">**Group by**: Updates the grouping of the rows in the grid to reflect either resources, roles, or categories based on the user's needs.</span></span>

![Групиране по бутон](media/navigation6.png)

### <a name="previousnext"></a><span data-ttu-id="a8ca8-134">Предишен/следващ</span><span class="sxs-lookup"><span data-stu-id="a8ca8-134">Previous/Next</span></span>

<span data-ttu-id="a8ca8-135">**Предишен**/**Следващ**: Актуализирайте видимите периоди от време във фазовите мрежи.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-135">**Previous**/**Next**: Update the visible time periods on the time-phased grids.</span></span>

![Бутони Предишен и Следващ](media/navigation2.png)

### <a name="timescale"></a><span data-ttu-id="a8ca8-137">Времева скала</span><span class="sxs-lookup"><span data-stu-id="a8ca8-137">Timescale</span></span>

<span data-ttu-id="a8ca8-138">**Времева скала**: Променете обобщението на фазовите данни между дни, седмици, месеци и години.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-138">**Timescale**: Change the aggregation of the time-phased data between days, weeks, months, and years.</span></span>

![Бутон за времева скала](media/navigation3.png)

### <a name="expand"></a><span data-ttu-id="a8ca8-140">Разгъни</span><span class="sxs-lookup"><span data-stu-id="a8ca8-140">Expand</span></span>

<span data-ttu-id="a8ca8-141">**Разгъване**: Предаване на видимата решетка на цял екран, осигурявайки повече възможност да видите допълнителни роли.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-141">**Expand**: Render the visible grid to full screen providing more ability to see additional roles.</span></span>

![Бутон за разгъване](media/navigation4.png)

### <a name="time-phase-by"></a><span data-ttu-id="a8ca8-143">Време-фаза по</span><span class="sxs-lookup"><span data-stu-id="a8ca8-143">Time-phase by</span></span>

<span data-ttu-id="a8ca8-144">**Време-фаза по**: Актуализирайте групирането на редовете в мрежата, за да отразява приблизителните разходи за прогнозни продажби.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-144">**Time-phase by**: Update the grouping of the rows in the grid to reflect cost estimates for sales estimates.</span></span> <span data-ttu-id="a8ca8-145">Този контрол се отнася и за скрипта за оценка и мрежата за проследяване.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-145">This control also applies to the estimate script and the tracking grid.</span></span>

![Бутон Време-фаза по](media/navigation0.png)

### <a name="add-column"></a><span data-ttu-id="a8ca8-147">Добавяне на колона</span><span class="sxs-lookup"><span data-stu-id="a8ca8-147">Add column</span></span>

<span data-ttu-id="a8ca8-148">**Добавяне на колона**: Позволява на потребителя да дефинира видимите колони в мрежата.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-148">**Add column**: Allows the user to define the visible columns in the grid.</span></span> <span data-ttu-id="a8ca8-149">Само предварително подготвени колони могат да се добавят към решетките във формуляра **Планиран проект**.</span><span class="sxs-lookup"><span data-stu-id="a8ca8-149">Only out-of-the-box columns can be added to the grids in the **Project Planning** form.</span></span>

![Бутон за добавяне на колона](media/navigation5.png)
