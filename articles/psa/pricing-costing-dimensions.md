---
title: Начална страница на измерения за ценообразуване и остойностяване
description: Тази тема предоставя общ преглед на ценовите измерения.
author: rumant
ms.custom:
- dyn365-projectservice
- intro-internal
ms.date: 10/01/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 5c8c28839f5e7b3259afbea4ab400d0c4fca95fd
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368868"
---
# <a name="pricing-and-costing-dimensions-home-page"></a><span data-ttu-id="babf5-103">Начална страница на измерения за ценообразуване и остойностяване</span><span class="sxs-lookup"><span data-stu-id="babf5-103">Pricing and costing dimensions home page</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="babf5-104">Размерите, използвани за определяне на ценообразуването и себестойността на труда в организации, базирани на проекти, се влияят от следните атрибути:</span><span class="sxs-lookup"><span data-stu-id="babf5-104">The dimensions used to set labor pricing and costing in project-based organizations are influenced by the following attributes:</span></span>

- <span data-ttu-id="babf5-105">Хората, които извършват работа, подобна на техния опит, роля или география</span><span class="sxs-lookup"><span data-stu-id="babf5-105">People doing work similar to their experience, role, or geography</span></span>
- <span data-ttu-id="babf5-106">Работа, която трябва да се извършва, подобно на сложността или времето на деня</span><span class="sxs-lookup"><span data-stu-id="babf5-106">Work to be performed similar to its complexity or time of day</span></span>

<span data-ttu-id="babf5-107">Предвид типичния характер на тези атрибути на работата и хората, необходими за изпълнението на работата, в Project Service Automation има два типа стойности на измерение на ценообразуването:</span><span class="sxs-lookup"><span data-stu-id="babf5-107">Given the typical nature of these attrubutes of the work and the people required to perform the work, there are two types of pricing dimension values available in Project Service Automation:</span></span> 

- <span data-ttu-id="babf5-108">**Набори от опции** – Атрибути, които са фиксирани изброявания за набор от стойности.</span><span class="sxs-lookup"><span data-stu-id="babf5-108">**Option sets** - Attributes that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="babf5-109">**Въз основа на обект** – Атрибути, които могат да имат разнообразен набор от стойности, които са крайни, но могат да се променят с течение на времето.</span><span class="sxs-lookup"><span data-stu-id="babf5-109">**Entity-based values** - Attributes that can have a varied set of values that are finite but can change over time.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="babf5-110">Ценови измерения</span><span class="sxs-lookup"><span data-stu-id="babf5-110">Pricing dimensions</span></span>

<span data-ttu-id="babf5-111">PSA се доставя с набор от ценовите измерения по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="babf5-111">PSA ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="babf5-112">Можете да ги видите, като отидете в **Project Service** > **Параметри**.</span><span class="sxs-lookup"><span data-stu-id="babf5-112">You can view these by going to **Project Service** > **Parameters**.</span></span> <span data-ttu-id="babf5-113">В записа на параметъра, в раздела **Ценови измерения, базирани на сума**, проверете дали ролята, **msdyn_resourcecategory** и организационна единица, **msdyn_organizationalunit** имат полета **Приложимо за продажби** и **Приложимо за разходи**, зададени на **Да**.</span><span class="sxs-lookup"><span data-stu-id="babf5-113">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="babf5-114">Това ще ви позволи да зададете цената и разходите за всяка комбинация от роля и организационна единица.</span><span class="sxs-lookup"><span data-stu-id="babf5-114">This will allow you to set up the price and cost for each role and organizational unit combination.</span></span>

![Екранна снимка на параметри на Project Service с маркирана опция „Приложимо за продажби“](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> <span data-ttu-id="babf5-116">Ако сте използвали стандартните полета на роля и организационна единица като ценови измерения преди версия 3 на PSA, няма да има никаква видима промяна.</span><span class="sxs-lookup"><span data-stu-id="babf5-116">If you have been the using out-of-the box fields of role and organizational unit as pricing dimensions prior to version 3 of PSA, there will not be any observable change.</span></span> <span data-ttu-id="babf5-117">Можете да продължите да използвате Project Service както обикновено.</span><span class="sxs-lookup"><span data-stu-id="babf5-117">You can continue to use Project Service as usual.</span></span> 

<span data-ttu-id="babf5-118">Ако имате нужда от цена или разход за вашите ресурси с помощта на допълнителни атрибути, можете да създадете персонализирани полета, обекти и измерения.</span><span class="sxs-lookup"><span data-stu-id="babf5-118">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="babf5-119">За повече информация вижте следните теми, но имайте предвид, че трябва да изпълните процедурите в реда, посочен по-долу:</span><span class="sxs-lookup"><span data-stu-id="babf5-119">For more information, see the following topics, however note that you must complete the procedures in the order listed below:</span></span>

- [<span data-ttu-id="babf5-120">Създаване на персонализирани полета и обекти</span><span class="sxs-lookup"><span data-stu-id="babf5-120">Create custom fields and entities</span></span>](create-custom-fields-entities.md)
- [<span data-ttu-id="babf5-121">Добавяне на персонализирани полета към настройка на цени и обекти за транзакции</span><span class="sxs-lookup"><span data-stu-id="babf5-121">Add custom fields to price setup and transactional entities</span></span>](field-references.md)
- [<span data-ttu-id="babf5-122">Настройване на персонализирани полета като измерения на ценообразуване </span><span class="sxs-lookup"><span data-stu-id="babf5-122">Set up custom fields as pricing dimensions</span></span>](set-up-pricing-dimensions.md)
- [<span data-ttu-id="babf5-123">Актуализиране на атрибути на добавка за включване на нови ценови измерения</span><span class="sxs-lookup"><span data-stu-id="babf5-123">Update plug-in attributes to include new pricing dimensions</span></span>](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a><span data-ttu-id="babf5-124">Ценообразуване на времето на човешките ресурси</span><span class="sxs-lookup"><span data-stu-id="babf5-124">Pricing human resource time</span></span>
<span data-ttu-id="babf5-125">Как дадена организация ценообразува времето на човешките ресурси често е важно стратегическо съображение, което пряко засяга рентабилността на организацията.</span><span class="sxs-lookup"><span data-stu-id="babf5-125">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="babf5-126">Работете с финансовите екипи и ръководителите, когато вашата организация е готова да определи как иска да настрои ставките за фактуриране и разходи за времето на човешките ресурси.</span><span class="sxs-lookup"><span data-stu-id="babf5-126">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="babf5-127">Други съображения за ценообразуване включват дали да се използват повторно полета или обекти, които в момента не са ценови измерения, но се прилагат като ценово измерение за вашата организация.</span><span class="sxs-lookup"><span data-stu-id="babf5-127">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="babf5-128">Полета, като **Категория транзакция** (**msdyn_transactioncategory**) и **Наличен ресурс** (**bookableresource**), са примери за кандидат измерения.</span><span class="sxs-lookup"><span data-stu-id="babf5-128">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="babf5-129">Съобразете дали ценовото ви измерение трябва да бъде таблица или набор от опции.</span><span class="sxs-lookup"><span data-stu-id="babf5-129">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="babf5-130">Ако предвиждате промени в стойностите на измерение, които ще надхвърлят 10 или 12, и имате нужда от допълнителни атрибути за тези стойности, създайте обект, а не набор от опции.</span><span class="sxs-lookup"><span data-stu-id="babf5-130">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, create an entity rather than an option set.</span></span> <span data-ttu-id="babf5-131">Поддържането на набор от опции, като например добавяне или премахване на стойности, изисква администратор или разработчик, докато добавянето на нови редове към таблица може да се извърши от повечето бизнес потребители.</span><span class="sxs-lookup"><span data-stu-id="babf5-131">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most business users.</span></span>

<span data-ttu-id="babf5-132">Примерът по-долу показва ставки за фактуриране, които са настроени въз основа на ролята и организационната единица, към която принадлежи ресурсът.</span><span class="sxs-lookup"><span data-stu-id="babf5-132">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="babf5-133">Процентът на разходите обикновено се базира на групата работна заплата на служителя и на организационната единица, към която принадлежи.</span><span class="sxs-lookup"><span data-stu-id="babf5-133">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="babf5-134">В този пример таблиците за ставка за фактуриране и ставка за разходите ще изглеждат като следните.</span><span class="sxs-lookup"><span data-stu-id="babf5-134">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="babf5-135">**Примерни ставки за фактуриране**</span><span class="sxs-lookup"><span data-stu-id="babf5-135">**Sample bill rates**</span></span>

| <span data-ttu-id="babf5-136">Роля</span><span class="sxs-lookup"><span data-stu-id="babf5-136">Role</span></span>        | <span data-ttu-id="babf5-137">Организационна единица</span><span class="sxs-lookup"><span data-stu-id="babf5-137">Org Unit</span></span>    |<span data-ttu-id="babf5-138">Единица</span><span class="sxs-lookup"><span data-stu-id="babf5-138">Unit</span></span>      |<span data-ttu-id="babf5-139">Цена</span><span class="sxs-lookup"><span data-stu-id="babf5-139">Price</span></span>      |<span data-ttu-id="babf5-140">Валута</span><span class="sxs-lookup"><span data-stu-id="babf5-140">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="babf5-141">За разработчици</span><span class="sxs-lookup"><span data-stu-id="babf5-141">Developer</span></span>   | <span data-ttu-id="babf5-142">Contoso US</span><span class="sxs-lookup"><span data-stu-id="babf5-142">Contoso US</span></span>  |<span data-ttu-id="babf5-143">Час</span><span class="sxs-lookup"><span data-stu-id="babf5-143">Hour</span></span> | <span data-ttu-id="babf5-144">200</span><span class="sxs-lookup"><span data-stu-id="babf5-144">200</span></span>|<span data-ttu-id="babf5-145">USD</span><span class="sxs-lookup"><span data-stu-id="babf5-145">USD</span></span>     |
| <span data-ttu-id="babf5-146">За разработчици</span><span class="sxs-lookup"><span data-stu-id="babf5-146">Developer</span></span>   | <span data-ttu-id="babf5-147">Contoso Индия</span><span class="sxs-lookup"><span data-stu-id="babf5-147">Contoso India</span></span> |<span data-ttu-id="babf5-148">Час</span><span class="sxs-lookup"><span data-stu-id="babf5-148">Hour</span></span>|   <span data-ttu-id="babf5-149">112</span><span class="sxs-lookup"><span data-stu-id="babf5-149">112</span></span>|<span data-ttu-id="babf5-150">USD</span><span class="sxs-lookup"><span data-stu-id="babf5-150">USD</span></span>     |


<span data-ttu-id="babf5-151">**Примерни ставки за разходи**</span><span class="sxs-lookup"><span data-stu-id="babf5-151">**Sample cost rates**</span></span>

| <span data-ttu-id="babf5-152">Група работна заплата</span><span class="sxs-lookup"><span data-stu-id="babf5-152">Salary Band</span></span>     | <span data-ttu-id="babf5-153">Организационна единица</span><span class="sxs-lookup"><span data-stu-id="babf5-153">Org Unit</span></span>    |<span data-ttu-id="babf5-154">Единица</span><span class="sxs-lookup"><span data-stu-id="babf5-154">Unit</span></span>      |<span data-ttu-id="babf5-155">Цена</span><span class="sxs-lookup"><span data-stu-id="babf5-155">Price</span></span>      |<span data-ttu-id="babf5-156">Валута</span><span class="sxs-lookup"><span data-stu-id="babf5-156">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="babf5-157">Моята фирма_група1</span><span class="sxs-lookup"><span data-stu-id="babf5-157">My company_Band1</span></span> | <span data-ttu-id="babf5-158">Contoso US</span><span class="sxs-lookup"><span data-stu-id="babf5-158">Contoso US</span></span>  |<span data-ttu-id="babf5-159">Час</span><span class="sxs-lookup"><span data-stu-id="babf5-159">Hour</span></span> | <span data-ttu-id="babf5-160">145</span><span class="sxs-lookup"><span data-stu-id="babf5-160">145</span></span>|<span data-ttu-id="babf5-161">USD</span><span class="sxs-lookup"><span data-stu-id="babf5-161">USD</span></span>     |
| <span data-ttu-id="babf5-162">Моята фирма_група2</span><span class="sxs-lookup"><span data-stu-id="babf5-162">My company_Band2</span></span> | <span data-ttu-id="babf5-163">Contoso Индия</span><span class="sxs-lookup"><span data-stu-id="babf5-163">Contoso India</span></span> |<span data-ttu-id="babf5-164">Час</span><span class="sxs-lookup"><span data-stu-id="babf5-164">Hour</span></span>|   <span data-ttu-id="babf5-165">67</span><span class="sxs-lookup"><span data-stu-id="babf5-165">67</span></span>|<span data-ttu-id="babf5-166">USD</span><span class="sxs-lookup"><span data-stu-id="babf5-166">USD</span></span>     |


[!INCLUDE[footer-include](../includes/footer-banner.md)]