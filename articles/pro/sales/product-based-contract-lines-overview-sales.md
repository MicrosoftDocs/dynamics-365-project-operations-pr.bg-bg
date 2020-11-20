---
title: Общ преглед на базирани на продукти аспекти на договор – олекотено
description: Тази тема предоставя информация за аспекти на договор, базирани на продукти.
author: rumant
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: eb09140eae5383b882db73195d0360a836ece791
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177858"
---
# <a name="product-based-contract-lines-overview---lite"></a><span data-ttu-id="da4c8-103">Общ преглед на базирани на продукти аспекти на договор – олекотено</span><span class="sxs-lookup"><span data-stu-id="da4c8-103">Product-based contract lines overview - lite</span></span>

<span data-ttu-id="da4c8-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="da4c8-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="da4c8-105">Можете да създадете базирани на продукти договорни линии в Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="da4c8-105">You can create product-based contract lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="da4c8-106">Аспекти на договор, базирани на продукти, могат да бъдат ръчно създадени редове или могат да бъдат елементи от продуктовия каталог.</span><span class="sxs-lookup"><span data-stu-id="da4c8-106">Product-based contract lines can be manually created lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="da4c8-107">Продуктов каталог</span><span class="sxs-lookup"><span data-stu-id="da4c8-107">Product catalog</span></span>

<span data-ttu-id="da4c8-108">Продуктите в продуктовия каталог имат единица и група единици по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="da4c8-108">The products in the product catalog have a default unit and unit group.</span></span> <span data-ttu-id="da4c8-109">Ако няколко продукта споделят един и същ набор от атрибути, можете да създадете семейство продукти, която също има тези атрибути.</span><span class="sxs-lookup"><span data-stu-id="da4c8-109">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="da4c8-110">Всички продукти в едно семейство продукти наследяват един и същ набор от атрибути.</span><span class="sxs-lookup"><span data-stu-id="da4c8-110">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="da4c8-111">Например фирма продава абонаментни лицензи за различни видове софтуер.</span><span class="sxs-lookup"><span data-stu-id="da4c8-111">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="da4c8-112">Всеки абонаментен софтуер има следните два атрибута:</span><span class="sxs-lookup"><span data-stu-id="da4c8-112">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="da4c8-113">Брой потребители</span><span class="sxs-lookup"><span data-stu-id="da4c8-113">Number of users</span></span>
- <span data-ttu-id="da4c8-114">Продължителност на абонамента (в месеци)</span><span class="sxs-lookup"><span data-stu-id="da4c8-114">Subscription duration (in months)</span></span>

<span data-ttu-id="da4c8-115">За да поддържате този тип каталог, създайте продуктово семейство с име **Абонаментен софтуер**.</span><span class="sxs-lookup"><span data-stu-id="da4c8-115">To maintain this type of catalog, create a product family that is named **Subscription Software**.</span></span> <span data-ttu-id="da4c8-116">Добавете атрибутите, **Брой потребители** и **Продължителност на абонамента** към семейството продукти.</span><span class="sxs-lookup"><span data-stu-id="da4c8-116">Add the attributes, **Number of users** and **Subscription duration** to the product family.</span></span> <span data-ttu-id="da4c8-117">След това добавете отделни продукти към **Абонаментен софтуер** продуктово семейство.</span><span class="sxs-lookup"><span data-stu-id="da4c8-117">Then, add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-contract"></a><span data-ttu-id="da4c8-118">Добавяне на елементи от продуктов каталог към договор по проект</span><span class="sxs-lookup"><span data-stu-id="da4c8-118">Add product catalog items to a project Contract</span></span>

<span data-ttu-id="da4c8-119">Договорите по проекти имат секции за два вида редове: редове, базирани на проекти и базирани на продукти.</span><span class="sxs-lookup"><span data-stu-id="da4c8-119">Project contracts have sections for two types of lines, project-based and product-based.</span></span> <span data-ttu-id="da4c8-120">Продуктовите линии включват всички продукти и единици в ценовата листа на продукта в договора.</span><span class="sxs-lookup"><span data-stu-id="da4c8-120">Product-based lines include all of the products and units in the product price list on the contract.</span></span> <span data-ttu-id="da4c8-121">Продукти, които не са част от ценовата листа за продукти по договор, могат да бъдат добавени.</span><span class="sxs-lookup"><span data-stu-id="da4c8-121">Products that aren't part of contract's product price list can be added.</span></span>

<span data-ttu-id="da4c8-122">Можете да изберете продукти от други ценови листи или директно от продуктовия каталог.</span><span class="sxs-lookup"><span data-stu-id="da4c8-122">You can select products from other price lists, or directly from the product catalog.</span></span> <span data-ttu-id="da4c8-123">Когато избирате продукти директно от продуктов каталог, ценовата листа по подразбиране на този продукт се използва за получаване на продажната цена на продукта.</span><span class="sxs-lookup"><span data-stu-id="da4c8-123">When you select products directly from a product catalog, the default price list of that product is used for the product's sales price.</span></span> <span data-ttu-id="da4c8-124">Ако не е зададена ценова листа по подразбиране, цената се задава на 0 (нула).</span><span class="sxs-lookup"><span data-stu-id="da4c8-124">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="da4c8-125">Ако редът на договор е базиран на продуктов каталог, можете да заместите продажната цена директно в реда.</span><span class="sxs-lookup"><span data-stu-id="da4c8-125">If a contract line is based on a product catalog, you can override the sales price directly on the line.</span></span> <span data-ttu-id="da4c8-126">Договорната линия има поле **Ценообразуване** с двете стойности:</span><span class="sxs-lookup"><span data-stu-id="da4c8-126">A contract line has the **Pricing** field with the two values:</span></span>

- <span data-ttu-id="da4c8-127">**Заместване на ценообразуване**</span><span class="sxs-lookup"><span data-stu-id="da4c8-127">**Override pricing**</span></span>
- <span data-ttu-id="da4c8-128">**Да се използва това по подразбиране**</span><span class="sxs-lookup"><span data-stu-id="da4c8-128">**Use default**</span></span>

<span data-ttu-id="da4c8-129">Ако зададете полето **Ценообразуване** на **Заместване на ценообразуване**, не се задава цена по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="da4c8-129">If you set the **Pricing** field to **Override pricing**, the default price isn't set.</span></span> <span data-ttu-id="da4c8-130">Въведете цената за продукта в аспектите на договора.</span><span class="sxs-lookup"><span data-stu-id="da4c8-130">Enter a price for the product on the contract line.</span></span> <span data-ttu-id="da4c8-131">Ако зададете полето на **Използвай по подразбиране**, използва се стандартната продажна цена и полето не може да се редактира.</span><span class="sxs-lookup"><span data-stu-id="da4c8-131">If you set the field to **Use default**, the default sales price is used and the field can't be edited.</span></span>

<span data-ttu-id="da4c8-132">След като инсталирате Project Operations, продажните цени по подразбиране се въвеждат в базираните на продукт аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="da4c8-132">After you install Project Operations, default sales prices are entered on the product-based lines on a contract.</span></span> <span data-ttu-id="da4c8-133">След това полето **Ценообразуване** се задава на **Заместване на ценообразуване**, така че да можете да редактирате цената по подразбиране в аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="da4c8-133">The **Pricing** field is set to **Override pricing** so that you can edit the default price on the contract lines.</span></span> <span data-ttu-id="da4c8-134">Това е специфично за Project Operations заместване на продуктово базираното поведение на линии в Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="da4c8-134">This is a Project Operations-specific override to product-based lines behavior in Dynamics 365 Sales.</span></span>
