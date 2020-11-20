---
title: Управление на сложни единици за базирани на продукт аспекти на договор – олекотено
description: Тази тема предоставя информация за подпомагане продажбата на продукти, базирани на абонамент.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a58a13c8186f36e6031fe3c6f3c3a57ea920ac9e
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177363"
---
# <a name="manage-complex-units-for-product-based-contract-lines---lite"></a><span data-ttu-id="ae22b-103">Управление на сложни единици за базирани на продукт аспекти на договор – олекотено</span><span class="sxs-lookup"><span data-stu-id="ae22b-103">Manage complex units for product-based contract lines - lite</span></span>

<span data-ttu-id="ae22b-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="ae22b-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ae22b-105">Dynamics 365 Project Operations използва количествени коефициенти, за да поддържа продажбата на продукти, базирани на абонамент.</span><span class="sxs-lookup"><span data-stu-id="ae22b-105">Dynamics 365 Project Operations uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="ae22b-106">За продукти, базирани на абонамент, количеството в договора или аспектите на договора по проект се изразява като брой на потребителски месеци.</span><span class="sxs-lookup"><span data-stu-id="ae22b-106">For subscription-based products, the quantity on the contract or project contract line is expressed as the number of user-months.</span></span>

<span data-ttu-id="ae22b-107">Цената на абонаментния софтуер се съхранява в каталога като цена за потребител на месец.</span><span class="sxs-lookup"><span data-stu-id="ae22b-107">The price of subscription software is stored in the catalog as the price per-user, per-month.</span></span> <span data-ttu-id="ae22b-108">По време на процеса на продажба цената в аспектите на договора обикновено е цената за потребител на месец, която е договорена и сконтирана от агента по продажби.</span><span class="sxs-lookup"><span data-stu-id="ae22b-108">During the sales process, the price on the contract line is usually the per-user, per-month price that was negotiated and discounted by the sales agent.</span></span> <span data-ttu-id="ae22b-109">Всяка сделка има различен брой потребители и различен брой абонаментни месеци.</span><span class="sxs-lookup"><span data-stu-id="ae22b-109">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="ae22b-110">Количеството, което се използва за изчисляване на сумата на аспектите на договора, е произведение от броя на потребителите и броя на абонаментите месеци.</span><span class="sxs-lookup"><span data-stu-id="ae22b-110">The quantity used to calculate the amount of the contract line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="ae22b-111">За да подкрепи този вид продажба, Project Operations поддържа концепцията за *количествени коефициенти*.</span><span class="sxs-lookup"><span data-stu-id="ae22b-111">To support this type of sale, Project Operations supports the concept of *quantity factors*.</span></span> <span data-ttu-id="ae22b-112">Количествените коефициенти се опират на атрибутите на продукта.</span><span class="sxs-lookup"><span data-stu-id="ae22b-112">Quantity factors rely on product attributes.</span></span> <span data-ttu-id="ae22b-113">Когато конфигурирате специфични свойства за даден продукт, можете да маркирате поднабор от тези свойства или всички свойства като количествени коефициенти.</span><span class="sxs-lookup"><span data-stu-id="ae22b-113">When you configure specific properties for a product, you can flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="ae22b-114">Project Operations проверява дали само числови свойства или свойства на продукта, които имат числов тип данни, са маркирани като количествени коефициенти.</span><span class="sxs-lookup"><span data-stu-id="ae22b-114">Project Operations validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="ae22b-115">Когато продукт с конфигурирани количествени коефициенти се добави към аспекти на договор, полето **Количество** става само за четене.</span><span class="sxs-lookup"><span data-stu-id="ae22b-115">When a product with configured quantity factors is added to a contract line, the **Quantity** field  becomes read-only.</span></span> <span data-ttu-id="ae22b-116">След като въведете стойности за свойствата на продукта, които са количествени коефициенти, Project Operations изчислява количеството на аспектите на договора.</span><span class="sxs-lookup"><span data-stu-id="ae22b-116">After you enter values for product properties that are quantity factors, Project Operations calculates the quantity of the contract line.</span></span>

<span data-ttu-id="ae22b-117">Например Dynamics 365 Sales може да има следните свойства:</span><span class="sxs-lookup"><span data-stu-id="ae22b-117">For example, Dynamics 365 Sales might have the following properties:</span></span>

- <span data-ttu-id="ae22b-118">**Брой потребители**: Броят на потребителите.</span><span class="sxs-lookup"><span data-stu-id="ae22b-118">**No of users**: The number of users.</span></span>
- <span data-ttu-id="ae22b-119">**Брой месеци**: Броят на абонаментните месеци.</span><span class="sxs-lookup"><span data-stu-id="ae22b-119">**No of Months**: The number of subscription months.</span></span>
- <span data-ttu-id="ae22b-120">**SKU на продукт**: Единици за съхранение на склад (SKU) за продукта.</span><span class="sxs-lookup"><span data-stu-id="ae22b-120">**Product SKU**: The stock keeping unit (SKU) for the product.</span></span>

<span data-ttu-id="ae22b-121">Свойствата **Брой потребители** и **Брой месеци** могат да бъдат маркирани като количествени коефициенти чрез редактиране на свойствата на реда на продукта.</span><span class="sxs-lookup"><span data-stu-id="ae22b-121">The **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span>

<span data-ttu-id="ae22b-122">За да създадете количествени коефициенти от свойства на продукт, изпълнете следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="ae22b-122">To create quantity factors from product properties, complete the following steps.</span></span>

1. <span data-ttu-id="ae22b-123">В **Project Operations** изберете **Продажби-продукти**.</span><span class="sxs-lookup"><span data-stu-id="ae22b-123">On the **Project Operations**, select **Sales-Products**.</span></span>
2. <span data-ttu-id="ae22b-124">Отворете продукта, за който трябва да зададете количествени коефициенти.</span><span class="sxs-lookup"><span data-stu-id="ae22b-124">Open the product for which you need to set up quantity factors.</span></span> <span data-ttu-id="ae22b-125">Уверете се, че продуктът има предварително зададени свойства.</span><span class="sxs-lookup"><span data-stu-id="ae22b-125">Make sure that the product has properties already set up.</span></span>
3. <span data-ttu-id="ae22b-126">На страницата **Информация за проекта** изберете раздела **Количествени коефициенти**.</span><span class="sxs-lookup"><span data-stu-id="ae22b-126">On the **Project Information** page, select the **Quantity Factors** tab.</span></span>
4. <span data-ttu-id="ae22b-127">В подмрежата изберете **+ Ново изчисление на поле**.</span><span class="sxs-lookup"><span data-stu-id="ae22b-127">In the subgrid, select **+ New field computation**.</span></span>
5. <span data-ttu-id="ae22b-128">Въведете името на **количествения коефициент** и изберете стойността на свойството, което съответства на изчислението на полето.</span><span class="sxs-lookup"><span data-stu-id="ae22b-128">Enter the name of the **Quantity Factor** and select the property value that maps to the field computation.</span></span>
6. <span data-ttu-id="ae22b-129">Запис и затваряне на формуляра.</span><span class="sxs-lookup"><span data-stu-id="ae22b-129">Save and close the form.</span></span>
7. <span data-ttu-id="ae22b-130">Повторете стъпки 2-6 за всички свойства, които заедно ще съставят количеството за базираните на проект аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="ae22b-130">Repeat steps 2-6 for all the properties that together will make up the quantity for the product-based contract line.</span></span>

<span data-ttu-id="ae22b-131">При зададени количествени коефициенти, когато потребителят създава аспекти на договор за този продукт, количеството на аспектите на договор се заключва.</span><span class="sxs-lookup"><span data-stu-id="ae22b-131">With quantity factors set up, when the user creates a contract line for this product, the quantity of the contract line is locked.</span></span> <span data-ttu-id="ae22b-132">След това количеството се изчислява като произведение от стойностите на имотите за тези аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="ae22b-132">The quantity is then calculated as a product of the property values for that contract line.</span></span>
