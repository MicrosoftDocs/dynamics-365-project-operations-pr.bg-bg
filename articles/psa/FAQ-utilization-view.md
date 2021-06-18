---
title: Преглед на платимото използване на ресурси
description: Тази тема предоставя информация за изгледа на използване на ресурси.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: e1c123854209b3cb5c310e3bbcb242c9219279a8
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5992821"
---
# <a name="view-chargeable-utilization-for-resources"></a><span data-ttu-id="dd6d7-103">Преглед на платимото използване на ресурси</span><span class="sxs-lookup"><span data-stu-id="dd6d7-103">View chargeable utilization for resources</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]
 
<span data-ttu-id="dd6d7-104">**Изгледът за използване** на страницата **Използване на ресурсите на Project Service** показва платимото използване за всеки наличен ресурс.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-104">The **Utilization View** on the **Project Service Resource Utilization** page shows the chargeable utilization for each bookable resource.</span></span> <span data-ttu-id="dd6d7-105">Тъй като изгледът е базиран на таблото на графика, ще намерите много от същите функции.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-105">Because the view is based on the schedule board, you’ll find many of the same functions.</span></span>

> ![Екранна снимка на изгледа за използване](media/FAQ-utilization-1.png)
 

<span data-ttu-id="dd6d7-107">Изчисляването на платимо използване работи, както следва:</span><span class="sxs-lookup"><span data-stu-id="dd6d7-107">The chargeable utilization calculation works as follows:</span></span>

   <span data-ttu-id="dd6d7-108">Платимо използване = (платими действителни часове)/(капацитет на ресурс)</span><span class="sxs-lookup"><span data-stu-id="dd6d7-108">Chargeable utilization = (Chargeable actual hours) / (resource capacity)</span></span>

<span data-ttu-id="dd6d7-109">Клетките представляват изчисленото платимо използване за избрания период (дни, седмици или месеци).</span><span class="sxs-lookup"><span data-stu-id="dd6d7-109">The cells represent the calculated chargeable utilization for the selected period (days, weeks, or months).</span></span>

<span data-ttu-id="dd6d7-110">Цветовете във всяка клетка показват платимото използване за ресурс в сравнение с тяхното целево платимо използване.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-110">The colors in each cell show the chargeable utilization for a resource as compared to their target chargeable utilization.</span></span> 

<span data-ttu-id="dd6d7-111">Целевото използване може да бъде зададено или в ролята на ресурса по подразбиране, или в самия индивидуален ресурс.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-111">The target utilization can be set on the resource’s default role or on the individual resource itself.</span></span> <span data-ttu-id="dd6d7-112">Изчислението първо взема под внимание лицето за целта и след това ролята на ресурс по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-112">The calculation looks at the individual for the target first, and then to the resource’s default role.</span></span>

## <a name="set-target-on-a-resource"></a><span data-ttu-id="dd6d7-113">Задаване на цел за ресурс</span><span class="sxs-lookup"><span data-stu-id="dd6d7-113">Set target on a resource</span></span>

1. <span data-ttu-id="dd6d7-114">Отидете на **Ресурси** \> **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-114">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="dd6d7-115">Изберете ресурс, за да отворите записа.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-115">Select a resource to open the record.</span></span> 
3. <span data-ttu-id="dd6d7-116">В раздела **Project Service** можете да зададете целевото използване на ресурса.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-116">On the **Project Service** tab, you can set the resource’s target utilization.</span></span>

> ![Екранна снимка на използването на раздела „Project Service” за задаване на целево използване](media/FAQ-utilization-2.png)
 
## <a name="set-target-utilization-on-a-role"></a><span data-ttu-id="dd6d7-118">Задаване на целево използване за роля</span><span class="sxs-lookup"><span data-stu-id="dd6d7-118">Set target utilization on a role</span></span>

1. <span data-ttu-id="dd6d7-119">Отидете на **Ресурси** \> **Роли на ресурси**.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-119">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="dd6d7-120">Изберете роля и отворете записа.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-120">Select a role and open the record.</span></span> 
3. <span data-ttu-id="dd6d7-121">Задайте целевото използване за ролята.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-121">Set the target utilization for the role.</span></span>

> ![Екранна снимка на използването на роли на ресурс за задаване на целево използване](media/FAQ-utilization-3.png)
 
## <a name="calculate-chargeable-utilization-for-a-resource"></a><span data-ttu-id="dd6d7-123">Изчисляване на платимото използване на ресурс</span><span class="sxs-lookup"><span data-stu-id="dd6d7-123">Calculate chargeable utilization for a resource</span></span>

<span data-ttu-id="dd6d7-124">За да изчислите платимото използване за даден ресурс, трябва да изпълните някои предварителни условия.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-124">To calculate chargeable utilization for a resource, you will need to complete some pre-requisites.</span></span> 

### <a name="set-default-role-for-individual-resource"></a><span data-ttu-id="dd6d7-125">Задаване на роля по подразбиране за индивидуален ресурс</span><span class="sxs-lookup"><span data-stu-id="dd6d7-125">Set default role for individual resource</span></span>

<span data-ttu-id="dd6d7-126">Първо, целевото използване трябва да бъде зададено или за индивидуален ресурс, или за роли на ресурс.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-126">First, the target utilization must be set on either the individual resource or on resource roles.</span></span> <span data-ttu-id="dd6d7-127">Ако използвате роли на ресурс за цели, всеки индивидуален ресурс трябва да има роля по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-127">If you are using resource roles for targets, each individual resource must have a default role.</span></span> 

1. <span data-ttu-id="dd6d7-128">За целта отидете на **Ресурси** \> **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-128">To set this, go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="dd6d7-129">Изберете ресурс, отворете записа, след което изберете раздела **Project Service**.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-129">Select a resource, open the record, and then select the **Project Service** tab.</span></span> 
3. <span data-ttu-id="dd6d7-130">В мрежата **Роля на ресурса** се уверете, че има една роля за ресурса и **По подразбиране** е зададено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-130">In the **Resource Role** grid, make sure there’s one role for the resource and **Is Default** is set to **Yes**.</span></span>
 
### <a name="change-billing-type-for-resource-role"></a><span data-ttu-id="dd6d7-131">Промяна на типа фактуриране за ролята на ресурс</span><span class="sxs-lookup"><span data-stu-id="dd6d7-131">Change billing type for resource role</span></span>

<span data-ttu-id="dd6d7-132">Ролите на ресурс трябва да бъдат зададени да имат тип фактуриране **Платими**.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-132">The resource roles must be set to have a billing type of **Chargeable**.</span></span> 

1. <span data-ttu-id="dd6d7-133">Отидете на **Ресурси** \> **Роли на ресурси**.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-133">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="dd6d7-134">Отворете записа, който искате да актуализирате, и след това задайте типа фактуриране по подразбиране на **Платимо**.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-134">Open the record you want to update, and then set the billing type default to **Chargeable**.</span></span>

### <a name="set-working-hours-for-resource-role"></a><span data-ttu-id="dd6d7-135">Задаване на работни часове за роля на ресурс</span><span class="sxs-lookup"><span data-stu-id="dd6d7-135">Set working hours for resource role</span></span>
 
<span data-ttu-id="dd6d7-136">Ресурсът трябва да има работни часове за изчисляването на капацитет.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-136">The resource must have working hours for the capacity calculation.</span></span> 

1. <span data-ttu-id="dd6d7-137">Отидете на **Ресурси** \> **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-137">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="dd6d7-138">Изберете ресурс, за да отворите запис и след това изберете **Показване на работни часове**.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-138">Select a resource to open the record, and then select **Show Work Hours**.</span></span> 
3. <span data-ttu-id="dd6d7-139">Можете да актуализирате групово списъка с ресурси, като приложите **Шаблон за работни часове** от изгледа **Списък с ресурси**.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-139">You can bulk-update the list of resources by applying a **Work Hour Template** from the **Resource List** view.</span></span>

## <a name="troubleshooting-chargeable-actual-hours"></a><span data-ttu-id="dd6d7-140">Отстраняване на проблеми с платими действителни часове</span><span class="sxs-lookup"><span data-stu-id="dd6d7-140">Troubleshooting chargeable actual hours</span></span>

<span data-ttu-id="dd6d7-141">Платимите действителни часове се получават от обекта **Действителни данни**.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-141">The chargeable actual hours are sourced from the **Actuals** entity.</span></span> <span data-ttu-id="dd6d7-142">Действителните данни с тип фактуриране **Платимо** са включени в изчислението и по тази причина трябва да имате проекти, където действителните данни са платими.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-142">Actuals with a billing type of **Chargeable** are included in the calculation and, for this reason, you must have projects where the actuals that are chargeable.</span></span>

<span data-ttu-id="dd6d7-143">Ако не виждате платимо използване, ето някои неща, които можете да проверите:</span><span class="sxs-lookup"><span data-stu-id="dd6d7-143">If you are not seeing chargeable utilization, here are some things you can check:</span></span>

- <span data-ttu-id="dd6d7-144">Ресурсът има работни часове, определени за производителност.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-144">The resource has working hours defined for capacity.</span></span>
- <span data-ttu-id="dd6d7-145">Ресурсът има или индивидуално определена цел на използване, или има присвоена роля по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-145">The resource has either an individually defined utilization target or has a default role assigned to it.</span></span> <span data-ttu-id="dd6d7-146">Ролята има определена за нея цел за използване.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-146">The role has a utilization target defined for it.</span></span>
- <span data-ttu-id="dd6d7-147">Действителните данни имат тип фактуриране **Платимо** за периода, за който очаквате изчисляване на използването.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-147">Actuals have a billing type of **Chargeable** for the period you are expecting a utilization calculation for.</span></span> <span data-ttu-id="dd6d7-148">Проверете следното, ако виждате действителни данни с типове фактуриране, различни от „Платимо“:</span><span class="sxs-lookup"><span data-stu-id="dd6d7-148">Check the following if you are seeing actuals with billing types other than chargeable:</span></span>

  - <span data-ttu-id="dd6d7-149">Ролята, използвана за действителните данни, има тип на фактуриране по подразбиране, различен от „Платимо”.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-149">The role used on the actual has a default billing type of something other than chargeable.</span></span>
  - <span data-ttu-id="dd6d7-150">Ролята в реда на договор на проекта, резервна за проекта, е зададена на неплатима.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-150">The role on the project contract line backing the project has been set to non-chargeable.</span></span>
  - <span data-ttu-id="dd6d7-151">Проектът няма свързан ред на договор.</span><span class="sxs-lookup"><span data-stu-id="dd6d7-151">The project does not have an associated contract line.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]