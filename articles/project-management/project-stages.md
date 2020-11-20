---
title: Етапи на проект
description: Тази тема предоставя информация за етапи на проект, които са налични в Microsoft Dynamics Project Operations.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
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
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: aa3d692a46165b01eafbd7619578cead8dd912d6
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127460"
---
# <a name="project-stages"></a><span data-ttu-id="a5474-103">Етапи на проект</span><span class="sxs-lookup"><span data-stu-id="a5474-103">Project stages</span></span>

<span data-ttu-id="a5474-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="a5474-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a5474-105">Етапите на проект са проектирани, за да отразяват състоянието на проекта, докато е в ход.</span><span class="sxs-lookup"><span data-stu-id="a5474-105">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="a5474-106">Могат да се използват персонализации за автоматично актуализиране на етапите с потоци на бизнес процеси, Power Automate или разширения на добавки.</span><span class="sxs-lookup"><span data-stu-id="a5474-106">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="a5474-107">Следните етапи са дефинирани в потока на бизнес процес по подразбиране:</span><span class="sxs-lookup"><span data-stu-id="a5474-107">The following stages are defined in the default business process flow:</span></span>

- <span data-ttu-id="a5474-108">Ново</span><span class="sxs-lookup"><span data-stu-id="a5474-108">New</span></span>
- <span data-ttu-id="a5474-109">Оферта</span><span class="sxs-lookup"><span data-stu-id="a5474-109">Quote</span></span>
- <span data-ttu-id="a5474-110">План</span><span class="sxs-lookup"><span data-stu-id="a5474-110">Plan</span></span>
- <span data-ttu-id="a5474-111">Доставяне</span><span class="sxs-lookup"><span data-stu-id="a5474-111">Deliver</span></span>
- <span data-ttu-id="a5474-112">Завършени</span><span class="sxs-lookup"><span data-stu-id="a5474-112">Complete</span></span>
- <span data-ttu-id="a5474-113">Закрий</span><span class="sxs-lookup"><span data-stu-id="a5474-113">Close</span></span> 

## <a name="new"></a><span data-ttu-id="a5474-114">Ново</span><span class="sxs-lookup"><span data-stu-id="a5474-114">New</span></span>

<span data-ttu-id="a5474-115">Когато създавате проект, етапът на проекта се задава на **Нов**.</span><span class="sxs-lookup"><span data-stu-id="a5474-115">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="a5474-116">Ако проектът е създаден от шаблон, той може да има график, прогнозна оценка и данни за екипа.</span><span class="sxs-lookup"><span data-stu-id="a5474-116">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="a5474-117">В противен случай това е скица на проекта и останалите компоненти трябва да бъдат въведени.</span><span class="sxs-lookup"><span data-stu-id="a5474-117">Otherwise, it's an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="a5474-118">Оферта</span><span class="sxs-lookup"><span data-stu-id="a5474-118">Quote</span></span>

<span data-ttu-id="a5474-119">Когато свържете проект с оферта или го създадете от оферта, етапът на проект се задава на **Оферта** и прогнозните начална и крайна дата се актуализират.</span><span class="sxs-lookup"><span data-stu-id="a5474-119">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="a5474-120">Докато проектът е в етапа **Оферта**, разделът **Продажби** на страницата **Обект на проекта** показва подробности за офертата.</span><span class="sxs-lookup"><span data-stu-id="a5474-120">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="a5474-121">План</span><span class="sxs-lookup"><span data-stu-id="a5474-121">Plan</span></span>

<span data-ttu-id="a5474-122">Когато спечелите оферта, свързана с даден проект, и проектът се придвижи до фаза **Договор**, етапът се актуализира на **План**.</span><span class="sxs-lookup"><span data-stu-id="a5474-122">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="a5474-123">Докато проектът е в етапа **План**, страницата **Обект на проекта** показва подробности за договора.</span><span class="sxs-lookup"><span data-stu-id="a5474-123">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="a5474-124">Доставяне</span><span class="sxs-lookup"><span data-stu-id="a5474-124">Deliver</span></span>

<span data-ttu-id="a5474-125">Когато планът на проекта е завършен и сте готови да стартирате проекта, мениджърът на проекта трябва да актуализира етапа на проекта на **Доставяне**, за да покаже, че проектът е стартиран.</span><span class="sxs-lookup"><span data-stu-id="a5474-125">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="a5474-126">Завършен</span><span class="sxs-lookup"><span data-stu-id="a5474-126">Complete</span></span> 

<span data-ttu-id="a5474-127">Когато работата по проекта е завършена, мениджърът на проекта може да актуализира етапа на **Завършено**.</span><span class="sxs-lookup"><span data-stu-id="a5474-127">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="a5474-128">Чрез актуализиране на етапа на проекта на **Завършен** мениджърът на проекта показва, че работата е 100% завършена, но че проектът се поддържа отворен, така че всички чакащи записи за време или разходи да могат да бъдат записани.</span><span class="sxs-lookup"><span data-stu-id="a5474-128">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="a5474-129">Затваряне</span><span class="sxs-lookup"><span data-stu-id="a5474-129">Close</span></span>

<span data-ttu-id="a5474-130">Когато всички транзакции бъдат записани за проекта, мениджърът на проекта може да актуализира етапа на **Затваряне**.</span><span class="sxs-lookup"><span data-stu-id="a5474-130">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="a5474-131">От този момент не могат да се записват транзакции и проектът се задава като само за четене.</span><span class="sxs-lookup"><span data-stu-id="a5474-131">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>

