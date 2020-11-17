---
title: Разширяване на времеви записи
description: Тази тема предоставя информация за това как разработчиците могат да разширят контрола за въвеждане на време.
author: stsporen
manager: Annbe
ms.date: 10/08/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 190ad9e1f9ced690aee953ed992bf7aa2844c3b3
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071719"
---
# <a name="extending-time-entries"></a>Разширяване на времеви записи

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

Dynamics 365 Project Operations включва персонализиран контрол за въвеждане на време. Тази контрола включва следните функции:

- Въведете време хоризонтално за една седмица
- Общо за ден, ред или седмица
- Копирайте редове или седмици
- Въвеждане на време през HH: mm или HH.hh (автоматично се преобразува в HH.hh)
- Импортиране от задания, резервации или срещи

Удължаването на времето за въвеждане е възможно в две области:
- [Добавете персонализирани записи за време за собствена употреба](#add)
- [Персонализиране на контролата за седмичния времеви запис](#customize)

## <a name="add-custom-time-entries-for-your-own-use"></a><a name="add"></a>Добавете персонализирани записи за време за собствена употреба

Въвеждането на времето е основна същност, използвана в множество сценарии. През априлска вълна 1 2020 беше представено основното решение на TESA. TESA предоставя обект **Настройки** и нова роля на защита **Потребител за времеви запис**. Новите полета **msdyn_start** и **msdyn_end** , които имат пряко отношение към **msdyn_duration** , също са включени. Новият обект, права за достъп, и полетата позволяват по-унифициран подход към времето в множество продукти.


### <a name="time-source-entity"></a>Обект на източник на време
| Поле | Описание | 
|-------|------------|
| Име  | Името на записа на източника на време, използван като стойност за избор при създаването на времеви записи. |
| Източник на време по подразбиране [Източник на време: isdefault] | По подразбиране само един източник на време може да бъде маркиран по подразбиране. Това позволява на записите по подразбиране да бъдат източник на време, ако такъв не е посочен. |
|Тип източник на време [Източник на време: тип източник] | Типът източник е опция (тип източник на времеви запис), която позволява свързването на източника на време с приложение. Microsoft запазва стойности, по-големи от 190 000 000.|


### <a name="time-entries-and-the-time-source-entity"></a>Въвеждане на време и обект на източника на време
Всеки запис на време е свързан със запис на източник на време. Този запис определя как и кои приложения да обработват въвеждането на времето.

Въвеждането на времето винаги е един непрекъснат блок от време със свързани началото, края и продължителността.

Логиката автоматично ще актуализира записа за въвеждане на време в следните ситуации:

- Ако са предоставени две от трите следващи полета, третото се изчислява автоматично: 

    - **msdyn_start**
    - **msdyn_end**
    - **msdyn_duration**

- Полетата **msdyn_start** и **msdyn_end** отчитат часовата зона.
- Записи във времето, създадени само с **msdyn_date** и **msdyn_duration** посоченото ще започне в полунощ. Полетата **msdyn_start** и **msdyn_end** ще се актуализират съответно.

#### <a name="time-entry-types"></a>Типове времеви записи

Записите за въвеждане на време имат асоцииран тип, който определя поведението в потока на подаване за свързаното приложение.

|Етикет | Стойност|
|-----|-----|
|При почивка   |192,355,000|
|Пътуване | 192,355,001|
|Извънреден труд   | 192,354,320|
|Работа   | 192,350,000|
|Отсъствие    | 192,350,001|
|Отпуска   | 192,350,002|



## <a name="customize-the-weekly-time-entry-control"></a><a name="customize"></a>Персонализиране на контролата за седмичния времеви запис
Разработчиците могат да добавят допълнителни полета и справки към други обекти и да прилагат персонализирани бизнес правила в подкрепа на своите бизнес сценарии.

### <a name="add-custom-fields-with-lookups-to-other-entities"></a>Добавяне на персонализирани полета със справочни полета за други обекти
Има три основни стъпки за добавяне на персонализирано поле към мрежата на седмични записи за време.

1. Добавете персонализирано поле в диалоговия прозорец за бързо създаване.
2. Конфигурирайте мрежата, за да се показва персонализираното поле.
3. Добавете персонализираното поле към потока от задачи за редактиране на ред или потока от задачи за редактиране на клетка.

Уверете се, че новото поле има необходимите валидирания в потока от задачи за редактиране на ред или клетка. Като част от тази стъпка заключете полето въз основа на състоянието на записа за време.

### <a name="add-the-custom-field-to-the-quick-create-dialog-box"></a>Добавяне на персонализираното поле в диалоговия прозорец за бързо създаване
Добавете персонализираното поле към диалоговия прозорец за бързо създаване **Създаване на запис за време**. След това, когато времевите записи бъдат добавени, стойност може да бъде добавена чрез избиране на **Създаване**.

### <a name="configure-the-grid-to-show-the-custom-field"></a>Конфигуриране на мрежата, за да се показва персонализираното поле
Има два начина за добавяне на персонализирано поле към мрежата на седмични записи за време:

  - Персонализирайте изгледа и добавете персонализирано поле
  - Създаване на нов персонализиран времеви запис по подразбиране 


#### <a name="customize-a-view-and-add-a-custom-field"></a>Персонализирайте изгледа и добавете персонализирано поле

Персонализирайте изгледа **Моите седмични записи за време** и добавете персонализирано поле към него. Можете да изберете позицията и размера на персонализирано поле в мрежата, като редактирате тези свойства в изгледа.

#### <a name="create-a-new-default-custom-time-entry"></a>Създаване на нов персонализиран времеви запис по подразбиране

Този изглед трябва да съдържа полетата **Описание** и **Външни коментари** в допълнение към колоните, които искате да имате в мрежата. 

1. Изберете позицията, размера и реда на сортиране по подразбиране на мрежата, като редактирате тези свойства в изгледа. 
2. Конфигурирайте персонализираната контрола за този изглед, така че да е контрола **Мрежа за записи за време**. 
3. Добавете тази контрола към изгледа и я изберете за уеб, телефон и таблет. 
4. Конфигурирайте параметрите за мрежата за седмични записи за време. 
5. Задайте полето **Начална дата** на **msdyn_date** , задайте полето **Продължителност** на **msdyn_duration** и задайте полето **Състояние** на **msdyn_entrystatus**. 
6. За изгледа по подразбиране, **Списък на състоянието само за четене** полето е зададено на **192350002,192350003,192350004**. Полето **Редакция на реда на задачите** е зададено на **msdyn_timeentryrowedit**. Полето **Поток на задача за редактиране на клетка** е зададено на **msdyn_timeentryedit**. 
7. Можете да персонализирате тези полета, за да добавите или премахнете състояние само за четене или да използвате различна функционалност, базирана на задачи (TBX), за редактиране на редове или клетки. Тези полета вече са обвързани със статична стойност.


> [!NOTE] 
> И двете опции ще премахнат някои стандартни филтрирания в обектите **Проект** и **Задача на проект** , така че всички справочни изгледи за обектите ще бъдат видими. Стандартно се виждат само съответните справочни изгледи.

Определете подходящия поток от задачи за персонализираното поле. Ако сте добавили полето към мрежата, трябва да отидете в потока от задачи за редактиране на ред, който се използва за полета, които се прилагат за целия ред от записи за време. Ако персонализираното поле има уникална стойност всеки ден, като например персонализирано поле за **Краен час** , трябва да отидете в потока от задачи за редактиране на клетка.

За да добавите персонализираното поле към поток от задачи, плъзнете елемент **Поле** в съответната позиция на страницата и след това задайте свойствата на полето. Задайте свойството **Източник** на **Запис за време** и задайте свойството **Поле за данни** на персонализираното поле. Свойството **Поле** посочва показваното име на TBX страницата. Изберете **Прилагане** , за да запазите промените в полето и след това изберете **Актуализиране** , за да запазите промените на страницата.

За да използвате нова потребителска TBX страница вместо това, създайте нов процес. Задайте категорията на **Поток на бизнес процес** , задайте обекта на **Запис за време** и задайте типа на бизнес процеса на **Изпълнение на процес като поток от задачи**. Под **Свойства** свойството **Име на страница** трябва да бъде зададено на показваното име за страницата. Добавете всички съответни полета към TBX страницата. Запишете и активирайте процеса. Актуализирайте свойството на персонализираната контрола за съответния поток от задачи на стойността на **Име** в процеса.

### <a name="add-new-option-set-values"></a>Добавяне на стойности на нов набор от опции
За да добавите стойности на набор от опции към стандартно поле, отворете страницата за редактиране за полето и след това под **Тип** изберете **Редактиране** до набора от опции. Добавете нова опция, която има персонализиран етикет и цвят. Ако искате да добавите ново състояние на запис за време, стандартното поле се нарича **Състояние на запис** , а не **Състояние**.

### <a name="designate-a-new-time-entry-status-as-read-only"></a>Обозначаване на ново състояние на запис за време като само за четене
За да обозначите ново състояние на запис за време като само за четене, добавете новата стойност на записа за време в свойството **Списък със състояния само за четене**. Редактируемата част на мрежата на записа за време ще бъде заключена за редове, които имат новото състояние.
След това добавете бизнес правила, за да заключите всички полета в TBX страниците **Редактиране на ред на записи за време** и **Редактиране на записи за време**. Можете да осъществите достъп до бизнес правилата за тези страници, като отворите редактора на поток на бизнес процес за страницата и след това изберете **Бизнес правила**. Можете да добавите новото състояние към условието в съществуващите бизнес правила или да добавите ново бизнес правило за новото състояние.

### <a name="add-custom-validation-rules"></a>Добавяне на персонализирани правила за валидиране
Има два типа правила за валидиране, които можете да добавите за седмичното изживяване на мрежата за въвеждане на време:

- Клиентски бизнес правила, които работят в диалогови прозорци за бързо създаване и на TBX страници.
- Проверки на добавки от страна на сървъра, които се прилагат за всички актуализации за въвеждане на време.

#### <a name="business-rules"></a>Бизнес правила
Използвайте бизнес правила, за да заключвате и отключвате полета, въвеждате стойности по подразбиране в полетата и дефинирате валидации, които изискват информация само от записа на текущия запис за време. Можете да осъществите достъп до бизнес правилата за TBX страница, като отворите редактора на поток на бизнес процес за страницата и след това изберете **Бизнес правила**. След това можете да редактирате съществуващите бизнес правила или да добавите ново бизнес правило. За още по-персонализирани валидирания можете да използвате бизнес правило за изпълнение на JavaScript.

#### <a name="plug-in-validations"></a>Валидирания на добавки
Използвайте добавки за всички валидирания, които изискват повече контекст, отколкото е наличен в един запис за запис на време, или за всички валидирания, които искате да стартирате за вградени актуализации в мрежата. За да завършите валидирането, създайте персонализирана добавка в обекта **Запис за време**.

### <a name="copying-time-entries"></a>Копиране на времеви записи
Използвайте изгледа **Копирайте колони за въвеждане на време** за да дефинирате списъка с полетата за копиране по време на въвеждане на време. **Дата** и **Продължителност** са задължителни полета и не трябва да се премахват от изгледа.