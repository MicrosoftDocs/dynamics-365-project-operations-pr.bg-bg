---
title: Преглед на предложени ресурси
description: Тази тема предоставя информация за това как да предлагате ресурси за проекти.
author: ruhercul
manager: AnnBe
ms.date: 11/05/2020
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
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: fa0515b9d6a0023c05c37d2bcfa6a403f48927cb
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279260"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="6c3ac-103">Преглед на предложени ресурси</span><span class="sxs-lookup"><span data-stu-id="6c3ac-103">Review proposed resources</span></span>

<span data-ttu-id="6c3ac-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="6c3ac-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="6c3ac-105">Мениджърите на ресурси могат да предлагат ресурс на мениджъра на проекта с помощта на заявка за ресурс.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="6c3ac-106">От мрежата за заявки или от самата заявка изберете **Търсене на ресурси**.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="6c3ac-107">На страницата **Асистент за планиране** изберете ресурса и след това в прозореца **Създаване на резервация на ресурс** в полето **Състояние на резервация** изберете **Резервиране**.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="6c3ac-108">Получават се следните актуализации на състоянието:</span><span class="sxs-lookup"><span data-stu-id="6c3ac-108">The following status updates occur:</span></span>

- <span data-ttu-id="6c3ac-109">На страницата **Асистент за планиране** индикаторите на състоянието се актуализират, за да покажат, че резервацията е предложена, а не е потвърдена.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="6c3ac-110">В заявката за ресурс състоянието се променя на **Нуждае се от преглед**.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="6c3ac-111">В раздела **Екип** на проекта стойността на състоянието на общия член на екипа **Състояние на заявка** се променя на **Нуждае се от преглед**.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="6c3ac-112">Мениджърът на проекта може да приеме или да отхвърли предложението.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="6c3ac-113">Когато мениджърите на ресурси обработват заявки за ресурси, те могат да използват някой от следните подходи:</span><span class="sxs-lookup"><span data-stu-id="6c3ac-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="6c3ac-114">Предлагане на множество ресурси за удовлетворяване на търсенето, ако не е налице един ресурс за изпълнение на изискваните часове.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="6c3ac-115">Предложените часове след това се поделят между множество ресурси, които могат да удовлетворят необходимите часове.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="6c3ac-116">В този сценарий часовете не могат да се припокриват.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="6c3ac-117">Предлагане на по-малко ресурси, отколкото са необходими.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="6c3ac-118">В този сценарий капацитетът на предложения ресурс е по-малък от необходимите часове, които е посочил заявителят.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="6c3ac-119">Ето защо, когато заявителят приема предложените ресурси, се създава неизпълнено изискване за ресурси, за да се регистрира оставащото търсене.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="6c3ac-120">Резервиране на множество ресурси за удовлетворяване на търсенето, ако не е налице един ресурс за изпълнение на работата.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="6c3ac-121">Резервиране на по-малко ресурси, отколкото са необходими.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-121">Book fewer resources than are required.</span></span> <span data-ttu-id="6c3ac-122">В този сценарий резервираните часове са по-малко от необходимите.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="6c3ac-123">Системата ви напътства да предлагате ресурси вместо резервации, така че запитващият може да проверява и да проследява оставащото търсене.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="6c3ac-124">Наличност на ресурс</span><span class="sxs-lookup"><span data-stu-id="6c3ac-124">Resource availability</span></span>

<span data-ttu-id="6c3ac-125">Важно е мениджърите на ресурси да могат да преглеждат наличността на ресурси и да актуализират резервациите.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-125">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="6c3ac-126">В някои случаи няма официално търсене (заявка за ресурс), но мениджърът на ресурси трябва да отговаря на непланирано търсене, което идва чрез канали, като например имейл, телефонен разговор или незабавно съобщение.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-126">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="6c3ac-127">Мениджърите на ресурси използват таблото на графика, за да актуализират ресурсите и резервациите.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-127">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="6c3ac-128">Работните часове на ресурса се използват като основа за изчисляване на наличността на ресурс.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-128">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="6c3ac-129">Резервациите на ресурси консумират капацитета на ресурсите.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-129">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="6c3ac-130">Таблото на графика използва цветове и оцветяване, за да показва резервации, наличност и надхвърлено количество резервации, както и състоянието на резервациите.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-130">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="6c3ac-131">Настройка в настройките на таблото на графика ви позволява да показвате легенда.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-131">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="6c3ac-132">Ако до отделен наличен ресурс на таблото за планиране се появи стрелка надясно, ресурсът може да бъде разгънат, за да покаже подробности за работата, за която е резервиран ресурсът.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-132">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="6c3ac-133">Тъй като Dynamics 365 Project Operations използва системата Universal Resource Scheduling, ако сте инсталирали също и Dynamics 365 Field Service, можете да прегледате подробностите за резервации на ресурси за проекти, работни поръчки и всички други обекти, към които сте разширили планирането.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-133">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="6c3ac-134">За да видите повече подробности за отделния ресурс, щракнете с десния бутон върху него, за да отворите картата на ресурса.</span><span class="sxs-lookup"><span data-stu-id="6c3ac-134">To view more details about an individual resource, right-click it to open the resource card.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]