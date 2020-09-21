---
title: Внедрете персонализирани полета за мобилно приложение Microsoft Dynamics 365 Project Timesheet на iOS и Android
description: Тази тема предоставя общи модели за използване на разширения за внедряване на персонализирани полета.
author: KimANelson
manager: AnnBe
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: 4564bbda-34ea-4647-a9bc-f6ef17b1038b
ms.search.region: Global
ms.search.industry: Service industries
ms.author: knelson
ms.dyn365.ops.version: 10.0.3
ms.search.validFrom: 2019-05-29
ms.openlocfilehash: 16c3b79dcaaf8c5c491587618256694f82f44753
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749245"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a><span data-ttu-id="89c95-103">Внедрете персонализирани полета за мобилно приложение Microsoft Dynamics 365 Project Timesheet на iOS и Android</span><span class="sxs-lookup"><span data-stu-id="89c95-103">Implement custom fields for the Microsoft Dynamics 365 Project Timesheet mobile app on iOS and Android</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="89c95-104">Тази тема предоставя общи модели за използване на разширения за внедряване на персонализирани полета.</span><span class="sxs-lookup"><span data-stu-id="89c95-104">This topic provides common patterns for using extensions to implement custom fields.</span></span> <span data-ttu-id="89c95-105">Обхванати са следните теми:</span><span class="sxs-lookup"><span data-stu-id="89c95-105">The following topics are covered:</span></span>

- <span data-ttu-id="89c95-106">Различните типове данни, които персонализираната рамкова област поддържа</span><span class="sxs-lookup"><span data-stu-id="89c95-106">The various data types that the custom field framework supports</span></span>
- <span data-ttu-id="89c95-107">Как да показвате полета само за четене или за редактиране в записите в разписанието и да запазвате предоставените от потребителя стойности обратно в базата данни</span><span class="sxs-lookup"><span data-stu-id="89c95-107">How to show read-only or editable fields on timesheet entries, and save user-provided values back to the database</span></span>
- <span data-ttu-id="89c95-108">Как да покажа полета само за четене в заглавката на работния лист</span><span class="sxs-lookup"><span data-stu-id="89c95-108">How to show read-only fields on the timesheet header</span></span>
- <span data-ttu-id="89c95-109">Как да интегрирате друга персонализирана бизнес логика, за да въведете стойности по подразбиране в полетата и да направите допълнителна проверка</span><span class="sxs-lookup"><span data-stu-id="89c95-109">How to integrate other custom business logic to enter default values in fields and do additional validation</span></span>

## <a name="audience"></a><span data-ttu-id="89c95-110">Публика</span><span class="sxs-lookup"><span data-stu-id="89c95-110">Audience</span></span>

<span data-ttu-id="89c95-111">Тази тема е предназначена за разработчици, които интегрират своите потребителски полета в мобилно приложение Microsoft Dynamics 365 Project Timesheet, което е достъпно за Apple iOS и Google Android.</span><span class="sxs-lookup"><span data-stu-id="89c95-111">This topic is intended for developers who are integrating their custom fields into the Microsoft Dynamics 365 Project Timesheet mobile application that is available for Apple iOS and Google Android.</span></span> <span data-ttu-id="89c95-112">Предполага се, че читателите са запознати с X ++ разработката и функционалността на работния график на проекта.</span><span class="sxs-lookup"><span data-stu-id="89c95-112">The assumption is that readers are familiar with X++ development and project timesheet functionality.</span></span>

## <a name="data-contract--tstimesheetcustomfield-x-class"></a><span data-ttu-id="89c95-113">Договор за данни - клас TSTimesheetCustomField X ++</span><span class="sxs-lookup"><span data-stu-id="89c95-113">Data contract – TSTimesheetCustomField X++ class</span></span>

<span data-ttu-id="89c95-114">Класът **TSTimesheetCustomField** е класът на X ++ договор за данни, който представлява информация за персонализирано поле за функционалност на разписанието.</span><span class="sxs-lookup"><span data-stu-id="89c95-114">The **TSTimesheetCustomField** class is the X++ data contract class that represents information about a custom field for timesheet functionality.</span></span> <span data-ttu-id="89c95-115">Списъците на персонализираните обекти на полета се предават както в договора за данни TSTimesheetDetails, така и в договора за данни TSTimesheetEntry, за да се покажат персонализирани полета в мобилното приложение.</span><span class="sxs-lookup"><span data-stu-id="89c95-115">Lists of the custom field objects are passed on both the TSTimesheetDetails data contract and the TSTimesheetEntry data contract to show custom fields in the mobile app.</span></span>

- <span data-ttu-id="89c95-116">**TSTimesheetDetails** - Договорът за заглавие на работния лист.</span><span class="sxs-lookup"><span data-stu-id="89c95-116">**TSTimesheetDetails** - The timesheet header contract.</span></span>
- <span data-ttu-id="89c95-117">**TSTimesheetEntry** - Договорът за транзакция на разписанието.</span><span class="sxs-lookup"><span data-stu-id="89c95-117">**TSTimesheetEntry** - The timesheet transaction contract.</span></span> <span data-ttu-id="89c95-118">Групи от тези обекти, които имат една и съща информация за проекта и **timesheetLineRecId** стойност представляват ред.</span><span class="sxs-lookup"><span data-stu-id="89c95-118">Groups of these objects that have the same project information and **timesheetLineRecId** value constitute a line.</span></span>

### <a name="fieldbasetype-types"></a><span data-ttu-id="89c95-119">fieldBaseType (Типове)</span><span class="sxs-lookup"><span data-stu-id="89c95-119">fieldBaseType (Types)</span></span>

<span data-ttu-id="89c95-120">Свойството **FieldBaseType** на обекта **TsTimesheetCustom** определя вида на полето, което се появява в приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-120">The **FieldBaseType** property on the **TsTimesheetCustom** object determines the type of the field that appears in the app.</span></span> <span data-ttu-id="89c95-121">Следните стойности **Видове**, които се поддържат.</span><span class="sxs-lookup"><span data-stu-id="89c95-121">The following **Types** values that are supported.</span></span>

| <span data-ttu-id="89c95-122">Типове стойност</span><span class="sxs-lookup"><span data-stu-id="89c95-122">Types value</span></span> | <span data-ttu-id="89c95-123">Тип</span><span class="sxs-lookup"><span data-stu-id="89c95-123">Type</span></span>              | <span data-ttu-id="89c95-124">Забележки</span><span class="sxs-lookup"><span data-stu-id="89c95-124">Notes</span></span> |
|-------------|-------------------|-------|
| <span data-ttu-id="89c95-125">0</span><span class="sxs-lookup"><span data-stu-id="89c95-125">0</span></span>           | <span data-ttu-id="89c95-126">Низ (и изброяване)</span><span class="sxs-lookup"><span data-stu-id="89c95-126">String (and Enum)</span></span> | <span data-ttu-id="89c95-127">Полето се появява като текстово поле.</span><span class="sxs-lookup"><span data-stu-id="89c95-127">The field appears as a text field.</span></span> |
| <span data-ttu-id="89c95-128">1</span><span class="sxs-lookup"><span data-stu-id="89c95-128">1</span></span>           | <span data-ttu-id="89c95-129">Integer</span><span class="sxs-lookup"><span data-stu-id="89c95-129">Integer</span></span>           | <span data-ttu-id="89c95-130">Стойността се показва като число без десетични знаци.</span><span class="sxs-lookup"><span data-stu-id="89c95-130">The value is shown as a number without decimal places.</span></span> |
| <span data-ttu-id="89c95-131">2</span><span class="sxs-lookup"><span data-stu-id="89c95-131">2</span></span>           | <span data-ttu-id="89c95-132">Истински</span><span class="sxs-lookup"><span data-stu-id="89c95-132">Real</span></span>              | <span data-ttu-id="89c95-133">Стойността се показва като число, което има десетични знаци.</span><span class="sxs-lookup"><span data-stu-id="89c95-133">The value is shown as a number that has decimal places.</span></span><p><span data-ttu-id="89c95-134">За да покажете реалната стойност като валута в приложението, използвайте свойството **fieldExtensedType**.</span><span class="sxs-lookup"><span data-stu-id="89c95-134">To show the real value as a currency in the app, use the **fieldExtenededType** property.</span></span> <span data-ttu-id="89c95-135">Можете да използвате свойството **numberOfDecimals** да задава броя на десетичните знаци, които се показват.</span><span class="sxs-lookup"><span data-stu-id="89c95-135">You can use the **numberOfDecimals** property to set the number of decimal places that are shown.</span></span></p> |
| <span data-ttu-id="89c95-136">3</span><span class="sxs-lookup"><span data-stu-id="89c95-136">3</span></span>           | <span data-ttu-id="89c95-137">Date</span><span class="sxs-lookup"><span data-stu-id="89c95-137">Date</span></span>              | <span data-ttu-id="89c95-138">Форматите на датите се определят от потребителската настройка **Дата, часове и цифров формат**, посочена в **Предпочитание за език и държава/регион** в **Потребителски опции**.</span><span class="sxs-lookup"><span data-stu-id="89c95-138">Date formats are determined by the user's **Date, times, and number format** setting that is specified under **Language and country/region preference** in **User options**.</span></span> |
| <span data-ttu-id="89c95-139">4</span><span class="sxs-lookup"><span data-stu-id="89c95-139">4</span></span>           | <span data-ttu-id="89c95-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="89c95-140">Boolean</span></span>           | |
| <span data-ttu-id="89c95-141">15</span><span class="sxs-lookup"><span data-stu-id="89c95-141">15</span></span>          | <span data-ttu-id="89c95-142">GUID</span><span class="sxs-lookup"><span data-stu-id="89c95-142">GUID</span></span>              | |
| <span data-ttu-id="89c95-143">16</span><span class="sxs-lookup"><span data-stu-id="89c95-143">16</span></span>          | <span data-ttu-id="89c95-144">Int64</span><span class="sxs-lookup"><span data-stu-id="89c95-144">Int64</span></span>             | |

- <span data-ttu-id="89c95-145">Ако свойството **stringOptions** не е предоставено за обекта **TSTimesheetCustomField**, полето със свободен текст се предоставя на потребителя.</span><span class="sxs-lookup"><span data-stu-id="89c95-145">If the **stringOptions** property isn't provided on the **TSTimesheetCustomField** object, a free-text field is provided to the user.</span></span>

    <span data-ttu-id="89c95-146">Свойството **stringLength** може да се използва за задаване на максималната дължина на низа, която потребителите могат да въведат.</span><span class="sxs-lookup"><span data-stu-id="89c95-146">The **stringLength** property can be used to set the maximum string length that users can enter.</span></span>

- <span data-ttu-id="89c95-147">Ако свойството **stringOptions** е предоставено на обекта **TSTimesheetCustomField**, тези елементи от списъка са единствените стойности, които потребителите могат да изберат с помощта на бутоните за опции (радиобутони).</span><span class="sxs-lookup"><span data-stu-id="89c95-147">If the **stringOptions** property is provided on the **TSTimesheetCustomField** object, those list elements are the only values that users can select by using option buttons (radio buttons).</span></span>

    <span data-ttu-id="89c95-148">В този случай полето на низа може да действа като стойност на изброяване с цел въвеждане от потребителя.</span><span class="sxs-lookup"><span data-stu-id="89c95-148">In this case, the string field can act as an enum value for the purpose of user entry.</span></span> <span data-ttu-id="89c95-149">За да запишете стойността в базата данни като преброяване, ръчно картографирайте стойността на низа обратно към стойността на преброяването, преди да запишете в базата данни, като използвате верига от команди (вижте "Използване на верига от команди в класа TSTimesheetEntryService, за да запишете запис от работен лист от приложението обратно към базата данни "в раздела по-нататък в тази тема за пример).</span><span class="sxs-lookup"><span data-stu-id="89c95-149">To save the value to the database as an enum, manually map the string value back to the enum value before you save to the database by using chain of command (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a><span data-ttu-id="89c95-150">fieldExtendedType (TSCustomFieldExtendedType)</span><span class="sxs-lookup"><span data-stu-id="89c95-150">fieldExtendedType (TSCustomFieldExtendedType)</span></span>

<span data-ttu-id="89c95-151">Можете да използвате това свойство, за да форматирате реалните стойности като валута.</span><span class="sxs-lookup"><span data-stu-id="89c95-151">You can use this property to format real values as currency.</span></span> <span data-ttu-id="89c95-152">Този подход е приложим само когато стойността **fieldBaseType** е **Истинска**.</span><span class="sxs-lookup"><span data-stu-id="89c95-152">This approach is applicable only when the **fieldBaseType** value is **Real**.</span></span>

- <span data-ttu-id="89c95-153">**TSCustomFieldExtendedType:None** - Не се прилага форматиране.</span><span class="sxs-lookup"><span data-stu-id="89c95-153">**TSCustomFieldExtendedType:None** – No formatting is applied.</span></span>
- <span data-ttu-id="89c95-154">**TSCustomFieldExtendedType::Currency** - Форматирайте стойността като валута.</span><span class="sxs-lookup"><span data-stu-id="89c95-154">**TSCustomFieldExtendedType::Currency** – Format the value as currency.</span></span>

    <span data-ttu-id="89c95-155">Когато форматирането на валута е активно, полето **stringValue** може да се използва предайте кода на валутата, който трябва да бъде показан в приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-155">When currency formatting is active, the **stringValue** field can be used pass the currency code that should be shown in the app.</span></span> <span data-ttu-id="89c95-156">Стойността е стойност само за четене.</span><span class="sxs-lookup"><span data-stu-id="89c95-156">The value is a read-only value.</span></span>

    <span data-ttu-id="89c95-157">Полето **realValue** съдържа паричната сума, която трябва да бъде записана в базата данни.</span><span class="sxs-lookup"><span data-stu-id="89c95-157">The **realValue** field contains the money amount that should be saved to the database.</span></span>

### <a name="fieldsection-tscustomfieldsection"></a><span data-ttu-id="89c95-158">fieldSection (TSCustomFieldSection)</span><span class="sxs-lookup"><span data-stu-id="89c95-158">fieldSection (TSCustomFieldSection)</span></span>

<span data-ttu-id="89c95-159">Можете да използвате това свойство, за да посочите къде трябва да се показва потребителското поле в приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-159">You can use this property specify where the custom field should appear in the app.</span></span>

- <span data-ttu-id="89c95-160">**TSCustomFieldSection::Header** - Полето ще се появи в раздела **Вижте повече подробности** в приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-160">**TSCustomFieldSection::Header** – The field will appear in the **View more details** section in the app.</span></span> <span data-ttu-id="89c95-161">Тези полета винаги са само за четене.</span><span class="sxs-lookup"><span data-stu-id="89c95-161">These fields are always read-only.</span></span>
- <span data-ttu-id="89c95-162">**TSCustomFieldSection::Line** - Полето ще се появи след всички полета за ред в записите в разписанието.</span><span class="sxs-lookup"><span data-stu-id="89c95-162">**TSCustomFieldSection::Line** – The field will appear after all the out-of-box line fields on timesheet entries.</span></span> <span data-ttu-id="89c95-163">Тези полета могат да бъдат или за редактиране, или само за четене.</span><span class="sxs-lookup"><span data-stu-id="89c95-163">These fields can be either editable or read-only.</span></span>

### <a name="fieldname-fieldnameshort"></a><span data-ttu-id="89c95-164">fieldName (FieldNameShort)</span><span class="sxs-lookup"><span data-stu-id="89c95-164">fieldName (FieldNameShort)</span></span>

<span data-ttu-id="89c95-165">Това свойство идентифицира полето, когато стойностите, които предоставя приложението, се записват обратно в базата данни.</span><span class="sxs-lookup"><span data-stu-id="89c95-165">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="tablename-tablenameshort"></a><span data-ttu-id="89c95-166">tableName (TableNameShort)</span><span class="sxs-lookup"><span data-stu-id="89c95-166">tableName (TableNameShort)</span></span>

<span data-ttu-id="89c95-167">Това свойство идентифицира полето, когато стойностите, които предоставя приложението, се записват обратно в базата данни.</span><span class="sxs-lookup"><span data-stu-id="89c95-167">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="iseditable-noyes"></a><span data-ttu-id="89c95-168">isEditable (NoYes)</span><span class="sxs-lookup"><span data-stu-id="89c95-168">isEditable (NoYes)</span></span>

<span data-ttu-id="89c95-169">Задайте това свойство на **Да**, за да посочите, че полето в раздела за въвеждане на разписанието трябва да се редактира от потребителите.</span><span class="sxs-lookup"><span data-stu-id="89c95-169">Set this property to **Yes** to specify that the field in the timesheet entry section should be editable by users.</span></span> <span data-ttu-id="89c95-170">Задайте свойството на **Не**, за да направите полето само за четене.</span><span class="sxs-lookup"><span data-stu-id="89c95-170">Set the property to **No** to make the field read-only.</span></span>

### <a name="ismandatory-noyes"></a><span data-ttu-id="89c95-171">isMandatory (NoYes)</span><span class="sxs-lookup"><span data-stu-id="89c95-171">isMandatory (NoYes)</span></span>

<span data-ttu-id="89c95-172">Задайте това свойство на **Да**, за да посочите, че полето в раздела за въвеждане на разписанието трябва да е задължително.</span><span class="sxs-lookup"><span data-stu-id="89c95-172">Set this property to **Yes** to specify that the field in the timesheet entry section should be mandatory.</span></span>

### <a name="label-str"></a><span data-ttu-id="89c95-173">label (str)</span><span class="sxs-lookup"><span data-stu-id="89c95-173">label (str)</span></span>

<span data-ttu-id="89c95-174">Това свойство указва етикета, който се показва до полето в приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-174">This property specifies the label that is shown next the field in the app.</span></span>

### <a name="stringoptions-list-of-strings"></a><span data-ttu-id="89c95-175">stringOptions (Списък с низове)</span><span class="sxs-lookup"><span data-stu-id="89c95-175">stringOptions (List of Strings)</span></span>

<span data-ttu-id="89c95-176">Това свойство е приложимо само когато **fieldBaseType** е зададено на **Низ**.</span><span class="sxs-lookup"><span data-stu-id="89c95-176">This property is applicable only when **fieldBaseType** is set to **String**.</span></span> <span data-ttu-id="89c95-177">Ако е зададено **stringOptions**, низовите стойности, които са достъпни за избор чрез бутони за опции (радиобутони), се определят от низовете в списъка.</span><span class="sxs-lookup"><span data-stu-id="89c95-177">If **stringOptions** is set, the string values that are available for selection via option buttons (radio buttons) are specified by the strings in the list.</span></span> <span data-ttu-id="89c95-178">Ако не са предоставени низове, е разрешено въвеждането на свободен текст в полето на низа (вижте "Използвайте верига от команди в класа TSTimesheetEntryService, за да запишете запис на работен лист от приложението обратно в базата данни" по-долу в тази тема за пример) .</span><span class="sxs-lookup"><span data-stu-id="89c95-178">If no strings are provided, free-text entry in the string field is allowed (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="stringlength-int"></a><span data-ttu-id="89c95-179">stringLength (int)</span><span class="sxs-lookup"><span data-stu-id="89c95-179">stringLength (int)</span></span>

<span data-ttu-id="89c95-180">Това свойство указва максималната дължина за поле на низ.</span><span class="sxs-lookup"><span data-stu-id="89c95-180">This property specifies the maximum length for a string field.</span></span> <span data-ttu-id="89c95-181">Това е приложимо само когато **fieldBaseType** е зададено на **Низ**.</span><span class="sxs-lookup"><span data-stu-id="89c95-181">It's applicable only when **fieldBaseType** is set to **String**.</span></span>

### <a name="numberofdecimals-int"></a><span data-ttu-id="89c95-182">numberOfDecimals (int)</span><span class="sxs-lookup"><span data-stu-id="89c95-182">numberOfDecimals (int)</span></span>

<span data-ttu-id="89c95-183">Това свойство указва броя на десетичните знаци, които се показват за реално поле.</span><span class="sxs-lookup"><span data-stu-id="89c95-183">This property specifies the number of decimal places that are shown for a real field.</span></span> <span data-ttu-id="89c95-184">Това е приложимо само когато **fieldBaseType** е зададено на **Реално**.</span><span class="sxs-lookup"><span data-stu-id="89c95-184">It's applicable only when **fieldBaseType** is set to **Real**.</span></span>

### <a name="ordersequence-int"></a><span data-ttu-id="89c95-185">orderSequence (int)</span><span class="sxs-lookup"><span data-stu-id="89c95-185">orderSequence (int)</span></span>

<span data-ttu-id="89c95-186">Това свойство контролира реда, в който потребителските полета се показват в приложението, когато са посочени повече от едно персонализирано поле.</span><span class="sxs-lookup"><span data-stu-id="89c95-186">This property controls the order in which the custom fields are shown in the app when more than one custom field is specified.</span></span> <span data-ttu-id="89c95-187">Първо се показват полетата с по-ниски числа.</span><span class="sxs-lookup"><span data-stu-id="89c95-187">Fields that have lower numbers are shown first.</span></span>

### <a name="booleanvalue-boolean"></a><span data-ttu-id="89c95-188">booleanValue (булево)</span><span class="sxs-lookup"><span data-stu-id="89c95-188">booleanValue (boolean)</span></span>

<span data-ttu-id="89c95-189">За полета на **Булев** тип, това свойство предава булевата стойност на полето между сървъра и приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-189">For fields of the **Boolean** type, this property passes the Boolean value of the field between the server and the app.</span></span>

### <a name="guidvalue-guid"></a><span data-ttu-id="89c95-190">guidValue (guid)</span><span class="sxs-lookup"><span data-stu-id="89c95-190">guidValue (guid)</span></span>

<span data-ttu-id="89c95-191">За полета на **GUID** тип, това свойство предава глобален еднозначен идентификатор (GUID) между сървъра и приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-191">For fields of the **GUID** type, this property passes the globally unique identifier (GUID) value of the field between the server and the app.</span></span>

### <a name="int64value-int64"></a><span data-ttu-id="89c95-192">int64Value (int64)</span><span class="sxs-lookup"><span data-stu-id="89c95-192">int64Value (int64)</span></span>

<span data-ttu-id="89c95-193">За полета на **Int64** тип, това свойство предава стойностta Int64 на полето между сървъра и приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-193">For fields of the **Int64** type, this property passes the int64 value of the field between the server and the app.</span></span>

### <a name="intvalue-int"></a><span data-ttu-id="89c95-194">intValue (int)</span><span class="sxs-lookup"><span data-stu-id="89c95-194">intValue (int)</span></span>

<span data-ttu-id="89c95-195">За полета на **Int** тип, това свойство предава стойностta Int на полето между сървъра и приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-195">For fields of the **Int** type, this property passes the int value of the field between the server and the app.</span></span>

### <a name="realvalue-real"></a><span data-ttu-id="89c95-196">realValue (реално)</span><span class="sxs-lookup"><span data-stu-id="89c95-196">realValue (real)</span></span>

<span data-ttu-id="89c95-197">За полета на **Real** тип, това свойство предава стойностta Real на полето между сървъра и приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-197">For fields of the **Real** type, this property passes the real value of the field between the server and the app .</span></span>

### <a name="stringvalue-str"></a><span data-ttu-id="89c95-198">stringValue (str)</span><span class="sxs-lookup"><span data-stu-id="89c95-198">stringValue (str)</span></span>

<span data-ttu-id="89c95-199">За полета на **Низ** тип, това свойство предава низовата стойност на полето между сървъра и приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-199">For fields of the **String** type, this property passes the string value of the field between the server and the app.</span></span> <span data-ttu-id="89c95-200">Използва се и за полета от тип **Истински**, които са форматирани като валута.</span><span class="sxs-lookup"><span data-stu-id="89c95-200">It's also used for fields of the **Real** type that are formatted as currency.</span></span> <span data-ttu-id="89c95-201">За тези полета свойството се използва за предаване на кода на валутата на приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-201">For those fields, the property is used to pass the currency code to the app.</span></span>

### <a name="datevalue-date"></a><span data-ttu-id="89c95-202">dateValue (date)</span><span class="sxs-lookup"><span data-stu-id="89c95-202">dateValue (date)</span></span>

<span data-ttu-id="89c95-203">За полета на **Дата** тип, това свойство предава стойностta дата на полето между сървъра и приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-203">For fields of the **Date** type, this property passes the date value of the field between the server and the app.</span></span>

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a><span data-ttu-id="89c95-204">Показване и запазване на персонализирано поле в раздела за въвеждане на разписанието</span><span class="sxs-lookup"><span data-stu-id="89c95-204">Show and save a custom field in the timesheet entry section</span></span>

<span data-ttu-id="89c95-205">По-долу е екранна снимка от мобилното приложение на създаване на запис на работен лист.</span><span class="sxs-lookup"><span data-stu-id="89c95-205">Below is a screenshot from the mobile app of a timesheet entry creation.</span></span> <span data-ttu-id="89c95-206">Той показва полетата извън кутията и персонализирано поле в раздела „Въвеждане на време“, наречен „Тестов низ“ с вече зададена стойност на изброяване на „Втора опция“.</span><span class="sxs-lookup"><span data-stu-id="89c95-206">It shows the out-of-box fields and a custom field in the "Time entry" section called "Test string" with an enum value of "Second option" already set.</span></span>

![Тествайте персонализирано поле в низа в приложението](media/timesheet-entry.jpg)



<span data-ttu-id="89c95-208">По-долу има екранна снимка от мобилното приложение на потребителя, избираща една от опциите за изброяване, налични за персонализираното поле "Тестов низ".</span><span class="sxs-lookup"><span data-stu-id="89c95-208">Below is a screenshot from the mobile app of the user selecting one of the enum options available for the "Test string" custom field.</span></span>  <span data-ttu-id="89c95-209">Двете опции са „Първа опция“ и „Втора опция“, показани като радио бутони.</span><span class="sxs-lookup"><span data-stu-id="89c95-209">The two options are "First option" and "Second option" shown as radio buttons.</span></span> <span data-ttu-id="89c95-210">В момента е избрана втората опция.</span><span class="sxs-lookup"><span data-stu-id="89c95-210">The second option is currently selected.</span></span>

![Бутони с опции (радиобутони) за полето за тестване на потребителски низ](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="89c95-212">Разширете таблицата TSTimesheetLine, така че да има персонализирано поле</span><span class="sxs-lookup"><span data-stu-id="89c95-212">Extend the TSTimesheetLine table so that it has a custom field</span></span>

<span data-ttu-id="89c95-213">В типичните сценарии е вероятно данните за персонализирано поле в раздела за въвеждане на разписание да бъдат запазени в таблицата TSTimesheetLine.</span><span class="sxs-lookup"><span data-stu-id="89c95-213">In typical scenarios, it's likely that the data for a custom field in the timesheet entry section will be saved to the TSTimesheetLine table.</span></span> <span data-ttu-id="89c95-214">Други таблици обаче могат да се използват, ако данните могат да бъдат извлечени въз основа на предоставения запис TSTimesheetTrans или ако той няма конкретен контекст на записа (например, ако полето е зададено като само за четене в параметрите на проекта) .</span><span class="sxs-lookup"><span data-stu-id="89c95-214">However, other tables can be used if the data can be retrieved based on a TSTimesheetTrans record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="89c95-215">Обърнете внимание, че потребителските полета не трябва да имат подкрепящи записи на база данни.</span><span class="sxs-lookup"><span data-stu-id="89c95-215">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="89c95-216">Те могат да се генерират динамично въз основа на X ++ логика.</span><span class="sxs-lookup"><span data-stu-id="89c95-216">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="89c95-217">Този подход може да бъде полезен в сценарии само за четене (вижте раздела "Използване на верига от команди в класа TSTimesheetDetails, метод buildCustomFieldListForHeader за попълване на подробности за разписанието" за пример за динамично генерирани стойности на персонализирано поле.)</span><span class="sxs-lookup"><span data-stu-id="89c95-217">This approach can be useful in read-only scenarios (see the “Use chain of command on the TSTimesheetDetails class, buildCustomFieldListForHeader method to fill in timesheet details” section for an example of dynamically generated custom field values.)</span></span>

<span data-ttu-id="89c95-218">По-долу е екранна снимка от Visual Studio на дървото на обекта на приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-218">Below is a screenshot from Visual Studio of the Application Object Tree.</span></span> <span data-ttu-id="89c95-219">Той показва разширение на таблицата TSTimesheetLine с поле TestLineString, добавено като персонализирано поле.</span><span class="sxs-lookup"><span data-stu-id="89c95-219">It shows an extension of the TSTimesheetLine table with the TestLineString field added as a custom field.</span></span>

![Линеен низ](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a><span data-ttu-id="89c95-221">Използвайте верига от команди на метода buildCustomFieldList на класа TSTimesheetSettings, за да покажете поле в раздела за въвеждане на разписанието</span><span class="sxs-lookup"><span data-stu-id="89c95-221">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the timesheet entry section</span></span>

<span data-ttu-id="89c95-222">Този код контролира настройките на дисплея за полето в приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-222">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="89c95-223">Например той контролира вида на полето, етикета, дали полето е задължително и в кой раздел се появява полето.</span><span class="sxs-lookup"><span data-stu-id="89c95-223">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="89c95-224">Следващият пример показва низово поле за въвеждане на време.</span><span class="sxs-lookup"><span data-stu-id="89c95-224">The following example shows a string field on time entries.</span></span> <span data-ttu-id="89c95-225">Това поле има две опции **Първи вариант** и **Втори вариант**, които са достъпни чрез бутони с опции (радиобутони).</span><span class="sxs-lookup"><span data-stu-id="89c95-225">This field has two options, **First option** and **Second option**, that are available via option buttons (radio buttons).</span></span> <span data-ttu-id="89c95-226">Полето в приложението е свързано с полето **TestLineString**, което се добавя към таблицата TSTimesheetLine.</span><span class="sxs-lookup"><span data-stu-id="89c95-226">The field in the app is associated with the **TestLineString** field that is added to the TSTimesheetLine table.</span></span>

<span data-ttu-id="89c95-227">Обърнете внимание на използването на **TSTimesheetCustomField::newFromMetatdata()** метод за опростяване на инициализацията на свойствата на персонализираното поле: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength** и **numberOfDecimals**.</span><span class="sxs-lookup"><span data-stu-id="89c95-227">Note the use of the **TSTimesheetCustomField::newFromMetatdata()** method to simplify the initialization of the custom field properties: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength**, and **numberOfDecimals**.</span></span> <span data-ttu-id="89c95-228">Можете също така да зададете тези параметри ръчно, както предпочитате.</span><span class="sxs-lookup"><span data-stu-id="89c95-228">You can also set these parameters manually, as you prefer.</span></span>

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a><span data-ttu-id="89c95-229">Използвайте верига от команди на метода buildCustomFieldListForEntry на класа TSTimesheetEntry, за да въведете стойности записа на разписанието</span><span class="sxs-lookup"><span data-stu-id="89c95-229">Use chain of command on the buildCustomFieldListForEntry method of the TSTimesheetEntry class to enter values in a timesheet entry</span></span>

<span data-ttu-id="89c95-230">Методът **buildCustomFieldListForEntry** се използва за въвеждане на стойности в запазените редове на работния лист в мобилното приложение.</span><span class="sxs-lookup"><span data-stu-id="89c95-230">The **buildCustomFieldListForEntry** method is used to enter values on the saved timesheet lines in the mobile app.</span></span> <span data-ttu-id="89c95-231">За параметър се взема запис TSTimesheetTrans.</span><span class="sxs-lookup"><span data-stu-id="89c95-231">It takes a TSTimesheetTrans record as a parameter.</span></span> <span data-ttu-id="89c95-232">Полета от този запис могат да се използват за попълване на стойността на персонализираното поле в приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-232">Fields from that record can be used to fill in the custom field value in the app.</span></span>

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

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a><span data-ttu-id="89c95-233">Използвайте верига от команди в класа TSTimesheetEntryService, за да запишете запис на работен лист от приложението обратно в базата данни</span><span class="sxs-lookup"><span data-stu-id="89c95-233">Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database</span></span>

<span data-ttu-id="89c95-234">За да запазите персонализирано поле обратно в базата данни при типична употреба, трябва да разширите множество методи:</span><span class="sxs-lookup"><span data-stu-id="89c95-234">To save a custom field back to the database in typical usage, you must extend multiple methods:</span></span>

- <span data-ttu-id="89c95-235">Методът **timesheetLineNeedsUpdating** се използва, за да се определи дали редовият запис е променен от потребителя в приложението и трябва да бъде записан в базата данни.</span><span class="sxs-lookup"><span data-stu-id="89c95-235">The **timesheetLineNeedsUpdating** method is used to determine whether the line record has been changed by the user in the app and must be saved to the database.</span></span> <span data-ttu-id="89c95-236">Ако производителността не е проблем, този метод може да бъде опростен, така че винаги да се връща **вярно**.</span><span class="sxs-lookup"><span data-stu-id="89c95-236">If performance isn't a concern, this method can be simplified so that it always returns **true**.</span></span>
- <span data-ttu-id="89c95-237">Методите **populateTimesheetLineFromEntryDuringCreate** и **populateTimesheetLineFromEntryDuringUpdate** могат да бъдат разширени, така че да въвеждат стойности в записа на базата данни TSTimesheetLine от предоставения запис на договор за данни TSTimesheetEntry.</span><span class="sxs-lookup"><span data-stu-id="89c95-237">The **populateTimesheetLineFromEntryDuringCreate** and **populateTimesheetLineFromEntryDuringUpdate** methods can be extended so that they enter values in the TSTimesheetLine database record from the TSTimesheetEntry data contract record that is provided.</span></span> <span data-ttu-id="89c95-238">В примера, който следва, обърнете внимание как картографирането между полето на базата данни и полето за въвеждане се извършва ръчно чрез код X ++.</span><span class="sxs-lookup"><span data-stu-id="89c95-238">In the example that follows, notice how the mapping between the database field and the entry field is manually done via X++ code.</span></span>
- <span data-ttu-id="89c95-239">Методът **populateTimesheetWeekFromEntry** може също да бъде удължен, ако потребителското поле, което е съпоставено с обекта **TSTimesheetEntry** трябва да пише обратно в таблицата на базата данни TSTimesheetLineweek.</span><span class="sxs-lookup"><span data-stu-id="89c95-239">The **populateTimesheetWeekFromEntry** method can also be extended if the custom field that is mapped to the **TSTimesheetEntry** object must write back to the TSTimesheetLineweek database table.</span></span>

> [!NOTE]
> <span data-ttu-id="89c95-240">Следващият пример записва стойността **firstOption** или **secondOption**, която потребителят избира към базата данни като необработена низова стойност.</span><span class="sxs-lookup"><span data-stu-id="89c95-240">The following example saves the **firstOption** or **secondOption** value that the user selects to the database as a raw string value.</span></span> <span data-ttu-id="89c95-241">Ако полето на базата данни е поле на тип **Изброяване**, тези стойности могат да бъдат ръчно преобразувани в стойност на преброяване и след това да бъдат записани в поле за изброяване в таблицата на базата данни.</span><span class="sxs-lookup"><span data-stu-id="89c95-241">If the database field is a field of the **Enum** type, those values can be manually mapped to an enum value and then saved to an enum field on the database table.</span></span>

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

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a><span data-ttu-id="89c95-242">Показване на персонализирано поле в секцията на заглавка</span><span class="sxs-lookup"><span data-stu-id="89c95-242">Show a custom field in the timesheet header section</span></span>

<span data-ttu-id="89c95-243">По-долу е екранна снимка от мобилното приложение на потребител, преглеждащ разписанието.</span><span class="sxs-lookup"><span data-stu-id="89c95-243">Below is a screenshot from the mobile app of a user viewing a timesheet.</span></span> <span data-ttu-id="89c95-244">Бутонът „Повече информация“ е избран в горния десен ъгъл, за да се покаже опцията „Преглед на повече подробности“.</span><span class="sxs-lookup"><span data-stu-id="89c95-244">The "More information" button has been selected in the upper-right corner to show the "View more details" option.</span></span>  

![Команда за преглед на още подробности](media/show-more.png)

<span data-ttu-id="89c95-246">По-долу е екранна снимка от мобилното приложение, показващ секцията „Още” на разписанието.</span><span class="sxs-lookup"><span data-stu-id="89c95-246">Below is a screenshot from the mobile app showing the “More” section of a timesheet.</span></span> <span data-ttu-id="89c95-247">Потребителско поле, наречено "Скорост на използване на този работен лист (изчислено персонализирано поле)" е добавено към раздела за заглавие на работния лист.</span><span class="sxs-lookup"><span data-stu-id="89c95-247">A custom field called “Utilization rate of this timesheet (computed custom field)” has been added to the timesheet header section.</span></span> <span data-ttu-id="89c95-248">Стойността само за четене "0.667" е зададена в потребителското поле.</span><span class="sxs-lookup"><span data-stu-id="89c95-248">A read-only value of "0.667" is set on the custom field.</span></span>

![Секция „Още”](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="89c95-250">Разширете таблицата TSTimesheetTable, така че да има персонализирано поле</span><span class="sxs-lookup"><span data-stu-id="89c95-250">Extend the TSTimesheetTable table so that it has a custom field</span></span>

<span data-ttu-id="89c95-251">В типичните сценарии е вероятно данните за персонализирано поле в секцията заглавие ще бъдат изтеглени от таблицата TSTimesheetHeader.</span><span class="sxs-lookup"><span data-stu-id="89c95-251">In typical scenarios, it's likely that the data for a custom field in the header section will be pulled from the TSTimesheetHeader table.</span></span> <span data-ttu-id="89c95-252">Други таблици обаче могат да се използват, ако данните могат да бъдат извлечени въз основа на предоставения запис TSTimesheetTable или ако той няма конкретен контекст на записа (например, ако полето е зададено като само за четене в параметрите на проекта).</span><span class="sxs-lookup"><span data-stu-id="89c95-252">However, other tables can be used if the data can be retrieved based on a TSTimesheetTable record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="89c95-253">Обърнете внимание, че потребителските полета не трябва да имат подкрепящи записи на база данни.</span><span class="sxs-lookup"><span data-stu-id="89c95-253">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="89c95-254">Те могат да се генерират динамично въз основа на X ++ логика.</span><span class="sxs-lookup"><span data-stu-id="89c95-254">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="89c95-255">Примерът, който следва, показва този подход.</span><span class="sxs-lookup"><span data-stu-id="89c95-255">The example that follows shows this approach.</span></span>

<span data-ttu-id="89c95-256">Полетата в заглавната секция винаги са само за четене в приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-256">Fields in the header section are always read-only in the app.</span></span>

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a><span data-ttu-id="89c95-257">Използвайте верига от команди на метода buildCustomFieldList на класа TSTimesheetSettings, за да покажете поле в секцията на заглавката</span><span class="sxs-lookup"><span data-stu-id="89c95-257">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the header section</span></span>

<span data-ttu-id="89c95-258">Този код контролира настройките на дисплея за полето в приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-258">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="89c95-259">Например той контролира вида на полето, етикета, дали полето е задължително и в кой раздел се появява полето.</span><span class="sxs-lookup"><span data-stu-id="89c95-259">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="89c95-260">Следващият пример показва изчислена стойност в заглавната секция в приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-260">The following example shows a computed value in the header section in the app.</span></span>

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a><span data-ttu-id="89c95-261">Използвайте верига от команди на метода buildCustomFieldListForHeader на класа TSTimesheetDetails, за да попълните подробностите на разписанието</span><span class="sxs-lookup"><span data-stu-id="89c95-261">Use chain of command on the buildCustomFieldListForHeader method of the TSTimesheetDetails class to fill in timesheet details</span></span>

<span data-ttu-id="89c95-262">Методът **buildCustomFieldListForHeader** се използва за попълване в подробностите на подробностите за заглавка на разписание в мобилното приложение.</span><span class="sxs-lookup"><span data-stu-id="89c95-262">The **buildCustomFieldListForHeader** method is used to fill in the timesheet header details in the mobile app.</span></span> <span data-ttu-id="89c95-263">За параметър се взема запис TSTimesheetTable.</span><span class="sxs-lookup"><span data-stu-id="89c95-263">It takes a TSTimesheetTable record as a parameter.</span></span> <span data-ttu-id="89c95-264">Полета от този запис могат да се използват за попълване на стойността на персонализираното поле в приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-264">Fields from that record can be used to fill in the custom field value in the app.</span></span> <span data-ttu-id="89c95-265">Следващият пример не чете никакви стойности от базата данни.</span><span class="sxs-lookup"><span data-stu-id="89c95-265">The following example doesn't read any values from the database.</span></span> <span data-ttu-id="89c95-266">Вместо това използва X ++ логика, за да генерира изчислена стойност, която след това се показва в приложението.</span><span class="sxs-lookup"><span data-stu-id="89c95-266">Instead, it uses X++ logic to generate a computed value that is then shown in the app.</span></span>


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

## <a name="other-configurabilityextensibility-opportunities"></a><span data-ttu-id="89c95-267">Други възможности за конфигуриране / разширяемост</span><span class="sxs-lookup"><span data-stu-id="89c95-267">Other configurability/extensibility opportunities</span></span>

### <a name="adding-additional-validation-for-the-app"></a><span data-ttu-id="89c95-268">Добавяне на допълнителна проверка за приложението</span><span class="sxs-lookup"><span data-stu-id="89c95-268">Adding additional validation for the app</span></span>

<span data-ttu-id="89c95-269">Съществуващата логика за функционалността на разписанието на ниво база данни ще продължи да работи, както се очаква.</span><span class="sxs-lookup"><span data-stu-id="89c95-269">Existing logic for timesheet functionality at the database level will still work as expected.</span></span> <span data-ttu-id="89c95-270">За да прекъснете завършването на операциите за запис или изпращане и да покажете конкретно съобщение за грешка, можете да добавите **хвърляне на грешка ("съобщение до потребителя")** към кода чрез разширение на верига от команди.</span><span class="sxs-lookup"><span data-stu-id="89c95-270">To interrupt the completion of save or submit operations and show a specific error message, you can add **throw error("message to user")** to the code via a chain of command extension.</span></span> <span data-ttu-id="89c95-271">Ето три примера за полезни разширяеми методи:</span><span class="sxs-lookup"><span data-stu-id="89c95-271">Here are three examples of useful extensible methods:</span></span>

- <span data-ttu-id="89c95-272">Ако **validateWrite** в таблицата TSTimesheetLine се връща **невярно** по време на операция за запазване на ред за работен лист в мобилното приложение се показва съобщение за грешка.</span><span class="sxs-lookup"><span data-stu-id="89c95-272">If **validateWrite** on the TSTimesheetLine table returns **false** during a save operation for a timesheet line, an error message is shown in the mobile app.</span></span>
- <span data-ttu-id="89c95-273">Ако **validateSubmit** в таблицата TSTimesheetTable се връща **невярно** по време на подаването на разписанието в приложението на потребителя се показва съобщение за грешка.</span><span class="sxs-lookup"><span data-stu-id="89c95-273">If **validateSubmit** on the TSTimesheetTable table returns **false** during timesheet submission in the app, an error message is shown to the user.</span></span>
- <span data-ttu-id="89c95-274">Логика, която запълва полета (например, **Свойство на линията**) по време на метод **вмъкване** в таблицата TSTimesheetLine ще продължи да работи.</span><span class="sxs-lookup"><span data-stu-id="89c95-274">Logic that fills in fields (for example, **Line Property**) during the **insert** method on the TSTimesheetLine table will still run.</span></span>

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a><span data-ttu-id="89c95-275">Скриване и маркиране на полетата извън кутията само за четене чрез конфигурация</span><span class="sxs-lookup"><span data-stu-id="89c95-275">Hiding and marking out-of-box fields as read-only via configuration</span></span>

<span data-ttu-id="89c95-276">От параметрите на проекта можете да направите полетата извън полето само за четене или скрити в мобилното приложение.</span><span class="sxs-lookup"><span data-stu-id="89c95-276">From the project parameters, you can make out-of-box fields read-only or hidden in the mobile app.</span></span> <span data-ttu-id="89c95-277">Задайте опциите в секцията **Мобилни разписания** на раздела **Таблица за работно време** на страницата **Управление на проекти и счетоводни параметри**.</span><span class="sxs-lookup"><span data-stu-id="89c95-277">Set the options in the **Mobile timesheets** section on the **Timesheet** tab of the **Project management and accounting parameters** page.</span></span>

![Параметри на проекта](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a><span data-ttu-id="89c95-279">Промяна на дейностите, които са достъпни за избор чрез разширения</span><span class="sxs-lookup"><span data-stu-id="89c95-279">Changing the activities that are available for selection via extensions</span></span>

<span data-ttu-id="89c95-280">Дейностите, които са на разположение за избор на проект, се попълват чрез **getActivitiesForProject()** и **getActivityQuery()** методи в клас **TsTimesheetProjectService**.</span><span class="sxs-lookup"><span data-stu-id="89c95-280">The activities that are available for selection for a project are filled in via the **getActivitiesForProject()** and **getActivityQuery()** methods in the **TsTimesheetProjectService** class.</span></span> <span data-ttu-id="89c95-281">Можете да използвате командна верига, за да промените това поведение, за да съответства на вашия бизнес сценарий за дейностите, които са достъпни за избор за конкретен проект.</span><span class="sxs-lookup"><span data-stu-id="89c95-281">You can use chain of command to change this behavior to match your business scenario for the activities that are available for selection for a specific project.</span></span>

### <a name="entering-a-default-project-category-on-timesheet-entries"></a><span data-ttu-id="89c95-282">Въвеждане на категория на проекта по подразбиране в записите в разписанието</span><span class="sxs-lookup"><span data-stu-id="89c95-282">Entering a default project category on timesheet entries</span></span>

<span data-ttu-id="89c95-283">Вписването на категория на проекта по подразбиране в записите в разписанието се извършва на три нива.</span><span class="sxs-lookup"><span data-stu-id="89c95-283">Entry of a default project category on timesheet entries occurs at three levels.</span></span> <span data-ttu-id="89c95-284">Можете да използвате командна верига, за да разширите поведението на всяко или всички от тези нива, за да постигнете желаното поведение.</span><span class="sxs-lookup"><span data-stu-id="89c95-284">You can use chain of command to extend the behavior at any or all of these levels to achieve the desired behavior.</span></span> <span data-ttu-id="89c95-285">Използва се следната йерархия:</span><span class="sxs-lookup"><span data-stu-id="89c95-285">The following hierarchy is used:</span></span>

1. <span data-ttu-id="89c95-286">Приложението се опитва да постави категорията по подразбиране от ресурса на проекта.</span><span class="sxs-lookup"><span data-stu-id="89c95-286">The app tries to put the default category from the project resource.</span></span> <span data-ttu-id="89c95-287">Тази категория по подразбиране е зададена в методите **getCurrentUserResource** и **getDelegatedResourcesForCurrentUser** в класа **TSTimesheetSettingsService**.</span><span class="sxs-lookup"><span data-stu-id="89c95-287">This default category is set in the **getCurrentUserResource** and **getDelegatedResourcesForCurrentUser** methods in the **TSTimesheetSettingsService** class.</span></span>
2. <span data-ttu-id="89c95-288">Ако категорията по подразбиране не е предоставена на ниво ресурс на проекта, приложението се опитва да я изтегли от активността на проекта.</span><span class="sxs-lookup"><span data-stu-id="89c95-288">If the default category isn't provided at the project resource level, the app tries to pull it from the project activity.</span></span> <span data-ttu-id="89c95-289">Тази категория по подразбиране е зададена в метода **getActivitiesForProject** в класа **TSTimesheetProjectServic**.</span><span class="sxs-lookup"><span data-stu-id="89c95-289">This default category is set in the **getActivitiesForProject** method in the **TSTimesheetProjectService** class.</span></span>
3. <span data-ttu-id="89c95-290">Ако категорията по подразбиране не е предоставена на ниво дейност по проекта, категорията по подразбиране се взема от параметрите на проекта.</span><span class="sxs-lookup"><span data-stu-id="89c95-290">If the default category isn't provided at the project activity level, the default category it taken from the project parameters.</span></span> <span data-ttu-id="89c95-291">Тази категория по подразбиране е зададена в метода **getProjectDetailsbyRule** в класа **TSTimesheetProjectServic**.</span><span class="sxs-lookup"><span data-stu-id="89c95-291">This default category is set in the **getProjectDetailsbyRule** method in the **TSTimesheetProjectService** class.</span></span>
