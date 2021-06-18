---
title: Защото цената по подразбиране е нула за действителни данни на цена на разходи?
description: Отстраняване на причината защо дадена цена е по подразбиране 0 в действителни данни за цена на разход.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 8/22/2018
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
ms.openlocfilehash: 03c958635dec66b0f243872dfb929eba6a20119b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5992687"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="de174-103">Защо цената по подразбиране е нула в действителните данни за стойност на разход</span><span class="sxs-lookup"><span data-stu-id="de174-103">Why is the price defaulting to zero on expense cost actuals</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="de174-104">Този често задаван въпрос се отнася за действителните данни за разходи, където класът на транзакция е зададен на „Разход” и типът на транзакция е „Разход”.</span><span class="sxs-lookup"><span data-stu-id="de174-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="de174-105">Отстраняване на неизправност за ставки за разход в действителни стойности за цена на разход</span><span class="sxs-lookup"><span data-stu-id="de174-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="de174-106">Отидете на свързания запис на разход и се уверете, че има сума в полето за запис на разход.</span><span class="sxs-lookup"><span data-stu-id="de174-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="de174-107">Ако първоначалният запис за разход няма попълнено поле за сума, сте изолирали проблема.</span><span class="sxs-lookup"><span data-stu-id="de174-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="de174-108">За да решите този проблем, създайте повторно записа за разход с валидна сума и го одобрете.</span><span class="sxs-lookup"><span data-stu-id="de174-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]