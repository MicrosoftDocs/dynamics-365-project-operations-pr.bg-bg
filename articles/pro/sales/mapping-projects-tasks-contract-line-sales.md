---
title: Нанасяне на проекти и задачи към базирани на проект аспекти на договор – олекотено
description: Тази тема предоставя информация за добавяне и премахване на проекти и задачи към аспекти на договор.
author: rumant
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 30a74f683a032d5bd6caed347f4d0a948376d267
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177633"
---
# <a name="map-projects-and-tasks-to-a-project-based-contract-line---lite"></a>Нанасяне на проекти и задачи към базирани на проект аспекти на договор – олекотено

_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_

В аспекти на договор, базирани на проект, можете да съпоставите конкретни задачи в проект с аспектите на договора.

Когато нанасяте конкретни задачи към аспекти на договор, методът на фактуриране, опциите за платимост, ограниченията, които не трябва да се надвишават и клиентите, дефинирани в аспектите на договор, ще се прилагат само за тези конкретни задачи.

Ако имате сценарий, при който една фаза на проект, например фазата „Прототип”, е с фиксирана цена, а всички останали фази са за време и материал, ще можете да свържете фазата „Прототип” и всички свързани дъщерни задачи с аспектите на договора за тази фаза с метод на фактуриране с фиксирана цена.

Всички останали фази в съставната структура на работата (ССР) на проекта могат да се свържат с аспекти на договор, базирани на време и материали.

## <a name="associate-tasks-to-project-based-contract-lines"></a>Свързване на задачи с базирани на проект аспекти на договор

Задачите могат да се свържат с аспекти на договор от раздела **Платими задачи** на страницата **Аспекти на договор** или от раздела **Фактуриране на задача** на страницата **Проект**.

### <a name="from-the-contract-line-page"></a>От страницата на аспектите на договор

Изпълнете следните стъпки, за да свържете задачи по проект с аспекти на договор от раздела **Платими задачи** на страницата **Аспекти на договор**.

1. В раздела **Общи** на базирани на проект аспекти на договор се уверете, че полето **Проект** е попълнено.
2. В полето **Включени задачи** изберете **Само избрани задачи**.
3. Запишете промените. Формулярът ще се обнови и разделът **Платими задачи** ще стане видим.
4. Изберете раздела **Платими задачи** и в подмрежата изберете **Добавяне на задача на аспекти на договор**.
5. На страницата **Задачи на аспекти на договор** в падащия списък **Задачи** изберете задачата. 
6. Въведете информация в полето **Тип фактуриране** и след това изберете **Записване и затваряне**. Избраната задача е свързана с аспектите на договора.

> [!NOTE]
> Това не е най-оптималният начин за свързване на задачи по проект с аспекти на договор. Всеки проект ще трябва да бъде ръчно свързан в този случай. Предпочитаният начин е от раздела **Фактуриране на задача** на страницата **Проект**.

### <a name="from-the-project-page"></a>От страницата на проекта

Това е оптималният метод за свързване на задачи с аспекти на договор. Можете да изберете няколко задачи и да свържете всички, както и техните дъщерни задачи, към избраните аспекти на договор. Изпълнете следните стъпки, за да свържете задачите към аспектите на договора от страницата **Проект**.

1. В раздела **Общи** на базирани на проект аспекти на договор се уверете, че полето **Проект** е попълнено.
2. В полето **Включени задачи** изберете **Само избрани задачи**.
3. Запишете базираните на проект аспекти на договор. Формулярът ще се обнови и разделът **Платими задачи** ще стане видим. Това е само за целите на проверката.
4. В раздела **Общи** на базираните на проект аспекти на договор, в полето **Проект** изберете връзката към проекта.
5. На страницата **Проект** изберете раздела **Настройка на фактуриране на задача**.
6. Има две мрежи. Едната мрежа е за аспекти на договор, които се отнасят за целия проект. Втората мрежа се прилага за настройката на фактуриране за конкретната задача. Във втората мрежа изберете една или повече задачи и след това изберете **Свързване на аспекти на договор**.
7. В диалоговата страница, която се отваря, изберете аспекти на договор от падащото меню.
8. Използвайте падащия списък **Тип фактуриране**, за да маркирате задачите като платими или неплатими.
9. Поставете отметка в квадратчето, за да посочите дали връзката трябва да включва и дъщерни задачи на избраните задачи. Поставянето на отметка в квадратчето също ще свърже дъщерните задачи на избраните задачи с аспектите на договора.
10. Изберете **ОК**, за да затворите диалоговия прозорец.

## <a name="unassociate-tasks-from-project-based-contract-lines"></a>Премахване на връзката на задачи от базирани на проект аспекти на договор

### <a name="from-the-contract-line-page"></a>От страницата на аспектите на договор

Изпълнете следните стъпки, за да премахнете връзката на задачи по проект от аспектите на договора в раздела **Платими задачи** на страницата **Аспекти на договор**.

1. В раздела **Платими задачи** изберете **Изтриване на задача на аспекти на договор**.
2. Предупредително съобщение показва, че премахването на тази връзка може да доведе до анулиране на всички действителни данни, записани по-рано в задачата. Изберете **OK** в диалоговия прозорец, за да премахнете връзката между задачата и базираните на проект аспекти на договор. 

> [!NOTE]
> Това не изтрива задачата от проекта. Вместо това премахва връзката на задачата от базираните на проект аспекти на договор.

### <a name="from-the-project-page"></a>От страницата на проекта

Това е по-оптимален начин за премахване на връзката на задачи от аспекти на договор. Можете да изберете няколко задачи и да премахнете връзката на всички, както и на техните дъщерни задачи, от избраните аспекти на договор. Изпълнете следните стъпки, за да премахнете връзката на задачите от аспектите на договора.

1. От раздела **Общи** на базираните на проект аспекти на договор, в полето **Проект** щракнете върху връзката за проекта.
2. На страницата **Проект** изберете раздела **Настройка на фактуриране на задача**.
3. На страницата има две мрежи. Едната мрежа е за аспекти на договор, които се прилагат към целия проект, а втората се прилага за настройка на фактуриране за конкретна задача. Във втората мрежа изберете една или повече задачи и след това изберете **Премахване на свързаност на аспекти на договор**.
4. В диалоговата страница, която се отваря, изберете аспекти на договор от падащото меню.
5. Поставете отметка в квадратчето, за да посочите дали връзката трябва да се премахне и от дъщерните задачи на избраните задачи. Поставянето на отметка в квадратчето ще премахне връзката и на дъщерните задачи на избраните задачи от аспектите на договора.
6. Изберете **OK**. Предупредително съобщение показва, че премахването на тази връзка може да доведе до анулиране на всички действителни данни, предварително записани в задачата. Изберете **OK** в диалоговия прозорец на предупреждението, за да премахнете връзката между задачата и базираните на проект аспекти на договор.