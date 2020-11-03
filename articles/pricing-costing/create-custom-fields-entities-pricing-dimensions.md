---
title: Създайте персонализирани полета и обекти като измерения на ценообразуване
description: Тази тема предоставя информация за това как да създадете персонализирани набори от опции или обекти.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 9dd43be79f8e906298578911b3bff03e66c2f1e5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071858"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="51a21-103">Създайте персонализирани полета и обекти като измерения на ценообразуване</span><span class="sxs-lookup"><span data-stu-id="51a21-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="51a21-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="51a21-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="51a21-105">Изпълнете следните стъпки всеки път, когато искате да създадете персонализиран набор от опции или обекта.</span><span class="sxs-lookup"><span data-stu-id="51a21-105">Complete the following steps any time that you want to create a custom option set or entity.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="51a21-106">Препоръчваме ви да направите всички промени в персонализираните ценови измерения в отделно решение.</span><span class="sxs-lookup"><span data-stu-id="51a21-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="51a21-107">Тази важна най-добра практика осигурява гъвкавост в бъдеще за актуализиране или премахване на промени, ако е необходимо, помага за повторното използване на вашата работа и улеснява пренасянето на тези промени на друг екземпляр.</span><span class="sxs-lookup"><span data-stu-id="51a21-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="51a21-108">След като сте направили всички необходими промени, експортирайте това решение като **Завършено решение** и го импортирайте в други екземпляри, за да използвате отново настройката за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="51a21-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="51a21-109">Създаване на персонализирано решение за ценови измерения</span><span class="sxs-lookup"><span data-stu-id="51a21-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="51a21-110">Отидете на **Настройки** > **Решения** и след това изберете **Нов** , за да създадете ново решение.</span><span class="sxs-lookup"><span data-stu-id="51a21-110">Go to **Settings** > **Solutions** , and then select **New** to create a new solution.</span></span> 
2. <span data-ttu-id="51a21-111">Наименувайте решението, **Ценови измерения на \<your organization name>** , въведете оставащата изисквана информация и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="51a21-111">Name the solution, **\<your organization name> pricing dimensions** , enter the remaining required information, and then select **Save**.</span></span>
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="51a21-112">Създаване на персонализирани полета и набори от опции в решението за ценови измерения</span><span class="sxs-lookup"><span data-stu-id="51a21-112">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="51a21-113">Ценовото измерение може да бъде набор от опции или обект.</span><span class="sxs-lookup"><span data-stu-id="51a21-113">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="51a21-114">И двете трябва да бъдат създадени в решението за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="51a21-114">Both must be created in your pricing solution.</span></span> <span data-ttu-id="51a21-115">Стъпките в тази процедура обясняват как да създадете измерения, базирани на обект, и измерения, базирани на набор от опции.</span><span class="sxs-lookup"><span data-stu-id="51a21-115">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="51a21-116">Измерения, базирани на обект</span><span class="sxs-lookup"><span data-stu-id="51a21-116">Entity-based dimensions</span></span>

1. <span data-ttu-id="51a21-117">Отидете на **Настройки** > **Решения** и след това щракнете двукратно върху **Ценови измерения на \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="51a21-117">Go to **Settings** > **Solutions** , and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="51a21-118">В мениджъра на решения, в левия навигационен екран, изберете **Обекти**.</span><span class="sxs-lookup"><span data-stu-id="51a21-118">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="51a21-119">Изберете **Нов** , за да създадете нов обект, наречен **Стандартна длъжност**.</span><span class="sxs-lookup"><span data-stu-id="51a21-119">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="51a21-120">Въведете останалата необходима информация и след това изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="51a21-120">Enter the remaining required information, and then select **Save**.</span></span>


### <a name="option-set-based-dimensions"></a><span data-ttu-id="51a21-121">Измерения, базирани на набор от опции</span><span class="sxs-lookup"><span data-stu-id="51a21-121">Option set-based dimensions</span></span> 
<span data-ttu-id="51a21-122">Можете да създадете две измерения, базирани на набор от опции.</span><span class="sxs-lookup"><span data-stu-id="51a21-122">You can create two option set-based dimensions.</span></span> <span data-ttu-id="51a21-123">Използвайте **Месторабота на ресурса** за проследяване на цената на работа в местоположението **У дома** и работа **На място** и използвайте **Работни часове за ресурси** със стойности **Редовни** и **Извънредни** , за да приложите надценка, когато работата е завършена.</span><span class="sxs-lookup"><span data-stu-id="51a21-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="51a21-124">Отидете на **Настройки** > **Решения** и щракнете двукратно върху **Ценови измерения на \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="51a21-124">Go to **Settings** > **Solutions** , and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="51a21-125">В мениджъра на решения, в левия навигационен екран, изберете **Набори от опции**.</span><span class="sxs-lookup"><span data-stu-id="51a21-125">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="51a21-126">Изберете **Нов** , за да създадете нов набор от опции, въведете останалата изисквана информация и след това изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="51a21-126">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="51a21-127">Създаване на данни за измерения, базирани на обекти</span><span class="sxs-lookup"><span data-stu-id="51a21-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="51a21-128">Можете ръчно да създавате данни за измерения, базирани на обекти, или с помощта на импортиране в Microsoft Excel или обаждане на отдела по обслужване.</span><span class="sxs-lookup"><span data-stu-id="51a21-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="51a21-129">Използвайте стъпките в тази процедура, за да създадете две стандартни заглавия **Системен инженер** и **Старши системен инженер** от базираното на обект измерение **Стандартна длъжност**.</span><span class="sxs-lookup"><span data-stu-id="51a21-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="51a21-130">Ако данните, които искате да създадете, са малки, както в следващия пример, можете да използвате стандартен формуляр.</span><span class="sxs-lookup"><span data-stu-id="51a21-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="51a21-131">Изберете **Разширено търсене** , изберете обекта **Стандартно заглавие** и след това изберете **Резултати**.</span><span class="sxs-lookup"><span data-stu-id="51a21-131">Select **Advanced Find** , select the entity **Standard Title** , and then select **Results**.</span></span> <span data-ttu-id="51a21-132">Всички редове в обекта **Стандартна длъжност** ще бъдат показани.</span><span class="sxs-lookup"><span data-stu-id="51a21-132">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="51a21-133">Изберете **Създаване** и в полето **Име** въведете „Системен инженер“ и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="51a21-133">Select **New** , and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
3. <span data-ttu-id="51a21-134">Затваряне на формуляра.</span><span class="sxs-lookup"><span data-stu-id="51a21-134">Close the form.</span></span> 
4. <span data-ttu-id="51a21-135">Повторете стъпки 1 – 3, за да създадете друга стандартна длъжност за „Старши системен инженер“.</span><span class="sxs-lookup"><span data-stu-id="51a21-135">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="51a21-136">Добавяне на всички необходими обекти и свързаните компоненти в решението за ценови измерения</span><span class="sxs-lookup"><span data-stu-id="51a21-136">Add all required entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="51a21-137">Ще трябва да добавите следните обекти към вашето решение за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="51a21-137">You will need to add the following entities to your pricing solution.</span></span> <span data-ttu-id="51a21-138">Използвайте стъпките в тази процедура, за да направите някои важни промени на схемата в решението за ценообразуване, така че обектите да разберат новите ценови измерения.</span><span class="sxs-lookup"><span data-stu-id="51a21-138">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="51a21-139">Изберете **Настройки** > **Решения** и щракнете двукратно върху **Ценови измерения на \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="51a21-139">Select **Settings** > **Solutions** , and double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="51a21-140">В мениджъра на решения, в левия навигационен екран, изберете **Добавяне на съществуващи**  >  **Обекти**.</span><span class="sxs-lookup"><span data-stu-id="51a21-140">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="51a21-141">В диалоговия прозорец **Компоненти на решения** изберете следните обекти:</span><span class="sxs-lookup"><span data-stu-id="51a21-141">In the **Solution Components** dialog box, select the following entities:</span></span>

  - <span data-ttu-id="51a21-142">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="51a21-142">Actual</span></span>
  - <span data-ttu-id="51a21-143">Наличен ресурс</span><span class="sxs-lookup"><span data-stu-id="51a21-143">Bookable Resource</span></span>
  - <span data-ttu-id="51a21-144">Ред за прогнозна оценка</span><span class="sxs-lookup"><span data-stu-id="51a21-144">Estimate Line</span></span>
  - <span data-ttu-id="51a21-145">Подробности за ред на фактура</span><span class="sxs-lookup"><span data-stu-id="51a21-145">Invoice Line Detail</span></span>
  - <span data-ttu-id="51a21-146">Счетоводен запис</span><span class="sxs-lookup"><span data-stu-id="51a21-146">Journal Line</span></span>
  - <span data-ttu-id="51a21-147">Подробности за ред на договор по проект</span><span class="sxs-lookup"><span data-stu-id="51a21-147">Project Contract Line Detail</span></span>
  - <span data-ttu-id="51a21-148">Член на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="51a21-148">Project Team Member</span></span>
  - <span data-ttu-id="51a21-149">Подробности за ред на оферта</span><span class="sxs-lookup"><span data-stu-id="51a21-149">Quote Line Detail</span></span>
  - <span data-ttu-id="51a21-150">Надценка над цена на роля</span><span class="sxs-lookup"><span data-stu-id="51a21-150">Role Price Markup</span></span>
  - <span data-ttu-id="51a21-151">Цена на роля</span><span class="sxs-lookup"><span data-stu-id="51a21-151">Role Price</span></span> 
  - <span data-ttu-id="51a21-152">Запис за време</span><span class="sxs-lookup"><span data-stu-id="51a21-152">Time Entry</span></span> 


> [!NOTE]
> <span data-ttu-id="51a21-153">Уверете се, че сте включили всички формуляри и изгледи за всеки от избраните обекти.</span><span class="sxs-lookup"><span data-stu-id="51a21-153">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="51a21-154">Когато бъдете подканени да включите зависими обекти за обектите, избрани по-горе, изберете **Не**.</span><span class="sxs-lookup"><span data-stu-id="51a21-154">When prompted to include any dependent entities for the entities selected above, select **No**.</span></span>

