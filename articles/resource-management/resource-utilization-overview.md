---
title: Общ преглед на използването на ресурси
description: Тази тема предоставя информация за използването на ресурси в Project Operations.
author: ruhercul
manager: Annbe
ms.date: 11/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 8b85464dbb68523b122116225a604f67e7236f3e
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401363"
---
# <a name="resource-utilization-overview"></a><span data-ttu-id="ac6a4-103">Общ преглед на използването на ресурси</span><span class="sxs-lookup"><span data-stu-id="ac6a4-103">Resource utilization overview</span></span>

<span data-ttu-id="ac6a4-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="ac6a4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ac6a4-105">Ресурсите могат да имат целево платимо използване.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-105">Resources can have a target billable utilization.</span></span> <span data-ttu-id="ac6a4-106">Това целево използване се дефинира като атрибут в ролята на ресурс по подразбиране или е зададено в записа на индивидуалния наличен ресурс.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-106">This target utilization is defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="ac6a4-107">Изчисленията на използването се базират на действителните часове, които ресурсите са отчели с помощта на одобрените записи за време.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-107">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="ac6a4-108">За изчисляване на използването се използват следните формули:</span><span class="sxs-lookup"><span data-stu-id="ac6a4-108">The following formulas are used to calculate utilization:</span></span>

  - <span data-ttu-id="ac6a4-109">Платимо използване = Платими действителни часове ÷ капацитет на ресурса</span><span class="sxs-lookup"><span data-stu-id="ac6a4-109">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
  - <span data-ttu-id="ac6a4-110">Неплатимо използване = действителното време с ИД на тип фактуриране = неплатимо, бонусно или неналично ÷ капацитет на ресурса</span><span class="sxs-lookup"><span data-stu-id="ac6a4-110">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
  - <span data-ttu-id="ac6a4-111">Вътрешно = действително време без договор за продажба ÷ капацитет на ресурса</span><span class="sxs-lookup"><span data-stu-id="ac6a4-111">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
  - <span data-ttu-id="ac6a4-112">Капацитет на ресурса = работни часове на ресурса – извън офиса – неработни дни</span><span class="sxs-lookup"><span data-stu-id="ac6a4-112">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="ac6a4-113">Можете да намерите изгледа **Използване на ресурси** в прозореца **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-113">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="ac6a4-114">Всяка клетка в мрежата представлява процента платимо използване на ресурса за даден период, като например ден, седмица или месец.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-114">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="ac6a4-115">За оцветяване на клетките се използват следните формули:</span><span class="sxs-lookup"><span data-stu-id="ac6a4-115">The following formulas are used to color the cells:</span></span>

  - <span data-ttu-id="ac6a4-116">**Зелено**: платимо използване > = целево използване на ресурс</span><span class="sxs-lookup"><span data-stu-id="ac6a4-116">**Green**: Billable utilization >= Resource target utilization</span></span>
  - <span data-ttu-id="ac6a4-117">**Жълто**: целево използване – 20 < = платимо използване < целево използване</span><span class="sxs-lookup"><span data-stu-id="ac6a4-117">**Yellow**: Target utilization – 20 <= Billable utilization < Target utilization</span></span>
  - <span data-ttu-id="ac6a4-118">**Червено**: платимо използване < целево използване – 20</span><span class="sxs-lookup"><span data-stu-id="ac6a4-118">**Red**: Billable utilization < Target utilization – 20</span></span>

<span data-ttu-id="ac6a4-119">Тъй като изгледът **Използване на ресурси** се базира на таблото на графика, можете да използвате възможностите за филтриране на таблото на графика, за да филтрирате резултатите си.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-119">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="ac6a4-120">Мрежата изисква да зададете целево използване за ролята или за отделния ресурс.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-120">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="ac6a4-121">За да направите тази настройка, отидете на **Ресурси** > **Роли на ресурси**.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-121">To do this setup, go to **Resources** > **Resource roles**.</span></span>

<span data-ttu-id="ac6a4-122">Освен това трябва да бъде присвоена роля по подразбиране на всеки наличен ресурс.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-122">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="ac6a4-123">Отидете на **Ресурси** > **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-123">Go to **Resources** > **Resources**.</span></span> <span data-ttu-id="ac6a4-124">В раздела **Project Service** проверете дали е дефинирана роля на ресурс и дали полето **Е по подразбиране** е зададено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-124">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field is set to **Yes**.</span></span> <span data-ttu-id="ac6a4-125">Можете да добавите допълнителни роли, където **Е по подразбиране** = **Не**.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-125">You can add additional roles where **Is Default** = **No**.</span></span> <span data-ttu-id="ac6a4-126">Ролята, където **Е по подразбиране** = **Да** се използва за оценка на използването на ресурса срещу целта за тази роля.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-126">The role where the **Is Default** = **Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="ac6a4-127">В раздела **Project Service** можете също да зададете индивидуално целева използване за ресурса.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-127">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="ac6a4-128">Изчисляване на използването след това използва целевото използване за оценка на целта на ресурса вместо целта на ролята по подразбиране на ресурса.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-128">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="ac6a4-129">Използването се показва само за ресурс само ако този ресурс има одобрено, платимо време през периода, който е показан в мрежата.</span><span class="sxs-lookup"><span data-stu-id="ac6a4-129">Utilization is only shown for a resource if that resource has approved, chargeable time during the period shown in the grid.</span></span>
