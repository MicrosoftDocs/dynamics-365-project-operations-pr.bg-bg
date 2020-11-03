---
title: Поръчки за продажба за проект
description: Тази статия описва различните методи, които можете да използвате за създаване на поръчки за покупка за проект. Методът, който използвате зависи от целта на поръчката за покупка и кога закупените артикули се консумират и таксуват по даден проект.
author: Yowelle
manager: AnnBe
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 83972
ms.assetid: 247e4d72-610b-4fa5-9873-601ed0f4b2d6
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: bd891aec5bcab66c5801a5d9ca8abbbf632d662d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071808"
---
# <a name="purchase-orders-for-a-project"></a><span data-ttu-id="64b2a-104">Поръчки за продажба за проект</span><span class="sxs-lookup"><span data-stu-id="64b2a-104">Purchase orders for a project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="64b2a-105">Тази статия описва различните методи, които можете да използвате за създаване на поръчки за покупка за проект.</span><span class="sxs-lookup"><span data-stu-id="64b2a-105">This article describes the various methods that you can use to create purchase orders for a project.</span></span> <span data-ttu-id="64b2a-106">Методът, който използвате зависи от целта на поръчката за покупка и кога закупените артикули се консумират и таксуват по даден проект.</span><span class="sxs-lookup"><span data-stu-id="64b2a-106">The method that you use depends on the purpose of the purchase order, and when the purchased items are consumed and charged to a project.</span></span>

### <a name="methods-for-creating-a-purchase-order"></a><span data-ttu-id="64b2a-107">Методи за създаване на поръчка за покупка</span><span class="sxs-lookup"><span data-stu-id="64b2a-107">Methods for creating a purchase order</span></span>

<span data-ttu-id="64b2a-108">Можете да използвате един от следните методи за създаване на поръчка за покупка в Управление на проекти и счетоводство.</span><span class="sxs-lookup"><span data-stu-id="64b2a-108">You can use one of the following methods to create a purchase order in Project management and accounting.</span></span> <span data-ttu-id="64b2a-109">Целта на поръчката за покупка определя кога поръчката за покупка се консумира и следователно кога артикулите се таксуват по даден проект.</span><span class="sxs-lookup"><span data-stu-id="64b2a-109">The purpose of the purchase order determines when the purchase order is consumed and, therefore, when items are charged to a project.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="64b2a-110">Метод</span><span class="sxs-lookup"><span data-stu-id="64b2a-110">Method</span></span></th>
<th><span data-ttu-id="64b2a-111">Цел</span><span class="sxs-lookup"><span data-stu-id="64b2a-111">Purpose</span></span></th>
<th><span data-ttu-id="64b2a-112">Консумация на артикули</span><span class="sxs-lookup"><span data-stu-id="64b2a-112">Consumption of items</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="64b2a-113">Създаване на поръчка за покупка директно от проект.</span><span class="sxs-lookup"><span data-stu-id="64b2a-113">Create a purchase order directly from a project.</span></span></td>
<td><span data-ttu-id="64b2a-114">Използвайте този метод за закупуване на артикули от външен доставчик за потребление по проект.</span><span class="sxs-lookup"><span data-stu-id="64b2a-114">Use this method to purchase items from an external vendor for consumption on a project.</span></span> <span data-ttu-id="64b2a-115">Можете да създадете поръчка за покупка по два начина:</span><span class="sxs-lookup"><span data-stu-id="64b2a-115">You can create the purchase order in two ways:</span></span>
<ul>
<li><span data-ttu-id="64b2a-116">От самия проект.</span><span class="sxs-lookup"><span data-stu-id="64b2a-116">From the project itself.</span></span> <span data-ttu-id="64b2a-117">В този случай проектът вече е дефиниран за поръчката за покупка.</span><span class="sxs-lookup"><span data-stu-id="64b2a-117">In this case, the project is already defined for the purchase order.</span></span></li>
<li><span data-ttu-id="64b2a-118">Чрез навигация до поръчката за закупуване на проект.</span><span class="sxs-lookup"><span data-stu-id="64b2a-118">By navigating to the project purchase order.</span></span> <span data-ttu-id="64b2a-119">Трябва да изберете както доставчика, така и проекта, за да създадете поръчка за покупка.</span><span class="sxs-lookup"><span data-stu-id="64b2a-119">You must select both the vendor and the project to create the purchase order for.</span></span></li>
</ul></td>
<td><span data-ttu-id="64b2a-120">Елементите се консумират, когато фактурата на доставчика се актуализира.</span><span class="sxs-lookup"><span data-stu-id="64b2a-120">Items are consumed when the vendor invoice is updated.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="64b2a-121">Създаване на поръчка за покупка от поръчка за продажби.</span><span class="sxs-lookup"><span data-stu-id="64b2a-121">Create a purchase order from a sales order.</span></span></td>
<td><span data-ttu-id="64b2a-122">Използвайте този метод, за да закупите артикули, когато създавате поръчка за продажба от проект.</span><span class="sxs-lookup"><span data-stu-id="64b2a-122">Use this method to purchase items when you create a sales order from a project.</span></span></td>
<td><span data-ttu-id="64b2a-123">Артикулите се консумират, когато поръчката за продажба е фактурирана на клиента.</span><span class="sxs-lookup"><span data-stu-id="64b2a-123">Items are consumed when the sales order is invoiced to the customer.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="64b2a-124">Създайте поръчка за покупка от изискване за артикул.</span><span class="sxs-lookup"><span data-stu-id="64b2a-124">Create a purchase order from an item requirement.</span></span></td>
<td><span data-ttu-id="64b2a-125">Използвайте този метод, за да закупите артикули, когато създавате изискване за артикул от проект.</span><span class="sxs-lookup"><span data-stu-id="64b2a-125">Use this method to purchase items when you create an item requirement from a project.</span></span></td>
<td><span data-ttu-id="64b2a-126">Артикулите се консумират, когато се актуализира бланката за опаковане на изискване за артикул.</span><span class="sxs-lookup"><span data-stu-id="64b2a-126">Items are consumed when the item requirement packing slip is updated.</span></span></td>
</tr>
</tbody>
</table>

> [!NOTE] 
> <span data-ttu-id="64b2a-127">Когато актуализирате фактурата на доставчика или фиша за опаковане, ще бъдете подканени да актуализирате фиша за опаковане според изискването за артикула.</span><span class="sxs-lookup"><span data-stu-id="64b2a-127">When you update the vendor invoice or packing slip, you're prompted to update the packing slip on the item requirement.</span></span>

<span data-ttu-id="64b2a-128">За повече информация вижте [Получавайте артикули по поръчка за покупка от изискването за артикул](tasks/receive-items-purchase-order-item-requirement.md).</span><span class="sxs-lookup"><span data-stu-id="64b2a-128">For more information, see [Receive items on purchase order from item requirement](tasks/receive-items-purchase-order-item-requirement.md).</span></span>

