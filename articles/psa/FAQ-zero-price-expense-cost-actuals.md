---
title: Защото цената по подразбиране е нула за действителни данни на цена на разходи?
description: Отстраняване на причината защо дадена цена е по подразбиране 0 в действителни данни за цена на разход.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 9f4ff8a96250d675faeda3246c2d0a6c5bd83286
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071841"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="1852c-103">Защото цената по подразбиране е нула за действителни данни на цена на разходи?</span><span class="sxs-lookup"><span data-stu-id="1852c-103">Why is the price defaulting to zero on expense cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="1852c-104">Този често задаван въпрос се отнася за действителните данни за разходи, където класът на транзакция е зададен на „Разход” и типът на транзакция е „Разход”.</span><span class="sxs-lookup"><span data-stu-id="1852c-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="1852c-105">Отстраняване на неизправност за ставки за разход в действителни стойности за цена на разход</span><span class="sxs-lookup"><span data-stu-id="1852c-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="1852c-106">Отидете на свързания запис на разход и се уверете, че има сума в полето за запис на разход.</span><span class="sxs-lookup"><span data-stu-id="1852c-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="1852c-107">Ако първоначалният запис за разход няма попълнено поле за сума, сте изолирали проблема.</span><span class="sxs-lookup"><span data-stu-id="1852c-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="1852c-108">За да решите този проблем, създайте повторно записа за разход с валидна сума и го одобрете.</span><span class="sxs-lookup"><span data-stu-id="1852c-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
