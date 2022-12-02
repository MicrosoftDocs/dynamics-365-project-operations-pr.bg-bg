---
title: Анализ на офертите по проекти
description: Тази статия предоставя информация за анализа на офертите по проекти.
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
ms.reviewer: johnmichalak
ms.openlocfilehash: 9db924c16c5eca17e7962ff1d88b09e581347fa5
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2022
ms.locfileid: "8919265"
---
# <a name="analysis-of-project-quotes"></a>Анализ на офертите по проекти

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Dynamics 365 Project Service Automation анализира офертите по проекти, за да изчисли рентабилността. Той също така анализира колко добре офертата е съобразена с очакванията на клиента за датата на доставка или датата на завършване, както и за бюджета.

## <a name="profitability-analysis"></a>Анализ на рентабилност

Project Service Automation анализира рентабилността, като използва брутния марж и коригирания брутен марж.

- Брутните маржове се изчисляват по следната формула:

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- Коригираният брутен марж се изчислява по следната формула:

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

Ако стойностите за брутния марж и коригирания брутен марж се различават с широк марж, голяма част от работата в офертата се класифицира като неплатима.

## <a name="analysis-of-customer-expectations"></a>Анализ на очакванията на клиента

Можете да анализирате офертите и да генерирате диаграми за очакванията на клиента за графика и бюджета, ако въведете стойности за следните полета:

- Полето **Заявена дата за доставка** в заглавката на офертата.
- Полето **Бюджет на клиента** за всеки ред на офертата (за базирани на проекти редове и базирани на продукти редове).

Анализът на очакванията на клиента за графика се извършва чрез сравняване на най-новата крайна дата на подробностите на реда на офертата със заявената дата на доставка във всички редове на офертата.

Анализът на очакванията на клиента за бюджета се извършва чрез сравняване на сбора от общия бюджет на клиента с оферираната сума от всички редове на офертата.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
