---
title: Нововъведения от август 2022 г. – Project Operations за сценарии, базирани на ресурс/неналичност
description: Тази статия предоставя информация за актуализациите на качеството, които са налични в изданието на Microsoft Dynamics 365 Project Operations от август 2022 г. за ресурси/не-заредени базирани сценарии.
author: ramagadu
ms.date: 07/19/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: 112dbb98de09ef342c03d122a29cb8025058e47f
ms.sourcegitcommit: 6b6c2bfd04e3e613ed1f38355c7cd47c3a56748d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/24/2022
ms.locfileid: "9348090"
---
# <a name="whats-new-august-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Нововъведения от август 2022 г. – Project Operations за сценарии, базирани на ресурс/неналичност

_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_

Тази статия се отнася за следните компоненти и версии на Microsoft Dynamics 365 Project Operations:

- Операции на проекта в Dataverse среда версия 4.45.0.53
- Управление на проекти и счетоводство в Dynamics 365 Finance среда версия 10.0.28

## <a name="project-operations-dual-write-maps-updates"></a>Актуализации на карти за двойно записване на Project Operations

В тази версия няма актуализации за Project Operations карти с двойно писане. За текущ списък и версии на Project Operations карти с двойно писане вижте [Версии на карти с двойно писане на Project Operations](../environment/resource-dual-write-maps.md).

Винаги изпълнявайте най-новата версия на картата във вашата среда и активирайте всички свързани карти на таблици, докато актуализирате решението си "Операции по Dataverse проекта" и версията на решението "Финанси". Някои функции и възможности може да не работят правилно, ако последната версия на картата не е активирана. Можете да видите активната версия на картата в колоната **Версия** на страницата **Двоен запис**. За да активирате нова версия на картата, изберете **Версии на табличната карта**, изберете най-новата версия и след това запишете избраната версия. Ако сте персонализирали карта на таблица извън кутията, приложете отново промените. За повече информация вижте [Управление на жизнения цикъл на приложение](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Ако срещнете проблем при стартиране на картата, следвайте инструкциите в [липсващата таблица колони проблем на карти](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) раздел на ръководството за отстраняване на неизправности с двойно запис.

## <a name="quality-updates"></a>Актуализации на качеството

### <a name="project-operations-on-dataverse"></a>Project Operations в Dataverse

| Област с функции | Номер за справка | Актуализация на качеството |
| --- | --- | --- |
|   Управление на възможности | 2762089 | Грешка при работа при затваряне на договора като загубен, ако автоматично записване е за деактивирано в орга.|

### <a name="project-management-and-accounting-in-finance"></a>Управление на проекти и счетоводство във Финанси

За информация относно корекциите на грешките, които са включени в тази актуализация, влезте в Microsoft Dynamics услуги за жизнен цикъл (LCS) и прегледайте статията от [БЗ](https://fix.lcs.dynamics.com/Issue/Details?bugId=694438).
