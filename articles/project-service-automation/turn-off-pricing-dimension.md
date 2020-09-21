---
title: Изключване на ценово измерение
description: Тази тема показва как да зададете ценови измерения в решението Project Service.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/06/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 689e5a8d-e39a-471d-a6c4-7e2fc3bb5590
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 5cf2cd86fb1eba50c8e08b2bd624669ab0b1deb3
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749323"
---
# <a name="turn-off-a-pricing-dimension"></a><span data-ttu-id="dc1d1-103">Изключване на ценово измерение</span><span class="sxs-lookup"><span data-stu-id="dc1d1-103">Turn off a pricing dimension</span></span>

<span data-ttu-id="dc1d1-104">Може да се наложи да преглеждате и актуализирате ценовата си стратегия на всеки няколко години.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-104">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="dc1d1-105">Всички актуализации, които правите, може да изискват да изключите съществуващо ценово измерение и да създадете ново.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-105">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="dc1d1-106">Например може да сте ценообразували преди по **Роля**, но сега сте решили да ценообразувате по **Трудов стаж**.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-106">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="dc1d1-107">Това може да изисква от вас да изключите **Роля** като ценово измерение и да създадете **Трудов стаж** като ново ценово измерение.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-107">This may require you to turn off **Role** as a pricing dimension and create **Work Expereince** as a new pricing dimension.</span></span> 

<span data-ttu-id="dc1d1-108">Изключването на ценово измерение, независимо дали е стандартно, или персонализирано, може да се извърши, като се зададат полетата **Приложимо за разходи** и **Приложимо за продажби** на ценовото измерение на **Не**.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-108">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="dc1d1-109">Когато направите това обаче, може да получите следното съобщение за грешка.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-109">However, when you do this, you might receive the following error message.</span></span>

![Вероятна грешка на бизнес процес при изключване на ценово измерение](media/Business-Process-Error.png)


<span data-ttu-id="dc1d1-111">Това съобщение за грешка показва, че има ценови записи, които преди това са били настроени за измерението, което се изключва.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-111">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="dc1d1-112">Всички записи на **Цена на роля** и **Надценка над цена на роля**, които се отнасят към измерение, трябва да бъдат изтрити преди приложимостта на измерението да може да бъде зададена на **Не**.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-112">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="dc1d1-113">Това правило се отнася за стандартните ценови измерения и всички персонализирани ценови измерения, които може да сте създали.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-113">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="dc1d1-114">Причината за тази проверка е, че Project Service има ограничение всеки запис на **Цена на роля** да има уникална комбинация от измерения.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-114">The reason for this validation is because Project Service has a constraint that each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="dc1d1-115">Например в ценова листа, наречена **Разходни ставки САЩ 2018**, имате следните редове за **Цена на роля**.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-115">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="dc1d1-116">Стандартна длъжност</span><span class="sxs-lookup"><span data-stu-id="dc1d1-116">Standard Title</span></span>         | <span data-ttu-id="dc1d1-117">Организационна единица</span><span class="sxs-lookup"><span data-stu-id="dc1d1-117">Org Unit</span></span>    |<span data-ttu-id="dc1d1-118">Единица</span><span class="sxs-lookup"><span data-stu-id="dc1d1-118">Unit</span></span>   |<span data-ttu-id="dc1d1-119">Цена</span><span class="sxs-lookup"><span data-stu-id="dc1d1-119">Price</span></span>  |<span data-ttu-id="dc1d1-120">Валута</span><span class="sxs-lookup"><span data-stu-id="dc1d1-120">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="dc1d1-121">Системен инженер</span><span class="sxs-lookup"><span data-stu-id="dc1d1-121">Systems Engineer</span></span>|<span data-ttu-id="dc1d1-122">Contoso САЩ</span><span class="sxs-lookup"><span data-stu-id="dc1d1-122">Contoso US</span></span>|<span data-ttu-id="dc1d1-123">Час</span><span class="sxs-lookup"><span data-stu-id="dc1d1-123">Hour</span></span>| <span data-ttu-id="dc1d1-124">100</span><span class="sxs-lookup"><span data-stu-id="dc1d1-124">100</span></span>|<span data-ttu-id="dc1d1-125">USD</span><span class="sxs-lookup"><span data-stu-id="dc1d1-125">USD</span></span>|
| <span data-ttu-id="dc1d1-126">Старши системен инженер</span><span class="sxs-lookup"><span data-stu-id="dc1d1-126">Senior Systems Engineer</span></span>|<span data-ttu-id="dc1d1-127">Contoso САЩ</span><span class="sxs-lookup"><span data-stu-id="dc1d1-127">Contoso US</span></span>|<span data-ttu-id="dc1d1-128">Час</span><span class="sxs-lookup"><span data-stu-id="dc1d1-128">Hour</span></span>| <span data-ttu-id="dc1d1-129">150</span><span class="sxs-lookup"><span data-stu-id="dc1d1-129">150</span></span>| <span data-ttu-id="dc1d1-130">USD</span><span class="sxs-lookup"><span data-stu-id="dc1d1-130">USD</span></span>|


<span data-ttu-id="dc1d1-131">Когато изключите **Стандартна длъжност** като ценово измерение и програмата за ценообразуване на Project Service търси цена, тя ще използва само стойността на **Организационна единица** от контекста на въвеждане.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-131">When you turn off **Standard Title** as the pricing dimension, and the Project Service pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="dc1d1-132">Ако **Организационната единица** на контекста на въвеждане е „Contoso САЩ“, резултатът ще бъде нееднозначен, защото и двата реда ще съвпадат.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-132">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="dc1d1-133">За да избегнете този сценарий, когато създавате записи **Цена на роля**, Project Service проверява дали комбинацията от измерения е уникална.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-133">To avoid this scenario, when you create **Role Price** records, Project Service validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="dc1d1-134">Ако измерението се изключи, след като са създадени записите **Цена на роля**, това ограничение може да бъде нарушено.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-134">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="dc1d1-135">Затова е необходимо, преди да изключите дадено измерение, да изтриете всички редове за **Цена на роля** и **Надценка над цена на роля**, които имат попълнена тази стойност на измерение.</span><span class="sxs-lookup"><span data-stu-id="dc1d1-135">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>

