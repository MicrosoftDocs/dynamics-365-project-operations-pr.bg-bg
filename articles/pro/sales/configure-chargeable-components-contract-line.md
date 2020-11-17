---
title: Конфигуриране на платими компоненти на базирани на проект аспекти на договор
description: Тази тема предоставя информация за това как да добавите таксуеми компоненти към договорни линии в Project Operations.
author: rumant
manager: Annbe
ms.date: 10/08/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4d665a6351d2315d185e64e4eb6b0b8859f7bbc4
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071727"
---
# <a name="configuring-chargeable-components-of-a-project-based-contract-line"></a>Конфигуриране на платими компоненти на базирани на проект аспекти на договор

_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_

Базираните на проект аспекти на договор имат *включени* компоненти и *таксуеми* компоненти.

Включените компоненти са компоненти, които са обект на:

  - Метод на фактуриране и разделяне на клиента
  - Ограничения, които да не се надвишават 
  - Настройки на честотата на фактурите, дефинирани на базиран на проекта ред на оферта

Подмножество от включените компоненти може да бъде маркирано като таксувано с помощта на полето **Тип фактуриране**. Полето **Тип фактуриране** е набор от опции, който позволява следните стойности в контекста на аспекти на договор:

  - Платими
  - Нетаксуеми

Компонентите, които се заплащат, могат да бъдат дефинирани за задачи, роли и категории транзакции.

Плащаемостта се определя в задачите за аспекти на договор по проект и се прилага за всички класове транзакции, включени в реда. Ако полето **Включете задачи** на аспекти на договор е празно или зададено на **Цял проект** , разделът **Платими задачи** няма да е наличен.

Плащаемостта се определя в ролите за аспекти на договор по проект и се прилага само за класа трансакция **Време**. Ако полето на аспекти на договор **Включете време** е зададено на **Не** , разделът **Платими роли** не е наличен.

Плащаемостта се определя в категориите трансакция за аспекти на договор по проект и се прилага само за класа трансакция **разход**. Ако полето на аспекти на договор **Включете разход** е зададено на **Не** , разделът **Платими категории** не е наличен.

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a>Актуализирайте проектна задача, за да бъде таксувана или без такса

Проектната задача може да бъде таксувана или без такса на специфични аспекти на договор, което прави възможна следната настройка:

Ако договорната линия, базирана на проект, включва **Време** и определена задача, **Т1** е свързано с него като изискуемо. Ако има втори ред на договор, който включва **Разходи** , можете да свържете Т1 задача на ред на договор като без такса. Резултатът е, че цялото време, записано в задачата, се заплаща и всички разходи не се заплащат.

Типът на таксуване на задача може да бъде конфигуриран на раздела **Платими задачи** на аспекти на договор чрез актуализиране на полето **Тип фактуриране** на подрешетка за задачи на аспекти на договор. Като алтернатива можете да актуализирате полето **Тип фактуриране** на подмрежата на настройката за фактуриране на задача на проект, което показва аспекти на договор, свързани със задача.

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a>Актуализирайте роля да бъде таксувана или без такса

Роля може да бъде изискуема или без такса за определен ред на договор.

Типът таксуване на роля може да бъде конфигуриран на раздела **Платими роли** на договорна линия. За да направите това, актуализирайте **Тип фактуриране** поле на **Платими роли** подрешетка.

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a>Актуализирайте категорията на трансакция, за да бъде таксувана или без такса

Категорията на транзакциите може да бъде изискуема или без такса за определен ред на договор.

Типът таксуване на трансакция може да бъде конфигуриран на раздела **Платими категории** на базиран на проект ред на договор. За да направите това, актуализирайте **Тип фактуриране** поле на **Платими категории** подрешетка.

### <a name="resolve-chargeability"></a>Решаване на възможността за фактуриране

Прогноза или действителни данни, създадени за времето, ще се считат за изискуем само ако **Време** е включено в ред на договор и ако **Задача** и **Роля** са конфигурирани като изискуеми на ред на договор.

Прогноза или действителни данни, създадени за разход, се считат за изискуеми само ако **разход** е включено в ред на договор и ако **Задача** и категории **Трансакция** са конфигурирани като изискуеми на ред на договор.


| Включва време | Включва разход | Включва задачи | Роля           | Категория       | Задача                                                                                                      |
|---------------|------------------|----------------|----------------|----------------|-----------------------------------------------------------------------------------------------------------|
| Да           | Да              | Целият проект | Платими     | Платими     | Таксуване по действителни данни за време: **Платимо** </br> Вид на фактурирането за действителни разходи: **Платимо**           |
| Да           | Да              | Избрани задачи | Платими     | Платими     | Таксуване по действителни данни за време: **Платимо** </br> Вид на фактурирането за действителни разходи: **Платимо**           |
| Да           | Да              | Избрани задачи | Нетаксуеми | Платими     | Таксуване по действително време: **Неплатимо** </br> Вид на фактурирането за действителни разходи: **Платимо**       |
| Да           | Да              | Избрани задачи | Платими     | Платими     | Таксуване по действително време: **Неплатимо** </br> Вид на фактурирането за действителни разходи: **Неплатимо** |
| Да           | Да              | Избрани задачи | Нетаксуеми | Платими     | Таксуване по действително време: **Неплатимо** </br> Вид на фактурирането за действителни разходи: **Неплатимо** |
| Да           | Да              | Избрани задачи | Нетаксуеми | Нетаксуеми | Таксуване по действително време: **Неплатимо** </br> Вид на фактурирането за действителни разходи: **Неплатимо** |
| No            | Да              | Целият проект | Не може да бъде зададено   | Платими     | Таксуване по действително време: **Неналично**</br>Вид на фактурирането за действителни разходи: **Платимо**          |
| No            | Да              | Целият проект | Не може да бъде зададено   | Нетаксуеми | Таксуване по действително време: **Неналично**</br> Вид на фактурирането за действителни разходи: **Неплатимо**     |
| Да           | No               | Целият проект | Платими     | Не може да бъде зададено   | Таксуване по действителни данни за време: **Платимо** </br> Вид на фактурирането за действителни разходи: **Неналично**        |
| Да           | No               | Целият проект | Нетаксуеми | Не може да бъде зададено   | Таксуване по действително време: **Неплатимо** </br>Вид на фактурирането за действителни разходи: **Неналично**   |