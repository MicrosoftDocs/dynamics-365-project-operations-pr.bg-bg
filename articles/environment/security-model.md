---
title: Защитен модел
description: Тази тема предоставя информация за можела на защита в Dynamics 365 Project Operations.
author: stsporen
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: e875d1765b5038e60830d626abb5bcd61749ece1
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071705"
---
# <a name="security-model"></a>Модел на защита

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

Microsoft Dynamics 365 Project Operations съдържа уникален модел на защита, който позволява базиран на роля модел на бизнес сигурност, с който си сътрудничи с Групи на Microsoft Office. 


## <a name="security-roles"></a>Права за достъп
Възможностите за предни операции на Project Operations включват следните роли:

| Роля                          | Описание                                                                                                                                                                 | Scope |
|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
| Оперативен мениджър              | Поддържа междупроектно отчитане.                                                                                                            | Бизнес единица              |
| Одобряващ на проект              | Одобрява време и разходи срещу проект.                                                                                                                              | Бизнес единица |
| Администратор на фактуриране по проект | Създава предложението за фактура.                                                                                                                                                 | Бизнес единица |
| Мениджър на проект               | Създава плана на проекта и изисква ресурси.                                                                                                                              | Бизнес единица |
| Ресурс на проект              | Членове на екипа, които могат да бъдат резервирани и да докладват времето.                                                                                                          | Бизнес единица|
| Мениджър на ресурси              | Всички функции за управление на ресурси, като например изпълнение на заявки за ресурси и резервации, отделени, за да поддържат хибриден мениджър на проекти + конфигурация на мениджър на ресурси и една-единствена и централизирана роля на мениджър на ресурси. | Бизнес единица |


Microsoft Project за мрежата включва следните роли:

| Роля           | Описание                                                                                                        | Scope  |
|----------------|--------------------------------------------------------------------------------------------------------------------|--------|
| Потребител на проекта   | Съвместен потребител на Project, който може да създава свои собствени проекти и да преглежда всички споделени с тях проекти. | Поотребител   |
| Система за проекти | Роля, използвана за контекста на приложението. Клиентите не трябва да използват тази системна роля.                                    | Глобално |

## <a name="security-enforcement"></a>Принудително изпълнение
Действия, които се изпълняват на ниво проект, се извършват в контекста на влезлия потребител. Това означава, че за да създаде, отвори или изтрие проект, потребителят трябва да има достъп в CDS. Достъпът в CDS може да бъде предоставен чрез всеки от възможните механизми, включени в платформата. Например потребител с по-голям обхват може да осъществи достъп до проекта или ако е извършено изрично действие за споделяне на проект, което предоставя на потребителя достъп.

Важно е да се вземе предвид това при създаването на проекти в Project Operations.

## <a name="modern-group-collaboration-with-project-operations"></a>Модерно групово сътрудничество с Project Operations
Project for the Web и Project Operations поддържат съвременни групи за сътрудничество. Потребителите, добавени към проекта чрез група, могат да редактират плана на проекта.

Project for the Web автоматично добавя потребители към групата при задаване.

Групите позволяват съвместно да се работи над разрешенията на проекта и подкрепящите артефакти за сътрудничество. Следващата диаграма изобразява събитията и промените в състоянието, които се случват по време на процеса на групово задаване.

Project Operations не създава група чрез имплицитно действие и го прави само чрез изричното действие на натискащи групи.

Търсене на член на група в диалог **Групово управление** , се ограничава до тези, които са зададени като част от групата за сигурност на средата. За допълнителна информация вижте [Управление на потребителския достъп до среди: групи за защита и лицензи](https://docs.microsoft.com/power-platform/admin/control-user-access).

![Групов режим](./media/groupsmode.png)

1. Проектът е създаден и притежаван от създаващия потребител.
2. Собственикът на проекта е актуализиран за екипа.
3. Екипът на собственика се съпоставя с посочената или създадена група на Office.
4. Първоначалният собственик на проекта се добавя към Office Group.

## <a name="deployment-recommendation"></a>Препоръка за внедряване
С развитието на модела за съвместна работа на Office ще се добавя функционалност, за да се осигури по-подробен контрол във времето. Клиентите, които внедряват Project Operations днес, се насърчават да се съсредоточат върху традиционния модел за защита на Microsoft Dynamics 365.

За повече информация вижте [Защита в Common Data Service](https://docs.microsoft.com/power-platform/admin/wp-security).

## <a name="project-operations-and-microsoft-dynamics-365-finance-security"></a>Project Operations и защита на Microsoft Dynamics 365 Finance
Project Operations включва следните роли:

- Мениджър на проект
- Счетоводител на проект

За повече информация относно защитата във Finance вижте [базирана на роля защита](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).

