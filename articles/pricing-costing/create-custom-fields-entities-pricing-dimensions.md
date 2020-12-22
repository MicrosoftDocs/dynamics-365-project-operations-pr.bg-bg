---
title: Създайте персонализирани полета и обекти като измерения на ценообразуване
description: Тази тема предоставя информация за това как да създадете персонализирани набори от опции или обекти.
author: rumant
manager: AnnBe
ms.date: 11/18/2020
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
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: fc5917856b8f28d36dc55593a68eba7823a00b36
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642800"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="d2b13-103">Създайте персонализирани полета и обекти като измерения на ценообразуване</span><span class="sxs-lookup"><span data-stu-id="d2b13-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="d2b13-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="d2b13-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d2b13-105">Изпълнете следните стъпки, когато искате да създадете персонализиран набор от опции или обект, за да го използвате като измерение на ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="d2b13-105">Complete the following steps when you want to create a custom option set or entity for using it as a pricing dimension.</span></span> <span data-ttu-id="d2b13-106">За повече информация вижте [Общ преглед на измерения за ценообразуване](pricing-dimensions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="d2b13-106">For more information, see [Pricing dimensions overview](pricing-dimensions-overview.md).</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="d2b13-107">Препоръчваме ви да направите всички промени в персонализираните ценови измерения в отделно решение.</span><span class="sxs-lookup"><span data-stu-id="d2b13-107">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="d2b13-108">Тази важна най-добра практика осигурява гъвкавост в бъдеще за актуализиране или премахване на промените при необходимост.</span><span class="sxs-lookup"><span data-stu-id="d2b13-108">This important best practice provides flexibility in the future to update or remove changes as needed.</span></span> <span data-ttu-id="d2b13-109">Това ще помогне и за повторното използване на работата и ще улесни пренасянето на тези промени в друг екземпляр. След като направите всички необходими промени, експортирайте това решение като **завършено решение** и го импортирайте в други екземпляри, за да използвате повторно настройката за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="d2b13-109">This will also help with re-use of your work and make it easier to port these changes to another instance After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="d2b13-110">Създаване на персонализирани полета и набори от опции в решението за ценови измерения</span><span class="sxs-lookup"><span data-stu-id="d2b13-110">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="d2b13-111">Ценовото измерение може да бъде набор от опции или обект.</span><span class="sxs-lookup"><span data-stu-id="d2b13-111">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="d2b13-112">И двете трябва да бъдат създадени в решението за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="d2b13-112">Both must be created in your pricing solution.</span></span> <span data-ttu-id="d2b13-113">Стъпките в тази процедура обясняват как да създадете измерения, базирани на обект, и измерения, базирани на набор от опции.</span><span class="sxs-lookup"><span data-stu-id="d2b13-113">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="d2b13-114">Измерения, базирани на обект</span><span class="sxs-lookup"><span data-stu-id="d2b13-114">Entity-based dimensions</span></span>
<span data-ttu-id="d2b13-115">За да създадете базирани на обект измерения, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="d2b13-115">To create entity-based dimensions, follow these steps:</span></span>

1. <span data-ttu-id="d2b13-116">Отидете на **Настройки** > **Решения** и след това щракнете двукратно върху **Ценови измерения на \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-116">Go to **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="d2b13-117">В мениджъра на решения, в левия навигационен екран, изберете **Обекти**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-117">In Solution Explorer, in the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="d2b13-118">Изберете **Нов**, за да създадете нов обект, наречен **Стандартна длъжност**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-118">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="d2b13-119">Въведете останалата необходима информация и след това изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-119">Enter the remaining required information, and then select **Save**.</span></span>

> ![Дефиниране на обекта „Стандартна длъжност“](media/Standard-Title-entity-definition.png)

### <a name="option-set-based-dimensions"></a><span data-ttu-id="d2b13-121">Измерения, базирани на набор от опции</span><span class="sxs-lookup"><span data-stu-id="d2b13-121">Option set-based dimensions</span></span> 
<span data-ttu-id="d2b13-122">Можете да създадете две измерения, базирани на набор от опции.</span><span class="sxs-lookup"><span data-stu-id="d2b13-122">You can create two option set-based dimensions.</span></span> 

- <span data-ttu-id="d2b13-123">Използвайте **Месторабота на ресурс** за проследяване на цената на работата в местоположението **У дома** и **На място**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work.</span></span> 
- <span data-ttu-id="d2b13-124">Използвайте **Работно време на ресурс** със стойности **Нормално** и **Извънредно**, за да приложите надценка при завършване на работата.</span><span class="sxs-lookup"><span data-stu-id="d2b13-124">Use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when the work is complete.</span></span>

<span data-ttu-id="d2b13-125">Следващата графика предоставя изглед на измерението **Месторабота на ресурс**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-125">The following graphic provides a view of the **Resource Work Location** dimension.</span></span> 

> ![Ценово измерение, базирано на набор от опции, наречено „Месторабота на ресурс“](media/Option-set-PD-called-Resource-Work-Location.png)

<span data-ttu-id="d2b13-127">Следващата графика предоставя изглед на измерението **Работно време на ресурс**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-127">The following graphic provides a view of the **Resource Work Hours** dimension.</span></span> 

> ![Ценово измерение, базирано на набор от опции, наречено „Работни часове на ресурс“](media/Option-set-PD-called-Resource-Work-Hours.png)

1. <span data-ttu-id="d2b13-129">Отидете на **Настройки** > **Решения** и щракнете двукратно върху **Ценови измерения на \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-129">Go to **Settings** > **Solutions**, and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="d2b13-130">В мениджъра на решения, в левия навигационен екран, изберете **Набори от опции**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-130">In Solution Explorer, in the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="d2b13-131">Изберете **Нов**, за да създадете нов набор от опции, въведете останалата изисквана информация и след това изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-131">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="d2b13-132">Създаване на данни за измерения, базирани на обекти</span><span class="sxs-lookup"><span data-stu-id="d2b13-132">Create data for entity-based dimensions</span></span>

<span data-ttu-id="d2b13-133">Можете ръчно да създавате данни за измерения, базирани на обекти, или с помощта на импортиране в Microsoft Excel или обаждане на отдела по обслужване.</span><span class="sxs-lookup"><span data-stu-id="d2b13-133">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="d2b13-134">Използвайте стъпките в тази процедура, за да създадете две стандартни заглавия **Системен инженер** и **Старши системен инженер** от базираното на обект измерение **Стандартна длъжност**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-134">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="d2b13-135">Ако данните, които искате да създадете, са малки, както в следващия пример, можете да използвате стандартен формуляр.</span><span class="sxs-lookup"><span data-stu-id="d2b13-135">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="d2b13-136">Изберете **Разширено търсене**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-136">Select **Advanced Find**.</span></span>
2. <span data-ttu-id="d2b13-137">Изберете обекта, **Стандартна длъжност** и след това изберете **Резултати**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-137">Select the entity **Standard Title**, and then select **Results**.</span></span> <span data-ttu-id="d2b13-138">Всички редове в обекта **Стандартна длъжност** ще бъдат показани.</span><span class="sxs-lookup"><span data-stu-id="d2b13-138">All of the rows in the **Standard Title** entity will be shown.</span></span>
3. <span data-ttu-id="d2b13-139">Изберете **Създаване** и в полето **Име** въведете „Системен инженер“ и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="d2b13-139">Select **New**, and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
4. <span data-ttu-id="d2b13-140">Затваряне на страницата.</span><span class="sxs-lookup"><span data-stu-id="d2b13-140">Close the page.</span></span> 
5. <span data-ttu-id="d2b13-141">Повторете стъпки 1 – 3, за да създадете друга стандартна длъжност за „Старши системен инженер“.</span><span class="sxs-lookup"><span data-stu-id="d2b13-141">Repeat steps 1-3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![Примерни данни за обект „Стандартна длъжност“](media/ST-data.png)
