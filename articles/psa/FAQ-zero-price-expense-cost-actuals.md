---
title: Защото цената по подразбиране е нула за действителни данни на цена на разходи?
description: Отстраняване на причината защо дадена цена е по подразбиране 0 в действителни данни за цена на разход.
author: rumant
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 306f169ee25d42ac3c9e63fa70956b9c50315829
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122105"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a>Защото цената по подразбиране е нула за действителни данни на цена на разходи?

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Този често задаван въпрос се отнася за действителните данни за разходи, където класът на транзакция е зададен на „Разход” и типът на транзакция е „Разход”.

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a>Отстраняване на неизправност за ставки за разход в действителни стойности за цена на разход

Отидете на свързания запис на разход и се уверете, че има сума в полето за запис на разход. Ако първоначалният запис за разход няма попълнено поле за сума, сте изолирали проблема.
 
За да решите този проблем, създайте повторно записа за разход с валидна сума и го одобрете.
