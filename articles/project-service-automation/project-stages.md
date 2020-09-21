---
title: Етапи на проекти
description: Тази тема предоставя информация за етапите на проекти.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 983c25a0-ed21-4151-a109-b385a88285fa
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 70aa057e127df7ba925e84f5d056a06a4cc8833e
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749259"
---
# <a name="project-stages"></a><span data-ttu-id="a688f-103">Етапи на проекти</span><span class="sxs-lookup"><span data-stu-id="a688f-103">Project stages</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a688f-104">Етапите на проекта се актуализират, за да отразяват състоянието на проекта с напредването му.</span><span class="sxs-lookup"><span data-stu-id="a688f-104">Project stages are updated to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="a688f-105">По подразбиране потокът на бизнес процес автоматично актуализира някои етапи на проекта, докато други се актуализират ръчно от мениджъра на проекта.</span><span class="sxs-lookup"><span data-stu-id="a688f-105">The default business process flow automatically updates some stages of the project while others are manually updated by the project manager.</span></span> 

<span data-ttu-id="a688f-106">Следните етапи са дефинирани в потока на бизнес процес по подразбиране:</span><span class="sxs-lookup"><span data-stu-id="a688f-106">The following stages are defined in the default BPF:</span></span>

- <span data-ttu-id="a688f-107">Нов</span><span class="sxs-lookup"><span data-stu-id="a688f-107">New</span></span>
- <span data-ttu-id="a688f-108">Оферта</span><span class="sxs-lookup"><span data-stu-id="a688f-108">Quote</span></span>
- <span data-ttu-id="a688f-109">План</span><span class="sxs-lookup"><span data-stu-id="a688f-109">Plan</span></span>
- <span data-ttu-id="a688f-110">Доставяне</span><span class="sxs-lookup"><span data-stu-id="a688f-110">Deliver</span></span>
- <span data-ttu-id="a688f-111">Завършен</span><span class="sxs-lookup"><span data-stu-id="a688f-111">Complete</span></span>
- <span data-ttu-id="a688f-112">Затваряне</span><span class="sxs-lookup"><span data-stu-id="a688f-112">Close</span></span> 

## <a name="new"></a><span data-ttu-id="a688f-113">Нов</span><span class="sxs-lookup"><span data-stu-id="a688f-113">New</span></span>

<span data-ttu-id="a688f-114">Когато създавате проект, етапът на проекта се задава на **Нов**.</span><span class="sxs-lookup"><span data-stu-id="a688f-114">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="a688f-115">Ако проектът е създаден от шаблон, той може да има график, прогнозна оценка и данни за екипа.</span><span class="sxs-lookup"><span data-stu-id="a688f-115">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="a688f-116">В противен случай това е просто скица на проекта и останалите компоненти трябва да бъдат въведени.</span><span class="sxs-lookup"><span data-stu-id="a688f-116">Otherwise, it's just an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="a688f-117">Оферта</span><span class="sxs-lookup"><span data-stu-id="a688f-117">Quote</span></span>

<span data-ttu-id="a688f-118">Когато свържете проект с оферта или го създадете от оферта, етапът на проект се задава на **Оферта** и прогнозните начална и крайна дата се актуализират.</span><span class="sxs-lookup"><span data-stu-id="a688f-118">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="a688f-119">Докато проектът е в етапа **Оферта**, разделът **Продажби** на страницата **Обект на проекта** показва подробности за офертата.</span><span class="sxs-lookup"><span data-stu-id="a688f-119">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="a688f-120">План</span><span class="sxs-lookup"><span data-stu-id="a688f-120">Plan</span></span>

<span data-ttu-id="a688f-121">Когато спечелите оферта, свързана с даден проект, и проектът се придвижи до фаза **Договор**, етапът се актуализира на **План**.</span><span class="sxs-lookup"><span data-stu-id="a688f-121">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="a688f-122">Докато проектът е в етапа **План**, страницата **Обект на проекта** показва подробности за договора.</span><span class="sxs-lookup"><span data-stu-id="a688f-122">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="a688f-123">Доставяне</span><span class="sxs-lookup"><span data-stu-id="a688f-123">Deliver</span></span>

<span data-ttu-id="a688f-124">Когато планът на проекта е завършен и сте готови да стартирате проекта, мениджърът на проекта трябва да актуализира етапа на проекта на **Доставяне**, за да покаже, че проектът е стартиран.</span><span class="sxs-lookup"><span data-stu-id="a688f-124">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="a688f-125">Завършен</span><span class="sxs-lookup"><span data-stu-id="a688f-125">Complete</span></span> 

<span data-ttu-id="a688f-126">Когато работата по проекта е завършена, мениджърът на проекта може да актуализира етапа на **Завършено**.</span><span class="sxs-lookup"><span data-stu-id="a688f-126">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="a688f-127">Чрез актуализиране на етапа на проекта на **Завършен** мениджърът на проекта показва, че работата е 100% завършена, но че проектът се поддържа отворен, така че всички чакащи записи за време или разходи да могат да бъдат записани.</span><span class="sxs-lookup"><span data-stu-id="a688f-127">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="a688f-128">Затваряне</span><span class="sxs-lookup"><span data-stu-id="a688f-128">Close</span></span>

<span data-ttu-id="a688f-129">Когато всички транзакции бъдат записани за проекта, мениджърът на проекта може да актуализира етапа на **Затваряне**.</span><span class="sxs-lookup"><span data-stu-id="a688f-129">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="a688f-130">От този момент не могат да се записват транзакции и проектът се задава като само за четене.</span><span class="sxs-lookup"><span data-stu-id="a688f-130">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>
