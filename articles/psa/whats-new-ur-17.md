---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 17, V3
description: Тази статия изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 17, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
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
ms.openlocfilehash: c8486ef689f0d8ab014c2248fc6e5d0fddc937e7
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2022
ms.locfileid: "8915677"
---
# <a name="project-service-automation-update-release-17-v3"></a>Project Service Automation, издание на актуализация 17, V3

[!include [banner](../includes/psa-now-project-operations.md)]

С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365. Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.  Това издание е съвместимо с Dynamics 365 9.x. За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения, за да инсталирате актуализацията. За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).

Тази статия изброява функциите и корекциите, които са нови или променени за PSA V3, издание на актуализация 17. Тази версия е с номер на компилация V3.10.6.34 и е общодостъпна за самостоятелно актуализиране от март 2020 г.


## <a name="update-release-17"></a>Издание на актуализация 17

### <a name="bug-fixes"></a>Корекции на грешки

**Общи**

- Поправено: Актуализиране на Project Service Automation, за да се наложат лицензи за членове на екипа (Центърът за ресурси на проекта ще включва метаданни 3.x на план за обслужване на членове на екипа)
 
**Време и разход**

- Поправено: Не е възможно да се промени прогнозата за разходите от ненулева цена на нула (0). Промяната се игнорира.

**Управление на проекти**

- Поправено: Проверка за нулеви стойности е добавена в името на позицията на член на екипа.
- Поправено: Полето **msdyn_userresourceid** на обекта **msdyn_resourceassignment** е оттеглено.
- Поправено: Надстройка от 2.x до 3.x сега обработва празни контури на усилието на присвоявания на задачите.

**Sales**

- Поправено: **Invoice.PreValidateInvoiceUpdate** вече обработва сценария за преназначаване на собствениците на записи правилно.
- Поправено: Когато класът на транзакциите е **Час**, **UnitGroup** не може да се редактира за всички обекти, включително, **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail** и **ContractLineDetails**. Въпреки това **Единица** не може да се редактира само за **JournalLine** и **InvoiceLineDetails**.




[!INCLUDE[footer-include](../includes/footer-banner.md)]
