---
title: Преглед на натрупаните фактури за проекти и договори по проекти
description: Тази тема предоставя информация за това как да преглеждате натрупванията на време, разходи и продукти и как да ги маркирате като готови за фактуриране.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom: ''
ms.author: rumant
ms.date: 03/11/2019
ms.topic: article
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 092455a131f556e4f943f6bb89d7e38358f0a697
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150475"
---
# <a name="review-the-invoicing-backlog-on-projects-and-project-contracts"></a><span data-ttu-id="93cd9-103">Преглед на натрупаните фактури за проекти и договори по проекти</span><span class="sxs-lookup"><span data-stu-id="93cd9-103">Review the invoicing backlog on projects and project contracts</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="93cd9-104">Когато дадена транзакция е готова за създаване и обработка на фактура, транзакцията трябва да бъде маркирана като **Готово за фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="93cd9-104">When a transaction is ready to have an invoice created and processed, the transaction should be marked **Ready to invoice**.</span></span> <span data-ttu-id="93cd9-105">Тази тема описва типовете транзакции, които могат да бъдат създадени.</span><span class="sxs-lookup"><span data-stu-id="93cd9-105">This topic describes the types of transactions that can be created.</span></span>

## <a name="review-the-time-and-material-billing-backlog"></a><span data-ttu-id="93cd9-106">Преглед на натрупването на време и материали за фактуриране</span><span class="sxs-lookup"><span data-stu-id="93cd9-106">Review the time and material billing backlog</span></span>

<span data-ttu-id="93cd9-107">Когато запис за време или разходи е подаден и одобрен за проект, PSA създава действителни данни за проекта.</span><span class="sxs-lookup"><span data-stu-id="93cd9-107">When a time or expense entry is submitted and approved for a project, PSA creates a project actual.</span></span> <span data-ttu-id="93cd9-108">Ако комбинацията от проекта и класа на транзакцията се съпоставят към ред на договор за проект тип време и материали, се създават две действителни данни, когато записът бъде одобрен:</span><span class="sxs-lookup"><span data-stu-id="93cd9-108">If the combination of the project and the transaction class are mapped to a contract line for a time-and-materials project, two actuals are created when the entry is approved:</span></span>

- <span data-ttu-id="93cd9-109">Действителни данни за разходи</span><span class="sxs-lookup"><span data-stu-id="93cd9-109">Cost actual</span></span> 
- <span data-ttu-id="93cd9-110">Нефактурирани действителни данни за продажби</span><span class="sxs-lookup"><span data-stu-id="93cd9-110">Unbilled sales actual</span></span>

<span data-ttu-id="93cd9-111">Нефактурираните действителни данни за продажби представляват натрупванията за фактуриране и състоянието им на фактуриране трябва да бъде зададено на **Готово за фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="93cd9-111">Unbilled sales actuals represent the billing backlog, and their billing status must be set to **Ready to Invoice**.</span></span> <span data-ttu-id="93cd9-112">Когато се създава фактура за проект, нефактурираните действителни данни за продажби, които са маркирани като **Готови за фактуриране**, се копират отгоре като подробности за ред на фактура.</span><span class="sxs-lookup"><span data-stu-id="93cd9-112">When a project invoice is created, unbilled sales actuals that are marked **Ready to Invoice** are copied over as invoice line details.</span></span>

<span data-ttu-id="93cd9-113">За да прегледате натрупванията за фактуриране за време и материали, отидете на **Продажби** \> **Фактуриране** \> **Натрупване за фактуриране на време и материали**.</span><span class="sxs-lookup"><span data-stu-id="93cd9-113">To review the billing backlog for time and materials, go to **Sales** \> **Billing** \> **Time and Material Billing Backlog**.</span></span> <span data-ttu-id="93cd9-114">Изберете всички нефактурирани действителни данни за продажби, които са готови да бъдат фактурирани, след което изберете **Готово за фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="93cd9-114">Select all the unbilled sales actuals that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="93cd9-115">Състоянието на фактуриране на тези действителни данни се променя на **Готово за фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="93cd9-115">The billing status of these actuals is changed to **Ready to Invoice**.</span></span>

![Натрупване за фактуриране на време и материали](media/TMBacklog.png)

## <a name="review-the-product-billing-backlog"></a><span data-ttu-id="93cd9-117">Преглед на натрупване за фактуриране на продукти</span><span class="sxs-lookup"><span data-stu-id="93cd9-117">Review the product billing backlog</span></span>

<span data-ttu-id="93cd9-118">В PSA, когато договор по проект има базирани на продукти редове на договор, тези редове се вземат предвид за фактуриране, когато се създава фактура за договора по проекта.</span><span class="sxs-lookup"><span data-stu-id="93cd9-118">In PSA, when a project contract has product-based contract lines, those lines are considered for invoicing whenever an invoice is created for the project contract.</span></span> <span data-ttu-id="93cd9-119">Всеки продукт, който има редове на договора, които са маркирани като **Готово за фактуриране**, се копира във фактурата по проекта като редове на фактура по проекта.</span><span class="sxs-lookup"><span data-stu-id="93cd9-119">Any product that has contract lines that are marked **Ready to Invoice** is copied over to the project invoice as project invoice lines.</span></span>

<span data-ttu-id="93cd9-120">За да прегледате натрупванията за фактуриране за продукти, отидете на **Продажби** \> **Фактуриране** \> **Натрупване за фактуриране на продукти**.</span><span class="sxs-lookup"><span data-stu-id="93cd9-120">To review the billing backlog for products, go to **Sales** \> **Billing** \> **Product Billing Backlog**.</span></span> <span data-ttu-id="93cd9-121">Изберете всички редове на договора, базирани на продукти, които са готови да бъдат фактурирани, след което изберете **Готово за фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="93cd9-121">Select all the product-based contract lines that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="93cd9-122">Състоянието на фактуриране на тези редове се променя на **Готово за фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="93cd9-122">The billing status of these lines is changed to **Ready to Invoice**.</span></span>

![Натрупване за фактуриране на продукти](media/ProductBacklog.png)

## <a name="review-billing-milestones-on-fixed-price-contracts"></a><span data-ttu-id="93cd9-124">Преглед на контролни точки за фактуриране по договори с фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="93cd9-124">Review billing milestones on fixed-price contracts</span></span>

<span data-ttu-id="93cd9-125">Всеки ред от договор по проект, който има метод за фактуриране фиксирана цена, трябва да дефинира контролни точки на договора.</span><span class="sxs-lookup"><span data-stu-id="93cd9-125">Each project contract line that has a fixed-price billing method must define contract milestones.</span></span> <span data-ttu-id="93cd9-126">Тези контролни точки на договора могат да бъдат фактурирани само ако са маркирани като **Готово за фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="93cd9-126">These contract milestones can be invoiced only if they are marked **Ready to Invoice**.</span></span> 

<span data-ttu-id="93cd9-127">За да прегледате контролните точки, отидете на **Продажби** \> **Фактуриране** \> **Контролни точки за фиксирана цена**.</span><span class="sxs-lookup"><span data-stu-id="93cd9-127">To review billing milestones, go to **Sales** \> **Billing** \> **Fixed Price Milestones**.</span></span> <span data-ttu-id="93cd9-128">Изберете всички контролни точки, които са готови да бъдат фактурирани, след което изберете **Готово за фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="93cd9-128">Select the milestones that are ready to be invoiced, and then select **Ready to invoice**.</span></span> <span data-ttu-id="93cd9-129">Състоянието на фактуриране на тези контролни точки се променя на **Готово за фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="93cd9-129">The billing status of these milestones is changed to **Ready to Invoice**.</span></span>

![Контролни точки на фиксирана цена](media/FPBacklog.png)
