---
title: Определяне на разходи за базирани на продукти редове на оферта
description: Тази тема предоставя информация за прилагането на себестойност към базиран на проект ред на оферта.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: d21ab159294cac66ffeb8abcf0943b4babd7b360
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4118910"
---
# <a name="costing-product-based-quote-lines"></a><span data-ttu-id="7b461-103">Определяне на разходи за базирани на продукти редове на оферта</span><span class="sxs-lookup"><span data-stu-id="7b461-103">Costing product-based quote lines</span></span>

<span data-ttu-id="7b461-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="7b461-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="7b461-105">Продуктово базирани редове на оферта в Dynamics 365 Project Operations също имат поле **себестойност**.</span><span class="sxs-lookup"><span data-stu-id="7b461-105">Product-based quote lines in Dynamics 365 Project Operations also have a **Cost Price** field.</span></span> <span data-ttu-id="7b461-106">Това поле се използва за проследяване на себестойността на продукта на реда на оферта и за изчисления на рентабилността надолу по веригата.</span><span class="sxs-lookup"><span data-stu-id="7b461-106">This field is used to track the cost price for the product on the quote line and for downstream profitability calculations.</span></span>

<span data-ttu-id="7b461-107">Когато за продукт от каталога се създава ред на оферта, базирана на продукта, цената на реда на оферта, базирана на продукта, е по подразбиране от **Стандартни разходи** поле в продуктовия каталог.</span><span class="sxs-lookup"><span data-stu-id="7b461-107">When a product-based quote line is created for a catalog product, the cost of the product-based quote line is defaulted from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="7b461-108">Полето за стандартни разходи в продуктовия каталог е настроено в основната валута на Организацията.</span><span class="sxs-lookup"><span data-stu-id="7b461-108">The standard cost field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="7b461-109">Единичната цена по подразбиране на продуктовата линия за котиране се преобразува във валутата на продажбите в офертата.</span><span class="sxs-lookup"><span data-stu-id="7b461-109">The default unit cost on the product-based quote line is converted to the sales currency on the quote.</span></span>

## <a name="unit-cost-on-a-product-based-quote-line"></a><span data-ttu-id="7b461-110">Разход за единица в базиран на продукт ред на оферта</span><span class="sxs-lookup"><span data-stu-id="7b461-110">Unit cost on a product-based quote line</span></span>

<span data-ttu-id="7b461-111">Целта да има единична себестойност на базирана на продукта линия за котиране е да се предвидят различни разходи за продукт за всяка продажба.</span><span class="sxs-lookup"><span data-stu-id="7b461-111">The purpose of having a unit cost on a product-based quote line is to allow for different costs for a product for each sale.</span></span> <span data-ttu-id="7b461-112">Това не е типичен сценарий, но понякога цената на продукта може да бъде намалена от доставчика в зависимост от клиента на окончателната продажба.</span><span class="sxs-lookup"><span data-stu-id="7b461-112">This is not a typical scenario, but sometimes the cost of the product may be discounted by the supplier depending on the customer of the final sale.</span></span>

<span data-ttu-id="7b461-113">Например:</span><span class="sxs-lookup"><span data-stu-id="7b461-113">For example:</span></span>

<span data-ttu-id="7b461-114">Fabrikam Robotics инсталира роботизирани оръжия на монтажните линии на A Datum Corporation.</span><span class="sxs-lookup"><span data-stu-id="7b461-114">Fabrikam Robotics is installing robotic arms at A Datum Corporation's assembly lines.</span></span> <span data-ttu-id="7b461-115">Fabrikam предоставя услуги за инсталиране, но роботизираните оръжия се доставят от роботиката на Trey.</span><span class="sxs-lookup"><span data-stu-id="7b461-115">Fabrikam provides installation services but the robotic arms are procured from Trey robotics.</span></span> <span data-ttu-id="7b461-116">Ако инсталирането на роботизирани оръжия в A Datum Corporation отвори нова индустриална вертикала за роботизираните оръжия на Trey, Trey може да даде специална отстъпка за тази сделка на Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="7b461-116">If the installation of robotic arms at A Datum Corporation opens a new industry vertical for Trey's robotic arms, Trey could give a special discount for this deal to Fabrikam.</span></span>

<span data-ttu-id="7b461-117">В този случай Fabrikam ще създаде базирана на продукта ред на оферта за Robotic Arms и ще въведе специална цена за единица за тази оферта.</span><span class="sxs-lookup"><span data-stu-id="7b461-117">In this case, Fabrikam will create product-based quote line for Robotic Arms and input a special per unit cost for this quote.</span></span> <span data-ttu-id="7b461-118">Тази цена се различава от стандартната цена на Trey Robotic Arms.</span><span class="sxs-lookup"><span data-stu-id="7b461-118">This cost is different from the standard cost of Trey Robotic Arms.</span></span>
