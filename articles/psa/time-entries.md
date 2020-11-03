---
title: Създаване на записи за време
description: Тази тема предоставя информация за това как да създадете записи за време.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/20/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 878413a24baa340b745a045a6991a63a00851c8b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071911"
---
# <a name="create-time-entries"></a><span data-ttu-id="b56d0-103">Създаване на записи за време</span><span class="sxs-lookup"><span data-stu-id="b56d0-103">Create time entries</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="b56d0-104">В предишните версии на Dynamics 365 Project Service Automation записите за време се въвеждаха ежеседмично.</span><span class="sxs-lookup"><span data-stu-id="b56d0-104">In previous versions of Dynamics 365 Project Service Automation, time entries were entered on a weekly basis.</span></span> <span data-ttu-id="b56d0-105">Във версия 3 на Project Service Automation записите за време се въвеждат ежедневно.</span><span class="sxs-lookup"><span data-stu-id="b56d0-105">In version 3 of Project Service Automation, time entries are entered on a daily basis.</span></span> <span data-ttu-id="b56d0-106">След като създадете няколко записа за време обаче, можете да ги създавате или копирате групово.</span><span class="sxs-lookup"><span data-stu-id="b56d0-106">However, after a few time entries have been created, you can bulk create or copy them.</span></span>

## <a name="create-a-time-entry"></a><span data-ttu-id="b56d0-107">Създаване на запис за време</span><span class="sxs-lookup"><span data-stu-id="b56d0-107">Create a time entry</span></span>

<span data-ttu-id="b56d0-108">Изпълнете следните стъпки, за да създадете запис за време.</span><span class="sxs-lookup"><span data-stu-id="b56d0-108">Follow these steps to create a time entry.</span></span>

1. <span data-ttu-id="b56d0-109">На страницата **Записи за време** изберете **Нов**.</span><span class="sxs-lookup"><span data-stu-id="b56d0-109">On the **Time Entries** page, select **New**.</span></span>
2. <span data-ttu-id="b56d0-110">В диалоговия прозорец **Бързо създаване: запис за време** въведете продължителността на записа за време в минути, часове или дни.</span><span class="sxs-lookup"><span data-stu-id="b56d0-110">In the **Quick Create: Time Entry** dialog box, enter the duration of the time entry in minutes, hours, or days.</span></span> <span data-ttu-id="b56d0-111">Продължителността трябва да се въведе в следния формат: *х* минути, *x* часа или *х* дни.</span><span class="sxs-lookup"><span data-stu-id="b56d0-111">The duration must be entered in the following format: *x* minutes, *x* hours, or *x* days.</span></span> <span data-ttu-id="b56d0-112">Часове и дни може също да бъдат въвеждани с десетични числа, като например, *x,x* часа или *x,x* дни.</span><span class="sxs-lookup"><span data-stu-id="b56d0-112">Hours and days can also be entered as decimal values, such as *x.x* hours or *x.x* days.</span></span>
3. <span data-ttu-id="b56d0-113">Изберете вида на записа за време и проекта, за който въвеждате записа за време.</span><span class="sxs-lookup"><span data-stu-id="b56d0-113">Select the type of time entry and the project that you're entering the time entry for.</span></span>
4. <span data-ttu-id="b56d0-114">В полето **Задача по проект** намерете задачата за този запис за време.</span><span class="sxs-lookup"><span data-stu-id="b56d0-114">In the **Project Task** field, find the task for this time entry.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b56d0-115">Ако създавате запис за време за задача, която не е присвоена на потребител, в полето **Задача по проекта** изберете бутона **Търсене** , изберете **Промяна на изгледа** , след което изберете **Всички активни задачи по проекта** за да изведете списък с всички задачи.</span><span class="sxs-lookup"><span data-stu-id="b56d0-115">If you're creating a time entry for a task that isn't assigned to a user, in the **Project Task** field, select the **Search** button, select **Change View** , and then select **All Active Project Tasks** to list all tasks.</span></span>

5. <span data-ttu-id="b56d0-116">Въведете описание, ако е необходимо описание, след което изберете **Записване и затваряне**.</span><span class="sxs-lookup"><span data-stu-id="b56d0-116">Enter a description, if a description is required, and then select **Save and Close**.</span></span>

<span data-ttu-id="b56d0-117">След като записът за време бъде създаден и записан, можете да го редактирате в мрежата за записи за време.</span><span class="sxs-lookup"><span data-stu-id="b56d0-117">After the time entry is created and saved, you can edit it in the time entry grid.</span></span> <span data-ttu-id="b56d0-118">Мрежата за записи за време поддържа два формата:</span><span class="sxs-lookup"><span data-stu-id="b56d0-118">The time entry grid supports two formats:</span></span>

- <span data-ttu-id="b56d0-119">Можете да въвеждате записи за време във формат **чч:мм**.</span><span class="sxs-lookup"><span data-stu-id="b56d0-119">You can enter time entries in **hh:mm** format.</span></span> <span data-ttu-id="b56d0-120">Този формат след това се преобразува в часове и дроби.</span><span class="sxs-lookup"><span data-stu-id="b56d0-120">This format is then converted to hours and fractions.</span></span>
- <span data-ttu-id="b56d0-121">Можете да въведете часове и дроби директно.</span><span class="sxs-lookup"><span data-stu-id="b56d0-121">You can enter hours and fractions directly.</span></span>

<span data-ttu-id="b56d0-122">Имайте предвид, че дробите на един час не са минути.</span><span class="sxs-lookup"><span data-stu-id="b56d0-122">Note that the fractions of an hour aren't minutes.</span></span> <span data-ttu-id="b56d0-123">Ето защо 1,5 часа представлява 1 час и 30 минути.</span><span class="sxs-lookup"><span data-stu-id="b56d0-123">Therefore, 1.5 hours represents 1 hour and 30 minutes.</span></span> <span data-ttu-id="b56d0-124">Същото правило важи и за дробите на ден.</span><span class="sxs-lookup"><span data-stu-id="b56d0-124">The same rule applies to fractions of a day.</span></span> <span data-ttu-id="b56d0-125">Един ден е 24 часа, а 0,5 дни представляват 12 часа.</span><span class="sxs-lookup"><span data-stu-id="b56d0-125">One day is 24 hours, and 0.5 days represents 12 hours.</span></span>

## <a name="bulk-create-time-entries"></a><span data-ttu-id="b56d0-126">Групово създаване на записи за време</span><span class="sxs-lookup"><span data-stu-id="b56d0-126">Bulk create time entries</span></span>

<span data-ttu-id="b56d0-127">След като са създадени няколко записа за време, можете да ги копирате, за да създадете групово допълнителни записи за време.</span><span class="sxs-lookup"><span data-stu-id="b56d0-127">After a few time entries have been created, you can copy them to create additional time entries in bulk.</span></span>

1. <span data-ttu-id="b56d0-128">На страницата **Записи за време** изберете **Копиране на седмица**.</span><span class="sxs-lookup"><span data-stu-id="b56d0-128">On the **Time Entries** page, select **Copy Week**.</span></span>
2. <span data-ttu-id="b56d0-129">В групата на полето **От период** в полетата **Начална дата** и **Крайна дата** , дефинирайте интервала от дати, от който да се копират записи за време.</span><span class="sxs-lookup"><span data-stu-id="b56d0-129">In the **From Period** field group, in the **Start Date** and **End Date** fields, define the date range to copy time entries from.</span></span>
3. <span data-ttu-id="b56d0-130">В групата на полето **В период** в полето **Начална дата** посочете датата, за която да се създадат записи за време.</span><span class="sxs-lookup"><span data-stu-id="b56d0-130">In the **To Period** field group, in the **Start Date** field, specify the date to create time entries for.</span></span>
4. <span data-ttu-id="b56d0-131">Изберете **Копиране** , за да създадете копие на записите за време, които съответстват на деня от седмицата, указан в групата на полето **В период**.</span><span class="sxs-lookup"><span data-stu-id="b56d0-131">Select **Copy** to create a copy of the time entries that correspond to the day of the week that is specified in the **To Period** field group.</span></span> <span data-ttu-id="b56d0-132">Например записът за време за понеделник от миналата седмица ще бъде копиран в понеделника на седмицата, посочена в групата на полето **В период**.</span><span class="sxs-lookup"><span data-stu-id="b56d0-132">For example, the time entry for Monday of last week is copied to Monday of the week that is specified in the **To Period** field group.</span></span>

## <a name="import-data-for-time-entries"></a><span data-ttu-id="b56d0-133">Импортиране на данни за записи за време</span><span class="sxs-lookup"><span data-stu-id="b56d0-133">Import data for time entries</span></span>

<span data-ttu-id="b56d0-134">Можете да импортирате данни от резервации и присвоявания за проекти.</span><span class="sxs-lookup"><span data-stu-id="b56d0-134">You can import data from project bookings and assignments.</span></span> <span data-ttu-id="b56d0-135">Когато импортирате данни, можете да укажете диапазона от дати за резервациите за импортиране и след това изрично да изберете резервациите, които трябва да бъдат създадени като **Чернова** на записи за време.</span><span class="sxs-lookup"><span data-stu-id="b56d0-135">When you import data, you can specify the date range of the bookings to import and then explicitly select the bookings that should be created as **Draft** time entries.</span></span>

## <a name="group-by-sort-search-and-filter-capabilities"></a><span data-ttu-id="b56d0-136">Възможности за групиране по, сортиране, търсене и филтриране</span><span class="sxs-lookup"><span data-stu-id="b56d0-136">Group by, sort, search, and filter capabilities</span></span>

<span data-ttu-id="b56d0-137">Можете да групирате и филтрирате записите за време по измеренията, указани в колоните.</span><span class="sxs-lookup"><span data-stu-id="b56d0-137">You can group and filter time entries by the dimensions that are specified in the columns.</span></span> <span data-ttu-id="b56d0-138">В полето **Групиране по** изберете измерението, което да се използва за филтриране на записите за време.</span><span class="sxs-lookup"><span data-stu-id="b56d0-138">In the **Group by** field, select the dimension to use to filter time entries.</span></span> <span data-ttu-id="b56d0-139">Можете също да сортирате записите за време във възходящ или низходящ ред, като използвате стрелката за сортиране в заглавките на колоните.</span><span class="sxs-lookup"><span data-stu-id="b56d0-139">You can also sort the time entry records in ascending or descending order by using the sort arrow on the column headings.</span></span> <span data-ttu-id="b56d0-140">Освен това можете да показвате или скривате записи, като изберете бутона **Филтриране** в заглавките на колоните и след това в полето **Търсене** въведете текста, който трябва да се използва за търсене на записи за време по име на проект, задача по проект, запис за време или ресурс.</span><span class="sxs-lookup"><span data-stu-id="b56d0-140">Additionally, you can show or hide entries by selecting the **Filter** button on the column headings, and then, in the **Search** box, entering the text that should be used to search for time entries by project name, project task, time entry, or resource.</span></span>
