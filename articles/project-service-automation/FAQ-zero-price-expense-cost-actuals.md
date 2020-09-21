---
title: Защото цената по подразбиране е нула за действителни данни на цена на разходи?
description: Отстраняване на причината защо дадена цена е по подразбиране 0 в действителни данни за цена на разход.
author: rumant
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 8/22/2018
ms.topic: article
ms.prod: Project Service
ms.technology: ''
ms.assetid: bc1ebc58-c733-4310-8435-572ed9a9fef9
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 3fb678822877a61d141de75aea29b7d5cdf292c4
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749277"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a>Защото цената по подразбиране е нула за действителни данни на цена на разходи?

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Този често задаван въпрос се отнася за действителните данни за разходи, където класът на транзакция е зададен на „Разход” и типът на транзакция е „Разход”.

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a>Отстраняване на неизправност за ставки за разход в действителни стойности за цена на разход

Отидете на свързания запис на разход и се уверете, че има сума в полето за запис на разход. Ако първоначалният запис за разход няма попълнено поле за сума, сте изолирали проблема.
 
За да решите този проблем, създайте повторно записа за разход с валидна сума и го одобрете.
