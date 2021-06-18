---
title: Общ преглед на базирана на продукт оферта – олекотен
description: Тази тема предоставя информация за работа с редове на оферти, базирани на продукти.
author: rumant
ms.date: 10/30/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5cc3a97194e01b14de054a93a6268c1f0c24bc25
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994438"
---
# <a name="product-based-quote-lines-overview---lite"></a><span data-ttu-id="8647f-103">Общ преглед на базирана на продукт оферта – олекотен</span><span class="sxs-lookup"><span data-stu-id="8647f-103">Product-based quote lines overview - lite</span></span>

<span data-ttu-id="8647f-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="8647f-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8647f-105">Можете да създавате редове на оферти, базирани на продукти, в Dynamics 365 Project Operations</span><span class="sxs-lookup"><span data-stu-id="8647f-105">You can create product-based quote lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="8647f-106">Редовете на оферти, базирани на продукти, могат да бъдат добавени ръчно или могат да бъдат елементи от продуктовия каталог.</span><span class="sxs-lookup"><span data-stu-id="8647f-106">Product-based quote lines can be manually added, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="8647f-107">Продуктов каталог</span><span class="sxs-lookup"><span data-stu-id="8647f-107">Product catalog</span></span>

<span data-ttu-id="8647f-108">Всеки продукт в продуктовия каталог има единица и опаковъчна единица по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="8647f-108">Each product in the product catalog has a default unit and unit group.</span></span> <span data-ttu-id="8647f-109">Ако няколко продукта споделят един и същ набор от атрибути, можете да създадете семейство продукти, което споделя тези атрибути.</span><span class="sxs-lookup"><span data-stu-id="8647f-109">If multiple products share the same set of attributes, you can create a product family that share those attributes.</span></span> 

<span data-ttu-id="8647f-110">Например фирма продава абонаментни лицензи за различни видове софтуер.</span><span class="sxs-lookup"><span data-stu-id="8647f-110">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="8647f-111">Всеки абонаментен софтуер има следните два атрибута:</span><span class="sxs-lookup"><span data-stu-id="8647f-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="8647f-112">Брой потребители</span><span class="sxs-lookup"><span data-stu-id="8647f-112">Number of users</span></span>
- <span data-ttu-id="8647f-113">Продължителност на абонамента, измерена в месеци</span><span class="sxs-lookup"><span data-stu-id="8647f-113">A subscription duration measured in months</span></span>

<span data-ttu-id="8647f-114">За поддържане на този тип каталог създайте семейство продукти, което се нарича **Абонаментен софтуер** и добавете броя потребители и продължителността на абонамента като атрибути.</span><span class="sxs-lookup"><span data-stu-id="8647f-114">To maintain this type of catalog, create a product family named **Subscription Software** and add the number of users and the subscription duration as attributes.</span></span> <span data-ttu-id="8647f-115">След това можете да добавяте отделни продукти към семейството продукти **Абонаментен софтуер**.</span><span class="sxs-lookup"><span data-stu-id="8647f-115">Next, you can add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="8647f-116">Добавяне на елементи от продуктов каталог към оферта по проект</span><span class="sxs-lookup"><span data-stu-id="8647f-116">Add product catalog items to a project quote</span></span>

<span data-ttu-id="8647f-117">Страниците **Оферта по проект** и **Договор по проект** имат секции за редове, базирани на проекти, и редове, базирани на продукти.</span><span class="sxs-lookup"><span data-stu-id="8647f-117">The **Project Quote** and **Project Contract** pages have sections for project-based lines and product-based lines.</span></span> <span data-ttu-id="8647f-118">За базирани на продукт редове падащият списък в реда на офертата или аспектите на договора по проект включва всички продукти и единици в ценовата листа на продукта.</span><span class="sxs-lookup"><span data-stu-id="8647f-118">For product-based lines, the drop-down list on the quote line or project contract line includes all the products and units in the product price list.</span></span> <span data-ttu-id="8647f-119">Можете също да добавяте продукти, които не са част от ценовата листа на продуктите.</span><span class="sxs-lookup"><span data-stu-id="8647f-119">You can also add products that aren't part of the product price list.</span></span>

<span data-ttu-id="8647f-120">Освен това можете да изберете продукти от други ценови листи или директно от продуктовия каталог.</span><span class="sxs-lookup"><span data-stu-id="8647f-120">Additionally, you can select products from other price lists or directly from the product catalog.</span></span> <span data-ttu-id="8647f-121">Когато избирате продукти директно от продуктов каталог, ценовата листа по подразбиране на този продукт се използва за получаване на продажната цена на продукта.</span><span class="sxs-lookup"><span data-stu-id="8647f-121">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="8647f-122">Ако не е зададена ценова листа по подразбиране, цената се задава на нула (0).</span><span class="sxs-lookup"><span data-stu-id="8647f-122">If a default price list isn't set, the price is set to zero (0).</span></span>

<span data-ttu-id="8647f-123">Когато редът на офертата е базиран на продуктов каталог, можете да заместите продажната цена директно в реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="8647f-123">When a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="8647f-124">Ред на оферта в полето **Ценообразуване** с две налични стойности:</span><span class="sxs-lookup"><span data-stu-id="8647f-124">A quote line in **Pricing** field with two available values:</span></span>

- <span data-ttu-id="8647f-125">**Заместване на ценообразуване**</span><span class="sxs-lookup"><span data-stu-id="8647f-125">**Override Pricing**</span></span>
- <span data-ttu-id="8647f-126">**По подразбиране**</span><span class="sxs-lookup"><span data-stu-id="8647f-126">**Use Default**</span></span>

<span data-ttu-id="8647f-127">Ако изберете **Заместване на ценообразуване**, цената по подразбиране не е зададена.</span><span class="sxs-lookup"><span data-stu-id="8647f-127">If you select **Override Pricing**, the default price isn't set.</span></span> <span data-ttu-id="8647f-128">Вместо това трябва да въведете цена за продукта в реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="8647f-128">Instead, you must enter a price for the product on the quote line.</span></span> <span data-ttu-id="8647f-129">Ако изберете **Използване на настройки по подразбиране**, се използва продажната цена по подразбиране и полето се заключва за редактиране.</span><span class="sxs-lookup"><span data-stu-id="8647f-129">If you select **Use Default**, the default sales price is used and the field is locked for editing.</span></span>

<span data-ttu-id="8647f-130">Продажните цени по подразбиране се въвеждат в базираните на продукт редове на оферта.</span><span class="sxs-lookup"><span data-stu-id="8647f-130">Default sales prices are entered on the product-based lines of a quote.</span></span> <span data-ttu-id="8647f-131">След това полето **Ценообразуване** се задава на **Заместване на ценообразуване**, така че да можете да редактирате цената по подразбиране в редовете на офертата.</span><span class="sxs-lookup"><span data-stu-id="8647f-131">The **Pricing** field is then set to **Override Pricing** so that you can edit the default price on the quote lines.</span></span> <span data-ttu-id="8647f-132">Това е заместване, специфично за Project Operations, за поведението на базираните на продукт редове в Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="8647f-132">This is a Project Operations-specific override to the product-based lines behavior in Dynamics 365 Sales.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]