---
title: Нанасяне на проекти и задачи към базиран на проект ред на оферта
description: Тази тема предоставя информация за това как да се съпоставят проекти и задачи на линия, базирана на проекти.
author: rumant
ms.date: 10/05/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d1c98d6a903393a0afc0e94d7f9859d55b9dc1f7
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994573"
---
# <a name="map-projects-and-tasks-to-a-project-based-quote-line"></a><span data-ttu-id="85c94-103">Нанасяне на проекти и задачи към базиран на проект ред на оферта</span><span class="sxs-lookup"><span data-stu-id="85c94-103">Map projects and tasks to a project-based quote line</span></span>

<span data-ttu-id="85c94-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="85c94-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="85c94-105">В базирани на проекти редове на оферта можете да картографирате конкретните задачи на проект, който вече е свързан с линия на редове на оферта.</span><span class="sxs-lookup"><span data-stu-id="85c94-105">On project-based quote lines, you can map the specific tasks of a project that is already associated to a quote line.</span></span>

<span data-ttu-id="85c94-106">Когато съпоставяте задачи с ред на оферта, следните елементи, които сте дефинирали в реда на оферта, ще се прилагат само за тези задачи:</span><span class="sxs-lookup"><span data-stu-id="85c94-106">When you map tasks to a quote line, the following items you defined on the quote line will only apply to those tasks:</span></span>

- <span data-ttu-id="85c94-107">Метод на фактуриране</span><span class="sxs-lookup"><span data-stu-id="85c94-107">Billing method</span></span>
- <span data-ttu-id="85c94-108">Настройване на платимост</span><span class="sxs-lookup"><span data-stu-id="85c94-108">Chargeability options</span></span>
- <span data-ttu-id="85c94-109">Ограничения, които да не се надвишават</span><span class="sxs-lookup"><span data-stu-id="85c94-109">Not-to-exceed limits</span></span>
- <span data-ttu-id="85c94-110">Клиенти</span><span class="sxs-lookup"><span data-stu-id="85c94-110">Customers</span></span>

<span data-ttu-id="85c94-111">Например може да имате проект, при който едната фаза е с фиксирана цена, а всички останали фази са време и материали.</span><span class="sxs-lookup"><span data-stu-id="85c94-111">For example, you might have a project where one phase is fixed price and all the other phases are time and materials.</span></span> <span data-ttu-id="85c94-112">В този случай можете да свържете първата фаза и всички нейни дъщерни задачи към линията за котиране за тази фаза с метод за таксуване с фиксирана цена.</span><span class="sxs-lookup"><span data-stu-id="85c94-112">In this case, you can associate the first phase, and all of its child tasks, to the quote line for that phase with a fixed price billing method.</span></span> <span data-ttu-id="85c94-113">След това можете да свържете всички останали фази с цитираната линия, базирана на времето и материалите.</span><span class="sxs-lookup"><span data-stu-id="85c94-113">You can then associate all the other phases to the time and materials-based quote line.</span></span>

## <a name="associate-tasks-to-project-based-quote-lines"></a><span data-ttu-id="85c94-114">Свързване на задачи към базирани на проект редове на оферта</span><span class="sxs-lookup"><span data-stu-id="85c94-114">Associate tasks to project-based quote lines</span></span>

<span data-ttu-id="85c94-115">Можете да свържете задачите с редове на оферта от следните местоположения:</span><span class="sxs-lookup"><span data-stu-id="85c94-115">You can associate tasks with quote lines from the following locations:</span></span>

- <span data-ttu-id="85c94-116">Страница **Проект** > раздел **Задача за фактуриране** (оптимален)</span><span class="sxs-lookup"><span data-stu-id="85c94-116">**Project** page > **Task billing** tab (optimal)</span></span>
- <span data-ttu-id="85c94-117">Страница **Оферта** > раздел **Платими задачи**</span><span class="sxs-lookup"><span data-stu-id="85c94-117">**Quote Line** page > **Chargeable tasks** tab</span></span> 

### <a name="from-the-project-page"></a><span data-ttu-id="85c94-118">От страницата на проекта</span><span class="sxs-lookup"><span data-stu-id="85c94-118">From the Project page</span></span>

<span data-ttu-id="85c94-119">Страницата на **Проекта** осигурява оптимално изживяване за свързване на задачите с редове на оферта.</span><span class="sxs-lookup"><span data-stu-id="85c94-119">The **Project** page provides the optimal experience for associating tasks to quote lines.</span></span> <span data-ttu-id="85c94-120">Можете да използвате тази страница, за да изберете множество задачи и да асоциирате всички, заедно с техните дъщерни задачи, към избрания ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="85c94-120">You can use this page to select multiple tasks and associate all of them, plus their child tasks, to the selected quote line.</span></span>

1. <span data-ttu-id="85c94-121">На раздела **Общи** базиран на проект ред на оферта проверете дали полето **Проект** е попълнено.</span><span class="sxs-lookup"><span data-stu-id="85c94-121">On the **General** tab of a project–based quote line, verify the **Project** field is filled out.</span></span>
2. <span data-ttu-id="85c94-122">В полето **Включени задачи** изберете **Само избрани задачи**.</span><span class="sxs-lookup"><span data-stu-id="85c94-122">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="85c94-123">Запишете базирания на проект ред на оферта.</span><span class="sxs-lookup"><span data-stu-id="85c94-123">Save the project-based quote line.</span></span> <span data-ttu-id="85c94-124">Когато формулярът се обнови, се показва разделът **Платими задачи**.</span><span class="sxs-lookup"><span data-stu-id="85c94-124">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="85c94-125">На раздела **Общи** изберете връзката за проекта от полето **Проект**.</span><span class="sxs-lookup"><span data-stu-id="85c94-125">On the **General** tab, select the link for the project from the **Project** field.</span></span>
5. <span data-ttu-id="85c94-126">На страницата **Проект** изберете раздела **Фактуриране на задача**.</span><span class="sxs-lookup"><span data-stu-id="85c94-126">On the **Project** page, select the **Task billing** tab.</span></span>
6. <span data-ttu-id="85c94-127">Във втората мрежа, която се отнася за специфична за задачите настройка за фактуриране, изберете една или повече задачи и след това изберете **Свързване на редове на оферта**.</span><span class="sxs-lookup"><span data-stu-id="85c94-127">In the second grid, which applies to task-specific billing setup, select one or more tasks and then select **Associate quote lines**.</span></span>
7. <span data-ttu-id="85c94-128">В диалоговата страница, която се появява, изберете ред с оферти, който показва базираните на проект редове на оферта в офертата.</span><span class="sxs-lookup"><span data-stu-id="85c94-128">In the dialog page that appears, select a quote line that displays project-based quote lines on the quote.</span></span>
8. <span data-ttu-id="85c94-129">В полето **Тип фактуриране** посочете дали тези задачи се заплащат или не се заплащат.</span><span class="sxs-lookup"><span data-stu-id="85c94-129">In the **Billing type** field, indicate if these tasks are chargeable or non-chargeable.</span></span>
9. <span data-ttu-id="85c94-130">Поставете отметка в квадратчето, за да посочите дали асоциацията трябва да включва дъщерни задачи на избраните задачи.</span><span class="sxs-lookup"><span data-stu-id="85c94-130">Select the check box to indicate if the association should include child tasks of the selected tasks.</span></span> <span data-ttu-id="85c94-131">Поставянето на отметка в квадратчето ще свърже дъщерните задачи на избраните задачи с реда на оферта.</span><span class="sxs-lookup"><span data-stu-id="85c94-131">Checking the box will associate the child tasks of the selected tasks to the quote line.</span></span>
10. <span data-ttu-id="85c94-132">Изберете **ОК**, за да затворите диалоговия прозорец.</span><span class="sxs-lookup"><span data-stu-id="85c94-132">Select **OK** to close the dialog.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="85c94-133">От страницата за ред на офертата</span><span class="sxs-lookup"><span data-stu-id="85c94-133">From the Quote line page</span></span>

<span data-ttu-id="85c94-134">Можете да асоциирате проектни задачи редове на оферта от раздела **Платими задачи** на страницата **Ред на оферта**.</span><span class="sxs-lookup"><span data-stu-id="85c94-134">You can associate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

>[!NOTE]
><span data-ttu-id="85c94-135">Оптималното място за свързване на проектни задачи към редове на оферта е в раздела **Задача за фактуриране** на страницата **Проект**.</span><span class="sxs-lookup"><span data-stu-id="85c94-135">The optimal place to associate project tasks to quote lines is on the **Task billing** tab on the **Project** page.</span></span> <span data-ttu-id="85c94-136">Ако свързвате задачи от раздела **Платими задачи** на страницата **Ред на оферта** трябва ръчно да свържете всеки проект.</span><span class="sxs-lookup"><span data-stu-id="85c94-136">If you associate tasks from the **Chargeable tasks** tab on **Quote line** page, you must manually associate each project.</span></span>

1. <span data-ttu-id="85c94-137">На раздела **Общи** на базиран на проект ред на оферта проверете дали има избран проект в полето **Проект**.</span><span class="sxs-lookup"><span data-stu-id="85c94-137">On the **General** tab of a project–based quote line, verify that there is a project selected in the **Project** field.</span></span>
2. <span data-ttu-id="85c94-138">В полето **Включени задачи** изберете **Само избрани задачи**.</span><span class="sxs-lookup"><span data-stu-id="85c94-138">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="85c94-139">Запишете базирания на проект ред на оферта.</span><span class="sxs-lookup"><span data-stu-id="85c94-139">Save the project-based quote line.</span></span> <span data-ttu-id="85c94-140">Когато формулярът се обнови, се показва разделът **Платими задачи**.</span><span class="sxs-lookup"><span data-stu-id="85c94-140">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="85c94-141">В раздела **Платими задачи** изберете **Добавете задача за ред на оферта**.</span><span class="sxs-lookup"><span data-stu-id="85c94-141">On the **Chargeable tasks** tab, select **Add a quote line task**.</span></span>
5. <span data-ttu-id="85c94-142">На страницата **Задача на ред на оферта** в полето **Задачи**, изберете задачата и в полето **Тип фактуриране** изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="85c94-142">On the **Quote line task** page, in the **Tasks** field, select the task and in the **Billing type** field, select **Save**.</span></span> 
6. <span data-ttu-id="85c94-143">Затваряне на страницата.</span><span class="sxs-lookup"><span data-stu-id="85c94-143">Close the page.</span></span> <span data-ttu-id="85c94-144">Сега избраната задача е свързана с реда на оферта.</span><span class="sxs-lookup"><span data-stu-id="85c94-144">The selected task is now associated to the quote line.</span></span>

## <a name="disassociate-tasks-from-projectbased-quote-lines"></a><span data-ttu-id="85c94-145">Отделяне на задачи от базирани на проект редове на оферта</span><span class="sxs-lookup"><span data-stu-id="85c94-145">Disassociate tasks from project–based quote lines</span></span>

### <a name="from-the-project-page"></a><span data-ttu-id="85c94-146">От страницата на проекта</span><span class="sxs-lookup"><span data-stu-id="85c94-146">From the Project page</span></span>

<span data-ttu-id="85c94-147">Този метод предоставя най-оптимално изживяване за отделяне на задачите от редове на оферта.</span><span class="sxs-lookup"><span data-stu-id="85c94-147">This method provides the most optimal experience for disassociating tasks from quote lines.</span></span> <span data-ttu-id="85c94-148">Можете да изберете множество задачи и да отделите всички, заедно с техните дъщерни задачи, от избрания ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="85c94-148">You can select multiple tasks and disassociate all of the them, plus their child tasks, from the selected quote line.</span></span>

1. <span data-ttu-id="85c94-149">На раздела **Общи** на базиран на проект ред на оферта проверете в полето **Проект** изберете връзката към проект.</span><span class="sxs-lookup"><span data-stu-id="85c94-149">On the **General** tab of a project–based quote line, in the **Project** field, select the project link.</span></span>
2. <span data-ttu-id="85c94-150">На страницата **Проект** изберете раздела **Фактуриране на задача**.</span><span class="sxs-lookup"><span data-stu-id="85c94-150">On the **Project** page, select the **Task billing** tab.</span></span>
3. <span data-ttu-id="85c94-151">Във втората мрежа, която се отнася за специфична за задачите настройка за фактуриране, изберете една или повече задачи и след това изберете **Отделяне на редове на оферта**.</span><span class="sxs-lookup"><span data-stu-id="85c94-151">In the second grid, which applies to task-specific billing setup, select one or more tasks, and then select **Disassociate quote lines**.</span></span>
4. <span data-ttu-id="85c94-152">В диалоговата страница, която се показва, изберете ред с оферти.</span><span class="sxs-lookup"><span data-stu-id="85c94-152">In the dialog page that appears, select a quote line.</span></span>
5. <span data-ttu-id="85c94-153">Поставете отметка в квадратчето, за да посочите дали асоциацията също трябва да се премахне от дъщерни задачи на избраните задачи.</span><span class="sxs-lookup"><span data-stu-id="85c94-153">Select the check box to indicate whether the association should also be removed from child tasks of the selected tasks.</span></span> <span data-ttu-id="85c94-154">Поставянето на отметка в квадратчето ще отдели и дъщерните задачи на избраните задачи от реда на оферта.</span><span class="sxs-lookup"><span data-stu-id="85c94-154">Checking the box will also disassociate the child tasks of the selected tasks to the quote line.</span></span>
6. <span data-ttu-id="85c94-155">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="85c94-155">Select **OK**.</span></span> <span data-ttu-id="85c94-156">Предупредително съобщение ви информира, че ако премахнете тази асоциация, всички действителни факти, записани по-рано в задачата, могат да бъдат обърнати.</span><span class="sxs-lookup"><span data-stu-id="85c94-156">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
7. <span data-ttu-id="85c94-157">Изберете **ОК**, за да продължите и да премахнете връзката между задачата и базовата линия на проекта.</span><span class="sxs-lookup"><span data-stu-id="85c94-157">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="85c94-158">От страницата за ред на офертата</span><span class="sxs-lookup"><span data-stu-id="85c94-158">From the Quote line page</span></span>

<span data-ttu-id="85c94-159">Можете също да отделите проектни задачи от редове на оферта от раздела **Платими задачи** на страницата **Ред на оферта**.</span><span class="sxs-lookup"><span data-stu-id="85c94-159">You can also disassociate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

1. <span data-ttu-id="85c94-160">В раздела **Платими задачи** изберете **Изтриване на задача на ред на оферта**.</span><span class="sxs-lookup"><span data-stu-id="85c94-160">On the **Chargeable tasks** tab, select **Delete a quote line task**.</span></span>
2. <span data-ttu-id="85c94-161">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="85c94-161">Select **OK**.</span></span> <span data-ttu-id="85c94-162">Предупредително съобщение ви информира, че ако премахнете тази асоциация, всички действителни факти, записани по-рано в задачата, могат да бъдат обърнати.</span><span class="sxs-lookup"><span data-stu-id="85c94-162">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
3. <span data-ttu-id="85c94-163">Изберете **ОК**, за да продължите и да премахнете връзката между задачата и базовата линия на проекта.</span><span class="sxs-lookup"><span data-stu-id="85c94-163">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

>[!NOTE]
> <span data-ttu-id="85c94-164">Тази процедура не изтрива задачата от проекта.</span><span class="sxs-lookup"><span data-stu-id="85c94-164">This procedure doesn't delete the task from the project.</span></span> <span data-ttu-id="85c94-165">Той само премахва асоциацията на задачите от базовата линия на проекта.</span><span class="sxs-lookup"><span data-stu-id="85c94-165">It only removes the task association from the project-based quote line.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]