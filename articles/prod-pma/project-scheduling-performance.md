---
title: Производителност на планиране на ресурс за проект
description: Тази тема предоставя информация за това как да подобрите ефективността на планирането на ресурси за голям брой проекти.
author: Yowelle
ms.date: 08/31/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.14
ms.search.validFrom: 2020-09-01
ms.openlocfilehash: 113023909f88cb4dd498190ef21b6955482b25dd
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010008"
---
# <a name="project-resource-scheduling-performance"></a><span data-ttu-id="12dc1-103">Производителност на планиране на ресурс за проект</span><span class="sxs-lookup"><span data-stu-id="12dc1-103">Project resource scheduling performance</span></span>

[!include [banner](../includes/banner.md)]
[!include [banner](../includes/preview-banner.md)]


<span data-ttu-id="12dc1-104">Проблеми с производителността, свързани с планирането на ресурси, могат да възникнат, когато броят на проектите достигне хиляди.</span><span class="sxs-lookup"><span data-stu-id="12dc1-104">Performance issues related to resource scheduling can occur when the number of projects reaches into the thousands.</span></span> <span data-ttu-id="12dc1-105">За да се подобри ефективността на планирането на ресурси, е налична функция, която позволява на потребителите да намалят времето, необходимо за стартиране на формуляра за наличност на ресурси.</span><span class="sxs-lookup"><span data-stu-id="12dc1-105">To improve resource scheduling performance, a feature is available that allows users to reduce the time that it takes to launch the resource availability form.</span></span> <span data-ttu-id="12dc1-106">По-конкретно, това премахва процеса на синхронизиране на ресурсния капацитет и използва таблицата **ResProjectResource** за ускоряване на търсенето на ресурси.</span><span class="sxs-lookup"><span data-stu-id="12dc1-106">Specifically, this removes the resource capacity roll-up synchronization process and uses the **ResProjectResource** table to speed up the resource lookup.</span></span> <span data-ttu-id="12dc1-107">Обърнете внимание, че **ResRollup** таблицата вече няма да се използва.</span><span class="sxs-lookup"><span data-stu-id="12dc1-107">Note that the **ResRollup** table will no longer be used.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="12dc1-108">Ако има зависимост или от процеса на синхронизиране на капацитета на ресурса, или от таблицата **ResProjectResource**, не използвайте тази функция.</span><span class="sxs-lookup"><span data-stu-id="12dc1-108">If there is a dependency on either the resource capacity roll-up synchronization process or the **ResProjectResource** table, do not use this feature.</span></span>

## <a name="enable-resource-scheduling-performance-enhancement"></a><span data-ttu-id="12dc1-109">Активирайте подобряване на производителността при планиране на ресурси</span><span class="sxs-lookup"><span data-stu-id="12dc1-109">Enable resource scheduling performance enhancement</span></span>
<span data-ttu-id="12dc1-110">За да активирате подобряване на производителността на график на ресурси, изпълнете следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="12dc1-110">To enable resource scheduling performance enhancement, complete the following steps.</span></span>

1. <span data-ttu-id="12dc1-111">Отидете на **Управление на функции** > **всичко** и в списъка с функции намерете **Активирайте функцията за подобряване на производителността за планиране на ресурсите на проекта**.</span><span class="sxs-lookup"><span data-stu-id="12dc1-111">Go to **Feature management** > **All**, and in the feature list, locate **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="12dc1-112">Изберете **Разрешаване сега**.</span><span class="sxs-lookup"><span data-stu-id="12dc1-112">Select **Enable now**.</span></span>

> [!NOTE]
> <span data-ttu-id="12dc1-113">Ако не можете да намерите функцията в списъка, изберете **Провери за актуализации**, за да опресните списъка.</span><span class="sxs-lookup"><span data-stu-id="12dc1-113">If you can't find the feature in the list, select **Check for updates** to refresh the list.</span></span>

3. <span data-ttu-id="12dc1-114">Опреснете браузъра си и след това отидете на **Управление на проекти и счетоводство** > **Периодични** > **Ресурси по проекта** > **Синхронизирайте капацитета на календарите на ресурсите във всички компании**.</span><span class="sxs-lookup"><span data-stu-id="12dc1-114">Refresh your browser, and then go to **Project management and accounting** > **Periodic** > **Project resources** > **Synchronize resource calendars capacity across all companies**.</span></span>
4. <span data-ttu-id="12dc1-115">Задайте **Премахнете съществуващите записи за капацитет** на **Да**, за да премахнете предишни данни.</span><span class="sxs-lookup"><span data-stu-id="12dc1-115">Set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="12dc1-116">Ако искате да генерирате допълнителни данни, задайте го на **Не**.</span><span class="sxs-lookup"><span data-stu-id="12dc1-116">If you want generate incremental data, set it to **No**.</span></span>
5. <span data-ttu-id="12dc1-117">В полето **Код на периода** изберете периода, в който трябва да се генерират данни.</span><span class="sxs-lookup"><span data-stu-id="12dc1-117">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="12dc1-118">Ако изберете код на период, не е необходимо да се определят начална и крайна дата.</span><span class="sxs-lookup"><span data-stu-id="12dc1-118">If you select a period code, a start and end date do not need to be defined.</span></span>
6. <span data-ttu-id="12dc1-119">Ако оставите полето **Код на периода** празно, изберете конкретни начална и крайна дата, за да генерирате данни.</span><span class="sxs-lookup"><span data-stu-id="12dc1-119">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
7. <span data-ttu-id="12dc1-120">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="12dc1-120">Select **OK**.</span></span>

 > [!NOTE]
 > <span data-ttu-id="12dc1-121">Това ще разпространи общи данни към таблицата **ResCalendarCapacity** във всички компании във вашата среда, така че пакетната работа трябва да се изпълнява само в едно юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="12dc1-121">This will distribute general data to the **ResCalendarCapacity** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="12dc1-122">Данните в тази пакетна работа са необходими за изчисляване на ресурсния капацитет чрез свързания календар.</span><span class="sxs-lookup"><span data-stu-id="12dc1-122">The data in this batch job is needed to calculate resource capacity through the associated calendar.</span></span>

8. <span data-ttu-id="12dc1-123">Отидете на **Управление на проекти и счетоводство** > **Периодични** > **Ресурси по проекта** > **Попълнете ресурсите на проекти във всички компании** и след това изберете **ОК**.</span><span class="sxs-lookup"><span data-stu-id="12dc1-123">Go to **Project management and accounting** > **Periodic** > **Project resources** > **Populate project resources across all companies** and then select **OK**.</span></span> <span data-ttu-id="12dc1-124">Това е скриптът за надстройка на данни за общи данни в **ResProjectResource**, **ResCalendarDateTimeRange** и **ResEffectiveDateTimeRange** таблици.</span><span class="sxs-lookup"><span data-stu-id="12dc1-124">This is the data upgrade script for general data in the **ResProjectResource**, **ResCalendarDateTimeRange**, and **ResEffectiveDateTimeRange** tables.</span></span> <span data-ttu-id="12dc1-125">Стойности за полето **PSAPRojSchedRole.RootActivity** също се актуализират.</span><span class="sxs-lookup"><span data-stu-id="12dc1-125">Values for the **PSAPRojSchedRole.RootActivity** field are also updated.</span></span> <span data-ttu-id="12dc1-126">Ако това не се изпълни, ще получите предупреждение, когато се опитате да изпълните операции по планиране на ресурси.</span><span class="sxs-lookup"><span data-stu-id="12dc1-126">If this is not run, you will receive a warning when you try to execute resource scheduling operations.</span></span>
 
## <a name="turn-off-resource-scheduling-performance-enhancement"></a><span data-ttu-id="12dc1-127">Изключете подобряване на производителността при планиране на ресурси</span><span class="sxs-lookup"><span data-stu-id="12dc1-127">Turn off resource scheduling performance enhancement</span></span>

1. <span data-ttu-id="12dc1-128">Отидете на **Управление на функции** > **всичко** и намерете **Активирайте функцията за подобряване на производителността за планиране на ресурсите на проекта**.</span><span class="sxs-lookup"><span data-stu-id="12dc1-128">Go to **Feature management** > **All**  and search for **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="12dc1-129">Изберете функцията и след това изберете бутона **Дезактивиране**.</span><span class="sxs-lookup"><span data-stu-id="12dc1-129">Select the feature, and then select the **Disable** button.</span></span>
3. <span data-ttu-id="12dc1-130">Обновете браузъра си.</span><span class="sxs-lookup"><span data-stu-id="12dc1-130">Refresh your browser.</span></span>
4. <span data-ttu-id="12dc1-131">Отидете на **Управление на проекти и счетоводство** > **Периодични** > **Синхронизация на капацитета** > **Синхронизирайте обобщените капацитети на ресурсите**.</span><span class="sxs-lookup"><span data-stu-id="12dc1-131">Go to **Project management and accounting** > **Periodic** > **Capacity synchronization** > **Synchronize resource capacity roll-ups**.</span></span>
5. <span data-ttu-id="12dc1-132">На **Синхронизиране на капацитет** страница, задайте **Премахнете съществуващите записи за капацитет** на **Да**, за да премахнете предишни данни.</span><span class="sxs-lookup"><span data-stu-id="12dc1-132">On the **Capacity roll-up synchronization** page, set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="12dc1-133">Ако искате да генерирате допълнителни данни, задайте на **Не**.</span><span class="sxs-lookup"><span data-stu-id="12dc1-133">If you want to generate incremental data, set it to **No**.</span></span>
6. <span data-ttu-id="12dc1-134">В полето **Код на периода** изберете периода, в който трябва да се генерират данни.</span><span class="sxs-lookup"><span data-stu-id="12dc1-134">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="12dc1-135">Ако изберете код на период, не е необходимо да се определят начална и крайна дата.</span><span class="sxs-lookup"><span data-stu-id="12dc1-135">If you select a period code, a start and end date do not need to be defined.</span></span>
7. <span data-ttu-id="12dc1-136">Ако оставите полето **Код на периода** празно, изберете конкретни начална и крайна дата, за да генерирате данни.</span><span class="sxs-lookup"><span data-stu-id="12dc1-136">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
8. <span data-ttu-id="12dc1-137">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="12dc1-137">Select **OK**.</span></span>

> [!NOTE]
> <span data-ttu-id="12dc1-138">Това ще разпространи общи данни към таблицата **ResRollup** във всички компании във вашата среда, така че пакетната работа трябва да се изпълнява само в едно юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="12dc1-138">This will distribute general data to the **ResRollup** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="12dc1-139">Тази партидна работа е необходима за всички изгледи **Наличност на ресурс**.</span><span class="sxs-lookup"><span data-stu-id="12dc1-139">This batch job is needed for all **Resource Availability** views.</span></span> <span data-ttu-id="12dc1-140">Ако тази партидна задача не се изпълни, **ResRollup** данните ще се генерират в движение, което може да отнеме време.</span><span class="sxs-lookup"><span data-stu-id="12dc1-140">If this batch job is not run, the **ResRollup** data will be generated on the fly, which can take time.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]