---
title: Създаване на персонализирани решения за ценови измерения
description: Тази тема обяснява как да създадете персонализирано решение при създаване на персонализирани размери за ценообразуване.
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
ms.openlocfilehash: ae7f22b9cb092e956d0f1eaf1f1997c8e97392f4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012303"
---
# <a name="create-custom-solutions-for-pricing-dimensions"></a><span data-ttu-id="e622b-103">Създаване на персонализирани решения за ценови измерения</span><span class="sxs-lookup"><span data-stu-id="e622b-103">Create custom solutions for pricing dimensions</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

> [!IMPORTANT]
> <span data-ttu-id="e622b-104">Всички промени в размера на персонализираните цени трябва да бъдат в отделно решение.</span><span class="sxs-lookup"><span data-stu-id="e622b-104">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="e622b-105">Тази важна най-добра практика осигурява гъвкавост в бъдеще за актуализиране или премахване на промени, ако е необходимо, помага за повторното използване на вашата работа и улеснява пренасянето на тези промени на друг екземпляр.</span><span class="sxs-lookup"><span data-stu-id="e622b-105">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="e622b-106">След като направите всички необходими промени, експортирайте това решение като **Завършено решение** и го импортирайте в други екземпляри, за да използвате отново настройката за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="e622b-106">After you make the required changes, export this solution as a **Managed solution**, and import it into other instances to reuse your pricing setup.</span></span>

1. <span data-ttu-id="e622b-107">Изберете **Настройки** > **Решения** и след това изберете **Създаване**.</span><span class="sxs-lookup"><span data-stu-id="e622b-107">Select **Settings** > **Solutions**, and then select **New**.</span></span> 
2. <span data-ttu-id="e622b-108">Наименувайте решението, **Ценови измерения на \<your organization name>**, въведете оставащата изисквана информация и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="e622b-108">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then select **Save**.</span></span>

> ![Създаване на персонализирано решение за ценови измерения](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="e622b-110">Добавяне на всички необходими обекти и свързаните компоненти в решението за ценови измерения</span><span class="sxs-lookup"><span data-stu-id="e622b-110">Add all required entities and related components to the Pricing dimension solution</span></span>
<span data-ttu-id="e622b-111">Ще трябва да добавите следните обекти на Project Service към вашето решение за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="e622b-111">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="e622b-112">Изпълнете стъпките в тази процедура, за да направите някои важни промени на схемата в решението за ценообразуване, така че обектите да разберат новите ценови измерения.</span><span class="sxs-lookup"><span data-stu-id="e622b-112">Complete the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="e622b-113">Изберете **Настройки** > **Решения** и след това щракнете двукратно върху **Ценови измерения на \<your organization name>**.</span><span class="sxs-lookup"><span data-stu-id="e622b-113">Select **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="e622b-114">В мениджъра на решения, в левия навигационен екран, изберете **Добавяне на съществуващи**  >  **Обекти**.</span><span class="sxs-lookup"><span data-stu-id="e622b-114">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="e622b-115">В диалоговия прозорец **Компоненти на решения** изберете следните обекти:</span><span class="sxs-lookup"><span data-stu-id="e622b-115">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="e622b-116">Действителен</span><span class="sxs-lookup"><span data-stu-id="e622b-116">Actual</span></span>
- <span data-ttu-id="e622b-117">Наличен ресурс</span><span class="sxs-lookup"><span data-stu-id="e622b-117">Bookable Resource</span></span>
- <span data-ttu-id="e622b-118">Ред за оценка</span><span class="sxs-lookup"><span data-stu-id="e622b-118">Estimate Line</span></span>
- <span data-ttu-id="e622b-119">Задача от проект</span><span class="sxs-lookup"><span data-stu-id="e622b-119">Project Task</span></span>
- <span data-ttu-id="e622b-120">Подробни данни на ред на фактура</span><span class="sxs-lookup"><span data-stu-id="e622b-120">Invoice Line Detail</span></span>
- <span data-ttu-id="e622b-121">Счетоводен запис</span><span class="sxs-lookup"><span data-stu-id="e622b-121">Journal Line</span></span>
- <span data-ttu-id="e622b-122">Подробни данни за аспекти на договор по проект</span><span class="sxs-lookup"><span data-stu-id="e622b-122">Project Contract Line Detail</span></span>
- <span data-ttu-id="e622b-123">Член на екипа на проект</span><span class="sxs-lookup"><span data-stu-id="e622b-123">Project Team Member</span></span>
- <span data-ttu-id="e622b-124">Подробности за ред на оферта</span><span class="sxs-lookup"><span data-stu-id="e622b-124">Quote Line Detail</span></span>
- <span data-ttu-id="e622b-125">Надценка над цена на роля</span><span class="sxs-lookup"><span data-stu-id="e622b-125">Role Price Markup</span></span>
- <span data-ttu-id="e622b-126">Цена на роля</span><span class="sxs-lookup"><span data-stu-id="e622b-126">Role Price</span></span> 
- <span data-ttu-id="e622b-127">Запис за време</span><span class="sxs-lookup"><span data-stu-id="e622b-127">Time Entry</span></span> 

> ![Добавяне на съществуващи обекти към решението за ценови измерения](media/Existing-entities-to-PD-solution.png)

> ![Избор на компоненти на решението](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="e622b-130">Уверете се, че сте включили всички формуляри и изгледи за всеки от избраните обекти.</span><span class="sxs-lookup"><span data-stu-id="e622b-130">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="e622b-131">Когато бъдете подканени да включите зависими обекти за избраните обекти изберете **Не**.</span><span class="sxs-lookup"><span data-stu-id="e622b-131">When prompted to include any dependent entities for the selected entities, select **No**.</span></span>

> ![Не включвай всички свързани компоненти](media/Do-not-include-required.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]