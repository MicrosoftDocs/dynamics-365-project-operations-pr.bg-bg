---
title: Копиране на ценови листи
description: Тази тема предоставя информация за това как да копирате ценови листи в Project Operations.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 91ee798a206ea5200780c8ebafc8f99cd9a3e219
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071859"
---
# <a name="copy-price-lists"></a>Копиране на ценови листи

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

Можете да създавате копия на ценови листи в Dynamics 365 Project Operations. Например можете да създадете ценоразписи за предстоящата година, като използвате ценоразпис от текущата година.  Или можете да копирате ценоразпис за цените на сметките и продажните цени от ценовите листи за разходи. 

За да направите копие на ценовата листа, изпълнете следните стъпки.

1. Отворете ценовата листа, от която искате да копирате, и изберете **Копие**.
2. Въведете необходимата информация, за да копирате ценовата листа. Следващата таблица показва съображения, които трябва да имате предвид при въвеждане на информация.

| Поле | Уместност, цел и насоки | Въздействие надолу по течението |
| --- | --- | --- |
| Име | Името на ценовата листа на източника с добавено **-copy**. | Ценовата листа включва тази стойност на всички страници на списъка и падащите опции. |
| Контекст | Въведете контекста, който искате за целевата ценова листа. | Ценова листа, което има контекст, зададен на **Разходи** , се използва за търсене на цената за разчети на разходите и фактически разходи. Ценова листа, което има контекст, зададен на **Продажби** се използва за търсене на цената за разчети на продажби и действителни данни за продажби. Само ценови листи, които имат зададен контекст **Продажби** могат да бъдат прикачени към ценова листа на проект за клиент, оферти или договор. |
| Начална дата | Началната дата на периода, в който е ценовата листа, е в сила. | Заедно с **Крайна дата** това поле се използва, за да се определи кой ценоразпис е приложим за определена прогнозна или действителна линия. |
| Крайна дата | Крайната дата на периода, в който е ценовата листа, е в сила. | Заедно с **Начална дата** това поле се използва, за да се определи кой ценоразпис е приложим за определена прогнозна или действителна линия. |
| Валута | Валутата на ценовата листа на източника. Това може да се променя. | Когато това се промени, всички получени ценови линии за труд, разходи и артикули от продуктовия каталог се преобразуват в целевата валута на ценовата листа по време на копирането. |
| Единица за време | Валутата на ценовата листа на източника. Това може да се променя. | Когато това се промени, всички получени ценови линии за елементи на труд се преобразуват в целевата единица на ценовата листа по време на копирането. Използва се преобразуването от настройката на единицата за единица време на ценовия списък на източника и целевата единица време. |
| Описание | Описание на ценовата листа на източника с добавено **-copy**. Това е текстово поле и ви позволява да имате многоредово описание на ценовата листа. | Това поле е показано в **Асоциираните** изгледи на ценовата листа в различни обекти, които имат свързани ценови листи. |

3. Записване на ценовата листа. 

## <a name="update-a-price-list-by-applying-a-mark-up-to-all-the-prices"></a>Актуализирайте ценоразпис, като приложите надценка към всички цени

1. На разделите **Роля** , **Категория** и **Елемент от ценовата листа** от ценова листа, можете да изберете **Актуализиране на цените** за прилагане на надценка за всички цени в подмрежата. 
2. На страницата за диалог, която се отваря, въведете надценка. Можете също така да въведете отрицателен процент на надценка, за да намалите цените с определен процент. 
3. Изберете **ОК** на страницата за диалог и след това проверете дали цените в подмрежата отразяват направените от вас промени.