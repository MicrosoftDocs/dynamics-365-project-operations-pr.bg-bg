---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 12, V3
description: Тази тема предоставя информация за новостите в актуализацията на Project Service Automation, издание 12, V3.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: 62c3a0c5cfbecb568faef570da309c20afd86de9
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071781"
---
# <a name="project-service-automation-update-release-12-v3"></a>Project Service Automation, издание на актуализация 12, V3
С удоволствие съобщаваме за най-новата актуализация за приложението Dynamics 365 Project Service Automation (PSA). Тази версия включва някои важни подобрения в качеството, производителността и използваемостта. Това издание е съвместимо с Dynamics 365 9.x. За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online и отидете на страницата с решения, за да инсталирате актуализацията. За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 12. Тази версия е с номер на компилация V3.10.2.34 и е общодостъпна за самостоятелно актуализиране от октомври 2019 г.

## <a name="update-release-12"></a>Издание на актуализация 12

### <a name="bug-fixes"></a>Корекции на грешки

- Време и разход

    - Поправено: Съобщенията за грешки при запис за време са актуализирани с по-подходящ контекст.
    - Поправено: Мрежата и графикът на записите за време правилно показват вертикалната лента за превъртане, когато е необходимо.
    - Поправено: Подадени записи за разход и време могат да се одобряват.
    - Поправено: Съобщението в диалоговия прозорец за потвърждение на отмяна на одобрение е коригиран, така че да отразява състоянието на одобрението при промяна от **Одобрено** на **Подадено**.
    - Поправено: Полетата **Цена** , **Единица** и **Количество** вече са заключени в записа на разход след одобрението му.

- Управление на проекти

    - Поправено: Действието **Създаване** в основния формуляр **Член на екипа** е премахнато.
    - Поправено: Присвояванията на ресурси са актуализирани, за да отчитат грешки при неточно закръгляване, които водят до промяна на крайната дата на задача.
    - Поправено: В мрежата на задачата уместните грешки от страна на сървъра се извеждат за потребителя.
    - Поправено: Името на члена на екипа вече се рендира в инструмента за избор на хора вместо името на позицията.

- Управление на ресурс

    - Поправено: Подробностите за изискване за ресурс за проекти, създадени от шаблон, вече използват календара на проекта.
    - Поправено: Уменията и компетенциите по подразбиране вече са от главни данни за роля до изискването за ресурс, създадено за тази роля.

- Sales

    - Поправено: Открити са дублирани ИД на обекти в основния формуляр **Договор**.
    - Поправено: Логиката е актуализирана, за да се вижда раздела **Анализ на оферта** , така че да показва настройката на метаданните на раздела.
    - Поправено: Датата на осчетоводяване на действителния запис сега идва от датата на записа за време/разход, а не от датата на одобрението.