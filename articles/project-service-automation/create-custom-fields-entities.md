---
title: Създаване на персонализирани полета и обекти
description: Тази тема обяснява как да създадете набори от опции и обекти в собственото си решение в платформата Power Apps.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/26/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: fb160bfd-e037-4a21-a968-3ff2e6e16481
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 7ee30e3bb6b8034ef226e2e9181195685355011f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749350"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="40bd7-103">Създаване на персонализирани полета и обекти</span><span class="sxs-lookup"><span data-stu-id="40bd7-103">Create custom fields and entities</span></span> 

<span data-ttu-id="40bd7-104">Изпълнете следните стъпки всеки път, когато искате да създадете персонализиран набор от опции или обект в платформата Power Apps.</span><span class="sxs-lookup"><span data-stu-id="40bd7-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="40bd7-105">Процедурите в тази тема трябва да бъдат изпълнени с помощта на уеб интерфейса на Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="40bd7-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="40bd7-106">Препоръчваме ви да направите всички промени в персонализираните ценови измерения в отделно решение.</span><span class="sxs-lookup"><span data-stu-id="40bd7-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="40bd7-107">Тази важна най-добра практика осигурява гъвкавост в бъдеще за актуализиране или премахване на промени, ако е необходимо, помага за повторното използване на вашата работа и улеснява пренасянето на тези промени на друг екземпляр.</span><span class="sxs-lookup"><span data-stu-id="40bd7-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="40bd7-108">След като сте направили всички необходими промени, експортирайте това решение като **Завършено решение** и го импортирайте в други екземпляри, за да използвате отново настройката за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="40bd7-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="40bd7-109">Създаване на персонализирано решение за ценови измерения</span><span class="sxs-lookup"><span data-stu-id="40bd7-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="40bd7-110">В PSA щракнете върху **Настройки** > **Решения** и след това щракнете върху **Нов**, за да създадете ново решение.</span><span class="sxs-lookup"><span data-stu-id="40bd7-110">In PSA, click **Settings** > **Solutions**, and then click **New** to create a new solution.</span></span> 
2. <span data-ttu-id="40bd7-111">Наименувайте решението, **Ценови измерения на \<име на организацията >**, въведете оставащата изисквана информация и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-111">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then click **Save**.</span></span>

> ![Създаване на персонализирано решение за ценови измерения](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="40bd7-113">Създаване на персонализирани полета и набори от опции в решението за ценови измерения</span><span class="sxs-lookup"><span data-stu-id="40bd7-113">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="40bd7-114">Ценовото измерение може да бъде набор от опции или обект.</span><span class="sxs-lookup"><span data-stu-id="40bd7-114">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="40bd7-115">И двете трябва да бъдат създадени в решението за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="40bd7-115">Both must be created in your pricing solution.</span></span> <span data-ttu-id="40bd7-116">Стъпките в тази процедура обясняват как да създадете измерения, базирани на обект, и измерения, базирани на набор от опции.</span><span class="sxs-lookup"><span data-stu-id="40bd7-116">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="40bd7-117">Измерения, базирани на обект</span><span class="sxs-lookup"><span data-stu-id="40bd7-117">Entity-based dimensions</span></span>

1. <span data-ttu-id="40bd7-118">В PSA щракнете върху **Настройки**  > **Решения** и след това щракнете двукратно върху **Ценови измерения на \<име на вашата организация>**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-118">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="40bd7-119">В мениджъра на решения, в левия навигационен екран, изберете **Обекти**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-119">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="40bd7-120">Щракнете върху **Нов**, за да създадете нов обект, наречен **Стандартна длъжност**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-120">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="40bd7-121">Въведете останалата необходима информация и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-121">Enter the remaining required information, and then click **Save**.</span></span>

> ![Дефиниране на обекта „Стандартна длъжност“](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="40bd7-123">Измерения, базирани на набор от опции</span><span class="sxs-lookup"><span data-stu-id="40bd7-123">Option set-based dimensions</span></span> 
<span data-ttu-id="40bd7-124">Можете да създадете две измерения, базирани на набор от опции.</span><span class="sxs-lookup"><span data-stu-id="40bd7-124">You can create two option set-based dimensions.</span></span> <span data-ttu-id="40bd7-125">Използвайте **Месторабота на ресурса** за проследяване на цената на работа в местоположението **У дома** и работа **На място** и използвайте **Работни часове за ресурси** със стойности **Редовни** и **Извънредни**, за да приложите надценка, когато работата е завършена.</span><span class="sxs-lookup"><span data-stu-id="40bd7-125">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="40bd7-126">В PSA щракнете върху **Настройки**  > **Решения** и след това щракнете двукратно върху **Ценови измерения на \<име на вашата организация>**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-126">In PSA, click **Settings** > **Solutions**, and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="40bd7-127">В мениджъра на решения, в левия навигационен екран, изберете **Набори от опции**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-127">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="40bd7-128">Щракнете върху **Нов**, за да създадете нов набор от опции, въведете останалата изисквана информация и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-128">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="40bd7-129">Ценово измерение, базирано на набор от опции, наречено „Месторабота на ресурс“</span><span class="sxs-lookup"><span data-stu-id="40bd7-129">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="40bd7-130">Ценово измерение, базирано на набор от опции, наречено „Работни часове на ресурс“</span><span class="sxs-lookup"><span data-stu-id="40bd7-130">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="40bd7-131">Създаване на данни за измерения, базирани на обекти</span><span class="sxs-lookup"><span data-stu-id="40bd7-131">Create data for entity-based dimensions</span></span>

<span data-ttu-id="40bd7-132">Можете ръчно да създавате данни за измерения, базирани на обекти, или с помощта на импортиране в Microsoft Excel или обаждане на отдела по обслужване.</span><span class="sxs-lookup"><span data-stu-id="40bd7-132">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="40bd7-133">Използвайте стъпките в тази процедура, за да създадете две стандартни заглавия **Системен инженер** и **Старши системен инженер** от базираното на обект измерение **Стандартна длъжност**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-133">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="40bd7-134">Ако данните, които искате да създадете, са малки, както в следващия пример, можете да използвате стандартен формуляр.</span><span class="sxs-lookup"><span data-stu-id="40bd7-134">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="40bd7-135">В PSA щракнете върху **Разширено търсене**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-135">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="40bd7-136">Изберете обекта, **Стандартна длъжност** и след това щракнете върху **Резултати**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-136">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="40bd7-137">Всички редове в обекта **Стандартна длъжност** ще бъдат показани.</span><span class="sxs-lookup"><span data-stu-id="40bd7-137">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="40bd7-138">Щракнете върху **Нов**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-138">Click **New**.</span></span> <span data-ttu-id="40bd7-139">В полето **Име** въведете „Системен инженер“ и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-139">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="40bd7-140">Затворете формуляра.</span><span class="sxs-lookup"><span data-stu-id="40bd7-140">Close the form.</span></span> 
4. <span data-ttu-id="40bd7-141">Повторете стъпки 1 – 3, за да създадете друга стандартна длъжност за „Старши системен инженер“.</span><span class="sxs-lookup"><span data-stu-id="40bd7-141">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="40bd7-142">Примерни данни за обект „Стандартна длъжност“</span><span class="sxs-lookup"><span data-stu-id="40bd7-142">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)

## <a name="add-all-required-psa-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="40bd7-143">Добавяне на всички необходими обекти в PSA и свързаните компоненти в решението за ценови измерения</span><span class="sxs-lookup"><span data-stu-id="40bd7-143">Add all required PSA entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="40bd7-144">Ще трябва да добавите следните обекти на Project Service към вашето решение за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="40bd7-144">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="40bd7-145">Използвайте стъпките в тази процедура, за да направите някои важни промени на схемата в решението за ценообразуване, така че обектите да разберат новите ценови измерения.</span><span class="sxs-lookup"><span data-stu-id="40bd7-145">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="40bd7-146">В PSA щракнете върху **Настройки**  > **Решения** и след това щракнете двукратно върху **Ценови измерения на \<име на вашата организация>**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-146">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="40bd7-147">В мениджъра на решения, в левия навигационен екран, изберете **Добавяне на съществуващи**  >  **Обекти**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-147">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="40bd7-148">В диалоговия прозорец **Компоненти на решения** изберете следните обекти:</span><span class="sxs-lookup"><span data-stu-id="40bd7-148">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="40bd7-149">Действителни данни</span><span class="sxs-lookup"><span data-stu-id="40bd7-149">Actual</span></span>
- <span data-ttu-id="40bd7-150">Наличен ресурс</span><span class="sxs-lookup"><span data-stu-id="40bd7-150">Bookable Resource</span></span>
- <span data-ttu-id="40bd7-151">Ред за прогнозна оценка</span><span class="sxs-lookup"><span data-stu-id="40bd7-151">Estimate Line</span></span>
- <span data-ttu-id="40bd7-152">Подробности за ред на фактура</span><span class="sxs-lookup"><span data-stu-id="40bd7-152">Invoice Line Detail</span></span>
- <span data-ttu-id="40bd7-153">Счетоводен запис</span><span class="sxs-lookup"><span data-stu-id="40bd7-153">Journal Line</span></span>
- <span data-ttu-id="40bd7-154">Подробности за ред на договор по проект</span><span class="sxs-lookup"><span data-stu-id="40bd7-154">Project Contract Line Detail</span></span>
- <span data-ttu-id="40bd7-155">Член на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="40bd7-155">Project Team Member</span></span>
- <span data-ttu-id="40bd7-156">Подробности за ред на оферта</span><span class="sxs-lookup"><span data-stu-id="40bd7-156">Quote Line Detail</span></span>
- <span data-ttu-id="40bd7-157">Надценка над цена на роля</span><span class="sxs-lookup"><span data-stu-id="40bd7-157">Role Price Markup</span></span>
- <span data-ttu-id="40bd7-158">Цена на роля</span><span class="sxs-lookup"><span data-stu-id="40bd7-158">Role Price</span></span> 
- <span data-ttu-id="40bd7-159">Запис за време</span><span class="sxs-lookup"><span data-stu-id="40bd7-159">Time Entry</span></span> 

> ![Добавяне на съществуващи обекти към решението за ценови измерения](media/Existing-entities-to-PD-solution.png)

> ![Избор на компоненти на решението](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="40bd7-162">Уверете се, че сте включили всички формуляри и изгледи за всеки от избраните обекти.</span><span class="sxs-lookup"><span data-stu-id="40bd7-162">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="40bd7-163">Когато бъдете подканени да включите зависими обекти за обектите, избрани по-горе, щракнете върху **Не**.</span><span class="sxs-lookup"><span data-stu-id="40bd7-163">When prompted to include any dependent entities for the entities selected above, click **No**.</span></span>

> ![Не включвай всички свързани компоненти](media/Do-not-include-required.png)


