---
title: Копиране на възможности, базирани на проект
description: Тази тема предоставя информация за това как да копирате базирани на проект възможности в Project Operations.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 89f5a63581f36b30634bdd302a6d360d6b5e75bd
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071759"
---
# <a name="copy-project-based-opportunities"></a>Копиране на възможности, базирани на проект

_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_


Възможностите за проекти могат лесно да бъдат копирани, за да се създадат нови възможности за проекти. 

1. Отидете на **Възможности за проекти** страница от списъка и изберете възможност от списъка. Или отворете страницата с подробности за конкретна възможност. 
2. От която и да е страница изберете **копие**. Ще се отвори диалогова страница, която съдържа следната информация за полето. В зависимост от избраните в този диалог стойности процесът на копиране може да се промени.

    | **Поле** | **Уместност, цел и насоки** | **Въздействие надолу по течението** |
    | --- | --- | --- |
    | Предмет на разговор | Въведете сродна темата на целевата възможност. Когато диалоговият прозорец се отвори, системата ще го зададе на темата на изходната възможност с **-копие** , приложено към него. | Няма въздействие за това поле надолу по веригата. |
    | Клиент | Препратки към записа на компанията или акаунта на клиента. Когато диалоговият прозорец се отвори, системата ще го настрои към акаунта в възможността на източник. | Това поле е основният клиент на възможността. |
    | Единица, сключваща договора | Организационната единица, която отговаря за доставката на проекти, свързани с тази сделка. Когато диалоговият прозорец се отвори, системата ще го настрои към договарящата се единица в възможността на източника. | Договарящата се единица е подразделението на компанията, което ще изпълнява проектите след приключване на сделката. Всяко сключващо звено има валута и тази валута се използва за отчитане на приблизителни и действителни разходи, направени по време на проекта. |
    | Валута | Валутата, според която се изпълняват трансакциите на сделката. Когато диалоговата страница се отвори, системата ще я зададе на валутата на възможността на източник. | Валутата се използва за задаване на ценоразпис по подразбиране и изграждане на финансови оценки по котировката. В крайна сметка валутата се използва за фактуриране на клиента при спечелване на сделката. |
    | Копиране на ценообразуването | Стойност Да / Не, която показва дали ценообразуването на възможността трябва да бъде копирано от възможността източник. | Ако **Да** е избрано, ценовите листи се копират от източника до целевата възможност. Ако **Не** е избрано, ценовите листи се възстановяват по подразбиране въз основа на най-новите ценови листи, които са настроени. |

3. Изберете **OK**. Системата създава копие на възможността за проект въз основа на избраните параметри и се отваря новата възможност за проект.