---
title: Начална страница на измерения за ценообразуване и остойностяване
description: Тази тема предоставя общ преглед на ценовите измерения.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 425d7bb8-9015-4f67-b9c9-cf3602e9afe8
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 2379d0d2e038f28a1a8df87a851e9bf7db7fe33f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749266"
---
# <a name="pricing-and-costing-dimensions-home-page"></a><span data-ttu-id="250be-103">Начална страница на измерения за ценообразуване и остойностяване</span><span class="sxs-lookup"><span data-stu-id="250be-103">Pricing and costing dimensions home page</span></span>

<span data-ttu-id="250be-104">Измеренията, които се използват в човешките ресурси за настройване на ценообразуване и разходи, попадат в две категории:</span><span class="sxs-lookup"><span data-stu-id="250be-104">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="250be-105">Хора</span><span class="sxs-lookup"><span data-stu-id="250be-105">People</span></span>
- <span data-ttu-id="250be-106">Планирана работа</span><span class="sxs-lookup"><span data-stu-id="250be-106">Planned work</span></span>

<span data-ttu-id="250be-107">Поради това има два типа ценови измерения, налични в Project Service Automation (PSA):</span><span class="sxs-lookup"><span data-stu-id="250be-107">Because of this, there are two types of pricing dimension values available in Project Service Automation (PSA):</span></span> 

- <span data-ttu-id="250be-108">**Набори от опции** – измерения, които са фиксирани изброявания за набор от стойности.</span><span class="sxs-lookup"><span data-stu-id="250be-108">**Option sets** - Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="250be-109">**Стойности, базирани на обект** – измерения, които могат да бъдат разнообразен набор от стойности.</span><span class="sxs-lookup"><span data-stu-id="250be-109">**Entity-based values** - Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="250be-110">Ценови измерения</span><span class="sxs-lookup"><span data-stu-id="250be-110">Pricing dimensions</span></span>

<span data-ttu-id="250be-111">PSA се доставя с набор от ценовите измерения по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="250be-111">PSA ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="250be-112">Можете да ги видите, като отидете в **Project Service** > **Параметри**.</span><span class="sxs-lookup"><span data-stu-id="250be-112">You can view these by going to **Project Service** > **Parameters**.</span></span> <span data-ttu-id="250be-113">В записа на параметъра, в раздела **Ценови измерения, базирани на сума**, проверете дали ролята, **msdyn_resourcecategory** и организационна единица, **msdyn_organizationalunit** имат полета **Приложимо за продажби** и **Приложимо за разходи**, зададени на **Да**.</span><span class="sxs-lookup"><span data-stu-id="250be-113">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="250be-114">Това ще ви позволи да зададете цената и разходите за всяка комбинация от роля и организационна единица.</span><span class="sxs-lookup"><span data-stu-id="250be-114">This will allow you to set up the price and cost for each role and organizational unit combination.</span></span>

![Екранна снимка на параметри на Project Service с маркирана опция „Приложимо за продажби“](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> <span data-ttu-id="250be-116">Ако сте използвали стандартните полета на роля и организационна единица като ценови измерения преди версия 3 на PSA, няма да има никаква видима промяна.</span><span class="sxs-lookup"><span data-stu-id="250be-116">If you have been the using out-of-the box fields of role and organizational unit as pricing dimensions prior to version 3 of PSA, there will not be any observable change.</span></span> <span data-ttu-id="250be-117">Можете да продължите да използвате Project Service както обикновено.</span><span class="sxs-lookup"><span data-stu-id="250be-117">You can continue to use Project Service as usual.</span></span> 

<span data-ttu-id="250be-118">Ако имате нужда от цена или разход за вашите ресурси с помощта на допълнителни атрибути, можете да създадете персонализирани полета, обекти и измерения.</span><span class="sxs-lookup"><span data-stu-id="250be-118">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="250be-119">За повече информация вижте следните теми, но имайте предвид, че трябва да изпълните процедурите в реда, посочен по-долу:</span><span class="sxs-lookup"><span data-stu-id="250be-119">For more information, see the following topics, however note that you must complete the procedures in the order listed below:</span></span>

- [<span data-ttu-id="250be-120">Създаване на персонализирани полета и обекти</span><span class="sxs-lookup"><span data-stu-id="250be-120">Create custom fields and entities</span></span>](create-custom-fields-entities.md)
- [<span data-ttu-id="250be-121">Добавяне на персонализирани полета към настройка на цени и обекти за транзакции</span><span class="sxs-lookup"><span data-stu-id="250be-121">Add custom fields to price setup and transactional entities</span></span>](field-references.md)
- [<span data-ttu-id="250be-122">Настройване на персонализирани полета като ценови измерения </span><span class="sxs-lookup"><span data-stu-id="250be-122">Set up custom fields as pricing dimensions</span></span>](set-up-pricing-dimensions.md)
- [<span data-ttu-id="250be-123">Актуализиране на атрибути на добавка за включване на нови ценови измерения</span><span class="sxs-lookup"><span data-stu-id="250be-123">Update plug-in attributes to include new pricing dimensions</span></span>](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a><span data-ttu-id="250be-124">Ценообразуване на времето на човешките ресурси</span><span class="sxs-lookup"><span data-stu-id="250be-124">Pricing human resource time</span></span>
<span data-ttu-id="250be-125">Как дадена организация ценообразува времето на човешките ресурси често е важно стратегическо съображение, което пряко засяга рентабилността на организацията.</span><span class="sxs-lookup"><span data-stu-id="250be-125">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="250be-126">Работете с финансовите екипи и ръководителите, когато вашата организация е готова да определи как иска да настрои ставките за фактуриране и разходи за времето на човешките ресурси.</span><span class="sxs-lookup"><span data-stu-id="250be-126">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="250be-127">Други съображения за ценообразуване включват дали да се използват повторно полета или обекти, които в момента не са ценови измерения, но се прилагат като ценово измерение за вашата организация.</span><span class="sxs-lookup"><span data-stu-id="250be-127">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="250be-128">Полета, като **Категория транзакция** (**msdyn_transactioncategory**) и **Наличен ресурс** (**bookableresource**), са примери за кандидат измерения.</span><span class="sxs-lookup"><span data-stu-id="250be-128">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="250be-129">Също така трябва да съобразите дали ценовото ви измерение трябва да бъде таблица или набор от опции.</span><span class="sxs-lookup"><span data-stu-id="250be-129">You should also consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="250be-130">Ако предвиждате промени в стойностите на измерение, които ще надхвърлят 10 или 12, и имате нужда от допълнителни атрибути за тези стойности, можете да създадете обект, а не набор от опции.</span><span class="sxs-lookup"><span data-stu-id="250be-130">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="250be-131">Поддържането на набор от опции, като например добавяне или премахване на стойности, изисква администратор или разработчик, докато добавянето на нови редове към таблица може да се извърши от повечето потребители.</span><span class="sxs-lookup"><span data-stu-id="250be-131">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="250be-132">Примерът по-долу показва ставки за фактуриране, които са настроени въз основа на ролята и организационната единица, към която принадлежи ресурсът.</span><span class="sxs-lookup"><span data-stu-id="250be-132">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="250be-133">Процентът на разходите обикновено се базира на групата работна заплата на служителя и на организационната единица, към която принадлежи.</span><span class="sxs-lookup"><span data-stu-id="250be-133">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="250be-134">В този пример таблиците за ставка за фактуриране и ставка за разходите ще изглеждат като следните.</span><span class="sxs-lookup"><span data-stu-id="250be-134">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="250be-135">**Примерни ставки за фактуриране**</span><span class="sxs-lookup"><span data-stu-id="250be-135">**Sample bill rates**</span></span>

| <span data-ttu-id="250be-136">Роля</span><span class="sxs-lookup"><span data-stu-id="250be-136">Role</span></span>        | <span data-ttu-id="250be-137">Организационна единица</span><span class="sxs-lookup"><span data-stu-id="250be-137">Org Unit</span></span>    |<span data-ttu-id="250be-138">Единица</span><span class="sxs-lookup"><span data-stu-id="250be-138">Unit</span></span>      |<span data-ttu-id="250be-139">Цена</span><span class="sxs-lookup"><span data-stu-id="250be-139">Price</span></span>      |<span data-ttu-id="250be-140">Валута</span><span class="sxs-lookup"><span data-stu-id="250be-140">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="250be-141">Разработчици</span><span class="sxs-lookup"><span data-stu-id="250be-141">Developer</span></span>   | <span data-ttu-id="250be-142">Contoso САЩ</span><span class="sxs-lookup"><span data-stu-id="250be-142">Contoso US</span></span>  |<span data-ttu-id="250be-143">Час</span><span class="sxs-lookup"><span data-stu-id="250be-143">Hour</span></span> | <span data-ttu-id="250be-144">200</span><span class="sxs-lookup"><span data-stu-id="250be-144">200</span></span>|<span data-ttu-id="250be-145">USD</span><span class="sxs-lookup"><span data-stu-id="250be-145">USD</span></span>     |
| <span data-ttu-id="250be-146">Разработчици</span><span class="sxs-lookup"><span data-stu-id="250be-146">Developer</span></span>   | <span data-ttu-id="250be-147">Contoso Индия</span><span class="sxs-lookup"><span data-stu-id="250be-147">Contoso India</span></span> |<span data-ttu-id="250be-148">Час</span><span class="sxs-lookup"><span data-stu-id="250be-148">Hour</span></span>|   <span data-ttu-id="250be-149">112</span><span class="sxs-lookup"><span data-stu-id="250be-149">112</span></span>|<span data-ttu-id="250be-150">USD</span><span class="sxs-lookup"><span data-stu-id="250be-150">USD</span></span>     |


<span data-ttu-id="250be-151">**Примерни ставки за разходи**</span><span class="sxs-lookup"><span data-stu-id="250be-151">**Sample cost rates**</span></span>

| <span data-ttu-id="250be-152">Група работна заплата</span><span class="sxs-lookup"><span data-stu-id="250be-152">Salary Band</span></span>     | <span data-ttu-id="250be-153">Организационна единица</span><span class="sxs-lookup"><span data-stu-id="250be-153">Org Unit</span></span>    |<span data-ttu-id="250be-154">Единица</span><span class="sxs-lookup"><span data-stu-id="250be-154">Unit</span></span>      |<span data-ttu-id="250be-155">Цена</span><span class="sxs-lookup"><span data-stu-id="250be-155">Price</span></span>      |<span data-ttu-id="250be-156">Валута</span><span class="sxs-lookup"><span data-stu-id="250be-156">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="250be-157">Моята фирма_група1</span><span class="sxs-lookup"><span data-stu-id="250be-157">My company_Band1</span></span> | <span data-ttu-id="250be-158">Contoso САЩ</span><span class="sxs-lookup"><span data-stu-id="250be-158">Contoso US</span></span>  |<span data-ttu-id="250be-159">Час</span><span class="sxs-lookup"><span data-stu-id="250be-159">Hour</span></span> | <span data-ttu-id="250be-160">145</span><span class="sxs-lookup"><span data-stu-id="250be-160">145</span></span>|<span data-ttu-id="250be-161">USD</span><span class="sxs-lookup"><span data-stu-id="250be-161">USD</span></span>     |
| <span data-ttu-id="250be-162">Моята фирма_група2</span><span class="sxs-lookup"><span data-stu-id="250be-162">My company_Band2</span></span> | <span data-ttu-id="250be-163">Contoso Индия</span><span class="sxs-lookup"><span data-stu-id="250be-163">Contoso India</span></span> |<span data-ttu-id="250be-164">Час</span><span class="sxs-lookup"><span data-stu-id="250be-164">Hour</span></span>|   <span data-ttu-id="250be-165">67</span><span class="sxs-lookup"><span data-stu-id="250be-165">67</span></span>|<span data-ttu-id="250be-166">USD</span><span class="sxs-lookup"><span data-stu-id="250be-166">USD</span></span>     |
