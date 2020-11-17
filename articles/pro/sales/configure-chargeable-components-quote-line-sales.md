---
title: Конфигуриране на платимите компоненти на ред на оферта
description: Тази тема предоставя информация за настройване на таксувани и неначисляеми компоненти на базирана на проект линия за оферти.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: e0b64d7edb21df127bf7544f044de7f3c496dfe3
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071941"
---
# <a name="configure-the-chargeable-components-of-a-quote-line"></a>Конфигуриране на платимите компоненти на ред на оферта

_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_

Базовата линия на проекта има концепцията за *включени* компоненти и *таксуеми* компоненти.

Включените компоненти са обект на:

  - Метод на фактуриране и разделяне на клиента
  - Ограничения, които да не се надвишават 
  - Настройки на честотата на фактурите, дефинирани на базирана на проекта линия за оферти

Подмножество от включените компоненти може да бъде маркирано като таксувано с помощта на полето **Тип фактуриране**. Полето **Тип фактуриране** е набор от опции, който позволява следните стойности в контекста на кавичка:

  - Платими
  - Нетаксуеми

Компонентите, които се заплащат, могат да бъдат дефинирани за задачи, роли и категории транзакции.

Плащаемостта се определя в задачите за котировъчен ред и се прилага за всички класове транзакции, включени в този ред. Ако полето **Включете задачи** е зададено на **Цял проект** или оставено празно, разделът **Платими задачи** не е наличен.

Плащаемостта се определя в ролите за ред на оферта и се прилага само за класа трансакция **Време**. Ако полето **Включете време** е зададено на **Не** на ред на оферта по проект разделът **Платими роли** не е наличен.

Плащаемостта се определя в категориите трансакция за ред на оферта и се прилага само за класа трансакция **разход**. Ако полето **Включете разходи** е зададено на **Не** на ред на оферта по проект разделът **Платими категории** не е наличен.

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a>Актуализирайте проектна задача, за да бъде таксувана или без такса

Проектната задача може да бъде таксувана или без такса в контекста на конкретен проект, базиран на котировка, което прави възможна следната настройка:

Ако ред на оферта, базиран на проект, включва **Време** и задачата **Т1** , задачата е свързана с ред на оферта като платена. Ако има втори ред, който включва **Разходи** , можете да свържете **Т1** задача на ред на оферта като без такса. Резултатът е, че цялото време, записано в задачата, се заплаща и всички разходи, записани в задачата, не се заплащат.

Типът на таксуване на задача може да бъде конфигуриран на раздела **Платими задачи** в раздела за котировки, базиран на проект, чрез актуализиране на полето **Тип фактуриране** на **Задачи за ред на оферта** подрешетка. Като алтернатива можете да актуализирате типа на фактуриране за проектна задача в **Тип фактуриране** поле в подмрежата на настройката за фактуриране на задача на проект, което показва редовете на офертите, свързани със задача.

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a>Актуализирайте роля да бъде таксувана или без такса

Ролята може да бъде изискуема или без такса в контекста на конкретен проект, базиран на котировка.

Типът на таксуване на роля може да бъде конфигуриран на раздела **Платими роли** на ред на оферта чрез актуализиране на полето **Тип фактуриране** на **Таксуеми роли** подрешетка.

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a>Актуализирайте категорията на трансакция, за да бъде таксувана или без такса

Категорията на транзакциите може да бъде изискуема или без такса за определен ред на офертата.

Типът на фактуриране на трансакция може да бъде конфигуриран на раздела **Платими категории** на ред на оферта чрез актуализиране на полето **Тип фактуриране** на **Таксуеми категории** подрешетка.

### <a name="resolve-chargeability"></a>Решаване на възможността за фактуриране
Прогноза или действителни данни, създадени за времето, ще се считат за изискуем само ако **Време** е включено в ред на оферта и ако **Задача** и **Роля** са конфигурирани като изискуеми на линията на офертата.

Прогноза или действителни данни, създадени за разход, ще се считат за изискуем само ако **разход** е включено в ред на оферта и ако **Задача** и **Категория на трансакция** са конфигурирани като изискуеми на линията на офертата.

| Включва време | Включва разход | Включени задачи | Роля | Категория | Задача | Плащане |
| --- | --- | --- | --- | --- | --- | --- |
| Да | Да | Целият проект | Платими | Платими | Не може да бъде зададено | Таксуване по действително време: Платимо </br>Вид на фактурирането за действителни разходи: Платимо |
| Да | Да | Само избрани задачи | Платими | Платими | Платими | Таксуване по действително време: Платимо</br>Вид на фактурирането за действителни разходи: Платимо |
| Да | Да | Само избрани задачи | Нетаксуеми | Платими | Платими | Таксуване по действително време: Неплатимо</br>Вид на фактурирането за действителни разходи: Платимо |
| Да | Да | Само избрани задачи | Платими | Платими | Нетаксуемо | Таксуване по действително време: Неплатимо</br> Вид на фактурирането за действителни разходи: Неплатимо |
| Да | Да | Само избрани задачи | Нетаксуемо | Платими | Нетаксуемо | Таксуване по действително време: Неплатимо</br> Вид на фактурирането за действителни разходи: Неплатимо |
| Да | Да | Само избрани задачи | Нетаксуемо | Нетаксуемо | Платими | Таксуване по действително време: Неплатимо</br> Вид на фактурирането за действителни разходи: Неплатимо |
| No | Да | Целият проект | Не може да бъде зададено | Платими | Не може да бъде зададено | Таксуване по действително време: Неналично </br>Вид на фактурирането за действителни разходи: Платимо |
| No | Да | Целият проект | Не може да бъде зададено | Нетаксуеми | Не може да бъде зададено | Таксуване по действително време: Неналично </br>Вид на фактурирането за действителни разходи: Неплатимо |
| Да | No | Целият проект | Платими | Не може да бъде зададено | Не може да бъде зададено | Таксуване по действително време: Платимо</br>Вид на фактурирането за действителни разходи: Неналично |
| Да | No | Целият проект | Нетаксуеми | Не може да бъде зададено | Не може да бъде зададено | Таксуване по действително време: Неплатимо </br>Вид на фактурирането за действителни разходи: Неналично |