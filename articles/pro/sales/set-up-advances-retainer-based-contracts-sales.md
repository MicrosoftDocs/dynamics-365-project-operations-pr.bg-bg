---
title: Базирани на авансови плащания и капаро договори
description: Тази тема предоставя информация за модели на договаряне, базирани на капаро, и аванси в Project Operations.
author: rumant
manager: Annbe
ms.date: 10/20/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5ccf8ff4fa52fa6ff9fe534dfbe6736afc24ffba
ms.sourcegitcommit: f8edff6422b82fdf2cea897faa6abb51e2c0c3c8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/21/2020
ms.locfileid: "4087808"
---
# <a name="advances-and-retainer-based-contracts"></a>Базирани на авансови плащания и капаро договори 


_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_

Dynamics 365 Project Operations поддържа базирани на капаро договори. Договорът, базиран на фиксатор, е договорен набор от равномерно разпределени плащания, за които клиентът ще бъде фактуриран през цялото време на проекта. Този тип договор обикновено се използва за модели на фактуриране, базирани на време и материал или потребление, където е необходимо да се даде на клиента предвидима фактура и график на плащанията. Действителните приходи, начислени за всеки период, се сверяват с плащането, получено от клиента в началото на периода. В съответствие с концепцията за модела за фактуриране на време и материали стойностите на приходите, натрупани за всеки период, могат да варират в зависимост от направените разходи. Ако натрупаните приходи са повече от сумата, получена в началото на периода, фирмата за доставка на проекти може:

- Фактурирайте само клиента за излишъка 
- Отложете съгласуването на приходите за следващия период на фактуриране и направете една окончателна сметка в края на проекта за всички останали несъгласувани приходи

Основната разлика между модела за договаряне, базиран на фиксатор, и модела на договор с фиксирана цена в Project Operations е, че в модела на договора с фиксирана цена сумата на фактурата не е обвързана или обвързана с направените разходи. Фактурирането следва подход, основан на крайъгълен камък, който е съобразен с направените разходи за този период. В договор, базиран на фиксатор, приходите, които могат да бъдат фактурирани, се записват въз основа на метода на фактуриране в договорения ред. Когато методът за фактуриране е време и материал, фактурираните приходи са обвързани с разходите, направени през даден период и могат да варират от период до период. Клиентът обаче се фактурира само за сумата на периодичния фиксатор. Системата използва друга фактура в края на периода, за да съгласува фактурираните приходи, записани през периода, със сумата, за която клиентът е бил фактуриран в началото на периода.

Предимството на този метод е, че разходите на клиента стават предвидими в графика за фиксиране, за разлика от типичния модел на време и материал. Организацията, която изпълнява проекта, има също така място за покриване на риска от възстановяване на направените разходи поради всякакви увеличения на обхвата, които моделът с фиксирана цена не би им позволил.

В допълнение към периодичния график, базиран на фиксатори, Project Operations могат да записват еднократен аванс от клиент и да го съгласуват с различните компоненти на разходите на проекта.

Фиксаторът в Project Operations не е достъпен за употреба, докато не бъде фактуриран на клиента. Това е посочено от следните полета в подмрежата за аванси и фиксатори.

| Поле | Уместност, цел и насоки | Въздействие надолу по течението |
| --- | --- | --- |
| Налична сума | Сумата, която е на разположение за използване върху фиксатора или авансовия запис. | До фактуриране на аванса или фиксатора, той не може да се използва, което означава, че наличната сума ще бъде нула. |
| Използвана сума | Сумата, която вече е използвана върху капарото или аванса. | Аванс или фиксатор може да бъде частично съгласуван във фактура с действителни разходи, които ще имат част, маркирана като вече използвана или консумирана. Остатъкът от сумата на аванса или фиксатора е на разположение за съгласуване на бъдеща фактура с действителни разходи. |