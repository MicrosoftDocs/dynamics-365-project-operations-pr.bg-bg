---
title: Разход за базирани на продукти аспекти на договор – олекотено
description: Тази тема предоставя информация за създаването
author: rumant
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 9458a57863244a68359f57185325c03a46bd6569
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003528"
---
# <a name="cost-product-based-contract-lines---lite"></a><span data-ttu-id="f46a3-103">Разход за базирани на продукти аспекти на договор – олекотено</span><span class="sxs-lookup"><span data-stu-id="f46a3-103">Cost product-based contract lines - lite</span></span>

<span data-ttu-id="f46a3-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="f46a3-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="f46a3-105">Продуктови договорни линии в Dynamics 365 Project Operations включват полето **Разходна цена**, което съхранява себестойността на продукта за изчисления на рентабилността надолу по веригата.</span><span class="sxs-lookup"><span data-stu-id="f46a3-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="f46a3-106">Когато се създава договорна линия, базирана на продукт, за каталожен продукт, цената на линията по подразбиране е от полето **Стандартни разходи** в продуктовия каталог.</span><span class="sxs-lookup"><span data-stu-id="f46a3-106">When a product-based contract line is created for a catalog product, the cost of the line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="f46a3-107">Полето **стандартни разходи** в продуктовия каталог е настроено в основната валута на Организацията.</span><span class="sxs-lookup"><span data-stu-id="f46a3-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="f46a3-108">Когато стойността на единицата по подразбиране е по договора, тя се преобразува във валутата на продажбите по договора.</span><span class="sxs-lookup"><span data-stu-id="f46a3-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="f46a3-109">Разход за единица в базирани на продукт аспекти на договор</span><span class="sxs-lookup"><span data-stu-id="f46a3-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="f46a3-110">Наличието на единична себестойност на базирани на продукта аспекти на договор позволява различни разходи за продукт за всяка продажба на единица.</span><span class="sxs-lookup"><span data-stu-id="f46a3-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="f46a3-111">Въпреки че не винаги е необходимо, има определени сценарии, при които цената на продукта може да бъде намалена за клиента от доставчика.</span><span class="sxs-lookup"><span data-stu-id="f46a3-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="f46a3-112">Помислете върху следния сценарий:</span><span class="sxs-lookup"><span data-stu-id="f46a3-112">Consider the following scenario:</span></span>

<span data-ttu-id="f46a3-113">Fabrikam Robotics инсталира роботизирани оръжия на монтажните линии на Adatum Corporation.</span><span class="sxs-lookup"><span data-stu-id="f46a3-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="f46a3-114">Fabrikam предоставя услуги за монтаж, но роботизираните оръжия са от Trey Research.</span><span class="sxs-lookup"><span data-stu-id="f46a3-114">Fabrikam provides installation services but the robotic arms are from Trey Research.</span></span> <span data-ttu-id="f46a3-115">Ако инсталирането на роботизирани оръжия в Adatum Corporation отвори нова индустриална вертикала за Trey Research, те могат да дадат специална отстъпка за тази сделка на Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="f46a3-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="f46a3-116">В този случай Fabrikam създава продуктова договорна линия за Robotic Arms.</span><span class="sxs-lookup"><span data-stu-id="f46a3-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms.</span></span> <span data-ttu-id="f46a3-117">За този договор се въвежда разход за единица.</span><span class="sxs-lookup"><span data-stu-id="f46a3-117">A per unit cost is entered for this contract.</span></span> <span data-ttu-id="f46a3-118">Цената е различна от цената на роботизираните оръжия от Trey Research.</span><span class="sxs-lookup"><span data-stu-id="f46a3-118">The cost is different from the cost of robotic arms from Trey Research.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]