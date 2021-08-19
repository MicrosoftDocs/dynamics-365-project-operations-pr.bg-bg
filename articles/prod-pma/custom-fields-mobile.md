---
title: Внедрете персонализирани полета за мобилно приложение Microsoft Dynamics 365 Project Timesheet на iOS и Android
description: Тази тема предоставя общи модели за използване на разширения за внедряване на персонализирани полета.
author: Yowelle
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.3
ms.search.validFrom: 2019-05-29
ms.openlocfilehash: 9f19a6d069c4f825be8515a6d26739c50d3b064698fc1872ede07a4e74ee4dcb
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/06/2021
ms.locfileid: "7005738"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a>Внедрете персонализирани полета за мобилно приложение Microsoft Dynamics 365 Project Timesheet на iOS и Android

[!include [banner](../includes/banner.md)]

Тази тема предоставя общи модели за използване на разширения за внедряване на персонализирани полета. Обхванати са следните теми:

- Различните типове данни, които персонализираната рамкова област поддържа
- Как да показвате полета само за четене или за редактиране в записите в разписанието и да запазвате предоставените от потребителя стойности обратно в базата данни
- Как да покажа полета само за четене в заглавката на работния лист
- Как да интегрирате друга персонализирана бизнес логика, за да въведете стойности по подразбиране в полетата и да направите допълнителна проверка

## <a name="audience"></a>Публика

Тази тема е предназначена за разработчици, които интегрират своите потребителски полета в мобилно приложение Microsoft Dynamics 365 Project Timesheet, което е достъпно за Apple iOS и Google Android. Предполага се, че читателите са запознати с X ++ разработката и функционалността на работния график на проекта.

## <a name="data-contract--tstimesheetcustomfield-x-class"></a>Договор за данни - клас TSTimesheetCustomField X ++

Класът **TSTimesheetCustomField** е класът на X ++ договор за данни, който представлява информация за персонализирано поле за функционалност на разписанието. Списъците на персонализираните обекти на полета се предават както в договора за данни TSTimesheetDetails, така и в договора за данни TSTimesheetEntry, за да се покажат персонализирани полета в мобилното приложение.

- **TSTimesheetDetails** - Договорът за заглавие на работния лист.
- **TSTimesheetEntry** - Договорът за транзакция на разписанието. Групи от тези обекти, които имат една и съща информация за проекта и **timesheetLineRecId** стойност представляват ред.

### <a name="fieldbasetype-types"></a>fieldBaseType (Типове)

Свойството **FieldBaseType** на обекта **TsTimesheetCustom** определя вида на полето, което се появява в приложението. Следните стойности **Видове**, които се поддържат.

| Типове стойност | Тип              | Забележки |
|-------------|-------------------|-------|
| 0           | Низ (и изброяване) | Полето се появява като текстово поле. |
| 1           | Integer           | Стойността се показва като число без десетични знаци. |
| 2           | Истински              | Стойността се показва като число, което има десетични знаци.<p>За да покажете реалната стойност като валута в приложението, използвайте свойството **fieldExtensedType**. Можете да използвате свойството **numberOfDecimals** да задава броя на десетичните знаци, които се показват.</p> |
| 3           | Date              | Форматите на датите се определят от потребителската настройка **Дата, часове и цифров формат**, посочена в **Предпочитание за език и държава/регион** в **Потребителски опции**. |
| 4           | Boolean           | |
| 15          | GUID              | |
| 16          | Int64             | |

- Ако свойството **stringOptions** не е предоставено за обекта **TSTimesheetCustomField**, полето със свободен текст се предоставя на потребителя.

    Свойството **stringLength** може да се използва за задаване на максималната дължина на низа, която потребителите могат да въведат.

- Ако свойството **stringOptions** е предоставено на обекта **TSTimesheetCustomField**, тези елементи от списъка са единствените стойности, които потребителите могат да изберат с помощта на бутоните за опции (радиобутони).

    В този случай полето на низа може да действа като стойност на изброяване с цел въвеждане от потребителя. За да запишете стойността в базата данни като преброяване, ръчно картографирайте стойността на низа обратно към стойността на преброяването, преди да запишете в базата данни, като използвате верига от команди (вижте "Използване на верига от команди в класа TSTimesheetEntryService, за да запишете запис от работен лист от приложението обратно към базата данни "в раздела по-нататък в тази тема за пример).

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a>fieldExtendedType (TSCustomFieldExtendedType)

Можете да използвате това свойство, за да форматирате реалните стойности като валута. Този подход е приложим само когато стойността **fieldBaseType** е **Истинска**.

- **TSCustomFieldExtendedType:None** - Не се прилага форматиране.
- **TSCustomFieldExtendedType::Currency** - Форматирайте стойността като валута.

    Когато форматирането на валута е активно, полето **stringValue** може да се използва предайте кода на валутата, който трябва да бъде показан в приложението. Стойността е стойност само за четене.

    Полето **realValue** съдържа паричната сума, която трябва да бъде записана в базата данни.

### <a name="fieldsection-tscustomfieldsection"></a>fieldSection (TSCustomFieldSection)

Можете да използвате това свойство, за да посочите къде трябва да се показва потребителското поле в приложението.

- **TSCustomFieldSection::Header** - Полето ще се появи в раздела **Вижте повече подробности** в приложението. Тези полета винаги са само за четене.
- **TSCustomFieldSection::Line** - Полето ще се появи след всички полета за ред в записите в разписанието. Тези полета могат да бъдат или за редактиране, или само за четене.

### <a name="fieldname-fieldnameshort"></a>fieldName (FieldNameShort)

Това свойство идентифицира полето, когато стойностите, които предоставя приложението, се записват обратно в базата данни.

### <a name="tablename-tablenameshort"></a>tableName (TableNameShort)

Това свойство идентифицира полето, когато стойностите, които предоставя приложението, се записват обратно в базата данни.

### <a name="iseditable-noyes"></a>isEditable (NoYes)

Задайте това свойство на **Да**, за да посочите, че полето в раздела за въвеждане на разписанието трябва да се редактира от потребителите. Задайте свойството на **Не**, за да направите полето само за четене.

### <a name="ismandatory-noyes"></a>isMandatory (NoYes)

Задайте това свойство на **Да**, за да посочите, че полето в раздела за въвеждане на разписанието трябва да е задължително.

### <a name="label-str"></a>label (str)

Това свойство указва етикета, който се показва до полето в приложението.

### <a name="stringoptions-list-of-strings"></a>stringOptions (Списък с низове)

Това свойство е приложимо само когато **fieldBaseType** е зададено на **Низ**. Ако е зададено **stringOptions**, низовите стойности, които са достъпни за избор чрез бутони за опции (радиобутони), се определят от низовете в списъка. Ако не са предоставени низове, е разрешено въвеждането на свободен текст в полето на низа (вижте "Използвайте верига от команди в класа TSTimesheetEntryService, за да запишете запис на работен лист от приложението обратно в базата данни" по-долу в тази тема за пример) .

### <a name="stringlength-int"></a>stringLength (int)

Това свойство указва максималната дължина за поле на низ. Това е приложимо само когато **fieldBaseType** е зададено на **Низ**.

### <a name="numberofdecimals-int"></a>numberOfDecimals (int)

Това свойство указва броя на десетичните знаци, които се показват за реално поле. Това е приложимо само когато **fieldBaseType** е зададено на **Реално**.

### <a name="ordersequence-int"></a>orderSequence (int)

Това свойство контролира реда, в който потребителските полета се показват в приложението, когато са посочени повече от едно персонализирано поле. Първо се показват полетата с по-ниски числа.

### <a name="booleanvalue-boolean"></a>booleanValue (булево)

За полета на **Булев** тип, това свойство предава булевата стойност на полето между сървъра и приложението.

### <a name="guidvalue-guid"></a>guidValue (guid)

За полета на **GUID** тип, това свойство предава глобален еднозначен идентификатор (GUID) между сървъра и приложението.

### <a name="int64value-int64"></a>int64Value (int64)

За полета на **Int64** тип, това свойство предава стойностta Int64 на полето между сървъра и приложението.

### <a name="intvalue-int"></a>intValue (int)

За полета на **Int** тип, това свойство предава стойностta Int на полето между сървъра и приложението.

### <a name="realvalue-real"></a>realValue (реално)

За полета на **Real** тип, това свойство предава стойностta Real на полето между сървъра и приложението.

### <a name="stringvalue-str"></a>stringValue (str)

За полета на **Низ** тип, това свойство предава низовата стойност на полето между сървъра и приложението. Използва се и за полета от тип **Истински**, които са форматирани като валута. За тези полета свойството се използва за предаване на кода на валутата на приложението.

### <a name="datevalue-date"></a>dateValue (date)

За полета на **Дата** тип, това свойство предава стойностta дата на полето между сървъра и приложението.

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a>Показване и запазване на персонализирано поле в раздела за въвеждане на разписанието

По-долу е екранна снимка от мобилното приложение на създаване на запис на работен лист. Той показва полетата извън кутията и персонализирано поле в раздела „Въвеждане на време“, наречен „Тестов низ“ с вече зададена стойност на изброяване на „Втора опция“.

![Тествайте персонализирано поле в низа в приложението.](media/timesheet-entry.jpg)



По-долу има екранна снимка от мобилното приложение на потребителя, избираща една от опциите за изброяване, налични за персонализираното поле "Тестов низ".  Двете опции са „Първа опция“ и „Втора опция“, показани като радио бутони. В момента е избрана втората опция.

![Бутони с опции (радиобутони) за полето за тестване на потребителски низ.](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a>Разширете таблицата TSTimesheetLine, така че да има персонализирано поле

В типичните сценарии е вероятно данните за персонализирано поле в раздела за въвеждане на разписание да бъдат запазени в таблицата TSTimesheetLine. Други таблици обаче могат да се използват, ако данните могат да бъдат извлечени въз основа на предоставения запис TSTimesheetTrans или ако той няма конкретен контекст на записа (например, ако полето е зададено като само за четене в параметрите на проекта) .

Обърнете внимание, че потребителските полета не трябва да имат подкрепящи записи на база данни. Те могат да се генерират динамично въз основа на X ++ логика. Този подход може да бъде полезен в сценарии само за четене (вижте раздела "Използване на верига от команди в класа TSTimesheetDetails, метод buildCustomFieldListForHeader за попълване на подробности за разписанието" за пример за динамично генерирани стойности на персонализирано поле.)

По-долу е екранна снимка от Visual Studio на дървото на обекта на приложението. Той показва разширение на таблицата TSTimesheetLine с поле TestLineString, добавено като персонализирано поле.

![Линеен низ.](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a>Използвайте верига от команди на метода buildCustomFieldList на класа TSTimesheetSettings, за да покажете поле в раздела за въвеждане на разписанието

Този код контролира настройките на дисплея за полето в приложението. Например той контролира вида на полето, етикета, дали полето е задължително и в кой раздел се появява полето.

Следващият пример показва низово поле за въвеждане на време. Това поле има две опции **Първи вариант** и **Втори вариант**, които са достъпни чрез бутони с опции (радиобутони). Полето в приложението е свързано с полето **TestLineString**, което се добавя към таблицата TSTimesheetLine.

Обърнете внимание на използването на **TSTimesheetCustomField::newFromMetatdata()** метод за опростяване на инициализацията на свойствата на персонализираното поле: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength** и **numberOfDecimals**. Можете също така да зададете тези параметри ръчно, както предпочитате.

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('Second option');
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a>Използвайте верига от команди на метода buildCustomFieldListForEntry на класа TSTimesheetEntry, за да въведете стойности записа на разписанието

Методът **buildCustomFieldListForEntry** се използва за въвеждане на стойности в запазените редове на работния лист в мобилното приложение. За параметър се взема запис TSTimesheetTrans. Полета от този запис могат да се използват за попълване на стойността на персонализираното поле в приложението.

```xpp
...
[ExtensionOf(classStr(TsTimesheetEntry))]
final class TsTimesheetEntry_Extension
{
    protected List buildCustomFieldListForEntry(TSTimesheetTrans _tsTimesheetTrans)
    {
        List customFieldList = next buildCustomFieldListForEntry(_tsTimesheetTrans);
        TSTimesheetLine tsTimesheetLine = _tsTimesheetTrans.timesheetLine();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        tsTimesheetCustomField.parmStringValue(tsTimesheetLine.TestLineString);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('second option;);
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a>Използвайте верига от команди в класа TSTimesheetEntryService, за да запишете запис на работен лист от приложението обратно в базата данни

За да запазите персонализирано поле обратно в базата данни при типична употреба, трябва да разширите множество методи:

- Методът **timesheetLineNeedsUpdating** се използва, за да се определи дали редовият запис е променен от потребителя в приложението и трябва да бъде записан в базата данни. Ако производителността не е проблем, този метод може да бъде опростен, така че винаги да се връща **вярно**.
- Методите **populateTimesheetLineFromEntryDuringCreate** и **populateTimesheetLineFromEntryDuringUpdate** могат да бъдат разширени, така че да въвеждат стойности в записа на базата данни TSTimesheetLine от предоставения запис на договор за данни TSTimesheetEntry. В примера, който следва, обърнете внимание как картографирането между полето на базата данни и полето за въвеждане се извършва ръчно чрез код X ++.
- Методът **populateTimesheetWeekFromEntry** може също да бъде удължен, ако потребителското поле, което е съпоставено с обекта **TSTimesheetEntry** трябва да пише обратно в таблицата на базата данни TSTimesheetLineweek.

> [!NOTE]
> Следващият пример записва стойността **firstOption** или **secondOption**, която потребителят избира към базата данни като необработена низова стойност. Ако полето на базата данни е поле на тип **Изброяване**, тези стойности могат да бъдат ръчно преобразувани в стойност на преброяване и след това да бъдат записани в поле за изброяване в таблицата на базата данни.

```xpp
...
[ExtensionOf(classStr(TSTimesheetEntryService))]
final class TSTimesheetEntryService_Extension
{
    protected boolean timesheetLineNeedsUpdating(TSTimesheetLine _tsTimesheetLine,
    TsTimesheetEntry _tsTimesheetEntry)
    {
        boolean ret = next timesheetLineNeedsUpdating(_tsTimesheetLine,
        _tsTimesheetEntry);
        if (!ret)
        {
            */ Loop through custom fields to see if value needs updating*/
            ListEnumerator enumerator =  _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    */ If Custom field value for TestLineString field has changed, We need to update the timesheet line.*/
                    if (_tsTimesheetLine.TestLineString != customField.parmStringValue())
                    {
                        ret = true;
                    }
                }
            }
        }
        return ret;
    }
    protected void populateTimesheetLineFromEntryDuringCreate(TSTimesheetLine
    _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
    {
        next populateTimesheetLineFromEntryDuringCreate(_tsTimesheetLine,
        _tsTimesheetEntry);
        this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
        _tsTimesheetEntry);
        }
        protected void populateTimesheetLineFromEntryDuringUpdate(TSTimesheetLine
        \_tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            next populateTimesheetLineFromEntryDuringUpdate(_tsTimesheetLine,
            _tsTimesheetEntry);
            this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
            _tsTimesheetEntry);
        }
        private void populateTimesheetLineFromCustomFields(TSTimesheetLine
        _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            ListEnumerator enumerator =
            _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    _tsTimesheetLine.TestLineString = customField.parmStringValue();
                }
            }
        }
    }
...
```

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a>Показване на персонализирано поле в секцията на заглавка

По-долу е екранна снимка от мобилното приложение на потребител, преглеждащ разписанието. Бутонът „Повече информация“ е избран в горния десен ъгъл, за да се покаже опцията „Преглед на повече подробности“.  

![Команда за преглед на още подробности.](media/show-more.png)

По-долу е екранна снимка от мобилното приложение, показващ секцията „Още” на разписанието. Потребителско поле, наречено "Скорост на използване на този работен лист (изчислено персонализирано поле)" е добавено към раздела за заглавие на работния лист. Стойността само за четене "0.667" е зададена в потребителското поле.

![Секция „Още”.](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a>Разширете таблицата TSTimesheetTable, така че да има персонализирано поле

В типичните сценарии е вероятно данните за персонализирано поле в секцията заглавие ще бъдат изтеглени от таблицата TSTimesheetHeader. Други таблици обаче могат да се използват, ако данните могат да бъдат извлечени въз основа на предоставения запис TSTimesheetTable или ако той няма конкретен контекст на записа (например, ако полето е зададено като само за четене в параметрите на проекта).

Обърнете внимание, че потребителските полета не трябва да имат подкрепящи записи на база данни. Те могат да се генерират динамично въз основа на X ++ логика. Примерът, който следва, показва този подход.

Полетата в заглавната секция винаги са само за четене в приложението.

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a>Използвайте верига от команди на метода buildCustomFieldList на класа TSTimesheetSettings, за да покажете поле в секцията на заглавката

Този код контролира настройките на дисплея за полето в приложението. Например той контролира вида на полето, етикета, дали полето е задължително и в кой раздел се появява полето.

Следващият пример показва изчислена стойност в заглавната секция в приложението.

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a>Използвайте верига от команди на метода buildCustomFieldListForHeader на класа TSTimesheetDetails, за да попълните подробностите на разписанието

Методът **buildCustomFieldListForHeader** се използва за попълване в подробностите на подробностите за заглавка на разписание в мобилното приложение. За параметър се взема запис TSTimesheetTable. Полета от този запис могат да се използват за попълване на стойността на персонализираното поле в приложението. Следващият пример не чете никакви стойности от базата данни. Вместо това използва X ++ логика, за да генерира изчислена стойност, която след това се показва в приложението.


```xpp
...
[ExtensionOf(classStr(TSTimesheetDetails))]
final class TSTimesheetDetails_Extension
{
    protected List buildCustomFieldListForHeader(TSTimesheetTable
    _tsTimesheetTable)
    {
        List customFieldList = next buildCustomFieldListForHeader(_tsTimesheetTable);
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        real utilizationRate = 0;
        if (_tsTimesheetTable.totalHours() != 0)
        {
            utilizationRate = _tsTimesheetTable.totalHoursBillable() /
            _tsTimesheetTable.totalHours();
        }
        tsTimesheetCustomField.parmRealValue(utilizationRate);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

## <a name="other-configurabilityextensibility-opportunities"></a>Други възможности за конфигуриране / разширяемост

### <a name="adding-additional-validation-for-the-app"></a>Добавяне на допълнителна проверка за приложението

Съществуващата логика за функционалността на разписанието на ниво база данни ще продължи да работи, както се очаква. За да прекъснете завършването на операциите за запис или изпращане и да покажете конкретно съобщение за грешка, можете да добавите **хвърляне на грешка ("съобщение до потребителя")** към кода чрез разширение на верига от команди. Ето три примера за полезни разширяеми методи:

- Ако **validateWrite** в таблицата TSTimesheetLine се връща **невярно** по време на операция за запазване на ред за работен лист в мобилното приложение се показва съобщение за грешка.
- Ако **validateSubmit** в таблицата TSTimesheetTable се връща **невярно** по време на подаването на разписанието в приложението на потребителя се показва съобщение за грешка.
- Логика, която запълва полета (например, **Свойство на линията**) по време на метод **вмъкване** в таблицата TSTimesheetLine ще продължи да работи.

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a>Скриване и маркиране на полетата извън кутията само за четене чрез конфигурация

От параметрите на проекта можете да направите полетата извън полето само за четене или скрити в мобилното приложение. Задайте опциите в секцията **Мобилни разписания** на раздела **Таблица за работно време** на страницата **Управление на проекти и счетоводни параметри**.

![Параметри на проект.](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a>Промяна на дейностите, които са достъпни за избор чрез разширения

Дейностите, които са на разположение за избор на проект, се попълват чрез **getActivitiesForProject()** и **getActivityQuery()** методи в клас **TsTimesheetProjectService**. Можете да използвате командна верига, за да промените това поведение, за да съответства на вашия бизнес сценарий за дейностите, които са достъпни за избор за конкретен проект.

### <a name="entering-a-default-project-category-on-timesheet-entries"></a>Въвеждане на категория на проекта по подразбиране в записите в разписанието

Вписването на категория на проекта по подразбиране в записите в разписанието се извършва на три нива. Можете да използвате командна верига, за да разширите поведението на всяко или всички от тези нива, за да постигнете желаното поведение. Използва се следната йерархия:

1. Приложението се опитва да постави категорията по подразбиране от ресурса на проекта. Тази категория по подразбиране е зададена в методите **getCurrentUserResource** и **getDelegatedResourcesForCurrentUser** в класа **TSTimesheetSettingsService**.
2. Ако категорията по подразбиране не е предоставена на ниво ресурс на проекта, приложението се опитва да я изтегли от активността на проекта. Тази категория по подразбиране е зададена в метода **getActivitiesForProject** в класа **TSTimesheetProjectServic**.
3. Ако категорията по подразбиране не е предоставена на ниво дейност по проекта, категорията по подразбиране се взема от параметрите на проекта. Тази категория по подразбиране е зададена в метода **getProjectDetailsbyRule** в класа **TSTimesheetProjectServic**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]