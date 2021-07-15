---
title: Общ преглед на асистента на графика
description: Тази тема предоставя информация за работа с асистента по график за резервиране на ресурси.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.custom: intro-internal
ms.openlocfilehash: 83583c97e4ecb5f1fdc0d8d98098afe8e12d27e4
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368103"
---
# <a name="schedule-assistant-overview"></a><span data-ttu-id="134b9-103">Общ преглед на асистента на графика</span><span class="sxs-lookup"><span data-stu-id="134b9-103">Schedule assistant overview</span></span>

<span data-ttu-id="134b9-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="134b9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="134b9-105">Асистентът по график се използва за резервиране на ресурси въз основа на изисквания, дефинирани от ръководителя на проекта.</span><span class="sxs-lookup"><span data-stu-id="134b9-105">The Schedule assistant is used to book resources based on requirements defined by the Project manager.</span></span> <span data-ttu-id="134b9-106">Асистентът по график разчита на параметрите, предоставени в изискването за ресурс, за да намери ресурса.</span><span class="sxs-lookup"><span data-stu-id="134b9-106">The schedule assistant relies on the parameters provided in the resource requirement to find the resource.</span></span> <span data-ttu-id="134b9-107">Асистентът по график препоръчва ресурси, които отговарят на съответните изисквания, като например времеви прозорци или необходими умения.</span><span class="sxs-lookup"><span data-stu-id="134b9-107">The Schedule assistant recommends resources that match relevant requirements, like time windows or skills needed.</span></span>

<span data-ttu-id="134b9-108">След като бъдат идентифицирани подходящи ресурси, мениджърът на ресурса или проекта може да резервира ресурса към произведението.</span><span class="sxs-lookup"><span data-stu-id="134b9-108">After suitable resources are identified, the Resource or Project manager can book the resource to the work.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="134b9-109">Предварителни изисквания</span><span class="sxs-lookup"><span data-stu-id="134b9-109">Prerequisites</span></span>

<span data-ttu-id="134b9-110">Асистентът по график е част от решение Universal Resource Scheduling.</span><span class="sxs-lookup"><span data-stu-id="134b9-110">The Schedule assistant is a part of the Universal Resource Scheduling solution.</span></span> <span data-ttu-id="134b9-111">Това решение е включено и инсталирано с Dynamics 365 Project Operations, Dynamics 365 Field Service и Dynamics 365 Customer Service.</span><span class="sxs-lookup"><span data-stu-id="134b9-111">This solution is included and installed with Dynamics 365 Project Operations, Dynamics 365 Field Service, and Dynamics 365 Customer Service.</span></span>

## <a name="matching-requirements-and-resources"></a><span data-ttu-id="134b9-112">Свързване на изисквания и ресурси</span><span class="sxs-lookup"><span data-stu-id="134b9-112">Matching requirements and resources</span></span>

<span data-ttu-id="134b9-113">Изискването за генериран ресурс се основава на подробности като:</span><span class="sxs-lookup"><span data-stu-id="134b9-113">A generated resource requirement is based on details such as:</span></span>

-   <span data-ttu-id="134b9-114">Характеристики</span><span class="sxs-lookup"><span data-stu-id="134b9-114">Characteristics</span></span>
-   <span data-ttu-id="134b9-115">Роли</span><span class="sxs-lookup"><span data-stu-id="134b9-115">Roles</span></span>
-   <span data-ttu-id="134b9-116">Бизнес единици</span><span class="sxs-lookup"><span data-stu-id="134b9-116">Business units</span></span>
-   <span data-ttu-id="134b9-117">Предпочитания за ресурси</span><span class="sxs-lookup"><span data-stu-id="134b9-117">Resource preferences</span></span>
-   <span data-ttu-id="134b9-118">Контури за усилие</span><span class="sxs-lookup"><span data-stu-id="134b9-118">Effort contours</span></span>
-   <span data-ttu-id="134b9-119">Часова зона</span><span class="sxs-lookup"><span data-stu-id="134b9-119">Time zone</span></span>

<span data-ttu-id="134b9-120">Асистентът по график използва тези подробности за филтриране на ресурси.</span><span class="sxs-lookup"><span data-stu-id="134b9-120">The Schedule assistant uses these details to filter resources.</span></span>

## <a name="launch-the-schedule-assistant"></a><span data-ttu-id="134b9-121">Стартиране на асистента на графика</span><span class="sxs-lookup"><span data-stu-id="134b9-121">Launch the Schedule assistant</span></span>

<span data-ttu-id="134b9-122">Има два начина, по които се стартира асистентът по график.</span><span class="sxs-lookup"><span data-stu-id="134b9-122">There are two ways in which the schedule assistant is launched.</span></span> <span data-ttu-id="134b9-123">Ако използвате хибридния режим, в мрежата на члена на екипа можете да изберете всеки член на екипа с неизпълнено изискване за ресурси и след това да изберете **Резервация**.</span><span class="sxs-lookup"><span data-stu-id="134b9-123">If you're using the hybrid mode, in the team member grid you can select any team member with an unfulfilled resource requirement, and then select **Book**.</span></span> <span data-ttu-id="134b9-124">Ако използвате централния режим, мениджърът на ресурси намира и избира ресурса.</span><span class="sxs-lookup"><span data-stu-id="134b9-124">If you're using the central mode, the Resource manager finds and selects the resource.</span></span>

## <a name="schedule-assistant-filters"></a><span data-ttu-id="134b9-125">Филтри на асистента за планиране</span><span class="sxs-lookup"><span data-stu-id="134b9-125">Schedule assistant filters</span></span>

<span data-ttu-id="134b9-126">След като асистентът по график стартира, подробностите от изискването за ресурс се показват като филтрирани стойности в левия прозорец.</span><span class="sxs-lookup"><span data-stu-id="134b9-126">After the Schedule assistant runs, the details from the resource requirement are displayed as filtered values in the left pane.</span></span> <span data-ttu-id="134b9-127">Мениджърът на ресурси или мениджърът на проекти може да прецизира резултатите, като коригира филтрите, за да отговори на нуждите от планиране.</span><span class="sxs-lookup"><span data-stu-id="134b9-127">The Resource manager or the Project manager can fine-tune results by adjusting filters to meet the scheduling needs.</span></span>

<span data-ttu-id="134b9-128">Филтърният прозорец показва опции, свързани с работата, включително:</span><span class="sxs-lookup"><span data-stu-id="134b9-128">The filter pane shows work-related options, including:</span></span>

-   <span data-ttu-id="134b9-129">Начало и край на работата</span><span class="sxs-lookup"><span data-stu-id="134b9-129">Work start and end</span></span>
-   <span data-ttu-id="134b9-130">Характеристики</span><span class="sxs-lookup"><span data-stu-id="134b9-130">Characteristics</span></span>
-   <span data-ttu-id="134b9-131">Роли</span><span class="sxs-lookup"><span data-stu-id="134b9-131">Roles</span></span>
-   <span data-ttu-id="134b9-132">Организационни единици</span><span class="sxs-lookup"><span data-stu-id="134b9-132">Organizational units</span></span>
-   <span data-ttu-id="134b9-133">Ресурсна фирма</span><span class="sxs-lookup"><span data-stu-id="134b9-133">Resourcing company</span></span>
-   <span data-ttu-id="134b9-134">Типове ресурси</span><span class="sxs-lookup"><span data-stu-id="134b9-134">Resource types</span></span>
-   <span data-ttu-id="134b9-135">Предпочитани ресурси</span><span class="sxs-lookup"><span data-stu-id="134b9-135">Preferred resources</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]