---
title: Определяне на календари на ресурси
description: Тази тема предоставя информация за това как да дефинирате календарите на работния час за ресурси в Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: daa49cf8ba9ba005a16777f590c4c06d024de529
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4123905"
---
# <a name="define-resource-calendars"></a><span data-ttu-id="a2bb9-103">Определяне на календари на ресурси</span><span class="sxs-lookup"><span data-stu-id="a2bb9-103">Define resource calendars</span></span>

<span data-ttu-id="a2bb9-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="a2bb9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a2bb9-105">Всеки резервиран ресурс, работещ по проект, трябва да има календар на работното време, за да определи тяхната наличност.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-105">Each bookable resource working on a project must have a calendar of working hours to define their availability.</span></span> <span data-ttu-id="a2bb9-106">Работното време за ресурс може да бъде дефинирано по два начина:</span><span class="sxs-lookup"><span data-stu-id="a2bb9-106">Workings hours for a resource can be defined in two ways:</span></span> 

   - <span data-ttu-id="a2bb9-107">Определете индивидуални календарни правила за ресурс</span><span class="sxs-lookup"><span data-stu-id="a2bb9-107">Define individual calendar rules for a resource</span></span>
   - <span data-ttu-id="a2bb9-108">Приложете съществуващ шаблон на календара за ресурса</span><span class="sxs-lookup"><span data-stu-id="a2bb9-108">Apply an existing calendar template for the resource</span></span>

## <a name="define-a-resources-working-hours"></a><span data-ttu-id="a2bb9-109">Определяне на работни часове на ресурс</span><span class="sxs-lookup"><span data-stu-id="a2bb9-109">Define a resource's working hours</span></span>

1. <span data-ttu-id="a2bb9-110">В менюто **Ресурси** изберете **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-110">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="a2bb9-111">От изгледа на мрежата изберете приложимото **Наличен ресурс**.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-111">From the grid view, select the applicable **Bookable Resource**.</span></span>
3. <span data-ttu-id="a2bb9-112">На страницата **Подробности за ресурса** изберете раздела **Работни часове**. По подразбиране календарът за резервируеми ресурси по подразбиране е работното време на шаблона за работен час по подразбиране, който е дефиниран за организацията.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-112">On the **Resource Details** page, select the **Working Hours** tab. By default, the bookable resources calendar defaults to the working hours of the default work hour template that is defined for the organization.</span></span>
4. <span data-ttu-id="a2bb9-113">За да актуализирате работното време, щракнете с десния бутон върху началната дата на предложеното правило на календара, което ще бъде определено.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-113">To update the working hours, right-click on the start date of the proposed calendar rule to be defined.</span></span> <span data-ttu-id="a2bb9-114">Използвайте менюто на правилото на календара, за да дефинирате правило на календара за определен ден, останалата част от поредицата или целия календар.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-114">Use the calendar rule menu to define a calendar rule for a specific day, the remainder of the series, or the entire calendar.</span></span>
5. <span data-ttu-id="a2bb9-115">След като опцията бъде избрана, можете да дефинирате:</span><span class="sxs-lookup"><span data-stu-id="a2bb9-115">After the option is selected, you can then define:</span></span>

    - <span data-ttu-id="a2bb9-116">Денят от седмицата, в който ще се прилага работното време.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-116">The day of the week where the working hours will apply.</span></span>
    - <span data-ttu-id="a2bb9-117">Работното време в рамките на всеки ден.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-117">The working times within each day.</span></span>
    - <span data-ttu-id="a2bb9-118">Часовата зона за правилото на календара.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-118">The time zone for the calendar rule.</span></span>
    - <span data-ttu-id="a2bb9-119">Ако е приложимо, неработно време също може да бъде посочено за правилото.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-119">If applicable, non-working time can also be specified for the rule.</span></span>

## <a name="applying-a-calendar-template-to-a-resource"></a><span data-ttu-id="a2bb9-120">Прилагане на шаблон на календар към ресурс</span><span class="sxs-lookup"><span data-stu-id="a2bb9-120">Applying a calendar template to a resource</span></span>

1. <span data-ttu-id="a2bb9-121">В менюто **Ресурси** изберете **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-121">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="a2bb9-122">От изгледа на мрежата изберете до 25 **Налични ресурси** да се актуализира.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-122">From the grid view, select up to 25 **Bookable Resources** to update.</span></span>
3. <span data-ttu-id="a2bb9-123">Изберете **Задаване на календар** и диалогов прозорец ще ви подкани със списък с наличните шаблони за работен час.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-123">Select **Set Calendar** and a dialog will prompt you with a list of available work hour templates.</span></span>
4. <span data-ttu-id="a2bb9-124">Изберете шаблона, който желаете да използвате, и след това изберете **Прилагане**.</span><span class="sxs-lookup"><span data-stu-id="a2bb9-124">Select the template you want to use, and then select **Apply**.</span></span>
