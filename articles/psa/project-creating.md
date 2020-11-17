---
title: Графици на проекти
description: Тази тема предоставя информация за това как да създадете график.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 3/01/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 9a6b27050a19d8a7f2ed35f74b42bb4f371ad069
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071855"
---
# <a name="project-schedules"></a>Графици на проекти 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Графикът на проекта информира каква работа трябва да бъде извършена, кои ресурси ще изпълняват работата, както и времевата рамка, в която тази работа трябва да бъде завършена. Той отразява цялата работа, свързана с предоставянето на проекта навреме. В Dynamics 365 Project Service Automation можете да създадете график на проект чрез разбиване на работата на управляеми задачи, прогнозиране на времето, което е необходимо за изпълнението на всяка задача, задаване на зависимости на задачите, задаване на продължителност на задачите и оценка на общите ресурси, които ще изпълняват задачите. Графикът на проекта се създава в раздела **График** на страницата на проекта.
 
## <a name="tasks"></a>Задачи

Първата стъпка в създаването на графика на проекта е да се разбие работата на управляеми части. Графикът в PSA поддържа следните функции:

- Основен възел на проект.
- Обобщаващи задачи или задачи в контейнер
- Задачи на краен възел

### <a name="project-root-node"></a>Основен възел на проект.

Основният възел на проекта е обобщената задача от най-високо ниво за проекта. Всички останали задачи по проекта се създават под него. Името на основния възел винаги се задава на името на проекта. Усилията, датите и продължителността на основния възел се обобщават въз основа на стойностите в йерархията под него. Не можете да редактирате свойствата на основния възел. Също така не можете да изтриете основния възел.

### <a name="summary-or-container-tasks"></a>Обобщаващи задачи или задачи в контейнер 

Обобщените задачи имат подзадачи или задачи на контейнер под тях. Те нямат работно усилие или разходи сами по себе си. Вместо това техните работни усилия и разходи са усреднен сбор от работните усилия и разходи за техните задачи на контейнер. Началната дата на обобщената задача е началната дата на задачите на контейнер, а крайната дата е крайната дата на задачите на контейнер. Името на обобщената задача може да се редактира, но не могат да се редактират свойствата за планиране (усилия, дати и продължителност). Ако изтриете обобщена задача, можете също да изтриете всички нейни задачи на контейнер.

### <a name="leaf-node-tasks"></a>Задачи на краен възел

Задачите на краен възел представляват най-подробната работа по проекта. Те имат прогнозни усилия, ресурси, планирани начална и крайна дати и продължителност.
 
## <a name="creating-a-task-hierarchy"></a>Създаване на йерархия на задачите

Можете да създадете йерархия на задачите с помощта на следните опции:

- бутон **Добавяне на задача**
- бутон **Задача с отстъп**
- бутон **Задача с обратен отстъп**
- бутони **Преместване нагоре** и **Преместване надолу**
- Достъпност и клавишни комбинации

### <a name="add-task"></a>Добавяне на задача

Бутонът **Добавяне на задача** ви позволява да създадете нова задача в йерархията. Ако не изберете позиция, задачата се вмъква в края. 

На всяка задача се присвоява ИД на график. ИД на графика представлява дълбочината и позицията на задачата в йерархията. Използва се структурно номериране. За задачи в първото ниво под основния възел на проекта се използва схема за номериране от 1, 2, 3 и т.н. За задачи под първото ниво се използва схема за номериране от 1.1, 1.2, 1.3 и т.н.

### <a name="indent-task"></a>Задача с отстъп

Когато дадена задача е с отстъп навътре, тя става дъщерна на задачата, която е точно над нея. След това ИД на графика на задачата се преизчислява така, че да се базира на ИД на графика на новия му родител, и следва схемата на структурно номериране. Родителската задача сега е обобщена задача или задача на контейнер. Затова тя се превръща в усреднен сбор за своите дъщерни задачи.

### <a name="outdent-task"></a>Задача с обратен отстъп 

Когато дадена задача е с обратен отстъп, тя вече не е дъщерна на задачата, която е била неин родител. След това ИД на графика се преизчислява така, че да отразява актуализираната дълбочина и позиция на задачата в йерархията. Усилията, разходите и датите на предишната родителска задача се преизчисляват така, че да не включват тази задача.

### <a name="move-up-and-move-down"></a>Преместване нагоре и преместване надолу 

Бутоните **Преместване нагоре** и **Преместване надолу** променят позицията на задача в рамките на родителската си йерархия. Промените от този тип не влияят върху усилията, разходите, датите или продължителността на задачата. Засяга се само ИД на графика на задачата. ИД на графика се преизчислява така, че да отразява новата позиция на задачата в списъка с дъщерни задачи на родителя.

### <a name="accessibility-and-keyboard-shortcuts"></a>Достъпност и клавишни комбинации

Мрежата на **График** е напълно достъпна и може да се използва с екранни четци, като например Narrator, JAWS или NVDA. Можете да се движите из областта на мрежата с помощта на клавишите със стрелки (както в Microsoft Excel), можете да използвате клавиша Tab, за да се придвижвате през интерактивни елементи на потребителския интерфейс и можете да използвате клавиша със стрелка надолу, клавиша Enter или интервала, за да изберете и извикате падащите менюта. Заглавките на колоните също са интерактивни. Можете да скриете и покажете колоните, да използвате клавиша Tab и клавишите със стрелки, за да се придвижвате през заглавките на колоните, и да използвате бутоните за действие в лентата с инструменти. Освен това можете да използвате следните клавишни комбинации:

- **Обновяване** : ALT + SHIFT + F5
- **Добавяне** : Alt + Shift + Insert
- **Изтриване** : Alt + Shift + Delete
- **Придвижване нагоре/надолу** : Alt + Shift + стрелки нагоре/надолу
- **Отстъп/обратен отстъп** : Alt + Shift + стрелки наляво/надясно
- **Разгъване/свиване на йерархични нива** : Alt + Shift + клавиши плюс/минус

## <a name="task-attributes"></a>Атрибути на задача

Името на задача описва работата, която трябва да бъде извършена. В PSA атрибутите, които са свързани със задача описват графика на задачата и нейните изисквания за осигуряване на персонал.

> ![Атрибути на задача](media/project-2.png)
 
### <a name="schedule-attributes"></a>Атрибути на графика

Атрибутите **Усилие** , **Начална дата** , **Крайна дата** и **Продължителност** дефинират графика за задачата.

Допълнителните атрибути на графика включват:

- **Часове усилия** : въведете прогноза за часовете, които са необходими за изпълнение на задачата. 
- **Продължителност** : укажете броя на работните дни, които са необходими за изпълнение на задачата.
- **ИД на график** : този автоматично генериран ИД се използва за подреждане на задачи в йерархията. Зависимостите между задачите управляват действителния ред, в който се обработват задачите.
 
### <a name="staffing-attributes"></a>Атрибути за персонал

Атрибутите за осигуряване на персонал са достъпни чрез полето **Ресурси** в графика. Можете или да потърсите съществуващ ресурс, или да щракнете върху **Създаване** и в прозореца **Бързо създаване** да добавите член на екипа по проекта като нов ресурс.

Полетата **Роля** , **Ресурсна единица** и **Име на позиция** се използват за описание на изискванията за осигуряване на персонал за задачата. Тези атрибути за осигуряване на персонал заедно с графика на задачите се използват за намиране на налични ресурси за изпълнение на тази задача.

**Роля** – укажете типа ресурс, който е необходим за изпълнение на задачата.

**Ресурсна единица** – Задайте единицата, от която трябва да бъдат присвоени ресурси за задачата. Този атрибут засяга прогнозната оценка на разходите и продажбите за задачата, ако разходите и ставката за фактуриране за ресурса са зададени на базата на ресурсните единици.

**Име на позиция** – въведете лесноразбираемо име за общия ресурс, който служи като контейнер за ресурса, който в крайна сметка ще изпълнява работата.

Полето **Ресурси** съдържа името на позицията на общия ресурс или наименувания ресурс, когато е намерен такъв.

Полето **Категория** съдържа стойностите, които показват по-широк тип работа, в която задачата може да бъде групирана. Това поле не засяга планирането или осигуряването на персонал. То се използва само за отчитане.

### <a name="task-dependencies"></a>Зависимости на задачите 

Можете да използвате графика в PSA, за да създадете предшестващи релации между задачите. Полето **Предшественик** под **Задачи** приема една или повече стойности, за да покаже задачите, от които зависи дадена задача. Когато към задача са присвоени стойности на предшестващи задачи, задачата може да започне само след като бъдат завършени всички предшестващи задачи. Поради зависимостта планираната начална дата на задачата се нулира до датата, когато предшестващите задачи са завършени.

Режимът на задачи не оказва влияние върху актуализациите, които се извършват по началната и крайната дата на предшестващите/зависимите задачи.

## <a name="task-mode"></a>Режим на задачи 

Режимът на задачи определя планирането на задачи на краен възел. PSA поддържа два режима на задача за всяка задача: автоматично планиране и ръчно планиране.

### <a name="auto-scheduling"></a>Автоматично планиране 
 
Когато режимът на задачи е зададен на **Автоматично планиране** за задача, системата за планиране на задачи използва правилата за планиране на атрибути на задачата, за да определи графика за изпълнение на задачата:

#### <a name="scheduling-rules"></a>Правила за планиране

По подразбиране, ако задача на краен възел няма предшественици, нейната начална дата се задава на началната дата в графика на проекта. Продължителността на задачата на краен възел винаги се изчислява като броя на работните дни между началната и крайната дати. Когато дадена задача се планира автоматично, системата за планиране следва правилата по-долу:

- Началната и крайната дати на задачата трябва да са работни дни съгласно календара за планиране на проекта. 
- За всяка задача, която има предшестващи задачи, началната дата се задава автоматично на последната крайна дата на нейните предшественици.
- Усилието се изчислява с помощта на следната формула: брой хора × продължителност х часове в стандартен работен ден в календара на проекта.

### <a name="manual-scheduling"></a>Ръчно планиране

Ако правилата за автоматично планиране не отговарят на вашите изисквания, можете да зададете режима на задачи за задачата на **Ръчно планирано**. Тази настройка спира системата за планиране от изчисляване на стойностите на други атрибути за планиране. Независимо от режима на задачи, ако зададете предшественици на задачи, това винаги ще оказва влияние на началната дата на зависима задача.