---
title: Единици и опаковъчни единици
description: Тази тема предоставя информация за това как да създавате единици и опаковъчни единици в Dynamics 365 Project Operations.
author: rumant
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
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
ms.openlocfilehash: 646e20189efb4aab56972f01a52b1bff19f2e79f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996058"
---
# <a name="units-and-unit-groups"></a><span data-ttu-id="74d5e-103">Единици и опаковъчни единици</span><span class="sxs-lookup"><span data-stu-id="74d5e-103">Units and unit groups</span></span>

<span data-ttu-id="74d5e-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="74d5e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="74d5e-105">Единиците са количествата или мерни единици, в които продавате своите продукти или услуги.</span><span class="sxs-lookup"><span data-stu-id="74d5e-105">Units are the quantities or measurements that you sell your products or services in.</span></span> <span data-ttu-id="74d5e-106">Ако например продавате консумативи за градинарство, може да продавате семена в единици от пакети, кутии или палети.</span><span class="sxs-lookup"><span data-stu-id="74d5e-106">For example, if you sell gardening supplies, you might sell seeds in units of packets, boxes, and pallets.</span></span> <span data-ttu-id="74d5e-107">Опаковъчната единица е колекция от тези различни единици.</span><span class="sxs-lookup"><span data-stu-id="74d5e-107">A unit group is a collection of these different units.</span></span>

<span data-ttu-id="74d5e-108">За да изпълните стъпките в тази тема, уверете се, че сте били назначени за ролята на системен администратор или мениджър на Sales Professional или имате еквивалентни разрешения.</span><span class="sxs-lookup"><span data-stu-id="74d5e-108">To complete the steps in this topic, make sure that you have been assigned to the System Administrator or Sales Professional Manager role or have equivalent permissions.</span></span>

## <a name="create-a-unit-group"></a><span data-ttu-id="74d5e-109">Създаване на опаковъчна единица</span><span class="sxs-lookup"><span data-stu-id="74d5e-109">Create a unit group</span></span>

1. <span data-ttu-id="74d5e-110">В картата на сайта изберете **Единици**.</span><span class="sxs-lookup"><span data-stu-id="74d5e-110">In the site map, select **Units**.</span></span>
2. <span data-ttu-id="74d5e-111">Изберете **Създаване** и в **Създайте група единици** диалогов прозорец, въведете името на устройството.</span><span class="sxs-lookup"><span data-stu-id="74d5e-111">Select **New**, and in the **Create Unit Group** dialog box, enter the unit name.</span></span>
3. <span data-ttu-id="74d5e-112">В полето **Основна единица** въведете най-малката обща мерна единица, в която ще се продава продуктът.</span><span class="sxs-lookup"><span data-stu-id="74d5e-112">In the **Primary unit** field, enter the lowest common unit of measure that the product will be sold in.</span></span> <span data-ttu-id="74d5e-113">Например можете да въведете „парче“ или „унция“.</span><span class="sxs-lookup"><span data-stu-id="74d5e-113">For example, you might enter "piece" or "ounce".</span></span>
4. <span data-ttu-id="74d5e-114">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="74d5e-114">Select **OK**.</span></span>

## <a name="add-units-to-a-unit-group"></a><span data-ttu-id="74d5e-115">Добавяне на единици към опаковъчна единица</span><span class="sxs-lookup"><span data-stu-id="74d5e-115">Add units to a unit group</span></span>

1. <span data-ttu-id="74d5e-116">Отворете опаковъчна единица и в раздела **Свързани** изберете **Единици**.</span><span class="sxs-lookup"><span data-stu-id="74d5e-116">Open a unit group, and on the **Related** tab, select **Units**.</span></span> <span data-ttu-id="74d5e-117">Ще видите, че основната единица е вече добавена.</span><span class="sxs-lookup"><span data-stu-id="74d5e-117">You will see that the primary unit is already added.</span></span>
2. <span data-ttu-id="74d5e-118">Изберете **Добавяне на нова единица** и на страницата **Бързо създаване: единица** в полето **Име** въведете nanem на единицата.</span><span class="sxs-lookup"><span data-stu-id="74d5e-118">Select **Add New Unit**, and on the **Quick Create: Unit** page, in the **Name** field, enter the nanem of the unit.</span></span>
3. <span data-ttu-id="74d5e-119">В полето **Количество** въведете количеството, което ще съдържа единицата.</span><span class="sxs-lookup"><span data-stu-id="74d5e-119">In the **QUantity** field, enter the quantity that the unit will contain.</span></span> <span data-ttu-id="74d5e-120">Ако например едно поле съдържа два броя, въведете „2“.</span><span class="sxs-lookup"><span data-stu-id="74d5e-120">For example, if a box contains two pieces, enter "2".</span></span> 
4. <span data-ttu-id="74d5e-121">В полето **Базова единица** изберете базова единица, за да установите най-ниската мерна единица за единицата.</span><span class="sxs-lookup"><span data-stu-id="74d5e-121">In the **Base unit** field, select a base unit to establish the lowest unit of measurement for the unit.</span></span> <span data-ttu-id="74d5e-122">Например, можете да изберете „Парче“.</span><span class="sxs-lookup"><span data-stu-id="74d5e-122">For example, you might select "Piece".</span></span>
5. <span data-ttu-id="74d5e-123">Изберете **Записване**:</span><span class="sxs-lookup"><span data-stu-id="74d5e-123">Select **Save**:</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]