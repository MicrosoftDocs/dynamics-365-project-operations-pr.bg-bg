---
title: Прогнози за ресурс
description: Тази тема предоставя информация за това как се изчисляват прогнози в Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 98a61746f172b50bf6fa29cb0d21462cd616f417
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286505"
---
# <a name="resource-estimates"></a><span data-ttu-id="86acf-103">Прогнози за ресурс</span><span class="sxs-lookup"><span data-stu-id="86acf-103">Resource estimates</span></span>

<span data-ttu-id="86acf-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="86acf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="86acf-105">Оценките на ресурсите идват от усилията във времето, които са дефинирани в структурата на разбивка на работата, заедно с приложимите измерения на ценообразуването.</span><span class="sxs-lookup"><span data-stu-id="86acf-105">Resource estimates come from time-phased effort that is defined in the work breakdown structure along with applicable pricing dimensions.</span></span> <span data-ttu-id="86acf-106">Обикновено изчислението е **скорост/час за всяка роля x часа.**</span><span class="sxs-lookup"><span data-stu-id="86acf-106">Typically, the calculation is **rate/hr for each role x hours.**</span></span> <span data-ttu-id="86acf-107">Постепенното усилие за всеки ресурс се съхранява в записа за присвояване на ресурс.</span><span class="sxs-lookup"><span data-stu-id="86acf-107">The time-phased effort for each resource is stored in the resource assignment record.</span></span> <span data-ttu-id="86acf-108">Ценообразуването се съхранява в предварително дефинирана ценова листа.</span><span class="sxs-lookup"><span data-stu-id="86acf-108">The pricing is stored in a pre-defined price list.</span></span> <span data-ttu-id="86acf-109">Преобразуването на мерни единици се прилага въз основа на приложимия ценоразпис.</span><span class="sxs-lookup"><span data-stu-id="86acf-109">Unit conversion is applied based on the applicable price list.</span></span>

![Прогнози за ресурс](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a><span data-ttu-id="86acf-111">Цена и валута за разходи за разход по подразбиране</span><span class="sxs-lookup"><span data-stu-id="86acf-111">Default cost price and cost currency</span></span>

<span data-ttu-id="86acf-112">Разходните цени са по подразбиране от организационната единица.</span><span class="sxs-lookup"><span data-stu-id="86acf-112">Cost prices are defaulted from the Organizational Unit.</span></span>

## <a name="default-bill-rate-and-sales-currency"></a><span data-ttu-id="86acf-113">Стойност на сметката и валута на продажбите по подразбиране</span><span class="sxs-lookup"><span data-stu-id="86acf-113">Default bill rate and sales currency</span></span>

<span data-ttu-id="86acf-114">Продажните цени се прилагат веднъж за сделка.</span><span class="sxs-lookup"><span data-stu-id="86acf-114">Sales prices are applied once per deal.</span></span> <span data-ttu-id="86acf-115">Йерархията по подразбиране на ценовата листа за продажба е следната:</span><span class="sxs-lookup"><span data-stu-id="86acf-115">The hierarchy for sale price list defaulting is as follows:</span></span>

1. <span data-ttu-id="86acf-116">Организация</span><span class="sxs-lookup"><span data-stu-id="86acf-116">Organization</span></span>
2. <span data-ttu-id="86acf-117">Клиент</span><span class="sxs-lookup"><span data-stu-id="86acf-117">Customer</span></span>
3. <span data-ttu-id="86acf-118">Оферта/договор</span><span class="sxs-lookup"><span data-stu-id="86acf-118">Quote/contract</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]