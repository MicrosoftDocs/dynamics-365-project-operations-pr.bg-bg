---
title: Възстановяване на ДДС при управление на разходи
description: Тази тема обяснява как да получавате възстановявания на допустими сделки с данък върху добавената стойност (ДДС).
author: suvaidya
manager: AnnBe
ms.date: 10/10/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 2c20e4a7fa9748e03bf1729fc2f7bdbfc2f292d1
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071688"
---
# <a name="vat-recovery-in-expense-management"></a>Възстановяване на ДДС при управление на разходи

_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_

За да получи възстановяване на допустими транзакции с данък върху добавената стойност (ДДС), компания или организация трябва да идентифицира, събере, провери и представи точна информация. Този процес включва множество задачи и в зависимост от размера на вашата компания може да включва няколко служители или роли.

За възстановяване на ДДС в модула **Управление на разходите** , трябва да бъдат изпълнени следните предпоставки:

- Данъчните кодове трябва да бъдат създадени за държави/региони, които са разпределени по разходни категории.
- За всеки данъчен код трябва да се създаде група за данък върху продажбите.
- Данъчен код върху продажби на артикул трябва да се създаде за всякак група за данък върху продажбите.

След като предпоставките са изпълнени, трябва да бъдат изпълнени следните стъпки, за да се поиска възстановяване на суми за транзакции с ДДС.

1. В отчета за разходите въведете данъчна информация за транзакциите с кредитни карти, за да идентифицирате допустими възстановявания на ДДС.
2. Проверете дали цялата данъчна информация е пълна и след това публикувайте отчета за разходите.
3. Обработвайте разходи, които отговарят на условията за международно възстановяване на ДДС.
4. Изпратете данните за възстановяване на ДДС на доставчика на трета страна, за да подадете международни декларации за възстановяване.
5. Процес на разходи за вътрешно възстановяване на ДДС.

Следващите раздели предоставят примери, които показват как служителите на Contoso изпълняват всяка стъпка.

## <a name="enter-tax-information-about-credit-card-transactions-to-identify-eligible-vat-refunds"></a>Въведете данъчна информация за транзакциите с кредитни карти, за да идентифицирате допустими възстановявания на ДДС

Нанси, търговски представител на Contoso, който е базиран в САЩ, наскоро се завърна от разпродажба в Обединеното кралство. По време на пътуването Нанси направи някои лични разходи за кредитни карти за хранене. Сега Нанси трябва да създаде отчет за разходите, за да съгласува разходите.

Когато Нанси въвежда информация в отчета за разходите, тя избира **Обединеното кралство** в полето **Държава/регион** на страницата **Редактиране на отчета за разходите**. След това списъкът с данъчните групи върху продажбите се филтрира, така че да показва само групите, които се прилагат за Обединеното кралство. Нанси избира група данък върху продажбите **Обединено кралство 001** и след това избира данъчна група **Хранене** за продажби на артикули. След това Нанси добавя нова транзакция за подаване. Тъй като в Обединеното кралство има само една група за данък върху продажбите и една група за данък върху продажбите на артикули, тази информация се попълва автоматично в отчета за разходите на Нанси.

Според политиката Contoso всички разходи трябва да имат съответстваща разписка. Следователно, когато Нанси запазва отчета за разходите, тя получава съобщение, в което се посочва, че трябва да приложи разписка за всяка транзакция, която е посочила в отчета си за разходите. Нанси потвърждава, че е прикачила цифрово изображение на всяка разписка за транзакция към отчета си за разходите и след това го представя за одобрение. След това тя изпраща хартиените бележки на екипа за обработка на бек-офиса. Този екип ще изпрати данните за възстановяване на ДДС на доставчика на трета страна, който подава международни декларации за възстановяване на ДДС за Contoso.

## <a name="verify-tax-information-and-post-an-expense-report"></a>Проверете данъчната информация и публикувайте отчет за разходите

Преди април координаторът на задълженията за Contoso може да публикува отчет за разходите, тя трябва да въведе данъчна информация, която липсва в нея. Тя отваря страницата **Подробности за отчета за разходите** и вижда одобрения от Нанси отчет за разходите. След това април отваря отчета за разходите, за да видите подробности за транзакциите. Тя вижда, че Нанси не е въвела група данъци върху продажбите на артикули за една от транзакциите. Тъй като тази информация не е предоставена, Април не може да публикува отчет за разходите. Следователно тя гледа на страницата **Данъчни конфигурации** в Управление на разходи и намира подходящата група данък върху продажбите на артикули за държавата/региона и вида на транзакцията. Април вече може да публикува отчета за разходите в главната книга.

Когато април публикува отчета за разходите, се създава работна позиция за възстановяване на ДДС. Този работен елемент е възложен на член на екипа за обработка на бек-офис. Април получава съобщение, което потвърждава, че публикуването е било успешно. Това съобщение също така изброява броя на транзакциите с ДДС, които са идентифицирани за възстановяване.

## <a name="process-expenses-that-are-eligible-for-international-vat-recovery"></a>Обработвайте разходи, които отговарят на условията за международно възстановяване на ДДС

Арни, член на екипа за обработка на бек-офис на Contoso, е отговорен за проверката дали цялата необходима информация за възстановяване на ДДС е включена в отчетите за разходите. Той отваря страницата **Възстановяване на данъци върху разходи** и избира отчета за разходите, който Нанси е подала. След това Арни проверява дали са прикачени всички необходими квитанции и дали са въведени правилните данъчни кодове на групата данъци и продажби на артикули.

Когато Арни получава хартиените разписки от Нанси, той ги проверява спрямо цифровите разписки и след това променя състоянието на отчета за разходите на **Готови за възстановяване**.

## <a name="send-vat-recovery-data-to-the-third-party-vendor"></a>Изпратете данните за възстановяване на ДДС на доставчика на трета страна

Когато Арни е готов да изпрати данните за отчета за разходите на доставчика на трета страна, който ще подаде декларациите за възстановяване на ДДС, той отваря страницата **Възстановяване на данъци върху разходи**. Той филтрира страницата така, че да показва само отчетите за разходите, които са маркирани като **Готови за възстановяване**. След това Арни избира **Файл** &gt; **Експортиране в Excel**. Информацията за ДДС от отчетите за разходите се експортира към работен лист на Microsoft Excel. Арни изпраща този работен лист на доставчика на трета страна и включва съобщение, в което се посочва, че хартиените разписки са изпратени от куриер.

## <a name="process-expenses-for-domestic-vat-recovery"></a>Процес на разходи за вътрешно възстановяване на ДДС

Арни трябва да провери дали транзакциите с отчета за разходите отговарят на условията за възстановяване на ДДС и че цифровите разписки са приложени към отчетите. За да започне да обработва допустими разходи за вътрешно възстановяване, Арни отваря страницата **Възстановяване на данъци върху разходи** и избира отчета за разходите, който изисква проверка. Той проверява дали касовите бележки са на името на компанията, а не на служителя. (За възстановяване на ДДС разписките трябва да са на името на фирмата.) След това Арни проверява дали са прикачени всички необходими квитанции и дали са въведени правилните данъчни кодове на групата данъци и продажби на артикули.

Когато Арни получава хартиените разписки, той променя състоянието на отчета за разходите на **Готови за възстановяване**. След това той може да подаде декларацията до съответния данъчен орган. В този случай подходящият данъчен орган в САЩ е Службата за вътрешни приходи (IRS).