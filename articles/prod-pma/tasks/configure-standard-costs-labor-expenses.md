---
title: Конфигурирайте стандартни разходи за труд и разходи
description: Тази тема обяснява как да настроите стандартни разходи за труд и разходи за проект.
author: Yowelle
manager: AnnBe
ms.date: 08/02/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjCostPriceHour, ProjSalesPriceHour, ProjCostPriceExpense, ProjSalesPriceCost
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: b16ed50584b2b4535d1c61fe7069708182a4820e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288321"
---
# <a name="configure-standard-costs-for-labor-and-expenses"></a><span data-ttu-id="e9bc3-103">Конфигурирайте стандартни разходи за труд и разходи</span><span class="sxs-lookup"><span data-stu-id="e9bc3-103">Configure standard costs for labor and expenses</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="e9bc3-104">Тази тема обяснява как да настроите стандартни разходи за труд и разходи за проект.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-104">This topic explains how to set up standard costs for labor and expenses for a project.</span></span> <span data-ttu-id="e9bc3-105">Тази задача използва набора от данни USSI.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-105">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="e9bc3-106">В навигационния екран отидете на **Модули > Управление на проекти и счетоводство > Настройка> Цени> Разходна цена (час)**.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-106">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Cost price (hour)**.</span></span>
2. <span data-ttu-id="e9bc3-107">Изберете **Нова**.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-107">Select **New**.</span></span>
3. <span data-ttu-id="e9bc3-108">В полето **Дата на влизане в сила** въведете дата.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-108">In the **Effective date** field, enter a date.</span></span>
4. <span data-ttu-id="e9bc3-109">В полето **себестойност**, въведете номер.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-109">In the **Cost price** field, enter a number.</span></span> <span data-ttu-id="e9bc3-110">Можете да зададете стандартна себестойност за категорията на проекта или можете да настроите себестойност по номер на работник, номер на проект, категория, дата или комбинация от тях.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-110">You can set up a standard cost price for the project category, or you can set up a cost price by worker number, project number, category, date, or any combination of these.</span></span> <span data-ttu-id="e9bc3-111">Разходната цена, която се прилага, е себестойността с най-високо ниво на детайлност.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-111">The cost price that is applied is the cost price with the highest level of detail.</span></span>  
5. <span data-ttu-id="e9bc3-112">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-112">Select **Save**.</span></span>
6. <span data-ttu-id="e9bc3-113">В навигационния екран отидете на **Модули > Управление на проекти и счетоводство > Настройка> Цени> Цена на продажба (час)**.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-113">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Sales price (hour)**.</span></span>
7. <span data-ttu-id="e9bc3-114">Изберете **Нова**.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-114">Select **New**.</span></span>
8. <span data-ttu-id="e9bc3-115">В полето **Дата на влизане в сила** въведете дата.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-115">In the **Effective date** field, enter a date.</span></span>
9. <span data-ttu-id="e9bc3-116">В полето **Валидно за** изберете опция.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-116">In the **Valid for** field, select an option.</span></span>
10. <span data-ttu-id="e9bc3-117">В полето **Ценообразуване**, въведете число.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-117">In the **Pricing** field, enter a number.</span></span> <span data-ttu-id="e9bc3-118">Можете да зададете стандартна продажна цена за часови транзакции или за категория проекти.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-118">You can set up a standard sales price for hour transactions or for a project category.</span></span> <span data-ttu-id="e9bc3-119">Можете също така да настроите продажните цени по номер на работник, номер на проект, категория, дата на транзакция или комбинация от тях.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-119">You can also set up sales prices by worker number, project number, category, transaction date, or any combination of these.</span></span> <span data-ttu-id="e9bc3-120">Действителната продажна цена, която се прилага, когато работник въведе транзакция в дневника Час, е продажната цена с най-високо ниво на детайлност.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-120">The actual sales price, which is applied when a worker enters a transaction in the Hour journal, is the sales price with the highest level of detail.</span></span> <span data-ttu-id="e9bc3-121">Например, ако са зададени както обща продажна цена, така и специфична за работника продажна цена, се използва специфична за работника продажна цена.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-121">For example, if both a general sales price and a worker-specific sales price are set up, the worker-specific sales price is used.</span></span>  
11. <span data-ttu-id="e9bc3-122">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-122">Select **Save**.</span></span>
12. <span data-ttu-id="e9bc3-123">Затваряне на страницата.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-123">Close the page.</span></span>
13. <span data-ttu-id="e9bc3-124">В навигационния екран отидете на **Модули > Управление на проекти и счетоводство > Настройка> Цени> Разходна цена (разход)**.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-124">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Cost price (expense)**.</span></span>
14. <span data-ttu-id="e9bc3-125">Изберете **Нова**.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-125">Select **New**.</span></span>
15. <span data-ttu-id="e9bc3-126">В полето **Дата на влизане в сила** въведете дата.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-126">In the **Effective date** field, enter a date.</span></span>
16. <span data-ttu-id="e9bc3-127">В полето **себестойност**, въведете номер.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-127">In the **Cost price** field, enter a number.</span></span> <span data-ttu-id="e9bc3-128">Могат да се попълнят множество полета, но това е минимумът, необходим за запазване на записа.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-128">Multiple fields can be filled in, but this is the minimum needed to save the record.</span></span>  
17. <span data-ttu-id="e9bc3-129">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-129">Select **Save**.</span></span>
18. <span data-ttu-id="e9bc3-130">В навигационния екран отидете на **Модули > Управление на проекти и счетоводство > Настройка> Цени> Цена на продажби (разход)**.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-130">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Sales price (expense)**.</span></span>
19. <span data-ttu-id="e9bc3-131">Изберете **Нова**.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-131">Select **New**.</span></span>
20. <span data-ttu-id="e9bc3-132">В полето **Дата на влизане в сила** въведете дата.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-132">In the **Effective date** field, enter a date.</span></span>
21. <span data-ttu-id="e9bc3-133">В полето **Валидно за** изберете опция.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-133">In the **Valid for** field, select an option.</span></span>
22. <span data-ttu-id="e9bc3-134">В полето **Ценообразуване**, въведете число.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-134">In the **Pricing** field, enter a number.</span></span> <span data-ttu-id="e9bc3-135">Действителната продажна цена, която се прилага, когато работник въведе транзакции в дневника за разходи, е продажната цена с най-високо ниво на детайлност.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-135">The actual sales price, which is applied when a worker enters transactions in an expense journal, is the sales price with the highest level of detail.</span></span> <span data-ttu-id="e9bc3-136">Например, ако са зададени както обща, така и специфична за работника продажна цена, се използва специфична за работника продажна цена.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-136">For example, if both a general and a worker-specific sales price are set up, the worker-specific sales price is used.</span></span>  
23. <span data-ttu-id="e9bc3-137">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="e9bc3-137">Select **Save**.</span></span>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]