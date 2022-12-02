---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 40, V3
description: Тази статия изброява функциите и корекциите, които са налични в Microsoft Dynamics 365 Project Service Automation Актуализирано издание 40, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/31/2022
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
ms.openlocfilehash: dca7f340b8d544b183aa0390ac3c11a38f536ed0
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912779"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-40-v3"></a>Какво е новото или промененото в Project Service Automation, издание на актуализация 40, V3

[!include [banner](../includes/psa-now-project-operations.md)]

С удоволствие обявяваме най-новата актуализация за приложението Microsoft Dynamics 365 Project Service Automation. Тази версия включва някои важни подобрения в качеството, производителността и използваемостта. Съвместим е с Dynamics 365 9.x. За да актуализирате до тази версия, посетете страницата на центъра за администриране за решенията на Dynamics 365 Online и инсталирайте актуализацията. За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).

Тази статия изброява функциите и корекциите, които са нови или променени за актуализацията на Project Service Automation, издание 40, V3. Тази версия има номер на компилация V3.10.61.61 и е общодостъпно чрез самостоятелна актуализация от февруари 2022 г.

## <a name="update-release-40"></a>Издание на актуализация 40

### <a name="features"></a>Функции
Фаза 1 на надстройката от Project Service Automation до Project Operations – Lite ще бъде пусната през февруари 2022 г. за всички клиенти. За да проверите дали отговаряте на изискванията, вижте [Надграждане от Project Service Automation към Project Operations](upgrade-project-operations-non-stocked.md). Ако приложението не се появи във вашия екземпляр в Център за администриране на Power Platform, свържете се с поддръжката и поискайте полетът да бъде активиран за вашите среди. Вашата заявка трябва да включва списък с идентификатори на среда, където полетът трябва да бъде активиран.

### <a name="bug-fixes"></a>Корекции на грешки

Следните проблеми са коригирани.

**Час и разход**
- Липсва запис на бележка, когато въвеждането на час е отхвърлено или отменено. 

**Продажби**

- Когато актуализирате оценките на разходите или продажбите с помощта на готови добавки, неправилно ви е разрешено да изпращате JSON полезни данни, които не са валидни извън потребителския интерфейс.
- Когато актуализирате редове с котировки с помощта на бързия изглед, имате право да активирате котировки.
