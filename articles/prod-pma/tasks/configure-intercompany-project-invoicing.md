---
title: Конфигурирайте фактуриране за вътрешнофирмен проект
description: Тази тема показва как да настроите фактуриране на проекти между две компании във вашата организация.
author: Yowelle
manager: AnnBe
ms.date: 07/29/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: VendTable, InterCompanyTradingRelationSetupVendor, SysDataAreaSelectLookup, ProjParameters, ProjPosting, ProjTransferPrice
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 9df15cb3712356a164de3507f5dbc17a9ff9a652
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288366"
---
# <a name="configure-intercompany-project-invoicing"></a><span data-ttu-id="4bfd9-103">Конфигурирайте фактуриране за вътрешнофирмен проект</span><span class="sxs-lookup"><span data-stu-id="4bfd9-103">Configure intercompany project invoicing</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="4bfd9-104">Тази тема показва как да настроите фактуриране на проекти между две компании във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-104">This topic shows how to set up project invoicing between two companies in your organization.</span></span> <span data-ttu-id="4bfd9-105">Тази задача използва набора от данни USSI.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-105">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="4bfd9-106">В навигационния екран отидете на **Модули > Сметки за плащане > Доставчици > Всички доставчици**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-106">In the navigation pane, go to **Modules > Accounts payable > Vendors > All vendors**.</span></span>
2. <span data-ttu-id="4bfd9-107">В списъка **Всички продавачи** намерете и изберете желания запис.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-107">In the **All vendors** list, find and select the desired record.</span></span>
3. <span data-ttu-id="4bfd9-108">В екрана за действие изберете **Общ**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-108">On the Action Pane, select **General**.</span></span>
4. <span data-ttu-id="4bfd9-109">Изберете **Междуфирмена**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-109">Select **Intercompany**.</span></span>
5. <span data-ttu-id="4bfd9-110">Комплект **Активен** на **Да**, за да се даде възможност за вътрешнофирмена търговия.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-110">Set **Active** to **Yes** to enable intercompany trading.</span></span>
6. <span data-ttu-id="4bfd9-111">В полето **Фирма клиент**, въведете или изберете стойност.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-111">In the **Customer company** field, enter or select a value.</span></span>
7. <span data-ttu-id="4bfd9-112">В полето **Моят акаунт**, въведете или изберете стойност.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-112">In the **My account** field, enter or select a value.</span></span>
8. <span data-ttu-id="4bfd9-113">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-113">Select **Save**.</span></span>
9. <span data-ttu-id="4bfd9-114">Затворете страниците, за да се върнете на началната страница.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-114">Close the pages to return to the home page.</span></span>
10. <span data-ttu-id="4bfd9-115">В навигационния екран отидете на **Модули > Управление на проекти и счетоводство > Настройка > Управление на проекти и параметри на счетоводство**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-115">In the navigation pane, go to **Modules > Project management and accounting > Setup > Project management and accounting parameters**.</span></span>
11. <span data-ttu-id="4bfd9-116">Изберете раздела **Междуфирмено**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-116">Select the **Intercompany** tab.</span></span>
12. <span data-ttu-id="4bfd9-117">Преместете плъзгача на **Да**, за да се даде възможност за вътрешнофирмено планиране на ресурси и разписания.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-117">Move the slider to **Yes** to enable intercompany resource scheduling and timesheets.</span></span>
13. <span data-ttu-id="4bfd9-118">В списъка маркирайте избрания ред.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-118">In the list, mark the selected row.</span></span>
14. <span data-ttu-id="4bfd9-119">Изберете **Нова**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-119">Select **New**.</span></span>
15. <span data-ttu-id="4bfd9-120">В полето **Кредитирано юридическо лице**, въведете или изберете стойност.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-120">In the **Borrowing legal entity** field, enter or select a value.</span></span>
16. <span data-ttu-id="4bfd9-121">Изберете квадратчето за отметка **Натрупан приход**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-121">Select the **Accrue revenue** check box.</span></span>
17. <span data-ttu-id="4bfd9-122">В полето **Категория на разписание по подразбиране**, въведете или изберете стойност.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-122">In the **Default timesheet category** field, enter or select a value.</span></span>
18. <span data-ttu-id="4bfd9-123">В полето **Категория на разход по подразбиране**, въведете или изберете стойност.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-123">In the **Default expense category** field, enter or select a value.</span></span>
19. <span data-ttu-id="4bfd9-124">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-124">Select **Save**.</span></span>
20. <span data-ttu-id="4bfd9-125">Затваряне на страницата.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-125">Close the page.</span></span>
21. <span data-ttu-id="4bfd9-126">В навигационния екран отидете на **Модули > Управление на проекти и счетоводство > Настройка> Публикуване > Настройка на публикация на счетоводна книга**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-126">In the navigation pane, go to **Modules > Project management and accounting > Setup > Posting > Ledger posting setup**.</span></span>
22. <span data-ttu-id="4bfd9-127">В полето **Типове сметки на главната книга** изберете опция.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-127">In the **Ledger account types** field, select an option.</span></span>
23. <span data-ttu-id="4bfd9-128">Изберете **Нова**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-128">Select **New**.</span></span>
24. <span data-ttu-id="4bfd9-129">В полето **Основен акаунт** на новия ред, посочете желаните стойности.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-129">In the **Main account** field of the new row, specify the desired values.</span></span>
25. <span data-ttu-id="4bfd9-130">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-130">Select **Save**.</span></span>
26. <span data-ttu-id="4bfd9-131">Затваряне на страницата.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-131">Close the page.</span></span>
27. <span data-ttu-id="4bfd9-132">В навигационния екран отидете на **Модули > Управление на проекти и счетоводство > Настройка> Цени> Цена на трансфер**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-132">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Transfer price**.</span></span>
28. <span data-ttu-id="4bfd9-133">Изберете **Нова**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-133">Select **New**.</span></span>
29. <span data-ttu-id="4bfd9-134">В полето **Дата на влизане в сила** въведете дата.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-134">In the **Effective date** field, enter a date.</span></span>
30. <span data-ttu-id="4bfd9-135">В полето **Кредитирано юридическо лице**, въведете или изберете стойност.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-135">In the **Borrowing legal entity** field, enter or select a value.</span></span>
31. <span data-ttu-id="4bfd9-136">В полето **Модел на трансферна цена** изберете опция.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-136">In the **Transfer price model** field, select an option.</span></span>
32. <span data-ttu-id="4bfd9-137">В полето **Ценообразуване**, въведете число.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-137">In the **Pricing** field, enter a number.</span></span>
33. <span data-ttu-id="4bfd9-138">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="4bfd9-138">Select **Save**.</span></span>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]