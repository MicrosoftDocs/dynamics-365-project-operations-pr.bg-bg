---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 45, V3
description: Тази статия изброява функциите и корекциите, които са налични в Microsoft Dynamics 365 Project Service Automation Актуализирано издание 45, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 07/14/2022
ms.topic: article
ms.author: ruhercul
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
ms.openlocfilehash: 98f7c973917d7d6334e6e0aeb15214c538b33143
ms.sourcegitcommit: 36fda4f45ddeb0f81d30bd1e22852727df644754
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2022
ms.locfileid: "9169173"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-45-v3"></a>Какво е новото или промененото в Project Service Automation, издание на актуализация 45, V3

[!include [banner](../includes/psa-now-project-operations.md)]

С удоволствие обявяваме най-новата актуализация за приложението Microsoft Dynamics 365 Project Service Automation. Тази версия включва някои важни подобрения в качеството, производителността и използваемостта. Съвместим е с Dynamics 365 9.x. За да актуализирате до тази версия, посетете страницата на центъра за администриране за решенията на Dynamics 365 Online и инсталирайте актуализацията. За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).

Тази статия изброява функциите и корекциите, които са нови или променени за актуализацията на Project Service Automation, издание 45, V3. Тази версия има номер на компилация V3.10.76.168 и обикновено се предлага чрез самообновяване през юли 2022 г.

## <a name="update-release-45"></a>Издание на актуализация 45

### <a name="bug-fixes"></a>Корекции на грешки

Следните проблеми са коригирани.

**Продажби**

- Потребителите не могат успешно да създават фактури, след като се опитат да създадат фактура без никакви нефактурирани продажби, ако също така преглеждат същото копие на страницата и не го опресняват.

**Час и разход**

- Когато модерните одобрения са активирани и е одобрено изтеглено одобрение на проект, етапът на запис се актуализира неправилно до **Заявката за изтегляне е одобрена**.
- Когато модерните одобрения са активирани и Cloud Flows е неактивен, процесът на одобрение не е успешен и потребителите, които подават или одобряват, не се уведомяват.
