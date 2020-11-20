---
title: Разход за базирани на продукти аспекти на договор – олекотено
description: Тази тема предоставя информация за създаването
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 0e961bcf32a5dd662b7cd27a23eb5f664c45c292
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177228"
---
# <a name="cost-product-based-contract-lines---lite"></a><span data-ttu-id="bba3b-103">Разход за базирани на продукти аспекти на договор – олекотено</span><span class="sxs-lookup"><span data-stu-id="bba3b-103">Cost product-based contract lines - lite</span></span>

<span data-ttu-id="bba3b-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="bba3b-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="bba3b-105">Продуктово базирани договорни линии в Dynamics 365 Project Operations включват **Разходна цена** поле, което съхранява себестойността на продукта за изчисления на рентабилността надолу по веригата.</span><span class="sxs-lookup"><span data-stu-id="bba3b-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="bba3b-106">Когато за продукт от каталога се създават аспекти на договор, базирана на продукта, цената на аспекти на договор, базирани на продукта, е по подразбиране от **Стандартни разходи** поле в продуктовия каталог.</span><span class="sxs-lookup"><span data-stu-id="bba3b-106">When a product-based contract line is created for a catalog product, the cost of the product-based contract line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="bba3b-107">Полето **стандартни разходи** в продуктовия каталог е настроено в основната валута на Организацията.</span><span class="sxs-lookup"><span data-stu-id="bba3b-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="bba3b-108">Когато стойността на единицата по подразбиране е по договора, тя се преобразува във валутата на продажбите по договора.</span><span class="sxs-lookup"><span data-stu-id="bba3b-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="bba3b-109">Разход за единица в базирани на продукт аспекти на договор</span><span class="sxs-lookup"><span data-stu-id="bba3b-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="bba3b-110">Наличието на единична себестойност на базирани на продукта аспекти на договор позволява различни разходи за продукт за всяка продажба на единица.</span><span class="sxs-lookup"><span data-stu-id="bba3b-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="bba3b-111">Въпреки че не винаги е необходимо, има определени сценарии, при които цената на продукта може да бъде намалена за клиента от доставчика.</span><span class="sxs-lookup"><span data-stu-id="bba3b-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="bba3b-112">Помислете върху следния сценарий:</span><span class="sxs-lookup"><span data-stu-id="bba3b-112">Consider the following scenario:</span></span>

<span data-ttu-id="bba3b-113">Fabrikam Robotics инсталира роботизирани оръжия на монтажните линии на Adatum Corporation.</span><span class="sxs-lookup"><span data-stu-id="bba3b-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="bba3b-114">Fabrikam предоставя услуги за инсталиране, но роботизираните оръжия се доставят от Trey Research.</span><span class="sxs-lookup"><span data-stu-id="bba3b-114">Fabrikam provides installation services but the robotic arms are procured from Trey Research.</span></span> <span data-ttu-id="bba3b-115">Ако инсталирането на роботизирани оръжия в Adatum Corporation отвори нова индустриална вертикала за Trey Research, те могат да дадат специална отстъпка за тази сделка на Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="bba3b-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="bba3b-116">В този случай Fabrikam създава продуктова договорна линия за Robotic Arms и въвежда разходи за единица за този договор, които са различни от стандартните разходи за роботизирани оръжия от Trey Research.</span><span class="sxs-lookup"><span data-stu-id="bba3b-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms and inputs a per unit cost for this contract that is different from the standard cost of robotic arms from Trey Research.</span></span>
