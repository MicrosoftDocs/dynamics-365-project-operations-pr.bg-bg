---
title: Създаване на оферти по проект от възможности
description: Тази тема предоставя информация за създаването на оферта на проект от възможност.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 606098473db479d0015e3a7a3c01a3d3b6de9db1
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071732"
---
# <a name="create-project-quotes-from-opportunities"></a><span data-ttu-id="cced1-103">Създаване на оферти по проект от възможности</span><span class="sxs-lookup"><span data-stu-id="cced1-103">Create project quotes from opportunities</span></span>

<span data-ttu-id="cced1-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="cced1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cced1-105">Оферти могат да бъдат създадени от възможностите за проекти по следните начини:</span><span class="sxs-lookup"><span data-stu-id="cced1-105">Quotes can be created from project opportunities in the following ways:</span></span>

- <span data-ttu-id="cced1-106">От раздела **Оферти** на страницата **Възможност за проект**</span><span class="sxs-lookup"><span data-stu-id="cced1-106">From the **Quotes** tab on the **Project Opportunity** page</span></span>
- <span data-ttu-id="cced1-107">От потока на процеса на продажби на възможност</span><span class="sxs-lookup"><span data-stu-id="cced1-107">From the Opportunity sales process flow</span></span>
- <span data-ttu-id="cced1-108">Чрез актуализиране на референтната възможност за съществуваща оферта</span><span class="sxs-lookup"><span data-stu-id="cced1-108">By updating the opportunity reference on an existing quote</span></span>

## <a name="from-the-quotes-tab-of-the-project-opportunity-page"></a><span data-ttu-id="cced1-109">От раздела Оферти на страницата Възможност на проект</span><span class="sxs-lookup"><span data-stu-id="cced1-109">From the Quotes tab of the Project Opportunity page</span></span>

<span data-ttu-id="cced1-110">За да създадете оферта за проект от дадена възможност, изпълнете следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="cced1-110">To create a project quote from an opportunity, complete the following steps.</span></span>

1. <span data-ttu-id="cced1-111">Отворете страницата **Възможност на проект** и изберете раздела **Оферти**.</span><span class="sxs-lookup"><span data-stu-id="cced1-111">Open the **Project Opportunity** page and select the **Quotes** tab.</span></span> 
2. <span data-ttu-id="cced1-112">В подмрежата **Оферти** изберете **+** , за да създадете нова оферта за проект въз основа на възможността.</span><span class="sxs-lookup"><span data-stu-id="cced1-112">On the **Quotes** sub-grid, select the **+** to create a new project quote based on the opportunity.</span></span> <span data-ttu-id="cced1-113">Всички линии за възможности и свързаните с тях ценови листи на проекта се копират в новата оферта от възможността.</span><span class="sxs-lookup"><span data-stu-id="cced1-113">All of the opportunity lines and related Project price lists are copied to the new quote from the opportunity.</span></span>

## <a name="from-the-opportunity-sales-process-flow"></a><span data-ttu-id="cced1-114">От потока на процеса на продажби на възможност</span><span class="sxs-lookup"><span data-stu-id="cced1-114">From the Opportunity sales process flow</span></span>

<span data-ttu-id="cced1-115">За да създадете оферта от поток на процес на продажби на възможност, изпълнете следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="cced1-115">To create a quote from the Opportunity sales process flow, complete the following steps.</span></span>

1. <span data-ttu-id="cced1-116">От потока на процеса на продажба на възможност отворете възможността.</span><span class="sxs-lookup"><span data-stu-id="cced1-116">From the Opportunity sales process flow, open the Opportunity.</span></span>
2. <span data-ttu-id="cced1-117">Изберете етапа **Квалифициране**.</span><span class="sxs-lookup"><span data-stu-id="cced1-117">Select the **Qualify** stage.</span></span> 
3. <span data-ttu-id="cced1-118">Изберете **Напред** и след това изберете **+ Създаване** , за да създадете нова оферта.</span><span class="sxs-lookup"><span data-stu-id="cced1-118">Select **Next** and then select **+ Create** to create a new quote.</span></span> <span data-ttu-id="cced1-119">Повечето от информацията на раздела **Обобщение** за тази нова оферта ще бъде по подразбиране от възможността.</span><span class="sxs-lookup"><span data-stu-id="cced1-119">Most of the information on the **Summary** tab for this new quote will have defaulted from the opportunity.</span></span> 
4. <span data-ttu-id="cced1-120">Въведете липсващата необходима информация или актуализирайте стойностите по подразбиране, ако е необходимо, в раздела **Обобщение** ,</span><span class="sxs-lookup"><span data-stu-id="cced1-120">Enter in any required information that is missing, or update defaulted values as necessary on the **Summary** tab,</span></span>
5. <span data-ttu-id="cced1-121">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="cced1-121">Select **Save**.</span></span> <span data-ttu-id="cced1-122">Новата оферта е създадена и свързана с възможността.</span><span class="sxs-lookup"><span data-stu-id="cced1-122">The new quote is created and associated to the opportunity.</span></span> <span data-ttu-id="cced1-123">Вече можете да видите информацията за офертата на раздела **Оферти** на страницата **Възможност**.</span><span class="sxs-lookup"><span data-stu-id="cced1-123">You can now view the quote information on the **Quotes** tab of the **Opportunity** page.</span></span> 

   <span data-ttu-id="cced1-124">Процесът на продажба на възможност преминава към следващия етап **Предложение**.</span><span class="sxs-lookup"><span data-stu-id="cced1-124">The Opportunity sales process moves to the next stage, **Propose**.</span></span>


## <a name="by-updating-the-opportunity-reference-on-an-existing-quote"></a><span data-ttu-id="cced1-125">Чрез актуализиране на референтната възможност за съществуваща оферта</span><span class="sxs-lookup"><span data-stu-id="cced1-125">By updating the opportunity reference on an existing quote</span></span>

<span data-ttu-id="cced1-126">Съществуваща оферта може да бъде свързана с възможност.</span><span class="sxs-lookup"><span data-stu-id="cced1-126">An existing quote can be linked to an Opportunity.</span></span> <span data-ttu-id="cced1-127">Изпълнете следните стъпки, за да актуализирате информацията за възможността за съществуваща оферта.</span><span class="sxs-lookup"><span data-stu-id="cced1-127">Complete the following steps to update the Opportunity information on an existing quote.</span></span>

1. <span data-ttu-id="cced1-128">Отворете страницата **Оферта** и изберете раздела **Обобщение**.</span><span class="sxs-lookup"><span data-stu-id="cced1-128">Open the **Quote** page and select the **Summary** tab.</span></span>
2. <span data-ttu-id="cced1-129">В полето **Възможност** изберете възможността, която искате да свържете с офертата.</span><span class="sxs-lookup"><span data-stu-id="cced1-129">In the **Opportunity** field, select the opportunity that you want to link to the quote.</span></span> <span data-ttu-id="cced1-130">Можете да видите цитата в мрежата **Оферти** на възможността.</span><span class="sxs-lookup"><span data-stu-id="cced1-130">You can see the quote in the **Quotes** grid of the Opportunity.</span></span> 
3. <span data-ttu-id="cced1-131">Използвайки процеса на продажба на възможност, възможността може да бъде преместена на следващия етап **Предложение**.</span><span class="sxs-lookup"><span data-stu-id="cced1-131">Using the Opportunity sales process, the opportunity can be moved to the next stage, **Propose**.</span></span> 

   <span data-ttu-id="cced1-132">Когато преместите възможност на този етап, можете да изберете тази оферта от списък с оферти, свързани с тази възможност.</span><span class="sxs-lookup"><span data-stu-id="cced1-132">When you move an opportunity to this stage, you can select this quote from a list of quotes associated with this opportunity.</span></span> <span data-ttu-id="cced1-133">Избирането на тази оферта показва, че продължавате напред с нея.</span><span class="sxs-lookup"><span data-stu-id="cced1-133">Selecting this quote indicates that you're moving forward with it.</span></span>

   <span data-ttu-id="cced1-134">Всички останали оферти, свързани с Възможността, ще останат достъпни и активни, докато не бъде спечелена една от тях.</span><span class="sxs-lookup"><span data-stu-id="cced1-134">All the other quotes associated with the Opportunity will still be available and active until one of them is won.</span></span> <span data-ttu-id="cced1-135">Можете да върнете процеса на продажба обратно към предишния етап **Квалифициране** и изберете друга оферта, с която да продължите напред.</span><span class="sxs-lookup"><span data-stu-id="cced1-135">You can move the sales process back to the previous stage **Qualify** , and pick another quote to move forward with.</span></span>
