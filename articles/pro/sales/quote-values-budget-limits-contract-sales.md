---
title: Обобщена информация за оферта по проект (Продажби)
description: Тази тема предоставя информация за информацията и настройките, които се отнасят за оферти на проекта и влияят върху тях. (Sales)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d050258ae457bb4392d5fa761442cfc7a444feb0
ms.sourcegitcommit: f6509f7d50de4d4ebb92c1bf2cfcdf09f17458eb
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/06/2020
ms.locfileid: "3966733"
---
# <a name="summary-information-on-a-project-quote-sales"></a>Обобщена информация за оферта по проект (Продажби)

_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_

Тази статия обяснява информацията, която се отнася за оферта за проект. Това включва настройките, които засягат всички редове на офертите, както и информация за цената, която е обобщена във всички договорени покупки, за да управлява KPI на офертата на проекта.

Следващата таблица изброява обобщените информационни полета за проектна оферта, които са уникални за Dynamics 365 Project Operations или имат някои важни промени в поведението от оферти на Dynamics 365 Sales.

| **Поле** | **Местонахождение** | **Уместност, цел и насоки** | **Въздействие надолу по течението** |
| --- | --- | --- | --- |
| Тип | Раздел „Обобщение” (скрит) | Този набор от опции хешира следните опции:</br>- Работен (базиран само когато е инсталиран Project Operations)</br>- Базирано на елемент (базиран само когато са инсталирани Project Operations и Sales)</br>- Базирана на сервизна поддръжка (налична, когато Dynamics 365 Field Service е инсталиран) | Когато използвате приложението Project Operations, стойността на това поле автоматично се задава на **На базата на работа**. Това класифицира офертата като проектно-базирана оферта. Офертата трябва да се основава на проект, за да се даде възможност за всички специфични за проекта разширения и функционалност. |
| Потенциален клиент | Раздел „Резюме“ | Препратка към записа на компанията или акаунта на клиента. Когато оферта се създава от възможност, това поле се копира от съответното поле на възможността. | Валутата в офертата на проекта е по подразбиране въз основа на валутата на клиента. Това обаче не може да се промени преди записването на офертата. |
| Диспечер на партньори | Раздел „Резюме“ | Името на мениджъра на акаунт за тази сделка. Когато оферта се създава от възможност, това поле се копира от съответното поле на възможността. | Мениджърът на акаунтите отговаря за управлението на взаимоотношенията с клиента чрез завършването на този проект. Въз основа на резервирания запис на ресурс, свързан с мениджъра на акаунти, възложителят по подразбиране задава офертата на проекта. |
| Единица, сключваща договора | Раздел „Резюме“ | Организационната единица, която отговаря за доставката на проекта или проектите, свързани с тази оферта. Когато оферта се създава от възможност, това поле се копира от съответното поле на възможността. | Възложителят е подразделението на компанията, което ще изпълнява проектите след приключване на сделката. Всяко сключващо звено има валута и тази валута се използва за отчитане на приблизителни и действителни разходи, направени по време на изпълнението на проекта. |
| Ценова листа за продукта | Раздел „Резюме“ | Това е ценовата листа, която се използва за определяне на цените по подразбиране на продуктовите котировъчни редове. Списъкът с опции за това поле показва списък с ценови листи, където валутата на ценовия лист съответства на валутата в офертата. Когато оферта се създава от възможност, това поле се копира от съответното поле на възможността. Това поле за възможността е по подразбиране от записа на акаунта, но може да бъде променено. | Когато дадена оферта бъде спечелена, стойността на полето се копира в договора по проект, който се създава. |
| Валута | Раздел „Резюме“ | Това показва валутата, която ще се използва за отчитане на стойността на тази сделка. Това е също и валутата, според която клиентът ще бъде фактуриран, ако сделката бъде спечелена. Когато оферта се създава от възможност, това поле се копира от съответното поле на възможността. Това поле за възможността е по подразбиране от записа на акаунта, но може да бъде променено от потребителя. | След като офертата бъде запазена, това поле вече не може да се редактира. Това се използва за довеждане по подразбиране на продукт и ценовите листи на проект на офертата. Валутата в офертата се използва за съответствие с валутата в ценовата листа. |
| Ограничение, което да не се надвишава | Раздел „Резюме“ | Това показва договореното ограничение на крайната стойност, с която клиентът се съгласява за тази сделка. | Това ограничение се оценява по време на изпълнение и е приложимо за всички договорени покупки и проекти, свързани с тази сделка. |
| Заявена дата за доставка | Раздел „Резюме“ | Когато оферта се създава от възможност, това поле се копира от съответното поле на възможността. | Тази дата се използва като крайна дата за генериране на графици за фактури. |

По-долу са разделите и KPI, налични в офертата на проекта, които са уникални за Project Operations или имат някои важни промени в поведението от оферти за продажби:

| **Поле** | **Местонахождение** | **Уместност, цел и насоки** |
| --- | --- | --- |
| Анализ на рентабилност | Раздел в офертата | Разделът показва следните метрики:</br>- Общ таксуем разход</br></br>- Общ нетаксуем разход</br>- Общ приход</br>- Общ приход (основа)</br>- Брутен марж</br>- Коригиран брутен марж|
| Сравнение с очаквания на клиент | Раздел в офертата | Този раздел показва следните метрики:</br>- Очаквано завършване</br>- Заявено завършване</br>- Бюджет на клиента</br>- Оферирана стойност |
| Анализ на оферта | Раздел в офертата | Този раздел обобщава следните най-добри KPI за оферта за проект</br>- Сравнение с очакванията на клиентите за бюджет и график</br>- Брутен марж</br>- Коригиран брутен марж |
