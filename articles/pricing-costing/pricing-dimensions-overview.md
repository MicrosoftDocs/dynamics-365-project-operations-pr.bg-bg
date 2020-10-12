---
title: Преглед на измеренията на ценообразуване
description: Тази тема предоставя информация за ценовите измерение в Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: fe2ab3a1b12c00e346e27709d66b5a0cb81a3b56
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898203"
---
# <a name="pricing-dimensions-overview"></a><span data-ttu-id="7e144-103">Преглед на измеренията на ценообразуване</span><span class="sxs-lookup"><span data-stu-id="7e144-103">Pricing dimensions overview</span></span>

<span data-ttu-id="7e144-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="7e144-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7e144-105">Измеренията, които се използват в човешките ресурси за настройване на ценообразуване и разходи, попадат в две категории:</span><span class="sxs-lookup"><span data-stu-id="7e144-105">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="7e144-106">Хора</span><span class="sxs-lookup"><span data-stu-id="7e144-106">People</span></span>
- <span data-ttu-id="7e144-107">Планирана работа</span><span class="sxs-lookup"><span data-stu-id="7e144-107">Planned work</span></span>

<span data-ttu-id="7e144-108">Поради това има два типа налични стойности на ценови измерения:</span><span class="sxs-lookup"><span data-stu-id="7e144-108">Because of this, there are two types of pricing dimension values available:</span></span>

- <span data-ttu-id="7e144-109">**Набори от опции**: Измерения, които са фиксирани изброявания за набор от стойности.</span><span class="sxs-lookup"><span data-stu-id="7e144-109">**Option sets**: Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="7e144-110">**Стойности, базирани на обект**: Измерения, които могат да бъдат разнообразен набор от стойности.</span><span class="sxs-lookup"><span data-stu-id="7e144-110">**Entity-based values**: Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="7e144-111">Ценови измерения</span><span class="sxs-lookup"><span data-stu-id="7e144-111">Pricing dimensions</span></span>

<span data-ttu-id="7e144-112">Dynamics 365 Project Operations се доставя с набор от размери за ценообразуване по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="7e144-112">Dynamics 365 Project Operations ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="7e144-113">Можете да видите тези ценови измерения, като отидете на **Project Operations** > **Параметри**.</span><span class="sxs-lookup"><span data-stu-id="7e144-113">You can view these pricing dimensions by going to **Project Operations** > **Parameters**.</span></span> <span data-ttu-id="7e144-114">В записа на параметъра, в раздела **Ценови измерения, базирани на сума**, проверете дали ролята, **msdyn_resourcecategory** и организационна единица, **msdyn_organizationalunit** имат полета **Приложимо за продажби** и **Приложимо за разходи**, зададени на **Да**.</span><span class="sxs-lookup"><span data-stu-id="7e144-114">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="7e144-115">С тази полета активирани можете да зададете цената и разходите за всяка комбинация от роля и организационна единица.</span><span class="sxs-lookup"><span data-stu-id="7e144-115">With these fields enabled, you can set up the price and cost for each role and organizational unit combination.</span></span>

<span data-ttu-id="7e144-116">Ако имате нужда от цена или разход за вашите ресурси с помощта на допълнителни атрибути, можете да създадете персонализирани полета, обекти и измерения.</span><span class="sxs-lookup"><span data-stu-id="7e144-116">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span>

## <a name="pricing-human-resource-time"></a><span data-ttu-id="7e144-117">Ценообразуване на времето на човешките ресурси</span><span class="sxs-lookup"><span data-stu-id="7e144-117">Pricing human resource time</span></span>
<span data-ttu-id="7e144-118">Как дадена организация ценообразува времето на човешките ресурси често е важно стратегическо съображение, което пряко засяга рентабилността на организацията.</span><span class="sxs-lookup"><span data-stu-id="7e144-118">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="7e144-119">Работете с финансовите екипи и ръководителите, когато вашата организация е готова да определи как иска да настрои ставките за фактуриране и разходи за времето на човешките ресурси.</span><span class="sxs-lookup"><span data-stu-id="7e144-119">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="7e144-120">Други съображения за ценообразуване включват дали да се използват повторно полета или обекти, които в момента не са ценови измерения, но се прилагат като ценово измерение за вашата организация.</span><span class="sxs-lookup"><span data-stu-id="7e144-120">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="7e144-121">Полета, като **Категория транзакция** (**msdyn_transactioncategory**) и **Наличен ресурс** (**bookableresource**), са примери за кандидат измерения.</span><span class="sxs-lookup"><span data-stu-id="7e144-121">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="7e144-122">Съобразете дали ценовото ви измерение трябва да бъде таблица или набор от опции.</span><span class="sxs-lookup"><span data-stu-id="7e144-122">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="7e144-123">Ако предвиждате промени в стойностите на измерение, които ще надхвърлят 10 или 12, и имате нужда от допълнителни атрибути за тези стойности, можете да създадете обект, а не набор от опции.</span><span class="sxs-lookup"><span data-stu-id="7e144-123">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="7e144-124">Поддържането на набор от опции, като например добавяне или премахване на стойности, изисква администратор или разработчик, докато добавянето на нови редове към таблица може да се извърши от повечето потребители.</span><span class="sxs-lookup"><span data-stu-id="7e144-124">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="7e144-125">Примерът по-долу показва ставки за фактуриране, които са настроени въз основа на ролята и организационната единица, към която принадлежи ресурсът.</span><span class="sxs-lookup"><span data-stu-id="7e144-125">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="7e144-126">Процентът на разходите обикновено се базира на групата работна заплата на служителя и на организационната единица, към която принадлежи.</span><span class="sxs-lookup"><span data-stu-id="7e144-126">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="7e144-127">В този пример таблиците за ставка за фактуриране и ставка за разходите ще изглеждат като следните.</span><span class="sxs-lookup"><span data-stu-id="7e144-127">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="7e144-128">**Примерни ставки за фактуриране**</span><span class="sxs-lookup"><span data-stu-id="7e144-128">**Sample bill rates**</span></span>

| <span data-ttu-id="7e144-129">Роля</span><span class="sxs-lookup"><span data-stu-id="7e144-129">Role</span></span>        | <span data-ttu-id="7e144-130">Организационна единица</span><span class="sxs-lookup"><span data-stu-id="7e144-130">Org Unit</span></span>    |<span data-ttu-id="7e144-131">Единица</span><span class="sxs-lookup"><span data-stu-id="7e144-131">Unit</span></span>      |<span data-ttu-id="7e144-132">Цена</span><span class="sxs-lookup"><span data-stu-id="7e144-132">Price</span></span>      |<span data-ttu-id="7e144-133">Валута</span><span class="sxs-lookup"><span data-stu-id="7e144-133">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="7e144-134">Разработчици</span><span class="sxs-lookup"><span data-stu-id="7e144-134">Developer</span></span>   | <span data-ttu-id="7e144-135">Contoso САЩ</span><span class="sxs-lookup"><span data-stu-id="7e144-135">Contoso US</span></span>  |<span data-ttu-id="7e144-136">Час</span><span class="sxs-lookup"><span data-stu-id="7e144-136">Hour</span></span> | <span data-ttu-id="7e144-137">200</span><span class="sxs-lookup"><span data-stu-id="7e144-137">200</span></span>|<span data-ttu-id="7e144-138">USD</span><span class="sxs-lookup"><span data-stu-id="7e144-138">USD</span></span>     |
| <span data-ttu-id="7e144-139">Разработчици</span><span class="sxs-lookup"><span data-stu-id="7e144-139">Developer</span></span>   | <span data-ttu-id="7e144-140">Contoso Индия</span><span class="sxs-lookup"><span data-stu-id="7e144-140">Contoso India</span></span> |<span data-ttu-id="7e144-141">Час</span><span class="sxs-lookup"><span data-stu-id="7e144-141">Hour</span></span>|   <span data-ttu-id="7e144-142">112</span><span class="sxs-lookup"><span data-stu-id="7e144-142">112</span></span>|<span data-ttu-id="7e144-143">USD</span><span class="sxs-lookup"><span data-stu-id="7e144-143">USD</span></span>     |


<span data-ttu-id="7e144-144">**Примерни ставки за разходи**</span><span class="sxs-lookup"><span data-stu-id="7e144-144">**Sample cost rates**</span></span>

| <span data-ttu-id="7e144-145">Група работна заплата</span><span class="sxs-lookup"><span data-stu-id="7e144-145">Salary Band</span></span>     | <span data-ttu-id="7e144-146">Организационна единица</span><span class="sxs-lookup"><span data-stu-id="7e144-146">Org Unit</span></span>    |<span data-ttu-id="7e144-147">Единица</span><span class="sxs-lookup"><span data-stu-id="7e144-147">Unit</span></span>      |<span data-ttu-id="7e144-148">Цена</span><span class="sxs-lookup"><span data-stu-id="7e144-148">Price</span></span>      |<span data-ttu-id="7e144-149">Валута</span><span class="sxs-lookup"><span data-stu-id="7e144-149">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="7e144-150">Моята фирма_група1</span><span class="sxs-lookup"><span data-stu-id="7e144-150">My company_Band1</span></span> | <span data-ttu-id="7e144-151">Contoso САЩ</span><span class="sxs-lookup"><span data-stu-id="7e144-151">Contoso US</span></span>  |<span data-ttu-id="7e144-152">Час</span><span class="sxs-lookup"><span data-stu-id="7e144-152">Hour</span></span> | <span data-ttu-id="7e144-153">145</span><span class="sxs-lookup"><span data-stu-id="7e144-153">145</span></span>|<span data-ttu-id="7e144-154">USD</span><span class="sxs-lookup"><span data-stu-id="7e144-154">USD</span></span>     |
| <span data-ttu-id="7e144-155">Моята фирма_група2</span><span class="sxs-lookup"><span data-stu-id="7e144-155">My company_Band2</span></span> | <span data-ttu-id="7e144-156">Contoso Индия</span><span class="sxs-lookup"><span data-stu-id="7e144-156">Contoso India</span></span> |<span data-ttu-id="7e144-157">Час</span><span class="sxs-lookup"><span data-stu-id="7e144-157">Hour</span></span>|   <span data-ttu-id="7e144-158">67</span><span class="sxs-lookup"><span data-stu-id="7e144-158">67</span></span>|<span data-ttu-id="7e144-159">USD</span><span class="sxs-lookup"><span data-stu-id="7e144-159">USD</span></span>     |