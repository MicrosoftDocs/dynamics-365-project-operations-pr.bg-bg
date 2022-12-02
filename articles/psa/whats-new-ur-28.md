---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 28, V3
description: Тази статия изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 28, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/26/2021
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
ms.openlocfilehash: 56a87bce55c560e541e20709b10d38b9512ffcee
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930581"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a>Какво е новото или промененото в Project Service Automation, издание на актуализация 28, V3

[!include [banner](../includes/psa-now-project-operations.md)]

С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365. Тази версия включва някои важни подобрения в качеството, производителността и използваемостта. Това издание е съвместимо с Dynamics 365 9.x. За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията. За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).

Тази статия изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 28. Тази версия е с номер на компилация V3.10.46.32 и е общодостъпна чрез самостоятелна актуализация от януари 2021.

## <a name="update-release-28"></a>Издание на актуализация 28

### <a name="bug-fixes"></a>Корекции на грешки

**Време и разход**

Следните проблеми са коригирани:

- Потребителите могат да използват **Групово редактиране** за актуализиране на записите за време, които са одобрени и изпратени.

**Управление на проекти**

Следните проблеми са коригирани:

- В случаите, когато GUID на задачата се интерпретира като число, задачите не могат да бъдат отворени за редактиране с помощта на **Редактиране на задача** в лентата на страницата **съставна структура на работата**.

**Sales**

Следните проблеми са коригирани:

- Изключване на нулева препратка се генерира, когато добавката **GetEstimatesForProject** бъде извикана.
- **Маркирайте готовност за фактуриране** в решетката на етапа само частично актуализира атрибутите, с изключение на атрибута **InvoiceStatus**, който се актуализира.



[!INCLUDE[footer-include](../includes/footer-banner.md)]
