---
title: Типове етапи на проект
description: Тази тема предоставя информация за етапите на проекти.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 06/19/2020
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
ms.openlocfilehash: 3503b17e54fc0b321582c30ce534e4cb3f497a5f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5283670"
---
# <a name="project-stage-types"></a><span data-ttu-id="aa8be-103">Типове етапи на проект</span><span class="sxs-lookup"><span data-stu-id="aa8be-103">Project stage types</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="aa8be-104">Етапите на проект са проектирани, за да отразяват състоянието на проекта, докато е в ход.</span><span class="sxs-lookup"><span data-stu-id="aa8be-104">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="aa8be-105">Могат да се използват персонализации за автоматично актуализиране на етапите с потоци на бизнес процеси, Power Automate или разширения на добавки.</span><span class="sxs-lookup"><span data-stu-id="aa8be-105">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="aa8be-106">Следните етапи са дефинирани в потока на бизнес процес по подразбиране:</span><span class="sxs-lookup"><span data-stu-id="aa8be-106">The following stages are defined in the default BPF:</span></span>

- <span data-ttu-id="aa8be-107">Нова</span><span class="sxs-lookup"><span data-stu-id="aa8be-107">New</span></span>
- <span data-ttu-id="aa8be-108">Оферта</span><span class="sxs-lookup"><span data-stu-id="aa8be-108">Quote</span></span>
- <span data-ttu-id="aa8be-109">План</span><span class="sxs-lookup"><span data-stu-id="aa8be-109">Plan</span></span>
- <span data-ttu-id="aa8be-110">Доставяне</span><span class="sxs-lookup"><span data-stu-id="aa8be-110">Deliver</span></span>
- <span data-ttu-id="aa8be-111">Завършен</span><span class="sxs-lookup"><span data-stu-id="aa8be-111">Complete</span></span>
- <span data-ttu-id="aa8be-112">Затваряне</span><span class="sxs-lookup"><span data-stu-id="aa8be-112">Close</span></span> 

## <a name="new"></a><span data-ttu-id="aa8be-113">Нов</span><span class="sxs-lookup"><span data-stu-id="aa8be-113">New</span></span>

<span data-ttu-id="aa8be-114">Когато създавате проект, етапът на проекта се задава на **Нов**.</span><span class="sxs-lookup"><span data-stu-id="aa8be-114">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="aa8be-115">Ако проектът е създаден от шаблон, той може да има график, прогнозна оценка и данни за екипа.</span><span class="sxs-lookup"><span data-stu-id="aa8be-115">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="aa8be-116">В противен случай това е просто скица на проекта и останалите компоненти трябва да бъдат въведени.</span><span class="sxs-lookup"><span data-stu-id="aa8be-116">Otherwise, it's just an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="aa8be-117">Оферта</span><span class="sxs-lookup"><span data-stu-id="aa8be-117">Quote</span></span>

<span data-ttu-id="aa8be-118">Когато свържете проект с оферта или го създадете от оферта, етапът на проект се задава на **Оферта** и прогнозните начална и крайна дата се актуализират.</span><span class="sxs-lookup"><span data-stu-id="aa8be-118">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="aa8be-119">Докато проектът е в етапа **Оферта**, разделът **Продажби** на страницата **Обект на проекта** показва подробности за офертата.</span><span class="sxs-lookup"><span data-stu-id="aa8be-119">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="aa8be-120">План</span><span class="sxs-lookup"><span data-stu-id="aa8be-120">Plan</span></span>

<span data-ttu-id="aa8be-121">Когато спечелите оферта, свързана с даден проект, и проектът се придвижи до фаза **Договор**, етапът се актуализира на **План**.</span><span class="sxs-lookup"><span data-stu-id="aa8be-121">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="aa8be-122">Докато проектът е в етапа **План**, страницата **Обект на проекта** показва подробности за договора.</span><span class="sxs-lookup"><span data-stu-id="aa8be-122">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="aa8be-123">Доставяне</span><span class="sxs-lookup"><span data-stu-id="aa8be-123">Deliver</span></span>

<span data-ttu-id="aa8be-124">Когато планът на проекта е завършен и сте готови да стартирате проекта, мениджърът на проекта трябва да актуализира етапа на проекта на **Доставяне**, за да покаже, че проектът е стартиран.</span><span class="sxs-lookup"><span data-stu-id="aa8be-124">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="aa8be-125">Завършен</span><span class="sxs-lookup"><span data-stu-id="aa8be-125">Complete</span></span> 

<span data-ttu-id="aa8be-126">Когато работата по проекта е завършена, мениджърът на проекта може да актуализира етапа на **Завършено**.</span><span class="sxs-lookup"><span data-stu-id="aa8be-126">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="aa8be-127">Чрез актуализиране на етапа на проекта на **Завършен** мениджърът на проекта показва, че работата е 100% завършена, но че проектът се поддържа отворен, така че всички чакащи записи за време или разходи да могат да бъдат записани.</span><span class="sxs-lookup"><span data-stu-id="aa8be-127">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="aa8be-128">Затваряне</span><span class="sxs-lookup"><span data-stu-id="aa8be-128">Close</span></span>

<span data-ttu-id="aa8be-129">Когато всички транзакции бъдат записани за проекта, мениджърът на проекта може да актуализира етапа на **Затваряне**.</span><span class="sxs-lookup"><span data-stu-id="aa8be-129">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="aa8be-130">От този момент не могат да се записват транзакции и проектът се задава като само за четене.</span><span class="sxs-lookup"><span data-stu-id="aa8be-130">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]