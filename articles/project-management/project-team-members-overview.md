---
title: Членове на екипа на проект
description: Тази тема предоставя информация за това как да работите с информация за членовете на проектния екип, атрибути и график.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: f4941803c657fab55ee2702d9f58d6e333592889
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907877"
---
# <a name="project-team-members"></a>Членове на екипа на проект

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

Членовете на проектния екип са участниците в проекта, които завършват работата по даден проект. Целта на мрежата на членовете на екипа е да предостави списък с посочени ресурси, които са ангажирани с ангажимента, и общи членове на екипа, които са ресурси за притежатели на места и ще бъдат наети по-късно.

От мрежата на членовете на екипа мениджърът на проекта и останалите участници в проекта имат възможността да видят кой е ангажиран с проекта. Те могат също да прегледат обобщение на своите резервации, планирани усилия и индивидуални задания за ресурси. Решетката на членовете на екипа позволява на мениджърите на проекти да определят изискванията за ресурси за общите членове на екипа и да управляват резервациите на съществуващите членове на екипа.

Следващата таблица изброява ключовите атрибути на член на проектния екип.

| Име на полето          | Описание                                                                                                                                                                  |
|--------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Метод за разпределение        | Методът на разпределение, използван за резервиране на ресурси по проекта.                                                                         |
| Тип фактуриране             | Изберете дали членът на екипа е класифициран като фактурируем.                                                                                                                                       |
| Наличен ресурс        | Наличният ресурс, избран да замени генеричния ресурс.                                                                                                                   |
| Състояние на изтриване            | Състоянието на изтриване на члена на екипа за проследяване на това дали има искане за изтриване, изпратено до PSS, и дали PSS изпраща обратно отговор успешно и в рамките на очакваното време. |
| Общо усилие (часове)     | Сумата от усилията на члена на екипа върху задачата му.                                                                                                                         |
| Приключено усилие (часове) | Проследяването на усилията, положени от члена на екипа по заданието му.                                                                                           |
| Оставащо усилие (часове) | Проследяването на все още незавършени усилия, положени от члена на екипа по заданието му.                                                                                    |
| Готово                   | Крайната дата на членство в екипа на ресурса.                                                                                                                                            |
| Часове с потвърдена резервация        | Твърдо резервирани часове на члена на екипа.                                                                                                                                                                |
| Име на позиция            | Името, използвано за идентифициране на общия ресурс.                                                                                                                                   |
| Ресурсна единица          | Организационната единица на ресурса, който извършва работата.                                                                                                                      |
| Одобряващ на проект         | Изберете дали члена на екипа може да одобрява време и разходи.                                                                                                                     |
| Необходими часове           | Необходимите часове за член на екипа от изискването за член на екипа.                                                                                                                       |
| Роля                     | Ролята, която членът на екипа изпълнява в този екип.                                                                                                                                |
| Описание на позиция     | Въведете описание на ролята на този член на екипа.                                                                                                                             |
| Часове с непотвърдена резервация        | Непотвърдено резервирани часове на члена на екипа.                                                                                                                                                                 |
| Старт                    | Началната дата на членството в екипа на ресурса.                                                                                                                                          |

От мрежата на члена на екипа могат да се предприемат следните действия:

- **Резервиране**: За организации, които изпълняват използването на метода на хибридните резервации, действието на книгата ще позволи на потребителите да резервират поименен ресурс въз основа на изискванията за изискване, генерирани от общия член на екипа
- **Генериране на изискване**: Това действие генерира изискването.
- **Посочете модел**: Позволява на мениджърите на проекти да коригират контурите на изискванията за ресурси на подробно ниво. Мениджърите на проекти могат да се приспособят към специфичните нужди на проекта в случаите, когато разпределението по подразбиране не се побира.
- **Изпрати заявка**: За организации, използващи централната методология за резервации.
- **Редактиране**: Атрибутите на члена на екипа могат да се редактират, включително организационна единица, роля и име на длъжността.
- **Поддържайте резервации**: Когато резервирането на ресурси трябва да се актуализира, поддържането на резервации позволява на мениджъра на проекта да коригира:

    - Старт
    - Край
    - Общо разпределение на усилията

- **Ново**: В допълнение към добавянето на ресурси директно от графика, мениджърите на проекти могат да добавят нови имена или общи членове на екипа от мрежата на членовете на екипа.
- **Изтрий**: Избирайки един или повече членове на екипа, мениджърът на проекта може да изтрие ресурси, които вече няма да участват в проекта. Изтриването на член на екипа също ще изтрие всички свързани назначения на ресурси и ще отмени всички съществуващи резервации.
