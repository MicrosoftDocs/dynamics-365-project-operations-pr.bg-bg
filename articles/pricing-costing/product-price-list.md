---
title: Ценови листи на продукт
description: Тази тема предоставя информация за ценовите листи в ценообразуването по каталог, използвани за проектни оферти и договори.
author: rumant
manager: AnnBe
ms.date: 04/05/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: e37f0bf9eef946ab4ebd658cef4e1269cbaf686d
ms.sourcegitcommit: ac90be6106592f883a0de39a75836fb40255d65a
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/09/2021
ms.locfileid: "5877477"
---
# <a name="product-price-lists"></a><span data-ttu-id="5d62f-103">Ценови листи на продукт</span><span class="sxs-lookup"><span data-stu-id="5d62f-103">Product price lists</span></span>

<span data-ttu-id="5d62f-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="5d62f-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

 <span data-ttu-id="5d62f-105">В Project Operations, **Ценови листи на продуктите** и свързаните с тях субекти на ценови листи поддържат функционалност за ценообразуване на продукти по базирани на продукти котировки и договорни линии.</span><span class="sxs-lookup"><span data-stu-id="5d62f-105">In Project Operations, **Product price lists** and related price list item entities support functionality for pricing products on product-based quote and contract lines.</span></span> <span data-ttu-id="5d62f-106">За продукти, използвани по проекти, се използват записите на ценовата листа за ценовите листи на проекти.</span><span class="sxs-lookup"><span data-stu-id="5d62f-106">For products used on projects, the price list item records for project price lists are used.</span></span> 

<span data-ttu-id="5d62f-107">Продуктите трябва да бъдат настроени така, че да имат разходни и ценови листи по подразбиране в продуктовия каталог.</span><span class="sxs-lookup"><span data-stu-id="5d62f-107">Products should be set up so that they have default cost and price lists in the product catalog.</span></span> <span data-ttu-id="5d62f-108">Използвайте цената от листата, стандартните разходи и текущите разходи, за да конфигурирате разходите и цените в списъка по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="5d62f-108">Use the list price, standard cost, and current cost to configure default cost and list prices.</span></span> <span data-ttu-id="5d62f-109">Цените в листата по подразбиране се използват в ред на оферта или ред на договор по проект само когато системата не може да намери ред на ценова листа за този продукт в ценовата листа на продукта за офертата или договора по проекта.</span><span class="sxs-lookup"><span data-stu-id="5d62f-109">The default list prices are used on a quote line or a project contract line only when the system can't find a price list line for that product in the product price list for the quote or project contract.</span></span>

<span data-ttu-id="5d62f-110">Себестойността в редовете на продуктовия каталог може да се променя между офертите.</span><span class="sxs-lookup"><span data-stu-id="5d62f-110">The cost price of product catalog lines can be changed between quotes.</span></span> <span data-ttu-id="5d62f-111">Тази възможност е важна, защото ако не проследявате точно разходите, не можете да определите оперативните печалби за ангажиментите по проекта.</span><span class="sxs-lookup"><span data-stu-id="5d62f-111">This capability is important, because if you don't accurately track costs, you can't determine operational profits on project engagements.</span></span> <span data-ttu-id="5d62f-112">По подразбиране стандартният разход за продукта се използва като себестойност.</span><span class="sxs-lookup"><span data-stu-id="5d62f-112">By default, the standard cost of the product is used as the cost price.</span></span> <span data-ttu-id="5d62f-113">Себестойността по подразбиране обаче може да се актуализира в реда на офертата, ако има различна себестойност за тази оферта.</span><span class="sxs-lookup"><span data-stu-id="5d62f-113">However, the default cost price can be updated on the quote line if there's a different cost price for that quote.</span></span>

## <a name="price-list-items"></a><span data-ttu-id="5d62f-114">Елементи в ценовата листа</span><span class="sxs-lookup"><span data-stu-id="5d62f-114">Price list items</span></span>

<span data-ttu-id="5d62f-115">Можете да добавяте продукти от продуктов каталог в различни ценови листи.</span><span class="sxs-lookup"><span data-stu-id="5d62f-115">You can add products from a product catalog to different price lists.</span></span> <span data-ttu-id="5d62f-116">Редовете на ценовата листа за продукти винаги се позовават на конкретна единица.</span><span class="sxs-lookup"><span data-stu-id="5d62f-116">Price list lines for products always reference a specific unit.</span></span> <span data-ttu-id="5d62f-117">Ценообразуването за продукт в ценова листа може да бъде конфигурирано като сума във валута.</span><span class="sxs-lookup"><span data-stu-id="5d62f-117">Pricing for a product on price list items can be configured as a currency amount.</span></span> <span data-ttu-id="5d62f-118">Или може да бъде конфигурирано като функция на цената от листата, текущата себестойност или стандартните разходи.</span><span class="sxs-lookup"><span data-stu-id="5d62f-118">Alternatively, it can be configured as a function of the list price, current cost, or standard cost.</span></span>

<span data-ttu-id="5d62f-119">Функционалността за ценообразуване поддържа различни опции за закръгляване, когато цените на продукт са конфигурирани като функция от цената от листата, стандартните разходи или текущите разходи.</span><span class="sxs-lookup"><span data-stu-id="5d62f-119">Pricing functionality supports various rounding options when product prices are configured as a function of the list price, standard cost, or current cost.</span></span> <span data-ttu-id="5d62f-120">Освен да се възползвате от няколко метода на ценообразуване и опции за закръгляване, можете да свържете списъците с отстъпки с елементи от ценовата листа.</span><span class="sxs-lookup"><span data-stu-id="5d62f-120">In addition to taking advantage of multiple pricing methods and rounding options, you can associate discount lists with price list items.</span></span> 

 
## <a name="default-product-price-list"></a><span data-ttu-id="5d62f-121">Ценова листа за продукти по подразбиране</span><span class="sxs-lookup"><span data-stu-id="5d62f-121">Default product price list</span></span>
<span data-ttu-id="5d62f-122">Всеки запис на клиент има поле **Ценова листа по подразбиране**, където можете да укажете ценова листа, която отговаря на валутата на клиента.</span><span class="sxs-lookup"><span data-stu-id="5d62f-122">Each customer record has a **Default Price List** field, where you can specify a price list that matches the currency of the customer.</span></span> <span data-ttu-id="5d62f-123">Стойността по подразбиране не се въвежда автоматично в това поле.</span><span class="sxs-lookup"><span data-stu-id="5d62f-123">A default value isn't automatically entered in this field.</span></span> <span data-ttu-id="5d62f-124">Когато съществува споразумение за персонализирано ценообразуване с конкретен клиент, можете да използвате това поле, за да свържете ценова листа с този клиент.</span><span class="sxs-lookup"><span data-stu-id="5d62f-124">When a custom pricing agreement with a specific customer exists, you can use this field to associate a price list with that customer.</span></span>

<span data-ttu-id="5d62f-125">Обектите „Възможност“, „Оферта“ и „Договор по проект“ използват следния ред, за да въведат ценови списъци на продукти по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="5d62f-125">The Opportunity, Quote, and Project Contract entities use the following order to enter default product price lists.</span></span> <span data-ttu-id="5d62f-126">Същият ред се използва за ценови листи за проекти.</span><span class="sxs-lookup"><span data-stu-id="5d62f-126">The same order is used for project price lists.</span></span>

1.  <span data-ttu-id="5d62f-127">Оферта</span><span class="sxs-lookup"><span data-stu-id="5d62f-127">Quote</span></span>
2.  <span data-ttu-id="5d62f-128">Възможност</span><span class="sxs-lookup"><span data-stu-id="5d62f-128">Opportunity</span></span>
3.  <span data-ttu-id="5d62f-129">Клиент</span><span class="sxs-lookup"><span data-stu-id="5d62f-129">Customer</span></span>
4.  <span data-ttu-id="5d62f-130">Глобални настройки</span><span class="sxs-lookup"><span data-stu-id="5d62f-130">Global settings</span></span> 

<span data-ttu-id="5d62f-131">По подразбиране полето **Продукт** в реда на офертата изброява всички активни продукти в ценовата листа на продукти на офертата.</span><span class="sxs-lookup"><span data-stu-id="5d62f-131">By default, the **Product** field on the quote line lists all the active products in the product price list of the quote.</span></span> <span data-ttu-id="5d62f-132">Ако даден продукт е бил деактивиран или е проект на продукт, той не е в списъка, дори ако е в ценовата листа.</span><span class="sxs-lookup"><span data-stu-id="5d62f-132">If a product has been inactivated, or if it's a draft product, it isn't listed, even if it's in the price list.</span></span> 

<span data-ttu-id="5d62f-133">Редове на продуктовия каталог се добавят като редове на фактура в първата фактура, която се създава за договор по проект.</span><span class="sxs-lookup"><span data-stu-id="5d62f-133">Product catalog lines are added as invoice lines on the first invoice that is created for a project contract.</span></span> <span data-ttu-id="5d62f-134">В чернова на фактура тези редове на фактурата могат да бъдат изтрити.</span><span class="sxs-lookup"><span data-stu-id="5d62f-134">On a draft invoice, those invoice lines can be deleted.</span></span> <span data-ttu-id="5d62f-135">В този случай редовете ще се повят в следваща фактура, докато не бъдат фактурирани или докато фактурата не бъде изпратена на клиента.</span><span class="sxs-lookup"><span data-stu-id="5d62f-135">In that case, the lines will appear on a subsequent invoice until they are invoiced, or until the invoice is sent to the customer.</span></span> <span data-ttu-id="5d62f-136">Не можете да фактурирате частично количество на ред на фактура за продукт.</span><span class="sxs-lookup"><span data-stu-id="5d62f-136">You can't invoice a partial quantity of a product invoice line.</span></span> <span data-ttu-id="5d62f-137">Когато редовете за продукти от договора по проекта се фактурират, се създават действителни данни.</span><span class="sxs-lookup"><span data-stu-id="5d62f-137">When the product lines from the project contract are invoiced, actuals are created.</span></span> <span data-ttu-id="5d62f-138">Тези действителни данни обаче не са свързани със свързания обект на проект.</span><span class="sxs-lookup"><span data-stu-id="5d62f-138">However, those actuals aren't linked to the related project entity.</span></span> <span data-ttu-id="5d62f-139">С други думи, редовете на договор, базирани на продукти, са независими от базирана на проект употреба.</span><span class="sxs-lookup"><span data-stu-id="5d62f-139">In other words, product-based project contract lines are independent of any project-based use.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]
