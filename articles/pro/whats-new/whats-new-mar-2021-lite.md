---
title: Нововъведения от март 2021 г. – олекотено внедряване на Project Operations
description: Тази тема предоставя информация за актуализациите на качеството, налични в изданието на леко внедряване на Project Operations от март 2021 г.
author: sigitac
manager: tfehr
ms.date: 03/03/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: bd1518ef8f5645bace63a222b92cfd16d9c19a21
ms.sourcegitcommit: f78087174a8512199a1bcbd7e8610bbc80e64801
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "5499976"
---
# <a name="whats-new-march-2021---project-operations-lite-deployment"></a><span data-ttu-id="e5c33-103">Нововъведения от март 2021 г. – олекотено внедряване на Project Operations</span><span class="sxs-lookup"><span data-stu-id="e5c33-103">What's new March 2021 - Project Operations lite deployment</span></span>

<span data-ttu-id="e5c33-104">_Прилага се за: Олекотено внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="e5c33-104">_Applies To: Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="e5c33-105">Тази тема се отнася за следните компоненти и версии на Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="e5c33-105">This topic applies to the following Dynamics 365 Project Operations components and versions:</span></span>

- <span data-ttu-id="e5c33-106">Project Operations в среда на Dataverse, версия 4.8.0.91</span><span class="sxs-lookup"><span data-stu-id="e5c33-106">Project Operations on Dataverse environment version 4.8.0.91</span></span> 

## <a name="quality-updates"></a><span data-ttu-id="e5c33-107">Актуализации на качеството</span><span class="sxs-lookup"><span data-stu-id="e5c33-107">Quality updates</span></span>

| <span data-ttu-id="e5c33-108">**Област с функции**</span><span class="sxs-lookup"><span data-stu-id="e5c33-108">**Feature area**</span></span> | <span data-ttu-id="e5c33-109">**Номер за справка**</span><span class="sxs-lookup"><span data-stu-id="e5c33-109">**Reference number**</span></span> | <span data-ttu-id="e5c33-110">**Актуализация на качеството**</span><span class="sxs-lookup"><span data-stu-id="e5c33-110">**Quality update**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="e5c33-111">Фактуриране и ценообразуване</span><span class="sxs-lookup"><span data-stu-id="e5c33-111">Billing and pricing</span></span> | <span data-ttu-id="e5c33-112">2133873</span><span class="sxs-lookup"><span data-stu-id="e5c33-112">2133873</span></span> | <span data-ttu-id="e5c33-113">Коригирано е показването на **Единична продажна цена** символ на валута в мрежата **Оценки на разходите**.</span><span class="sxs-lookup"><span data-stu-id="e5c33-113">Fixed the display of **Unit Sales Price** currency symbol in the **Expense Estimates** grid.</span></span> |
| <span data-ttu-id="e5c33-114">Фактуриране и ценообразуване</span><span class="sxs-lookup"><span data-stu-id="e5c33-114">Billing and pricing</span></span> | <span data-ttu-id="e5c33-115">2174616</span><span class="sxs-lookup"><span data-stu-id="e5c33-115">2174616</span></span> | <span data-ttu-id="e5c33-116">Когато се спечели оферта, цената на поръчката по поръчка се посочва в подробности за договора, които се копират от цената.</span><span class="sxs-lookup"><span data-stu-id="e5c33-116">When a quote is won, the contract custom pricelist is referenced on contract line details that are copied from the quote.</span></span> |
| <span data-ttu-id="e5c33-117">Управление на възможности</span><span class="sxs-lookup"><span data-stu-id="e5c33-117">Opportunity Management</span></span> | <span data-ttu-id="e5c33-118">2167475</span><span class="sxs-lookup"><span data-stu-id="e5c33-118">2167475</span></span> | <span data-ttu-id="e5c33-119">Фиксирана сума на данъка във фактурата за корекция, която създава нефактуриран действителен запис.</span><span class="sxs-lookup"><span data-stu-id="e5c33-119">Fixed tax amount in the correction invoice that originated an unbilled actual entry.</span></span> |
| <span data-ttu-id="e5c33-120">Управление на възможности</span><span class="sxs-lookup"><span data-stu-id="e5c33-120">Opportunity Management</span></span> | <span data-ttu-id="e5c33-121">2176285</span><span class="sxs-lookup"><span data-stu-id="e5c33-121">2176285</span></span> | <span data-ttu-id="e5c33-122">Сумата на данъка не трябва да се копира от данните за договора за продажба/ред на офертата, за да се детайлира договор за цена/ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="e5c33-122">Tax amount must not be copied from sales contract/quote line details to cost contract/quote line details.</span></span> |
| <span data-ttu-id="e5c33-123">Управление на възможности</span><span class="sxs-lookup"><span data-stu-id="e5c33-123">Opportunity Management</span></span> | <span data-ttu-id="e5c33-124">2188079</span><span class="sxs-lookup"><span data-stu-id="e5c33-124">2188079</span></span> | <span data-ttu-id="e5c33-125">Правилото за разделно таксуване не трябва да се създава за договори, които не са базирани на работа.</span><span class="sxs-lookup"><span data-stu-id="e5c33-125">Split billing rule must not be created for contracts that are not work-based.</span></span> |
| <span data-ttu-id="e5c33-126">Планиране и проследяване</span><span class="sxs-lookup"><span data-stu-id="e5c33-126">Planning and Tracking</span></span> | <span data-ttu-id="e5c33-127">2138853</span><span class="sxs-lookup"><span data-stu-id="e5c33-127">2138853</span></span> | <span data-ttu-id="e5c33-128">Функцията за копиране на проект е актуализирана, за да гарантира, че линиите за оценка на разходите, които референтните задачи се копират в целевия проект.</span><span class="sxs-lookup"><span data-stu-id="e5c33-128">Project copy function updated to ensure expense estimate lines that reference tasks are copied to the destination project.</span></span> |
| <span data-ttu-id="e5c33-129">Планиране и проследяване</span><span class="sxs-lookup"><span data-stu-id="e5c33-129">Planning and Tracking</span></span> | <span data-ttu-id="e5c33-130">2173259</span><span class="sxs-lookup"><span data-stu-id="e5c33-130">2173259</span></span> | <span data-ttu-id="e5c33-131">Функцията за копиране на проект е актуализирана, за да гарантира, че не се показва съобщение **Копиране на WBS** за грешка в определени сценарии.</span><span class="sxs-lookup"><span data-stu-id="e5c33-131">Project copy function updated to ensure it doesn't display the **Copying WBS** error message in certain scenarios.</span></span> |
| <span data-ttu-id="e5c33-132">Време и разход</span><span class="sxs-lookup"><span data-stu-id="e5c33-132">Time and Expense</span></span> | <span data-ttu-id="e5c33-133">2148910</span><span class="sxs-lookup"><span data-stu-id="e5c33-133">2148910</span></span> | <span data-ttu-id="e5c33-134">Отстранен проблем с показването на страницата **Редактиране на запис** в мрежата **Времеви запис**.</span><span class="sxs-lookup"><span data-stu-id="e5c33-134">Fixed display issue with the **Edit Entry** page in the **Time Entry** grid.</span></span> |
| <span data-ttu-id="e5c33-135">Време и разход</span><span class="sxs-lookup"><span data-stu-id="e5c33-135">Time and Expense</span></span> | <span data-ttu-id="e5c33-136">2159798</span><span class="sxs-lookup"><span data-stu-id="e5c33-136">2159798</span></span> | <span data-ttu-id="e5c33-137">Засилени контроли, за да се гарантира, че одобрените записи за разходи не могат да бъдат редактирани.</span><span class="sxs-lookup"><span data-stu-id="e5c33-137">Tightened controls to ensure approved expense entries can't be edited.</span></span> |


