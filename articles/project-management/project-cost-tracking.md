---
title: Проследяване на цената на проект
description: Тази тема предоставя информация за това как Project Operations проследява напредъка спрямо разходите за труд и разходите за даден проект.
author: rumant
ms.date: 03/22/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d37df64db1808722b7851c952c20be731aa2d670fe066c02ef90386712487407
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/06/2021
ms.locfileid: "6987783"
---
# <a name="labor-cost-tracking-on-projects"></a>Проследяване на разходите за труд по проекти

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

Dynamics 365 Project Operations проследява прогнозите за труда и харчи при най-ниската необходима детайлност по плана на проекта. Финансовата оценка на разходите за труд се основава на планираните усилия и родовите или наименовани ресурси, които се присвояват на всяка задача от възел в плана на проекта. Когато проектът започне и хората започнат да отчитат времето за различни проектни задачи, реалните разходи за труд се обобщават, което започва изчисляване на прогнозите.

## <a name="labor-cost-tracking-view"></a>Изглед за проследяване на разходи за труд

На страницата **Проекти** в раздела **Проследяване**, можете да изберете **Проследяване** > **Разходи**, за да отворите изгледа **Проследяване на разходите**, за да видите напредъка на разходите за труд за всяка задача в плана на проекта. Тази гледна точка също сравнява действителните разходи за труд, изразходвани за дадена задача, с планираните разходи за труд на задачата. Project Operations използва следните формули за изчисляване на показателите за разходите за труд:

- **Планирани разходи**: Прогнозна цена на всички задания на ресурси за всяка задача на възел на листа
- **Действителен разход**: Сума от всички фактически разходи за времето, записано за задачата
- **Процент на потреблението на разходите**: Действителни разходи ÷ Приблизителна оценка на разходите
- **Оставащи разходи**: Приблизителна оценка на разходите при завършване – Действителни разходи
- **Разход при завършване**: Оставащ разход + Действителни разходи
- **Разлика в разходите**: Планиран разход – Приблизителна оценка на разходите при завършване

Всяка задача показва прогноза за разликата в разходите за задачата. Ако приключената оценка на разходите е по-голяма от планираната, задачата се предвижда да надхвърли бюджета. Ако приключената оценка на разходите е по-малка от планираната, задачата се предвижда да бъде завършена под бюджета.

>[!NOTE]
> Project Operations показва само разходите за труд на страницата **Проект** на раздела **Проследяване**. Докато материалите и разходите могат да бъдат оценени и проследени за потребление, тези разходи не са включени в разходите, показани в раздела **Проследяване**. Този раздел е предназначен да работи само за препроектиране на разходите за труд чрез препроектиране на усилия.
Всички показани разходни суми се преобразуват във валутата на разходите на проекта от валутата на себестойността на проекта, използвана за определяне на разходната норма. Валутата на разходите по проекта е валутата на възложителя по проекта. Очакваните стойности на разходите за времето, които са показани в раздела **Оценки** на страницата **Проект** може да не се добави към планираните разходи на раздела **Проследяване**. Причината за това несъответствие е поради разликите в начина, по който прогнозираните разходи са обобщени в мрежата **Оценки** и как се изчислява планираната цена на мрежата **Проследяване**. 
>
> - **Раздел „Оценки“** изчислява прогнозната цена, като използва същата валута на ценовата ставка в ценовата листа. След това прогнозната цена във валутата на ценовия списък се преобразува в прогнозната цена във валутата на разходите на проекта. Очакваните разходи във валутата на проекта са показани закръглени до 2 знака след десетичната запетая. В нито един момент по време на това преобразуване не се прилага точност на валутата. 
> - В раздела **Проследяване** планирано изчисляване на разходите следва малко по-различен ред на изчисление, който включва прецизност на валутата, прилагана на два етапа: 
   ><ol>
   ><li>Очакваната сума на разходите във валутата на ценовия списък се преобразува в основната валута (конверсия 1).</li>
   ><li>Очакваната сума на разходите в базовата валутата се преобразува във валута на разход по проекта (конверсия 2). </li>
   ></ol>
   >Прецизността на валутата се прилага и в двете стъпки, за да се получат планирани разходи (в раздела **Проследяване**), който леко се отклонява от очакваните разходи (в изгледа **С времева фаза** на раздела **Оценки**). 
   
## <a name="reprojecting-costs-on-leaf-node-tasks"></a>Препроектиране на разходи за задачи на листни възли

Разходите за труд за задача на листен възел не могат да бъдат директно препроектирани в раздела **Проследяване** на **Страница на проекта**. Можете обаче да използвате изгледа **Проследяване на усилията** за препроектиране на останалите усилия по дадена задача. Това води до преизчисляване на оставащите разходи за задачата. По-долу е описано как работи това.

1. Мениджърът на проекти може да препроектира усилията по задачите, като актуализира стойността по подразбиране в полето **Оставащи усилия** с нова оценка на оставащите усилия по задачата. Препроектирането води до преизчисляване на оценката на усилията на задачата при завършване (EAC), процент на напредъка и прогнозираната дисперсия на усилията за задача. ОПЗ, оценка до завършване (ОДЗ) и процентът на напредъка по обобщаващи задачи също се преизчисляват и създават нова прогноза за разлика в усилията.
2. Въз основа на новата стойност за оставащите усилия по задачата, системата изчислява оставащите разходи за изгледа **Проследяване на разходите**. За да изчисли оставащите разходи въз основа на останалите усилия, системата първо изчислява средната цена на един час усилия за задачата като планирана цена или планирани усилия. Планираните разходи са сумата от разходите за всички задания на ресурси по задачата. Средната цена на час се използва за изчисляване на оставащите разходи за новопроектираното оставащо усилие по задачата.
3. Разходите при цялостно и процентното потребление на задачата за листовия възел се преизчисляват.
4. Разходите на стойността при завършване на обобщените задачи чак до основния възел се преизчисляват.

## <a name="reprojecting-costs-on-summary-tasks"></a>Препроектиране на разходи за задачи за обобщение

Можете да препроектирате разходите за труд за обобщени задачи или задачи за контейнери. Въпреки това, не можете директно да препроектирате разход за труд в обобщена задача по проект в раздела **Проследяване** на страницата **Страница на проекта**. Подобно на задачите на листовия възел, повторното проектиране на обобщени и контейнерни задачи може да се извърши с помощта на изгледа **Проследяване на усилията**. В този изглед можете да препроектирате останалите усилия за обобщена задача, причинявайки преизчисляване на оставащите разходи за обобщената задача. По-долу е описано как работи това.

1. Мениджърът на проекти може да препроектира усилията по обобщените задачите, като актуализира стойността по подразбиране на оставащи усилия с нова оценка на оставащите усилия по задачата. тази актуализация причинява преизчисляване на оценката на усилията на обобщената задачата при завършване (EAC), процент на напредъка и прогнозираната дисперсия на усилията за задача. ОДЗ, ОПЗ и процентът на напредъка по обобщаващи задачи също се преизчисляват и създават нова прогноза за разлика в усилията.
2. Въз основа на новата стойност за оставащите усилия по обобщената задачата, системата изчислява оставащите разходи за изгледа **Проследяване на разходите**. За да изчисли оставащите разходи въз основа на останалите усилия, системата първо изчислява средната цена на един час усилия за обобщената задача като планирана цена или планирани усилия. Средната цена на час се използва за преизчисляване на разхода за новопроектираното оставащо усилие по обобщената задача.
3. Разходите при цялостно и процентното потребление на обобщената задача за листовия възел се преизчисляват.
4. Новият разход при завършване се разпределя до дъщерни задачи в същото съотношение, както оригиналният планиран разход е бил в задачата.
5. Изчислява се новата стойност за разход при завършване за всяка от индивидуалните задачи до задачите в крайния възел. Въз основа на тази стойност, засегнатите дъщерни задачи до листните възли ще имат преизчислени остатъчни разходи и процент на потребление на разходите въз основа на цената на пълна стойност. Тази стойност води до нова прогноза за разликата в разхода на задачата. 


Полето **Ефективност на разходите** може да се зададе от данните за проследяване. Когато отклонението на цената за основния възел в изгледа **Проследяване на разходите** е отрицателно, можете да зададете това поле на **Под бюджета**. Когато отклонението на разходите за основния възел е положително, можете да зададете стойността на **Надвишен бюджет**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]