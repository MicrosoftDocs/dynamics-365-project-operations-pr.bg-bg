---
title: Заглавка/резюме на възможност
description: Тази тема предоставя информация за базирани на проекти сделки и базирани на проекти линии за възможности.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: c4e91c1a869347ac1182db2de1ab9244309eb856
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071695"
---
# <a name="opportunity-headersummary"></a>Заглавка/резюме на възможност

_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_


Заглавката на възможност или резюмето обхваща цялостната информация за сделка, базирана на проект, която се отнася за всички редове на базата на проект.

Базираните на проекти възможности в Dynamics 365 Project Operations са разширения на възможностите в Dynamics 365 Sales. Тези разширения предоставят допълнителна функционалност, която е специфична и необходима за възможностите, базирани на проекти. Тези разширения могат да включват нови полета и действия на лентата, налични в базирани на проекти възможности. Може да намерите някои полета, функционалност и логика по подразбиране, която е налична в Продажби не е налична в Project Operations.

Следващата таблица включва полетата в базирана на проект възможност, които са уникални за операциите на проекта или имат някои важни промени в поведението от Възможностите в продажбите.

| **Поле** | **Местонахождение** | **Уместност, цел и насоки** | **Въздействие надолу по течението** |
| --- | --- | --- | --- |
| Тип | Раздел „Общи” (скрит) | Този набор от опции има следните опции:</br>- Работен (налично само с Project Operations)</br>- Базирано на елемент (базиран само когато са инсталирани Project Operations и Sales)</br>- Базирана на сервизна поддръжка (налична, когато Field Service е инсталиран) | Когато използвате Project Operations, стойността на това поле автоматично се задава на **На базата на работа** , което класифицира възможността като базирана на проект. Възможността трябва да е базирана на проект, за да се активират всички специфични за проекта разширения и функционалност в процеса на продажби надолу по веригата за тази сделка. |
| Притежаваща фирма | Раздел „Общи” | Това е компанията или юридическото лице, което ще достави проекта за клиента. | Информацията за това поле ще бъде копирана в съответното поле на офертата на проекта, която е създадена от тази възможност. |
| Контакт | Раздел „Общи” | Препратка към основния контакт на клиента за тази сделка. | |
| Клиент | Раздел „Общи” | Препратка към записа на компанията или акаунта на клиента. | |
| Диспечер на партньори | Раздел „Общи” | Името на мениджъра на акаунт за тази базирана на проект възможност. | Мениджърът на акаунтите отговаря за управлението на взаимоотношенията с клиента чрез завършването на този проект. Въз основа на резервирания запис на ресурс, свързан с мениджъра на акаунти, договарящата се единица се задава по подразбиране. |
| Единица, сключваща договора | Раздел „Общи” | Организационната единица, която отговаря за доставката на проекта или проектите, свързани с тази сделка. | Възложителят е подразделението на компанията, което ще изпълнява проектите след приключване на сделката. Всяко сключващо звено има валута и тази валута се използва за отчитане на приблизителни и действителни разходи, направени по време на проекта. |

За всички останали полета и раздели на раздела **Обобщение** на възможността, вижте [Създаване или редактиране на възможности (Център за продажби и продажби)](https://docs.microsoft.com/dynamics365/sales-enterprise/create-edit-opportunity-sales).