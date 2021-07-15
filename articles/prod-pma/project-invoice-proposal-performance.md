---
title: Производителност на предложение за фактуриране по проект
description: Тази тема предоставя информация за подобрения на ефективността на предложенията за фактури по проекта.
author: Yowelle
ms.date: 06/16/2021
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ''
audience: Application User, IT Pro
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 20121-03-05
ms.dyn365.ops.version: 10.0.18
ms.openlocfilehash: 5a14acf51d277b16896d64c4b12ee00bfb326910
ms.sourcegitcommit: 3a4b181be08ef0428104d72b54a3e61ac2782f14
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/17/2021
ms.locfileid: "6269777"
---
# <a name="project-invoice-proposal-performance"></a><span data-ttu-id="60014-103">Производителност на предложение за фактуриране по проект</span><span class="sxs-lookup"><span data-stu-id="60014-103">Project invoice proposal performance</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="60014-104">Когато създавате ново предложение за фактура, може да срещнете проблеми с производителността, тъй като броят на проектите и подпроектите се увеличава.</span><span class="sxs-lookup"><span data-stu-id="60014-104">When you create a new invoice proposal you might encounter performance issues as the number of projects and subprojects increase.</span></span> <span data-ttu-id="60014-105">За подобряване на производителността е налична функция, която намалява времето, необходимо за създаване на ново предложение за фактура за осчетоводени транзакции на проекти.</span><span class="sxs-lookup"><span data-stu-id="60014-105">To improve performance, a feature is available that reduces the time needed to create a new invoice proposal for posted project transactions.</span></span>

## <a name="enable-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="60014-106">Разрешаване на подобряване на производителност на предложение за фактуриране по проект</span><span class="sxs-lookup"><span data-stu-id="60014-106">Enable project invoice proposal performance enhancement</span></span>
<span data-ttu-id="60014-107">За да активирате функцията за подобряване на изпълнението на предложението за фактура на проекта, изпълнете следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="60014-107">To enable the project invoice proposal performance enhancement feature, complete the following steps.</span></span>

1.  <span data-ttu-id="60014-108">Отидете на **Управление на функции** > **Всичко**.</span><span class="sxs-lookup"><span data-stu-id="60014-108">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="60014-109">Намерете в списъка с функции **Подобряване на изпълнението на предложението за фактура по проекта**.</span><span class="sxs-lookup"><span data-stu-id="60014-109">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="60014-110">Изберете **Разрешаване сега**.</span><span class="sxs-lookup"><span data-stu-id="60014-110">Select **Enable now**.</span></span>
3.  <span data-ttu-id="60014-111">Опреснете браузъра си и след това създайте ново предложение за фактура.</span><span class="sxs-lookup"><span data-stu-id="60014-111">Refresh your browser, and then create a new invoice proposal.</span></span>

## <a name="turn-off-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="60014-112">Изключване на подобряване на производителност на предложение за фактуриране по проект</span><span class="sxs-lookup"><span data-stu-id="60014-112">Turn off project invoice proposal performance enhancement</span></span>
<span data-ttu-id="60014-113">Изпълнете следните стъпки, за да изключите подобряването на изпълнението на предложението за фактура на проекта, изпълнете следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="60014-113">Complete the following steps to turn off the project invoice proposal performance enhancement.</span></span>

1.  <span data-ttu-id="60014-114">Отидете на **Управление на функции** > **Всичко**.</span><span class="sxs-lookup"><span data-stu-id="60014-114">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="60014-115">Намерете в списъка с функции **Подобряване на изпълнението на предложението за фактура по проекта**.</span><span class="sxs-lookup"><span data-stu-id="60014-115">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="60014-116">Изберете **Забраняване**.</span><span class="sxs-lookup"><span data-stu-id="60014-116">Select **Disable**.</span></span>
3.  <span data-ttu-id="60014-117">Обновете браузъра си.</span><span class="sxs-lookup"><span data-stu-id="60014-117">Refresh your browser.</span></span>

> [!NOTE]
> <span data-ttu-id="60014-118">Ефективността на предложението за фактура не може да се приложи, когато са активирани правилата за таксуване.</span><span class="sxs-lookup"><span data-stu-id="60014-118">Invoice proposal performance can't be applied when billing rules are enabled.</span></span>
> 
> <span data-ttu-id="60014-119">По време на пакетния процес за създаване на предложения за фактури, броят на подзадачите ще раздели задачите на максимален брой въз основа на броя на договорите с фактурирани транзакции, независимо от това, което сте въвели.</span><span class="sxs-lookup"><span data-stu-id="60014-119">During the batch process to create invoice proposals, the number of subtasks will split the tasks to a maximum number based on the number of contracts with invoiceable transactions, regardless of what you have entered.</span></span> <span data-ttu-id="60014-120">Например, ако въведете **3** за броя подзадачи за създаване на предложение за фактура в партида и има само два договора с фактурирани транзакции, създават се само две подзадачи.</span><span class="sxs-lookup"><span data-stu-id="60014-120">For example, if you enter **3** for the number of subtasks for invoice proposal creation in batch, and there are only two contracts with invoiceable transactions, only two subtasks are created.</span></span>
