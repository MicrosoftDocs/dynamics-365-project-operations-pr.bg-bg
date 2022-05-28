---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 42, V3
description: Тази тема изброява функциите и корекциите, които са налични в Microsoft Dynamics 365 Project Service Automation Актуализирано издание 42, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/05/2022
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
ms.openlocfilehash: 32cb7a4c5fc29d5c0dcec37dd395ae69037435a2
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/14/2022
ms.locfileid: "8589183"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-42-v3"></a>Какво е новото или промененото в Project Service Automation, издание на актуализация 42, V3

[!include [banner](../includes/psa-now-project-operations.md)]

С удоволствие обявяваме най-новата актуализация за приложението Microsoft Dynamics 365 Project Service Automation. Тази версия включва някои важни подобрения в качеството, производителността и използваемостта. Съвместим е с Dynamics 365 9.x. За да актуализирате до тази версия, посетете страницата на центъра за администриране за решенията на Dynamics 365 Online и инсталирайте актуализацията. За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).

Тази тема изброява функциите и корекциите, които са нови или променени за актуализацията на Project Service Automation, издание 42, V3. Тази версия има номер на създаване V3.10.73.61 и е общо достъпна чрез самостоятелно актуализиране от април 2022 г.

## <a name="update-release-42"></a>Издание на актуализация 42

### <a name="bug-fixes"></a>Корекции на грешки

Следните проблеми са коригирани.

**Час и разход**

- Когато даден времеви лист бъде отхвърлен, потребителят, който го е отхвърлил, е неправилно идентифициран като **Система**.
- Когато записите за време се импортират, **липсва стойността "Категория** ресурси".
- Одобряващите проекти могат да одобряват подадени проекти, когато разрешенията им не са специално зададени на **Can Approve**.

**Продажби**

- Когато действителните са регистрирани на не-корен ниво задачи, действителните разходи са неправилно обобщени.
