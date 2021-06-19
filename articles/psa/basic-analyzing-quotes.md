---
title: Анализ на офертите по проекти
description: Тази тема предоставя информация за анализа на офертите по проекти.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: acb3f1a2020cfd59f60f828e9092bd7ccde00077
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012438"
---
# <a name="analysis-of-project-quotes"></a><span data-ttu-id="cad16-103">Анализ на офертите по проекти</span><span class="sxs-lookup"><span data-stu-id="cad16-103">Analysis of project quotes</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="cad16-104">Dynamics 365 Project Service Automation анализира офертите по проекти, за да изчисли рентабилността.</span><span class="sxs-lookup"><span data-stu-id="cad16-104">Dynamics 365 Project Service Automation analyzes project quotes to estimate profitability.</span></span> <span data-ttu-id="cad16-105">Той също така анализира колко добре офертата е съобразена с очакванията на клиента за датата на доставка или датата на завършване, както и за бюджета.</span><span class="sxs-lookup"><span data-stu-id="cad16-105">It also analyzes how well the quote is aligned with customer expectations about the delivery date or completion date, and about the budget.tions.</span></span>

## <a name="profitability-analysis"></a><span data-ttu-id="cad16-106">Анализ на рентабилност</span><span class="sxs-lookup"><span data-stu-id="cad16-106">Profitability analysis</span></span>

<span data-ttu-id="cad16-107">Project Service Automation анализира рентабилността, като използва брутния марж и коригирания брутен марж.</span><span class="sxs-lookup"><span data-stu-id="cad16-107">Project Service Automation analyzes profitability by using the gross margin and the adjusted gross margin.</span></span>

- <span data-ttu-id="cad16-108">Брутните маржове се изчисляват по следната формула:</span><span class="sxs-lookup"><span data-stu-id="cad16-108">Gross margins are calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- <span data-ttu-id="cad16-109">Коригираният брутен марж се изчислява по следната формула:</span><span class="sxs-lookup"><span data-stu-id="cad16-109">The adjusted gross margin is calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

<span data-ttu-id="cad16-110">Ако стойностите за брутния марж и коригирания брутен марж се различават с широк марж, голяма част от работата в офертата се класифицира като неплатима.</span><span class="sxs-lookup"><span data-stu-id="cad16-110">If the values for gross margin and adjusted gross margin differ by a wide margin, much of the work in the quote is classified as non-chargeable.</span></span>

## <a name="analysis-of-customer-expectations"></a><span data-ttu-id="cad16-111">Анализ на очакванията на клиента</span><span class="sxs-lookup"><span data-stu-id="cad16-111">Analysis of customer expectations</span></span>

<span data-ttu-id="cad16-112">Можете да анализирате офертите и да генерирате диаграми за очакванията на клиента за графика и бюджета, ако въведете стойности за следните полета:</span><span class="sxs-lookup"><span data-stu-id="cad16-112">You can analyze quotes and generate charts for customer expectations about the schedule and budget if you enter values for the following fields:</span></span>

- <span data-ttu-id="cad16-113">Полето **Заявена дата за доставка** в заглавката на офертата.</span><span class="sxs-lookup"><span data-stu-id="cad16-113">The **Requested delivery date** field on the quote header.</span></span>
- <span data-ttu-id="cad16-114">Полето **Бюджет на клиента** за всеки ред на офертата (за базирани на проекти редове и базирани на продукти редове).</span><span class="sxs-lookup"><span data-stu-id="cad16-114">The **Customer budget** field for each quote line (for project-based lines and product-based lines).</span></span>

<span data-ttu-id="cad16-115">Анализът на очакванията на клиента за графика се извършва чрез сравняване на най-новата крайна дата на подробностите на реда на офертата със заявената дата на доставка във всички редове на офертата.</span><span class="sxs-lookup"><span data-stu-id="cad16-115">Analysis of customer expectations about the schedule is done by comparing the latest end date of the quote line detail with the requested delivery date across all quote lines in the quote.</span></span>

<span data-ttu-id="cad16-116">Анализът на очакванията на клиента за бюджета се извършва чрез сравняване на сбора от общия бюджет на клиента с оферираната сума от всички редове на офертата.</span><span class="sxs-lookup"><span data-stu-id="cad16-116">Analysis of customer expectations about the budget is done by comparing the sum of the total customer budget with the quoted amount across all quote lines.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]