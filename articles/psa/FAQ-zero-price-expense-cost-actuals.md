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
ms.openlocfilehash: a6e971ff0477d5a9cb8652541095538b9f9039c0870362077218df609871ed4f
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/06/2021
ms.locfileid: "6990933"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a>Защо цената по подразбиране е нула в действителните данни за стойност на разход

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Този често задаван въпрос се отнася за действителните данни за разходи, където класът на транзакция е зададен на „Разход” и типът на транзакция е „Разход”.

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a>Отстраняване на неизправност за ставки за разход в действителни стойности за цена на разход

Отидете на свързания запис на разход и се уверете, че има сума в полето за запис на разход. Ако първоначалният запис за разход няма попълнено поле за сума, сте изолирали проблема.
 
За да решите този проблем, създайте повторно записа за разход с валидна сума и го одобрете.


[!INCLUDE[footer-include](../includes/footer-banner.md)]