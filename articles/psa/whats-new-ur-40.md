---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 40, V3
description: Тази статия изброява функциите и корекциите, които са налични в Microsoft Dynamics 365 Project Service Automation актуализация издание 40, V3.
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

Тази статия изброява функциите и корекциите, които са нови или променени за Project Service автоматизация актуализация издание 40, V3. Тази версия има номер на компилация V3.10.61.61 и е общодостъпно чрез самостоятелна актуализация от февруари 2022 г.

## <a name="update-release-40"></a>Издание на актуализация 40

### <a name="features"></a>Функции
Фаза 1 на надстройката от Project Service Automation to Project Operations - Lite ще бъде пусната през февруари 2022 г. на всички клиенти. За да проверите за допустимост, вижте [Надстройка от Автоматизация на услугата за проекти до Операции по проекта](upgrade-project-operations-non-stocked.md). Ако приложението не се показва във вашия екземпляр в Power Platform Центъра за администриране, свържете се с поддръжката и поискайте полетът да бъде активиран за вашите среди. Вашето искане трябва да включва списък с идентификатори на средата, където полетът трябва да бъде активиран.

### <a name="bug-fixes"></a>Корекции на грешки

Следните проблеми са коригирани.

**Час и разход**
- Липсва запис за бележка, когато запис за време е отхвърлен или отменен. 

**Продажби**

- Когато актуализирате разходите или прогнозите за продажби с помощта на добавката "извън кутията", неправилно ви е разрешено да изпращате полезни данни на JSON, които не са валидни извън потребителския интерфейс.
- Когато актуализирате редове от оферти с помощта на бързия изглед, ви е разрешено да активирате оферти.
