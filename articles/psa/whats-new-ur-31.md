---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 31, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 31, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/26/2021
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
ms.openlocfilehash: 2e5fce003c25f9c5911e5a01fb4ec3e19c06c078e00b054472699a522b9cd070
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/06/2021
ms.locfileid: "7002138"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-31-v3"></a>Какво е новото или промененото в Project Service Automation, издание на актуализация 31, V3

[!include [banner](../includes/psa-now-project-operations.md)]

С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365. Тази версия включва някои важни подобрения в качеството, производителността и използваемостта. Това издание е съвместимо с Dynamics 365 9.x. За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията. За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).

Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 31. Тази версия има номер на компилацията V3.10.52.77 и е общодостъпна чрез самоактуализация от май 2021 г.

## <a name="update-release-31"></a>Издание на актуализация 31

### <a name="bug-fixes"></a>Корекции на грешки

**Време и разход**

Следните проблеми са коригирани:

- Командни бутони за контрол на въвеждане на време на страницата **Наличен ресурс** бяха объркващи.
- Изключено е изключение за нулева препратка в **Project.SetTrackingFields** при одобряване на запис на време.

**Управление на ресурси**

Следните проблеми са коригирани:

- **Създайте член на екипа** не показва правилно настройката на метаданните за настройка на резервация за **Статус на ангажираност по подразбиране**.
- При надстройка от PSA 1.X до 3.X, процесът на надстройка е неуспешен в **UpgradeResourceRequirements**.


**Продажби**

Следните проблеми са коригирани:

- Действителните приходи преобразуват сумите във валутата на проекта в мрежата за проследяване.
- Валутата по подразбиране е неясна при създаване на редове на дневници, редове за котировки и линии на договори в сценарии, при които основната валута на организацията се различава от валутата на проекта.
- Заявката **Изчаква валидиране на дневника за корекция** не се филтрира по проект.
- Останалите продажби се изчисляват неправилно за даден проект.
- Котировките, базирани на контакт, се провалят, когато са създадени без ценова листа.
- Когато изберете, не се показва въртящо устройство за обработка **Потвърдете фактурата**.
- Когато изберете, не се показва въртящо устройство за обработка **Създаване на фактура**.
- Затварянето на оферта като загубена не отменя резервациите.






