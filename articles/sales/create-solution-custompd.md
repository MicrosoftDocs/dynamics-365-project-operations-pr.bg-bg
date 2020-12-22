---
title: Създаване на решение за персонализирани измерения на ценообразуване
description: Тази тема предоставя информация за начина на създаване на решения за персонализирани ценови измерения.
author: Rumant
manager: tfehr
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 441501dff23d16960381b3f9fb4b2cceba2b3ba5
ms.sourcegitcommit: 869bde007805ef255f61b03937e4a44aeef61df9
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/12/2020
ms.locfileid: "4513959"
---
# <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="8d093-103">Създаване на решение за персонализирани измерения на ценообразуване</span><span class="sxs-lookup"><span data-stu-id="8d093-103">Create a solution for custom pricing dimensions</span></span>

 <span data-ttu-id="8d093-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="8d093-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span> 

>[!IMPORTANT]
><span data-ttu-id="8d093-105">Всички промени в размера на персонализираните цени трябва да бъдат в отделно решение.</span><span class="sxs-lookup"><span data-stu-id="8d093-105">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="8d093-106">Тази важна най-добра практика позволява гъвкавост за актуализиране или премахване на промени, ако е необходимо, помага за повторното използване на вашата работа и улеснява пренасянето на тези промени на други екземпляри.</span><span class="sxs-lookup"><span data-stu-id="8d093-106">This important best practice allows the flexibility to update or remove changes as needed, helps with re-use of your work, and makes it easier to port changes to other instances.</span></span> <span data-ttu-id="8d093-107">След като направите всички необходими промени, експортирайте това решение като **Завършено решение** и след това го импортирайте в други екземпляри за повторно използване.</span><span class="sxs-lookup"><span data-stu-id="8d093-107">After you make the required changes, export this solution as a **Managed** solution, and then import into other instances for reuse.</span></span>

## <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="8d093-108">Създаване на решение за персонализирани измерения на ценообразуване</span><span class="sxs-lookup"><span data-stu-id="8d093-108">Create a solution for custom pricing dimensions</span></span>

1.  <span data-ttu-id="8d093-109">Изберете **Настройки** > **Решения** и след това изберете **Създаване**.</span><span class="sxs-lookup"><span data-stu-id="8d093-109">Select **Settings** > **Solutions**, and then select **New**.</span></span>
2.  <span data-ttu-id="8d093-110">Задайте име на решението, *<your organization name> измерения за ценообразуване*.</span><span class="sxs-lookup"><span data-stu-id="8d093-110">Name the solution, *<your organization name> pricing dimensions*.</span></span>
3. <span data-ttu-id="8d093-111">Въведете останалата необходима информация и след това изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="8d093-111">Enter the remaining required information, and then select **Save**.</span></span>

  ![Създаване на решение за персонализирано измерение на ценообразуване](./media/Creation-of-custom-pricing-dimension-solution.png)
 
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="8d093-113">Добавяне на всички необходими обекти и свързаните компоненти в решението за ценови измерения</span><span class="sxs-lookup"><span data-stu-id="8d093-113">Add all required entities and related components to the Pricing dimension solution</span></span>

<span data-ttu-id="8d093-114">Добавете следните обекти на Project Service към решението за ценообразуване, за да направите важни промени в схемата в решението за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="8d093-114">Add the following Project Service entities to your pricing solution to make important schema changes in the pricing solution.</span></span> <span data-ttu-id="8d093-115">След като изпълните тази процедура, обектите ще разпознаят новите измерения на ценообразуването.</span><span class="sxs-lookup"><span data-stu-id="8d093-115">After you have completed this procedure, the entities will recognize the new pricing dimensions.</span></span>

1.  <span data-ttu-id="8d093-116">Изберете **Настройки** > **Решения** и след това щракнете двукратно върху **<*име на организацията*> измерения на ценообразуване**.</span><span class="sxs-lookup"><span data-stu-id="8d093-116">Select **Settings** > **Solutions**, and then double-click **<*your organization name*> pricing dimensions**.</span></span>
2.  <span data-ttu-id="8d093-117">В мениджъра на решения, в левия навигационен екран, изберете **Добавяне на съществуващи**  >  **Обекти**.</span><span class="sxs-lookup"><span data-stu-id="8d093-117">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3.  <span data-ttu-id="8d093-118">В диалоговия прозорец **Компоненти на решения** изберете следните обекти:</span><span class="sxs-lookup"><span data-stu-id="8d093-118">In the **Solution Components** dialog box, select the following entities:</span></span>
 
   - <span data-ttu-id="8d093-119">**Действителен**</span><span class="sxs-lookup"><span data-stu-id="8d093-119">**Actual**</span></span>
   - <span data-ttu-id="8d093-120">**Наличен ресурс**</span><span class="sxs-lookup"><span data-stu-id="8d093-120">**Bookable Resource**</span></span>
   - <span data-ttu-id="8d093-121">**Ред за оценка**</span><span class="sxs-lookup"><span data-stu-id="8d093-121">**Estimate Line**</span></span>
   - <span data-ttu-id="8d093-122">**Задача от проект**</span><span class="sxs-lookup"><span data-stu-id="8d093-122">**Project Task**</span></span>
   - <span data-ttu-id="8d093-123">**Подробни данни на ред на фактура**</span><span class="sxs-lookup"><span data-stu-id="8d093-123">**Invoice Line Detail**</span></span>
   - <span data-ttu-id="8d093-124">**Счетоводен запис**</span><span class="sxs-lookup"><span data-stu-id="8d093-124">**Journal Line**</span></span>
   - <span data-ttu-id="8d093-125">**Подробни данни за аспекти на договор по проект**</span><span class="sxs-lookup"><span data-stu-id="8d093-125">**Project Contract Line Detail**</span></span>
   - <span data-ttu-id="8d093-126">**Член на екипа на проект**</span><span class="sxs-lookup"><span data-stu-id="8d093-126">**Project Team Member**</span></span>
   - <span data-ttu-id="8d093-127">**Подробности за ред на оферта**</span><span class="sxs-lookup"><span data-stu-id="8d093-127">**Quote Line Detail**</span></span>
   - <span data-ttu-id="8d093-128">**Надценка над цена на роля**</span><span class="sxs-lookup"><span data-stu-id="8d093-128">**Role Price Markup**</span></span>
   - <span data-ttu-id="8d093-129">**Цена на роля**</span><span class="sxs-lookup"><span data-stu-id="8d093-129">**Role Price**</span></span>
   - <span data-ttu-id="8d093-130">**Запис за време**</span><span class="sxs-lookup"><span data-stu-id="8d093-130">**Time Entry**</span></span>
 
   ![Добавяне на решение за персонализирано измерение на ценообразуване за съществуващи обекти](./media/Existing-entities-to-PD-solution.png)
 
 4. <span data-ttu-id="8d093-132">За всеки обект прегледайте добавените компоненти и окончателния списък на активите на обекта за всеки обект.</span><span class="sxs-lookup"><span data-stu-id="8d093-132">For each entity, review the components being added and the final list of entity assets for each entity.</span></span> 

   >[!NOTE]
   > <span data-ttu-id="8d093-133">Включете всички формуляри и изгледи за всеки от избраните обекти.</span><span class="sxs-lookup"><span data-stu-id="8d093-133">Include all forms and views for each of the selected entities.</span></span>

  ![Добавени обекти](./media/solution-component-selection.png)


5.  <span data-ttu-id="8d093-135">Когато бъдете подканени да включите зависими обекти за избраните обекти, изберете **Не, не включвай задължителни компоненти.**</span><span class="sxs-lookup"><span data-stu-id="8d093-135">When prompted to include any dependent entities for the selected entities, select **No, do not include required components.**</span></span>

    ![Включване на зависими обекти](./media/Do-not-include-required.png)
