---
title: Настройка на ценова листа за продажби
description: Тази тема предоставя информация за ценови листи на продажби за ценообразуване на проект.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: 2a66802adfcadab7b4d34149b146ca3cb27c903e
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896448"
---
# <a name="sales-price-list-setup"></a><span data-ttu-id="a3afd-103">Настройка на ценова листа за продажби</span><span class="sxs-lookup"><span data-stu-id="a3afd-103">Sales price list setup</span></span>

<span data-ttu-id="a3afd-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="a3afd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a3afd-105">За проектни оферти и договори ценовата листа на проекта има различен модел на заместване на цените от продуктова ценова листа.</span><span class="sxs-lookup"><span data-stu-id="a3afd-105">For project quotes and contracts, a project price list has a different price override pattern than a product price list.</span></span> <span data-ttu-id="a3afd-106">В ред на оферта, базиран на продуктов каталог, можете да заместите цената с роли и категории директно в реда на офертата, защото всеки ред на офертата сочи към точно един елемент от каталога.</span><span class="sxs-lookup"><span data-stu-id="a3afd-106">On a product catalog–based quote line, you can override the price to roles and categories directly on the quote line, because each quote line points to exactly one catalog item.</span></span> <span data-ttu-id="a3afd-107">В ред на оферта, базиран на проект, обаче не можете да заместите цената с роли и категории директно в реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="a3afd-107">However, on a project-based quote line, you can't override the price to roles and categories directly on the quote line.</span></span> <span data-ttu-id="a3afd-108">Можете да използвате ценовата листа на проекта за работа с двата различни модела за отмяна.</span><span class="sxs-lookup"><span data-stu-id="a3afd-108">You can use the project price list to work with the two distinct override patterns.</span></span>

> [!NOTE]
> <span data-ttu-id="a3afd-109">Препоръчваме ви да имате отделна ценова листа за ресурсите за проекта и елементите от каталога поради разликите в поведението между двете, когато замествате ценообразуването.</span><span class="sxs-lookup"><span data-stu-id="a3afd-109">We recommend that you have a separate price list for your project resources and your catalog items, because of the behavior differences between the two when you override pricing.</span></span>

<span data-ttu-id="a3afd-110">Всеки от следните обекти може да има една или повече свързани ценови списъци за продажби за ценообразуване на проекта:</span><span class="sxs-lookup"><span data-stu-id="a3afd-110">Each of the following entities can have one or more associated sales price lists for project pricing:</span></span>

- <span data-ttu-id="a3afd-111">Клиент (акаунт)</span><span class="sxs-lookup"><span data-stu-id="a3afd-111">Customer (account)</span></span> 
- <span data-ttu-id="a3afd-112">Възможност</span><span class="sxs-lookup"><span data-stu-id="a3afd-112">Opportunity</span></span> 
- <span data-ttu-id="a3afd-113">Оферта</span><span class="sxs-lookup"><span data-stu-id="a3afd-113">Quote</span></span> 
- <span data-ttu-id="a3afd-114">Договор по проект</span><span class="sxs-lookup"><span data-stu-id="a3afd-114">Project Contract</span></span>

<span data-ttu-id="a3afd-115">Свързването на тези обекти с ценова листа се посочва от ценовите листи на проекта.</span><span class="sxs-lookup"><span data-stu-id="a3afd-115">The association of these entities with a price list is indicated by the project price lists.</span></span> <span data-ttu-id="a3afd-116">Можете да свържете една или повече ценови листи с обектите за продажби „Клиент“, „Възможност“, „Оферта“ и „Договор по проект“.</span><span class="sxs-lookup"><span data-stu-id="a3afd-116">You can associate one or more price lists with the Customer, Opportunity, Quote, and Project Contract sales entities.</span></span>

<span data-ttu-id="a3afd-117">Ценовата листа на проекта по подразбиране не се въвежда автоматично в запис на клиент.</span><span class="sxs-lookup"><span data-stu-id="a3afd-117">A default project price list isn't automatically entered on a customer record.</span></span> <span data-ttu-id="a3afd-118">Можете обаче ръчно да прикачите ценова листа на проект към записа на клиент.</span><span class="sxs-lookup"><span data-stu-id="a3afd-118">However, you can manually attach a project price list to the customer record.</span></span> <span data-ttu-id="a3afd-119">Въпреки това обаче трябва ръчно да прикачите ценова листа на проекта само когато имате споразумение за персонализирано ценообразуване с клиента.</span><span class="sxs-lookup"><span data-stu-id="a3afd-119">Nevertheless, you should manually attach a project price list only when you have a custom pricing agreement with the customer.</span></span> 

<span data-ttu-id="a3afd-120">Когато ценова листа на проект се прикачи към обект за продажби, се проверява следната информация:</span><span class="sxs-lookup"><span data-stu-id="a3afd-120">When a project price list is attached to a sales entity, the following information is validated:</span></span>

- <span data-ttu-id="a3afd-121">Ценовата листа има контекст на **Продажби**.</span><span class="sxs-lookup"><span data-stu-id="a3afd-121">The price list has a context of **Sales**.</span></span> 
- <span data-ttu-id="a3afd-122">Валутата на ценовата листа съвпада с валутата на клиента.</span><span class="sxs-lookup"><span data-stu-id="a3afd-122">The price list currency matches the customer currency.</span></span> 

<span data-ttu-id="a3afd-123">В договор по проект следният ред на приоритет се използва за автоматично задаване на свързани ценови списъци на проекта:</span><span class="sxs-lookup"><span data-stu-id="a3afd-123">On a project contract, the following order of precedence is used to automatically set related project price lists:</span></span>

1. <span data-ttu-id="a3afd-124">Оферта</span><span class="sxs-lookup"><span data-stu-id="a3afd-124">Quote</span></span>
2. <span data-ttu-id="a3afd-125">Възможност</span><span class="sxs-lookup"><span data-stu-id="a3afd-125">Opportunity</span></span>
3. <span data-ttu-id="a3afd-126">Клиент</span><span class="sxs-lookup"><span data-stu-id="a3afd-126">Customer</span></span> 
4. <span data-ttu-id="a3afd-127">Глобални настройки</span><span class="sxs-lookup"><span data-stu-id="a3afd-127">Global settings</span></span> 

<span data-ttu-id="a3afd-128">Когато ценова листа се въведе по подразбиране, системата проверява дали валутата съвпада с валутата на клиента и дали ценовите списъци по подразбиране, които са били въведени, имат контекст на **Продажби**.</span><span class="sxs-lookup"><span data-stu-id="a3afd-128">When a project price list is entered by default, the system validates that the currency matches the customer’s currency, and that the default price lists that have been entered have a context of **Sales**.</span></span>

<span data-ttu-id="a3afd-129">Можете да свържете няколко ценови листи на проекта с обектите „Клиент“, „Възможност“, „Оферта“ и „Договор по проект“.</span><span class="sxs-lookup"><span data-stu-id="a3afd-129">You can associate multiple project price lists with the Customer, Opportunity, Quote, and Project Contract entities.</span></span> <span data-ttu-id="a3afd-130">Тази възможност поддържа специфични за датата цени по подразбиране за дългосрочен договор по проект, където може да изисквате повече от една ценова листа, за да се вземат предвид актуализации на цените, които настъпват поради инфлация.</span><span class="sxs-lookup"><span data-stu-id="a3afd-130">This capability supports date-specific default prices for a long-running project contract, where you might require more than one price list to account for price updates that occur because of inflation.</span></span> <span data-ttu-id="a3afd-131">Въпреки това, ако ценовите листи, които свързвате с обекта „Клиент“, „Възможност“, „Оферта“ или „Договор по проект“ имат припокриване по дата на влизане в сила, цените по подразбиране може да са неправилни.</span><span class="sxs-lookup"><span data-stu-id="a3afd-131">However, if the price lists that you associate with the Customer, Opportunity, Quote, or Project Contract entity have overlapping date effectivity, the default prices might be incorrect.</span></span> <span data-ttu-id="a3afd-132">Затова трябва да се уверите, че ценови списъци на проекта, които имат припокриване по дата на влизане в сила, не са свързани с тези обекти.</span><span class="sxs-lookup"><span data-stu-id="a3afd-132">Therefore, you should make sure that project price lists that have overlapping date effectivity aren't associated with those entities.</span></span>
