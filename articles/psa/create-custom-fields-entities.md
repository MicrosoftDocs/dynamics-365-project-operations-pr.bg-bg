---
title: Създаване на персонализирани полета и обекти
description: Тази тема обяснява как да създадете набори от опции и обекти в собственото си решение в платформата Power Apps.
author: Rumant
ms.custom:
- dyn365-projectservice
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
ms.openlocfilehash: 3d838bde8a3d7cbc15e06fb3289924468c284a8a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998938"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="78ed3-103">Създаване на персонализирани полета и обекти</span><span class="sxs-lookup"><span data-stu-id="78ed3-103">Create custom fields and entities</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="78ed3-104">Изпълнете следните стъпки всеки път, когато искате да създадете персонализиран набор от опции или обект в платформата Power Apps.</span><span class="sxs-lookup"><span data-stu-id="78ed3-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="78ed3-105">Процедурите в тази тема трябва да бъдат изпълнени с помощта на уеб интерфейса на Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="78ed3-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="78ed3-106">Препоръчваме ви да направите всички промени в персонализираните ценови измерения в отделно решение.</span><span class="sxs-lookup"><span data-stu-id="78ed3-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="78ed3-107">Тази важна най-добра практика осигурява гъвкавост в бъдеще за актуализиране или премахване на промени, ако е необходимо, помага за повторното използване на вашата работа и улеснява пренасянето на тези промени на друг екземпляр.</span><span class="sxs-lookup"><span data-stu-id="78ed3-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="78ed3-108">След като сте направили всички необходими промени, експортирайте това решение като **Завършено решение** и го импортирайте в други екземпляри, за да използвате отново настройката за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="78ed3-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="78ed3-109">Създаване на персонализирани полета и набори от опции в решението за ценови измерения</span><span class="sxs-lookup"><span data-stu-id="78ed3-109">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="78ed3-110">Ценовото измерение може да бъде набор от опции или обект.</span><span class="sxs-lookup"><span data-stu-id="78ed3-110">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="78ed3-111">И двете трябва да бъдат създадени в решението за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="78ed3-111">Both must be created in your pricing solution.</span></span> <span data-ttu-id="78ed3-112">Стъпките в тази процедура обясняват как да създадете измерения, базирани на обект, и измерения, базирани на набор от опции.</span><span class="sxs-lookup"><span data-stu-id="78ed3-112">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="78ed3-113">Измерения, базирани на обект</span><span class="sxs-lookup"><span data-stu-id="78ed3-113">Entity-based dimensions</span></span>

1. <span data-ttu-id="78ed3-114">В PSA щракнете върху **Настройки** > **Решения** и след това щракнете двукратно върху **Ценови измерения на \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="78ed3-114">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="78ed3-115">В мениджъра на решения, в левия навигационен екран, изберете **Обекти**.</span><span class="sxs-lookup"><span data-stu-id="78ed3-115">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="78ed3-116">Щракнете върху **Нов**, за да създадете нов обект, наречен **Стандартна длъжност**.</span><span class="sxs-lookup"><span data-stu-id="78ed3-116">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="78ed3-117">Въведете останалата необходима информация и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="78ed3-117">Enter the remaining required information, and then click **Save**.</span></span>

> ![Дефиниране на обекта „Стандартна длъжност“](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="78ed3-119">Измерения, базирани на набор от опции</span><span class="sxs-lookup"><span data-stu-id="78ed3-119">Option set-based dimensions</span></span> 
<span data-ttu-id="78ed3-120">Можете да създадете две измерения, базирани на набор от опции.</span><span class="sxs-lookup"><span data-stu-id="78ed3-120">You can create two option set-based dimensions.</span></span> <span data-ttu-id="78ed3-121">Използвайте **Месторабота на ресурса** за проследяване на цената на работа в местоположението **У дома** и работа **На място** и използвайте **Работни часове за ресурси** със стойности **Редовни** и **Извънредни**, за да приложите надценка, когато работата е завършена.</span><span class="sxs-lookup"><span data-stu-id="78ed3-121">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="78ed3-122">В PSA щракнете върху **Настройки** > **Решения** и след това щракнете двукратно върху **Ценови измерения на \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="78ed3-122">In PSA, click **Settings** > **Solutions**, and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="78ed3-123">В мениджъра на решения, в левия навигационен екран, изберете **Набори от опции**.</span><span class="sxs-lookup"><span data-stu-id="78ed3-123">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="78ed3-124">Щракнете върху **Нов**, за да създадете нов набор от опции, въведете останалата изисквана информация и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="78ed3-124">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="78ed3-125">Ценово измерение, базирано на набор от опции, наречено „Месторабота на ресурс“</span><span class="sxs-lookup"><span data-stu-id="78ed3-125">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="78ed3-126">Ценово измерение, базирано на набор от опции, наречено „Работни часове на ресурс“</span><span class="sxs-lookup"><span data-stu-id="78ed3-126">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="78ed3-127">Създаване на данни за измерения, базирани на обекти</span><span class="sxs-lookup"><span data-stu-id="78ed3-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="78ed3-128">Можете ръчно да създавате данни за измерения, базирани на обекти, или с помощта на импортиране в Microsoft Excel или обаждане на отдела по обслужване.</span><span class="sxs-lookup"><span data-stu-id="78ed3-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="78ed3-129">Използвайте стъпките в тази процедура, за да създадете две стандартни заглавия **Системен инженер** и **Старши системен инженер** от базираното на обект измерение **Стандартна длъжност**.</span><span class="sxs-lookup"><span data-stu-id="78ed3-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="78ed3-130">Ако данните, които искате да създадете, са малки, както в следващия пример, можете да използвате стандартен формуляр.</span><span class="sxs-lookup"><span data-stu-id="78ed3-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="78ed3-131">В PSA щракнете върху **Разширено търсене**.</span><span class="sxs-lookup"><span data-stu-id="78ed3-131">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="78ed3-132">Изберете обекта, **Стандартна длъжност** и след това щракнете върху **Резултати**.</span><span class="sxs-lookup"><span data-stu-id="78ed3-132">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="78ed3-133">Всички редове в обекта **Стандартна длъжност** ще бъдат показани.</span><span class="sxs-lookup"><span data-stu-id="78ed3-133">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="78ed3-134">Щракнете върху **Нов**.</span><span class="sxs-lookup"><span data-stu-id="78ed3-134">Click **New**.</span></span> <span data-ttu-id="78ed3-135">В полето **Име** въведете „Системен инженер“ и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="78ed3-135">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="78ed3-136">Затворете формуляра.</span><span class="sxs-lookup"><span data-stu-id="78ed3-136">Close the form.</span></span> 
4. <span data-ttu-id="78ed3-137">Повторете стъпки 1 – 3, за да създадете друга стандартна длъжност за „Старши системен инженер“.</span><span class="sxs-lookup"><span data-stu-id="78ed3-137">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="78ed3-138">Примерни данни за обект „Стандартна длъжност“</span><span class="sxs-lookup"><span data-stu-id="78ed3-138">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]