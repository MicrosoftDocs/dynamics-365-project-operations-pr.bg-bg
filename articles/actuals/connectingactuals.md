---
title: Връзки за трансакции – Свързване на действителните данни от различни типове трансакции
description: В тази статия се обяснява как се използва връзка за транзакция, за да се свържат действителните данни от различни типове, за да се помогне за проследяване на рентабилността, изоставането при таксуване и таксуването спрямо небитирани изчисления на приходите.
author: rumant
ms.date: 03/25/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 19a78336099f54c5d6b36a963a90b9fd77e3d0af
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2022
ms.locfileid: "8926073"
---
# <a name="transaction-connections---link-actuals-of-different-transaction-types"></a>Връзки за трансакции – Свързване на действителните данни от различни типове трансакции

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

Записите за свързване на транзакции се създават, за да свържат действителните данни от различни видове, тъй като времето, разходите или използването на материали се движат в жизнения му цикъл от етапа на офертата или предварителната продажба с етапа на договора, одобренията и/или иззетилата, фактурирането и потенциално кредитното или коригиращото фактуриране.

Следващият пример показва типичната обработка на записи за време в жизнения цикъл на проекта в Project Operations.

> ![Записи за време за обработка в Операции по проекта.](media/basic-guide-17.png)

Обработката на записи за време в жизнен цикъл на проект операции проект следва тези стъпки: 

1. Подаването на запис за време води до създаване на два реда от дневника: един за разходи и един за небитирани продажби. 
2. Евентуалното одобрение на записа за време води до създаване на два действителни: един за разходи и един за небитирани продажби. Тези 2 действителни са свързани с помощта на транзакции връзки.
3. Когато потребителят създава фактура за проект, транзакцията на реда на фактура се създава с помощта на действителните данни за нефактурирани продажби.
4. Когато фактурата е потвърдена, това създава два нови действителни: небитирано обръщане на продажби и фактурирана продажба действителна. Небитираният реверниране на продажбите и оригиналният небитиран действителен продажби са свързани с помощта на връзки за заден ход на транзакции. Фактурирани продажби и оригиналните небитирани продажби действителни също са свързани, за да се покажат връзките между това, което някога е било изоставане или незавършено (НП) приходи към това, което сега се фактурира приходи.   

Всяко събитие в работния поток за обработка задейства създаването на записи в таблицата **Транзакция връзка**. Това помага да се изгради следа от релации между записите, които са създадени през време запис, ред от дневник, действителни и фактура ред подробности.

Следната таблица показва записите в **обекта транзакция връзка** за предходния работен поток.

|Събитие                   |Транзакция 1                 |Роля на транзакция 1 |Тип на транзакция 1       |Транзакция 2          |Роля на транзакция 2 |Тип на транзакция 2 |
|------------------------|------------------------------|---------------|-----------------------------|-----------------------------|-------------------|-------------------|
|Подаване на запис за време   |GUID на счетоводен запис (продажби)     |Нефактурирани продажби |msdyn_journalline            |GUID на счетоводен запис (разходи)     |Разходи            |msdyn_journalline  |
|Одобрение на времето           |GUID на действителни данни на нефактурирани (продажби)  |Нефактурирани продажби |msdyn_actual                 |GUID на действителни данни за разходи (разходи)       |Разходи            |msdyn_actual       |
|Създаване на фактура        |GUID на подробности за ред на фактура      |Фактурирани продажби   |msdyn_invoicelinetransaction |GUID на действителни данни на нефактурирани продажби   |Нефактурирани продажби  |msdyn_actual       |
|Потвърждаване на фактура    |GUID на сторниране на действителни данни         |Сторниране      |msdyn_actual                 |GUID на оригинални нефактурирани продажби |Оригинал        |msdyn_actual       |
|                        |GUID на фактурирани продажби             |Фактурирани продажби   |msdyn_actual                 |GUID на действителни данни на нефактурирани продажби   |Нефактурирани продажби  |msdyn_actual       |
|Корекция на чернова на фактура |GUID на транзакция по ред на фактура|Замяна      |msdyn_invoicelinetransaction |GUID на фактурирани продажби            |Оригинал        |msdyn_actual       |
|Потвърждаване на корекция на фактура|GUID на сторниране на фактурирани продажби  |Сторниране      |msdyn_actual                 |GUID на фактурирани продажби            |Оригинал        |msdyn_actual       |
|                        |Нов НЕБИТИРАН ГИД за продажби |Замяна            |msdyn_actual                 |GUID на фактурирани продажби            |Оригинал        |msdyn_actual       |


Следната илюстрация показва връзките, които са създадени между различни видове действителни данни на различни събития, като се използва примерът за записи във времето в Project Operations.

> ![Как действителните данни от различни типове са свързани помежду си в Project Operations.](media/TransactionConnections.png)

[!INCLUDE[footer-include](../includes/footer-banner.md)]