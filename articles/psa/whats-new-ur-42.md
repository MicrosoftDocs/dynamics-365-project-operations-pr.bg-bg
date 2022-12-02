---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 42, V3
description: Тази статия изброява функциите и корекциите, които са налични в Microsoft Dynamics 365 Project Service Automation Актуализирано издание 42, V3.
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
ms.openlocfilehash: e9911531e4acbd78db416f554c8d85c4f1fee1cf
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912702"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-42-v3"></a>Какво е новото или промененото в Project Service Automation, издание на актуализация 42, V3

[!include [banner](../includes/psa-now-project-operations.md)]

С удоволствие обявяваме най-новата актуализация за приложението Microsoft Dynamics 365 Project Service Automation. Тази версия включва някои важни подобрения в качеството, производителността и използваемостта. Съвместим е с Dynamics 365 9.x. За да актуализирате до тази версия, посетете страницата на центъра за администриране за решенията на Dynamics 365 Online и инсталирайте актуализацията. За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).

Тази статия изброява функциите и корекциите, които са нови или променени за актуализацията на Project Service Automation, издание 42, V3. Тази версия има номер на създаване V3.10.73.61 и е общо достъпна чрез самостоятелно актуализиране от април 2022 г.

## <a name="update-release-42"></a>Издание на актуализация 42

### <a name="bug-fixes"></a>Корекции на грешки

Следните проблеми са коригирани.

**Час и разход**

- Когато даден график е отхвърлен, потребителят, който го е отхвърлил, се идентифицира неправилно като **Система**.
- Когато се импортират записи за време, стойността **Категория ресурс** липсва.
- Одобряващите проекти могат да одобряват изпратени проекти, когато техните разрешения не са специално зададени **Може да одобри**.

**Продажби**

- Когато действителните стойности се записват на задачи на различно от основно ниво, действителните разходи се обобщават неправилно.
