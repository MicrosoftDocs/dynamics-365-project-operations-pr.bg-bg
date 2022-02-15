---
title: Редове за подизпълнение за време
description: Тази тема обяснява как да записвате линии на подизпълнители за време и да записвате закупуването на време от доставчици.
author: rumant
ms.date: 08/05/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 29b38ec9124502e4283b71d13434b1e0420bc413
ms.sourcegitcommit: 74a7e1c9c338fb8a4b0ad57c5560a88b6e02d0b2
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/23/2021
ms.locfileid: "7547231"
---
# <a name="subcontract-lines-for-time"></a>Редове за подизпълнение за време

[!include [banner](../../includes/dataverse-preview.md)]

_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_

Подизпълнител в Dynamics 365 Project Operations може да има линия за подизпълнение за време. Линиите на подизпълнители за време позволяват на ръководителя на проекта да купува време на ресурс на доставчик, за да изпълнява задачи по проекта и изисквания за ресурси.

За да създадете ред на подизпълнител за време в Project Operations, изпълнете следните стъпки.

1. В навигационния екран изберете **Подизпълнения**, и отворете подизпълнение.
2. В раздела **Редове за подизпълнение** изберете **Ново** за създаване на нова линия на подизпълнители.
3. На страницата **Бързо създаване** в полето **Клас на транзакция** изберете **Време**.
4. Въведете останалата необходима информация за поле и след това изберете **Запиши**.

  Следващата таблица предоставя информация за полетата на страницата **Ред на подизпълнение** и страницата **Бързо създаване**.

| **Поле** | **Описание** | **Функционално влияние** |
| --- | --- | --- |
| Име | Име на линията на подизпълнителите, за да ви помогне с идентификацията. | Това ще се показва като първа колона във всички справки, базирани на редове на подизпълнители. |
| Описание | Кратко описание на услугите, които се закупуват за подизпълнителя. |Нищо |
| Тип ред |   Тази стойност има стойност по подразбиране **базирано на количество**.| Нищо |
| Метод на фактуриране | Това е набор от опции, който представлява двата основни модела на договаряне, поддържани от Project Operations: **Фиксирана цена** и **Време и материал**. | Въз основа на избрания метод на фактуриране график на фактури, базиран на етапи, се предоставя за линиите на подизпълнители с метода на таксуване с фиксирана цена. |
| Клас на трансакция | Стойността по подразбиране е **Време**. | Това показва, че подизпълнителната линия се използва за записване на покупка на време на подизпълнител. |
| Роля | Изберете ролята на ресурсите на подизпълнителите, чието време се купува. | Ролята, изпълнявана от ресурсите на подизпълнителя, определя цената на покупката. |
| Заявено начало | Въведете датата, когато са необходими ресурси на подизпълнителя, за да започне работа. | Това се използва за избор на ценова листа за проект от ценоразписа на проекта, приложен към подизпълнението. Цената на ролята по договора за подизпълнение идва от тази ценова листа. |
| Заявен край | Въведете датата, на която приключва възлагането на ресурса на подизпълнителя. | Това ще се използва за показване на предупреждения, когато ръководителят на проекта черпи от капацитета за изисквания за ресурси, възникващи след тази дата. |
| Поръчано количество | Въведете броя часове на ролята, закупена от доставчика. | Това ще се използва за показване на предупреждения, когато ръководителят на проекта черпи с надвишаване от капацитета за изисквания за ресурси. |
| Опаковъчна единица | Стойността по подразбиране е **опаковъчна единица за време**, който не може да бъде променен. | Нищо|
| Единица | По подразбиране за това поле е основната единица за часове от **опаковъчна единица за време**. Можете да промените тази стойност, за да купите всяка единица от **опаковъчна единица за време**, като ден или седмица. | Комбинацията от **Роля** и **единица** ще се използва по подразбиране или се изчислява за единичната цена за реда на подизпълнението. |
| Единична цена | Цената на единица по подразбиране използва комбинацията от **Роля** и **единица** от ценоразписа на проекта, който е приложим за датата **Заявено начало** на линията на подизпълнители. | Когато в приложимия ценоразпис на проекта цената е зададена в различна единица от единицата на договора за подизпълнение, системата използва преобразуването на единица за изчисляване на единичната цена. |
| Междинна сума |    Това е поле само за четене, което се изчислява като Количество X Единична цена, ако са въведени както стойностите на количеството, така и единичната цена. Ако или Количество, Единична цена или и двете са празни, можете да въведете стойността в полето. | Нищо|
| Данък върху продажбите |   Въведете сумата на данъка върху продажбите. |Нищо |
| Обща сума | Общата сума на реда за подизпълнение, включително данъци. Това поле се изчислява като междинна сума + данък продажби.|Нищо |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]