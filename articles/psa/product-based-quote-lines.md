---
title: Редове на оферти, базирани на продукти
description: Тази тема предоставя информация за редове на оферти, базирани на продукти.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
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
ms.openlocfilehash: 55a5b5041a494892e6d96bf24e1bc132a26521dc
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4072000"
---
# <a name="product-based-quote-lines"></a><span data-ttu-id="1ca98-103">Редове на оферти, базирани на продукти</span><span class="sxs-lookup"><span data-stu-id="1ca98-103">Product-based quote lines</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]


<span data-ttu-id="1ca98-104">Можете да създавате редове на оферти, базирани на продукти, в Dynamics 365 Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="1ca98-104">You can create product-based quote lines in Dynamics 365 Project Service Automation.</span></span> <span data-ttu-id="1ca98-105">Редовете на оферти, базирани на продукти, могат да бъдат редове за „вписване“ или могат да бъдат елементи от продуктовия каталог.</span><span class="sxs-lookup"><span data-stu-id="1ca98-105">Product-based quote lines can be "write-in" lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="1ca98-106">Продуктов каталог</span><span class="sxs-lookup"><span data-stu-id="1ca98-106">Product catalog</span></span>

<span data-ttu-id="1ca98-107">Продуктите в продуктов каталог на Dynamics 365 имат единица и група единици по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="1ca98-107">The products in a Dynamics 365 product catalog have a default unit and unit group.</span></span> <span data-ttu-id="1ca98-108">Ако няколко продукта споделят един и същ набор от атрибути, можете да създадете семейство продукти, която също има тези атрибути.</span><span class="sxs-lookup"><span data-stu-id="1ca98-108">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="1ca98-109">Всички продукти в едно семейство продукти наследяват един и същ набор от атрибути.</span><span class="sxs-lookup"><span data-stu-id="1ca98-109">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="1ca98-110">Например фирма продава абонаментни лицензи за различни софтуерни продукти.</span><span class="sxs-lookup"><span data-stu-id="1ca98-110">For example, a company sells subscription licenses for a variety of software.</span></span> <span data-ttu-id="1ca98-111">Всеки абонаментен софтуер има следните два атрибута:</span><span class="sxs-lookup"><span data-stu-id="1ca98-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="1ca98-112">Брой потребители</span><span class="sxs-lookup"><span data-stu-id="1ca98-112">Number of users</span></span> 
- <span data-ttu-id="1ca98-113">Продължителност на абонамента (в месеци)</span><span class="sxs-lookup"><span data-stu-id="1ca98-113">Subscription duration (in months)</span></span>

<span data-ttu-id="1ca98-114">Добър начин да поддържате този тип каталог е да създадете група продукти, която се нарича **Абонаментен софтуер** и има **Брой потребители** и **Продължителност на абонамента** като атрибути.</span><span class="sxs-lookup"><span data-stu-id="1ca98-114">A good way to maintain this type of catalog is to create a product family that is named **Subscription Software** , and that has **Number of users** and **Subscription duration** as attributes.</span></span> <span data-ttu-id="1ca98-115">След това можете да добавите отделни продукти, като например **Dynamics 365 Sales** или **Dynamics 365 Field Service** към продуктовото семейство **Абонаментен софтуер**.</span><span class="sxs-lookup"><span data-stu-id="1ca98-115">You can then add individual products, such as **Dynamics 365 Sales** or **Dynamics 365 Field Service** to the **Subscription Software** product family.</span></span>

## <a name="adding-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="1ca98-116">Добавяне на елементи от продуктов каталог към оферта по проект</span><span class="sxs-lookup"><span data-stu-id="1ca98-116">Adding product catalog items to a project quote</span></span>

<span data-ttu-id="1ca98-117">Страниците за оферти по проекти и договори по проекти имат секции за два вида редове: редове, базирани на проекти, и редове, базирани на продукти.</span><span class="sxs-lookup"><span data-stu-id="1ca98-117">Project quote and project contract pages have sections for two types of lines: project-based lines and product-based lines.</span></span> <span data-ttu-id="1ca98-118">За редове, базирани на продукти, Dynamics 365 се използва за добавяне на елементи от продуктов каталог към оферта.</span><span class="sxs-lookup"><span data-stu-id="1ca98-118">For product-based lines, Dynamics 365 is used to add items from a product catalog to a quote.</span></span> <span data-ttu-id="1ca98-119">Падащият списък в реда на офертата или реда на договора по проект включва всички продукти и единици в ценовата листа на продукта, която е прикачена към офертата или договора по проекта.</span><span class="sxs-lookup"><span data-stu-id="1ca98-119">The drop-down list on the quote line or project contract line includes all the products and units in the product price list that is attached to the quote or project contract.</span></span> <span data-ttu-id="1ca98-120">Можете също да добавяте продукти, които не са част от ценовата листа за продукти на офертата.</span><span class="sxs-lookup"><span data-stu-id="1ca98-120">You can also add products that aren't part of quote's product price list.</span></span>

<span data-ttu-id="1ca98-121">Освен това можете да изберете продукти от други ценови листи или можете да изберете продукти директно от продуктовия каталог.</span><span class="sxs-lookup"><span data-stu-id="1ca98-121">Additionally, you can select products from other price lists, or you can select products directly from the product catalog.</span></span> <span data-ttu-id="1ca98-122">Когато избирате продукти директно от продуктов каталог, ценовата листа по подразбиране на този продукт се използва за получаване на продажната цена на продукта.</span><span class="sxs-lookup"><span data-stu-id="1ca98-122">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="1ca98-123">Ако не е зададена ценова листа по подразбиране, цената се задава на 0 (нула).</span><span class="sxs-lookup"><span data-stu-id="1ca98-123">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="1ca98-124">Ако редът на офертата е базиран на продуктов каталог, можете да заместите продажната цена директно в реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="1ca98-124">If a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="1ca98-125">Обърнете внимание, че ред на оферта в Dynamics 365 има поле **Ценообразуване**.</span><span class="sxs-lookup"><span data-stu-id="1ca98-125">Note that a quote line in Dynamics 365 has a **Pricing** field.</span></span> <span data-ttu-id="1ca98-126">Налични са две стойности:</span><span class="sxs-lookup"><span data-stu-id="1ca98-126">Two values are available:</span></span>

- <span data-ttu-id="1ca98-127">Заместване на ценообразуване</span><span class="sxs-lookup"><span data-stu-id="1ca98-127">Override pricing</span></span>  
- <span data-ttu-id="1ca98-128">Използване по подразбиране</span><span class="sxs-lookup"><span data-stu-id="1ca98-128">Use default</span></span>

<span data-ttu-id="1ca98-129">Ако зададете това поле на **Заместване на ценообразуване** , Dynamics 365 не задава цена по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="1ca98-129">If you set this field to **Override pricing** , Dynamics 365 doesn't set a default price.</span></span> <span data-ttu-id="1ca98-130">Трябва да въведете цена за продукта в реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="1ca98-130">You must enter a price for the product on the quote line.</span></span> <span data-ttu-id="1ca98-131">Ако зададете това поле на **Използване по подразбиране** , Dynamics 365 използва продажната цена по подразбиране и заключва полето, за да предотвратите редактирането.</span><span class="sxs-lookup"><span data-stu-id="1ca98-131">If you set this field to **Use default** , Dynamics 365 uses the default sales price and locks the field to prevent editing.</span></span>

<span data-ttu-id="1ca98-132">След като инсталирате PSA, продажните цени по подразбиране се въвеждат в базираните на продукт редове в оферта.</span><span class="sxs-lookup"><span data-stu-id="1ca98-132">After you install PSA, default sales prices are entered on the product-based lines on a quote.</span></span> <span data-ttu-id="1ca98-133">След това полето **Ценообразуване** се задава на **Заместване на ценообразуване** , така че да можете да редактирате цената по подразбиране в редовете на офертата.</span><span class="sxs-lookup"><span data-stu-id="1ca98-133">The **Pricing** field is then set to **Override pricing** so that you can edit the default price on the quote lines.</span></span>

> ![Задаване на заместване на ценообразуване](media/basic-guide-10.png)
 
## <a name="quantity-factors-for-products"></a><span data-ttu-id="1ca98-135">Количествени коефициенти за продукти</span><span class="sxs-lookup"><span data-stu-id="1ca98-135">Quantity factors for products</span></span>

<span data-ttu-id="1ca98-136">PSA използва количествени коефициенти, за да поддържа продажбата на продукти, базирани на абонамент.</span><span class="sxs-lookup"><span data-stu-id="1ca98-136">PSA uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="1ca98-137">За продукти, базирани на абонамент, количеството в реда на офертата или реда договора по проект се изразява като брой на потребителски месеци.</span><span class="sxs-lookup"><span data-stu-id="1ca98-137">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user months.</span></span>

<span data-ttu-id="1ca98-138">Обикновено цената на абонаментния софтуер се съхранява в каталога като цена за потребител на месец.</span><span class="sxs-lookup"><span data-stu-id="1ca98-138">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="1ca98-139">Въпреки това можете да използвате други времеви описания вместо това.</span><span class="sxs-lookup"><span data-stu-id="1ca98-139">However, you can use other time descriptions instead.</span></span> <span data-ttu-id="1ca98-140">По време на процеса на продажба цената в реда на офертата обикновено е цената за потребител на месец, която е договорена и сконтирана от агента по ИТ продажби.</span><span class="sxs-lookup"><span data-stu-id="1ca98-140">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="1ca98-141">Всяка сделка има различен брой потребители и различен брой абонаментни месеци.</span><span class="sxs-lookup"><span data-stu-id="1ca98-141">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="1ca98-142">Количеството, което се използва за изчисляване на сумата на реда на офертата, е произведение от броя на потребителите и броя на абонаментите месеци.</span><span class="sxs-lookup"><span data-stu-id="1ca98-142">The quantity that is used to compute the amount of the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="1ca98-143">За да подкрепи този вид продажба, PSA въведе концепцията за количествени коефициенти.</span><span class="sxs-lookup"><span data-stu-id="1ca98-143">To support this type of sale, PSA introduced the concept of quantity factors.</span></span> <span data-ttu-id="1ca98-144">Количествените коефициенти се опират на атрибутите на продукта в Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="1ca98-144">Quantity factors rely on the product attributes in Dynamics 365.</span></span> <span data-ttu-id="1ca98-145">Когато конфигурирате специфични свойства за даден продукт, PSA ви позволява да маркирате поднабор от тези свойства или всички свойства като количествени коефициенти.</span><span class="sxs-lookup"><span data-stu-id="1ca98-145">When you configure specific properties for a product, PSA lets you flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="1ca98-146">PSA проверява дали само числови свойства или свойства на продукта, които имат числов тип данни, са маркирани като количествени коефициенти.</span><span class="sxs-lookup"><span data-stu-id="1ca98-146">PSA validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="1ca98-147">Когато продукт, за който са конфигурирани количествени коефициенти, се добави към ред на оферта, полето **Количество** в реда на офертата става поле само за четене.</span><span class="sxs-lookup"><span data-stu-id="1ca98-147">When a product that quantity factors are configured for is added to a quote line, the **Quantity** field on the quote line becomes a read-only field.</span></span> <span data-ttu-id="1ca98-148">След като въведете стойности за свойствата на продукта, които са количествени коефициенти, PSA изчислява количеството на реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="1ca98-148">After you enter values for product properties that are quantity factors, PSA computes the quantity of the quote line.</span></span>

<span data-ttu-id="1ca98-149">Например Dynamics 365 може да има следните свойства:</span><span class="sxs-lookup"><span data-stu-id="1ca98-149">For example, Dynamics 365 might have the following properties:</span></span> 

- <span data-ttu-id="1ca98-150">**Брой потребители** – броят на потребителите</span><span class="sxs-lookup"><span data-stu-id="1ca98-150">**No of users** - The number of users</span></span> 
- <span data-ttu-id="1ca98-151">**Брой месеци** – броят на абонаментните месеци</span><span class="sxs-lookup"><span data-stu-id="1ca98-151">**No of Months** - The number of subscription months</span></span>
- <span data-ttu-id="1ca98-152">**SKU на продукт**</span><span class="sxs-lookup"><span data-stu-id="1ca98-152">**Product SKU**</span></span> 

<span data-ttu-id="1ca98-153">Свойствата **Брой потребители** и **Брой месеци** могат да бъдат маркирани като количествени коефициенти чрез редактиране на свойствата на реда на продукта.</span><span class="sxs-lookup"><span data-stu-id="1ca98-153">Tne **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span> 

> ![Маркиране на „Брой потребители“ и „Брой месеци“ като количествени коефициенти](media/basic-guide-11.png)
 
