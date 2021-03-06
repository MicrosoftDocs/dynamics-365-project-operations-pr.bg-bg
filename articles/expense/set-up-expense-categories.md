---
title: Настройване на категории разходи
description: Тази тема предоставя информация за това как да настроите категории разходи и споделени категории за отчети за разходите.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: f051d70f3dfe3b241dc0a206c0cdfda000f87c76
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896673"
---
# <a name="set-up-expense-categories"></a>Настройване на категории разходи

_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_

Когато служителите създават отчети за разходите, всеки разход, който записват, трябва да бъде свързан с категория разходи. Категориите на разходите се извличат от споделени категории, които могат да се споделят между юридическите лица във вашата организация. В зависимост от начина, по който е дефинирана вашата организация, тези категории разходи могат да се споделят и в други области. Въз основа на дефиницията на вашата организация и насоки от екипа за внедряване, трябва да определите дали категориите, които се използват в управлението на разходите, ще се използват само в управлението на разходите или трябва да се споделят в други области.

> [!NOTE]
> Тези категории могат да се споделят между управление на проекти и счетоводство и управление на разходите, или между управление на проекти и счетоводство и производство. Те обаче не могат да се споделят между управлението на разходите и производството.

Преди да започнете процеса на настройка, трябва да се вземат следните решения за всяка категория разходи:

- Каква е категорията на разхода? Примерите включват категории за полети, хотел или пробег.
- Може ли категорията на разходите да се използва и в управлението на проекти и счетоводството? Ако може, вие също трябва да вземете следните решения:

    - Кои сметки за разходи ще бъдат използвани за следните разходи?

        - Разход
        - Разпределение на изплащания
        - Стойност на разход за WIP
        - Елемент на разходите
        - Елемент на стойност на елемент на WIP
        - Натрупана загуба
        - WIP - натрупана загуба

    - Кои сметки за приходи ще бъдат използвани за следните източници на приходи?

        - Фактурирани приходи
        - Начислени приходи - Стойност на продажби
        - WIP-продажбена стойност
        - Натрупани приходи-производство
        - WIP-Продукция
        - Натрупани приходи-приход
        - WIP-приход
        - Натрупани приходи-абонамент
        - WIP-Абонамент

- Какъв е типът на разхода?
- Какъв е методът на плащане по подразбиране за категорията разходи?
- Трябва ли разходите в категорията на разходите да бъдат детайлизирани?
- Какъв е основният акаунт по подразбиране за категорията разходи?
- Каква е групата по данък върху продажбите по подразбиране за категорията на разходите?
- Разрешени ли са допълнителни методи на плащане за разходната категория? Ако да, какви са те?
- Има ли подкатегории в тази категория разходи? Ако има подкатегории, вие също трябва да вземете следните решения:

    - Изключена ли е някоя от подкатегориите от събирането на данъци?
    - Каква е групата за данък върху продажбите на артикули в подкатегориите?
