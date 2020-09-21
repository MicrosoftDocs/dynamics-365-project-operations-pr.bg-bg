---
title: Предлагане на ресурси за проекти
description: Тази тема предоставя информация за това как да предлагате ресурси за проекти.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: bdb0dcb2-4421-4ee1-b97d-89a8cdefbd8d
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 3a7f7c15c3c7a3c39f2b7b9eeb88b9cf0cfdc220
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749363"
---
# <a name="propose-project-resources"></a><span data-ttu-id="2b60a-103">Предлагане на ресурси за проекти</span><span class="sxs-lookup"><span data-stu-id="2b60a-103">Propose project resources</span></span>

<span data-ttu-id="2b60a-104">Мениджърите на ресурси могат да предлагат ресурс на мениджъра на проекта с помощта на заявка за ресурс.</span><span class="sxs-lookup"><span data-stu-id="2b60a-104">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="2b60a-105">От мрежата за заявки или от самата заявка изберете **Търсене на ресурси**.</span><span class="sxs-lookup"><span data-stu-id="2b60a-105">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="2b60a-106">На страницата **Асистент за планиране** изберете ресурса и след това в прозореца **Създаване на резервация на ресурс** в полето **Състояние на резервация** изберете **Резервиране**.</span><span class="sxs-lookup"><span data-stu-id="2b60a-106">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

    ![Предложеният ресурс е избран](media/Resource-Management-image62.png)

<span data-ttu-id="2b60a-108">Получават се следните актуализации на състоянието:</span><span class="sxs-lookup"><span data-stu-id="2b60a-108">The following status updates occur:</span></span>

- <span data-ttu-id="2b60a-109">На страницата **Асистент за планиране** индикаторите на състоянието се актуализират, за да покажат, че резервацията е предложена, а не е потвърдена.</span><span class="sxs-lookup"><span data-stu-id="2b60a-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>

    ![Индикатори на състоянието за предложена резервация на страницата „Асистент за планиране“](media/Resource-Management-image63.png)

- <span data-ttu-id="2b60a-111">В заявката за ресурс състоянието се променя на **Нуждае се от преглед**.</span><span class="sxs-lookup"><span data-stu-id="2b60a-111">On the resource request, the status is changed to **Needs Review**.</span></span>

    ![Състоянието на заявката за ресурс се променя на „Нуждае се от преглед“](media/Resource-Management-image64.png)

- <span data-ttu-id="2b60a-113">В раздела **Екип** на проекта стойността на състоянието на общия член на екипа **Състояние на заявка** се променя на **Нуждае се от преглед**.</span><span class="sxs-lookup"><span data-stu-id="2b60a-113">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

    ![Състояние на заявката за общ член на екипа е променено на „Нуждае се от преглед“ в раздела „Екип“](media/Resource-Management-image48.png)

<span data-ttu-id="2b60a-115">Мениджърът на проекта може да приеме или да отхвърли предложението.</span><span class="sxs-lookup"><span data-stu-id="2b60a-115">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="2b60a-116">Когато мениджърите на ресурси обработват заявки за ресурси, те могат да използват някой от следните подходи:</span><span class="sxs-lookup"><span data-stu-id="2b60a-116">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="2b60a-117">Предлагане на множество ресурси за удовлетворяване на търсенето, ако не е налице един ресурс за изпълнение на изискваните часове.</span><span class="sxs-lookup"><span data-stu-id="2b60a-117">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="2b60a-118">Предложените часове след това се поделят между множество ресурси, които могат да удовлетворят необходимите часове.</span><span class="sxs-lookup"><span data-stu-id="2b60a-118">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="2b60a-119">В този сценарий часовете не могат да се припокриват.</span><span class="sxs-lookup"><span data-stu-id="2b60a-119">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="2b60a-120">Предлагане на по-малко ресурси, отколкото са необходими.</span><span class="sxs-lookup"><span data-stu-id="2b60a-120">Propose fewer resources than are required.</span></span> <span data-ttu-id="2b60a-121">В този сценарий капацитетът на предложения ресурс е по-малък от необходимите часове, които е посочил заявителят.</span><span class="sxs-lookup"><span data-stu-id="2b60a-121">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="2b60a-122">Ето защо, когато заявителят приема предложените ресурси, се създава неизпълнено изискване за ресурси, за да се регистрира оставащото търсене.</span><span class="sxs-lookup"><span data-stu-id="2b60a-122">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="2b60a-123">Резервиране на множество ресурси за удовлетворяване на търсенето, ако не е налице един ресурс за изпълнение на работата.</span><span class="sxs-lookup"><span data-stu-id="2b60a-123">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="2b60a-124">Резервиране на по-малко ресурси, отколкото са необходими.</span><span class="sxs-lookup"><span data-stu-id="2b60a-124">Book fewer resources than are required.</span></span> <span data-ttu-id="2b60a-125">В този сценарий резервираните часове са по-малко от необходимите.</span><span class="sxs-lookup"><span data-stu-id="2b60a-125">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="2b60a-126">Системата ви напътства да предлагате ресурси вместо резервации, така че запитващият може да проверява и да проследява оставащото търсене.</span><span class="sxs-lookup"><span data-stu-id="2b60a-126">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="billable-utilization"></a><span data-ttu-id="2b60a-127">Платимо използване</span><span class="sxs-lookup"><span data-stu-id="2b60a-127">Billable utilization</span></span>

<span data-ttu-id="2b60a-128">Ресурсите могат да имат целево платимо използване.</span><span class="sxs-lookup"><span data-stu-id="2b60a-128">Resources can have a target billable utilization.</span></span> <span data-ttu-id="2b60a-129">Това целево използване се дефинира като атрибут в ролята на ресурс по подразбиране или е зададено в записа на индивидуалния наличен ресурс.</span><span class="sxs-lookup"><span data-stu-id="2b60a-129">This target utilization is either defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="2b60a-130">Изчисленията на използването се базират на действителните часове, които ресурсите са отчели с помощта на одобрените записи за време.</span><span class="sxs-lookup"><span data-stu-id="2b60a-130">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="2b60a-131">За изчисляване на използването се използват следните формули:</span><span class="sxs-lookup"><span data-stu-id="2b60a-131">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="2b60a-132">Платимо използване = Платими действителни часове ÷ капацитет на ресурса</span><span class="sxs-lookup"><span data-stu-id="2b60a-132">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="2b60a-133">Неплатимо използване = действителното време с ИД на тип фактуриране = неплатимо, бонусно или неналично ÷ капацитет на ресурса</span><span class="sxs-lookup"><span data-stu-id="2b60a-133">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="2b60a-134">Вътрешно = действително време без договор за продажба ÷ капацитет на ресурса</span><span class="sxs-lookup"><span data-stu-id="2b60a-134">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="2b60a-135">Капацитет на ресурса = работни часове на ресурса – извън офиса – неработни дни</span><span class="sxs-lookup"><span data-stu-id="2b60a-135">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="2b60a-136">Можете да намерите изгледа **Използване на ресурси** в прозореца **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="2b60a-136">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

![Изглед „Използване на ресурси“](media/Resource-Management-image65.png)

<span data-ttu-id="2b60a-138">Всяка клетка в мрежата представлява процента платимо използване на ресурса за даден период, като например ден, седмица или месец.</span><span class="sxs-lookup"><span data-stu-id="2b60a-138">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="2b60a-139">За оцветяване на клетките се използват следните формули:</span><span class="sxs-lookup"><span data-stu-id="2b60a-139">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="2b60a-140">**Зелено:** платимо използване \>= целево използване на ресурс</span><span class="sxs-lookup"><span data-stu-id="2b60a-140">**Green:** Billable utilization \>= Resource target utilization</span></span>
- <span data-ttu-id="2b60a-141">**Жълто:** целево използване – 20 \<= платимо използване \< целево използване</span><span class="sxs-lookup"><span data-stu-id="2b60a-141">**Yellow:** Target utilization – 20 \<= Billable utilization \< Target utilization</span></span>
- <span data-ttu-id="2b60a-142">**Червено:** платимо използване \< целево използване – 20</span><span class="sxs-lookup"><span data-stu-id="2b60a-142">**Red:** Billable utilization \< Target utilization – 20</span></span>

<span data-ttu-id="2b60a-143">Тъй като изгледът **Използване на ресурси** се базира на таблото на графика, можете да използвате възможностите за филтриране на таблото на графика, за да филтрирате резултатите си.</span><span class="sxs-lookup"><span data-stu-id="2b60a-143">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="2b60a-144">Мрежата изисква да зададете целево използване за ролята или за отделния ресурс.</span><span class="sxs-lookup"><span data-stu-id="2b60a-144">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="2b60a-145">За да направите тази настройка, отидете на **Ресурси** \> **Роли на ресурси**.</span><span class="sxs-lookup"><span data-stu-id="2b60a-145">To do this setup, go to **Resources** \> **Resource roles**.</span></span>

<span data-ttu-id="2b60a-146">Освен това трябва да бъде присвоена роля по подразбиране на всеки наличен ресурс.</span><span class="sxs-lookup"><span data-stu-id="2b60a-146">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="2b60a-147">Отидете на **Ресурси** \> **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="2b60a-147">Go to **Resources** \> **Resources**.</span></span> <span data-ttu-id="2b60a-148">В раздела **Project Service** проверете дали е дефинирана роля на ресурс и дали полето **Е по подразбиране** за нея е зададено на **Да**.</span><span class="sxs-lookup"><span data-stu-id="2b60a-148">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field for it is set to **Yes**.</span></span> <span data-ttu-id="2b60a-149">Можете да добавите допълнителни роли, където **Е по подразбиране = Не**.</span><span class="sxs-lookup"><span data-stu-id="2b60a-149">You can add additional roles where **Is Default = No**.</span></span> <span data-ttu-id="2b60a-150">Ролята, където **Е по подразбиране = Да** се използва за оценка на използването на ресурса срещу целта за тази роля.</span><span class="sxs-lookup"><span data-stu-id="2b60a-150">The role where the **Is Default = Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

![Зададена роля по подразбиране](media/Resource-Management-image67.png)

<span data-ttu-id="2b60a-152">В раздела **Project Service** можете също да зададете индивидуално целева използване за ресурса.</span><span class="sxs-lookup"><span data-stu-id="2b60a-152">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="2b60a-153">Изчисляване на използването след това използва целевото използване за оценка на целта на ресурса вместо целта на ролята по подразбиране на ресурса.</span><span class="sxs-lookup"><span data-stu-id="2b60a-153">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="2b60a-154">Използването се показва за ресурс само ако този ресурс има одобрено, платимо време през периода, който е показан в мрежата.</span><span class="sxs-lookup"><span data-stu-id="2b60a-154">Utilization is shown for a resource only if that resource has approved, chargeable time during the period that is shown in the grid.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="2b60a-155">Наличност на ресурс</span><span class="sxs-lookup"><span data-stu-id="2b60a-155">Resource availability</span></span>

<span data-ttu-id="2b60a-156">Важно е мениджърите на ресурси да могат да преглеждат наличността на ресурси и да актуализират резервациите.</span><span class="sxs-lookup"><span data-stu-id="2b60a-156">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="2b60a-157">В някои случаи няма официално търсене (заявка за ресурс), но мениджърът на ресурси трябва да отговаря на непланирано търсене, което идва чрез канали, като например имейл, телефонен разговор или незабавно съобщение.</span><span class="sxs-lookup"><span data-stu-id="2b60a-157">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="2b60a-158">Мениджърите на ресурси използват таблото на графика, за да актуализират ресурсите и резервациите.</span><span class="sxs-lookup"><span data-stu-id="2b60a-158">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="2b60a-159">Работните часове на ресурса се използват като основа за изчисляване на наличността на ресурс.</span><span class="sxs-lookup"><span data-stu-id="2b60a-159">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="2b60a-160">Резервациите на ресурси консумират капацитета на ресурсите.</span><span class="sxs-lookup"><span data-stu-id="2b60a-160">Resource bookings consume the capacity of the resources.</span></span>

![Табло на графика](media/Resource-Management-image68.png)

<span data-ttu-id="2b60a-162">Таблото на графика използва цветове и оцветяване, за да показва резервации, наличност и надхвърлено количество резервации, както и състоянието на резервациите.</span><span class="sxs-lookup"><span data-stu-id="2b60a-162">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="2b60a-163">Настройка в настройките на таблото на графика ви позволява да показвате легенда.</span><span class="sxs-lookup"><span data-stu-id="2b60a-163">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="2b60a-164">Ако до отделен наличен ресурс на таблото за планиране се появи стрелка надясно, ресурсът може да бъде разгънат, за да покаже подробности за работата, за която е резервиран ресурсът.</span><span class="sxs-lookup"><span data-stu-id="2b60a-164">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

![Разгънат наличен ресурс в таблото на графика](media/Resource-Management-image69.png)

<span data-ttu-id="2b60a-166">Тъй като Dynamics 365 Project Service Automation използва системата Universal Resource Scheduling, ако сте инсталирали също и Dynamics 365 Field Service, можете да прегледате подробностите за резервации на ресурси за проекти, работни поръчки и всички други обекти, към които сте разширили планирането.</span><span class="sxs-lookup"><span data-stu-id="2b60a-166">Because Dynamics 365 Project Service Automation uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

![Подробности за резервации на ресурси за проекти и работни поръчки](media/Resource-Management-image70.png)

<span data-ttu-id="2b60a-168">За да видите повече подробности за отделния ресурс, щракнете с десния бутон върху него, за да отворите картата на ресурса.</span><span class="sxs-lookup"><span data-stu-id="2b60a-168">To view more details about an individual resource, right-click it to open the resource card.</span></span>

![Карта на ресурс](media/Resource-Management-image71.png)
