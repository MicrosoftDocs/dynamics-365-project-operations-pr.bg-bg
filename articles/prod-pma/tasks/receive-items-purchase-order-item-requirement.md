---
title: Получавайте артикули по поръчка за покупка от изискването за артикул
description: Тази тема обяснява как да получавате артикули в поръчка за покупка от изискване за артикул.
author: Yowelle
ms.date: 08/06/2019
ms.topic: business-process
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage, ProjTable, ProjSalesItemReq, InventItemIdLookupSimple, PurchCreateFromSalesOrder, VendAccountItemLookup, PurchTable, PurchEditLines
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 0e0c4a75f1d86538cc773af1f7c0ae3c83ef0ad5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6011673"
---
# <a name="receive-items-on-purchase-order-from-item-requirement"></a><span data-ttu-id="63a72-103">Получавайте артикули по поръчка за покупка от изискването за артикул</span><span class="sxs-lookup"><span data-stu-id="63a72-103">Receive items on purchase order from item requirement</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="63a72-104">Тази тема обяснява как да получавате артикули в поръчка за покупка от изискване за артикул.</span><span class="sxs-lookup"><span data-stu-id="63a72-104">This topic explains how to receive items on a purchase order from an item requirement.</span></span>

<span data-ttu-id="63a72-105">Използвайки изискване за артикул вместо транзакция на артикул, можете да планирате доставка точно преди артикулът да бъде реално използван, да създадете поръчка за покупка, да включите артикула в рамката на търговското споразумение и да включите изискването за артикул в производственото планиране.</span><span class="sxs-lookup"><span data-stu-id="63a72-105">By using an item requirement instead of an item transaction, you can plan for delivery just before the item is actually used, create a purchase order, include the item in the trade-agreement framework, and include the item requirement in production planning.</span></span> 

<span data-ttu-id="63a72-106">Тази задача използва набора от данни USSI.</span><span class="sxs-lookup"><span data-stu-id="63a72-106">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="63a72-107">В навигационния екран отидете на **Модули > Управление на проекти и счетоводство > Проекти > Всички проекти**.</span><span class="sxs-lookup"><span data-stu-id="63a72-107">In the navigation pane, go to **Modules > Project management and accounting > Projects > All projects**.</span></span>
2. <span data-ttu-id="63a72-108">В списъка изберете връзката в желания ред.</span><span class="sxs-lookup"><span data-stu-id="63a72-108">In the list, select the link in the desired row.</span></span>
3. <span data-ttu-id="63a72-109">В екрана за действие изберете **План**.</span><span class="sxs-lookup"><span data-stu-id="63a72-109">On the Action Pane, select **Plan**.</span></span>
4. <span data-ttu-id="63a72-110">Изберете **Изисквания към артикулите**.</span><span class="sxs-lookup"><span data-stu-id="63a72-110">Select **Item requirements**.</span></span>
5. <span data-ttu-id="63a72-111">Изберете **Нова**.</span><span class="sxs-lookup"><span data-stu-id="63a72-111">Select **New**.</span></span>
6. <span data-ttu-id="63a72-112">В новия ред въведете или изберете стойност в полето **Номер на артикул**.</span><span class="sxs-lookup"><span data-stu-id="63a72-112">In the new row, enter or select a value in the **Item number** field.</span></span>
7. <span data-ttu-id="63a72-113">В полето **Количество**, въведете число.</span><span class="sxs-lookup"><span data-stu-id="63a72-113">In the **Quantity** field, enter a number.</span></span>
8. <span data-ttu-id="63a72-114">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="63a72-114">Select **Save**.</span></span>
9. <span data-ttu-id="63a72-115">В екрана за действие изберете **Управление**.</span><span class="sxs-lookup"><span data-stu-id="63a72-115">On the Action Pane, select **Manage**.</span></span>
10. <span data-ttu-id="63a72-116">Изберете **Функции**.</span><span class="sxs-lookup"><span data-stu-id="63a72-116">Select **Functions**.</span></span>
11. <span data-ttu-id="63a72-117">Избор на **Създаване на поръчка за покупка**.</span><span class="sxs-lookup"><span data-stu-id="63a72-117">Select **Create purchase order**.</span></span>
12. <span data-ttu-id="63a72-118">Изберете отметка в квадратчето **Включване на всички**.</span><span class="sxs-lookup"><span data-stu-id="63a72-118">Select the **Include all** check box.</span></span>
13. <span data-ttu-id="63a72-119">В полето **Акаунт на доставчик**, въведете или изберете стойност.</span><span class="sxs-lookup"><span data-stu-id="63a72-119">In the **Vendor account** field, enter or select a value.</span></span>
14. <span data-ttu-id="63a72-120">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="63a72-120">Select **OK**.</span></span>
15. <span data-ttu-id="63a72-121">В навигационния екран отидете на **Модули > Сметки за плащане > Поръчки за покупка > Всички поръчки за покупка**.</span><span class="sxs-lookup"><span data-stu-id="63a72-121">In the navigation pane, go to **Modules > Accounts payable > Purchase orders > All purchase orders**.</span></span>
16. <span data-ttu-id="63a72-122">В списъка изберете връзката в желания ред.</span><span class="sxs-lookup"><span data-stu-id="63a72-122">In the list, select the link in the desired row.</span></span>
17. <span data-ttu-id="63a72-123">В екрана за действие изберете **Покупка**.</span><span class="sxs-lookup"><span data-stu-id="63a72-123">On the Action Pane, select **Purchase**.</span></span>
18. <span data-ttu-id="63a72-124">Изберете **Потвърждение**.</span><span class="sxs-lookup"><span data-stu-id="63a72-124">Select **Confirm**.</span></span>
19. <span data-ttu-id="63a72-125">В екрана за действие изберете **Получаване**.</span><span class="sxs-lookup"><span data-stu-id="63a72-125">On the Action Pane, select **Receive**.</span></span>
20. <span data-ttu-id="63a72-126">Изберете **Разписка на продукта**.</span><span class="sxs-lookup"><span data-stu-id="63a72-126">Select **Product receipt**.</span></span>
21. <span data-ttu-id="63a72-127">В полето **Разписка на продукта** въведете стойност.</span><span class="sxs-lookup"><span data-stu-id="63a72-127">In the **Product receipt** field, type a value.</span></span>
22. <span data-ttu-id="63a72-128">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="63a72-128">Select **OK**.</span></span>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]