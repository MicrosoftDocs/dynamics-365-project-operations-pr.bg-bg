---
title: Промени на функции от Project Service Automation до Project Operations
description: Тази статия предоставя общ преглед на промените на функциите от Project Service Automation към Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/03/2022
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
ms.reviewer: johnmichalak
ms.openlocfilehash: a9c69fc4296d30763f3994a4955e64ab258ceb4f
ms.sourcegitcommit: 675e9f3615e701c5f998de3a5ea3e25df11ae107
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/09/2022
ms.locfileid: "9459913"
---
# <a name="feature-changes-from-project-service-automation-to-project-operations"></a>Промени на функции от Project Service Automation до Project Operations

Надстройката от Dynamics 365 Project Service Automation до Dynamics 365 Project Operations Lite ще бъде предоставена в три фази. Тази статия предоставя информация за основните промени, които можете да очаквате да видите, когато надстройката приключи.

| Доставка на надграждане | Фаза 1 <br>(януари 2022) | Фаза 2 <br>(ноември 2022 г.) | Фаза 3  |
|------------------|------------------------|---------------------------|---------------------------|
| Няма зависимост от съставната структура на работата (WBS) за проекти. | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| WBS е включен в рамките на текущо поддържаните ограничения на Project Operations. | &nbsp; | :heavy_check_mark: | :heavy_check_mark: |
| WBS извън поддържаните в момента ограничения на Project Operations, включително поддръжка за Project Desktop Client. | &nbsp; | &nbsp; | :heavy_check_mark: |

## <a name="project-management"></a>Управление на проекти

Най-значимите промени в потребителското изживяване ще бъдат в областта на планирането на проекти. Project Operations възприема нов модерен опит за управление на съставна структура на работата (WBS) чрез използване на възможностите за планиране, предоставени от [Project for the Web](https://support.microsoft.com/en-us/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5).

## <a name="differences-in-the-scheduling-experience"></a>Разлики във функцията за планиране

Следната таблица обобщава разликите в планирането между Project Service Automation и Project Operations.

|  Планиране     |   Project Operations   |   PSA   |
|-----------------|------------------------|---------|
| Шаблони за проекти - Възможност за дефиниране и прилагане на шаблони за проекти, когато проектът е създаден  |  &nbsp;    | :heavy_check_mark: |
| Интеграция на съставна структура на работата (WBS) по проекта с настолен клиент   |    &nbsp;  | :heavy_check_mark: |
| Ограничения - Започнете не по-рано от, завършете не по-късно от  | :heavy_check_mark: |   &nbsp;  |
| Етапи - Задачи с нулева продължителност   | :heavy_check_mark:  |  &nbsp;  |
| Задачите, управлявани от ресурси, ще зачитат наличността на присвоените ресурси   | :heavy_check_mark: |  &nbsp;    |
| Редактиране във времето - Редактирайте планове и работете всеки ден   |   &nbsp;  | :heavy_check_mark: |
| Автоматично/ръчно планиране - Използвайте механизма за планиране на проекта, за да планирате автоматично или ръчно задачи |  &nbsp; | :heavy_check_mark:  |
| Редактирайте големи проекти директно в потребителския интерфейс: Няма ограничение за размера на плановете, които могат да се редактират  | Ограничение от 500 задачи  | :heavy_check_mark:       |
| Процент на завършеност - Маркирайте напредъка на задачата   | :heavy_check_mark:  |  &nbsp;  |
| [Режими на график на проекта](../project-management/scheduling-modes.md) - Дефинирайте проекта като фиксирани единици, фиксирани усилия или фиксирана продължителност | :heavy_check_mark: | &nbsp; |
| Времева линия - Изградете и персонализирайте изгледа на времевата линия, за да визуализирате детайлите на графика и да комуникирате със заинтересованите лица. | :heavy_check_mark:  | &nbsp; |
| Базирани на усилие задачи - Поддръжка на системата за планиране при планиране на задача като базирана на усилие  | :heavy_check_mark:  | &nbsp; |
| Диалогов прозорец **Информация за задачите** - Запазване на детайлите на задачата с помощта на диалогов прозорец | :heavy_check_mark:  |  &nbsp;  |
| Плъзнете и пуснете - Избирайте няколко задачи и променяйте позицията им в WBS | :heavy_check_mark: | &nbsp;  |
| Гъвкави постоянни изгледи - Дефинирайте по-подробни изгледи на атрибутите на задачата   | :heavy_check_mark:  | &nbsp; |
| Сортиране и филтриране на WBS  | :heavy_check_mark:  | &nbsp; |
| Изглед на дъски за доставка на проект без каскада  | :heavy_check_mark:   | &nbsp; |
| Изглед на времева линия - Интерактивна диаграма на Гант, използвана за визуализиране и редактиране на WBS   | :heavy_check_mark:  | &nbsp; |
| Клавишни комбинации - Използвайте клавишни комбинации за обичайни операции, като отстъп или вмъкване  | :heavy_check_mark:  |  &nbsp; |
| Отмяна на много нива - Извършете анализ какво ще стане, за да разберете напълно въздействието на промените чрез обръщане и повторно прилагане на цял набор от операции | :heavy_check_mark: | &nbsp; |
| Изрязване/Копиране/Поставяне – Сътрудничество при разработването на график чрез копиране и поставяне на подробности за графика между приложенията  | :heavy_check_mark: | &nbsp; |
| Контролни списъци със задачи - Добавете до 20 елемента от контролен списък към задача   | :heavy_check_mark: | &nbsp; |

## <a name="project-planning"></a>Планиране на проект

Страницата **Проект** в Project Operations има значителен брой разлики в сравнение със страницата **Проект** в Project Service Automation.

Следните действия са премахнати от страницата **Проекти** като част от фаза 1 на надстройка:

  - **Отвори в MS Project**
  - **Създаване на шаблон**
  - **Премахни връзката от MS Project**

Страницата **Проект** в Project Operations включва следните нови раздели.

- **Оценки на материал**
- **Настройка на фактуриране на задача**

Разделът **Статус** е премахнат и полето **Статус** сега е в раздела **Резюме** с режима на планиране на проекта.

   ![Актуализации на страницата „Проект“.](media/projectform.png)

Разделът **График** е преименуван на раздел **Задача** и включва новото изживяване за планиране на проекти с Project for the Web.

   ![Нов раздел „Задачи по проект“.](media/tasktab.png)

## <a name="scheduling-modes"></a>Методи на планиране

Project Operations въведе нова функция, [Режими на планиране](../project-management/scheduling-modes.md). Всички съществуващи проекти на Project Service Automation ще бъдат по подразбиране с **Фиксирана продължителност** в Project Operations. Въпреки това, настройката по подразбиране за нови проекти може да се управлява, като отидете на **Настройки** > **Параметри** > **Параметър** > **Режим на график**.

   ![Настройки на параметрите на проекта за режим График.](media/projectparameter.png)

## <a name="project-planning-limits"></a>Ограничения на планиране на проект

Project Operations разчита на Project for the Web за всички операции по планиране на проекти. Project for the Web управлява съставната структура на работата, като използва ограниченията в следващата таблица.

| **Поле**                                          | **Ограничение**             |
|----------------------------------------------------|-----------------------|
| Максимален общ брой задачи за един проект                  | 500                   |
| Максимално общо времетраене за един проект               | 3650 дни (10 години)  |
| Максимален общ брой ресурси за един проект              | 300                   |
| Максимален общ брой връзки (само за наследник) за проект | 600                   |
| Максимален общ брой персонализирани полета за един проект          | 10                    |
| Максимално ниво на йерархия                            | 10 нива             |
| Максимален брой връзки (наследник + предшественик)            | 20                    |
| Максимална продължителност на задачата за листа                      | 1250 дни             |
| Максимална продължителност на обобщена задача                 | 3650 дни (10 години)  |
| Максимален брой ресурси, присвоени на задача               | 20 ресурса          |
| Поддържан период от време за задача                    | 1/1/2000 - 12/31/2149 |
| Елементи в контролен списък                                    | 20                    |

## <a name="project-planning-extensibility-and-development"></a>Разширяване и развитие на планирането на проекта

След като надстроите до Project Operations, трябва да използвате API на Project Scheduling, за да изпълните операции за създаване, актуализиране и изтриване на следните обекти:

|   Име на обекта           |   Логическо име на обект       |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Задача по проект            | msdyn_projecttask           |
| Зависимост на задачи от проект | msdyn_projecttaskdependency |
| Назначаване на ресурс     | msdyn_resourceassignment    |
| Набор на проекта          | msdyn_projectbucket         |
| Член на екипа на проект     | msdyn_projectteam           |

Ако в момента имате персонализации, които включват тези обекти, вижте [Използвайте API за график на проекта, за да извършвате операции с обекти за планиране](../project-management/schedule-api-preview.md) за насоки за изпълнение.

## <a name="data-model-changes"></a>Промени на модел данни

Като част от фаза на надграждане 1 има промени в модела данни. Тези промени са предимно полеви промени на съществуващи обекти. Във фаза 1 обектите **msydn_project** и **msdyn_projectteam** са рефакторинг на персонализации. 

> [!IMPORTANT]
> Този раздел ще бъде актуализиран с допълнителни обекти при завършване на бъдещи фази на надграждане.

Следните полета са заменени с нови полета.

|   Entity          |   Старо логическо име   |   Ново логическо име    |
|-------------------|----------------------|-----------------------|
| msdyn_project     | msdyn_actualhours    | msdyn_effortcompleted |
| msdyn_project     | msdyn_plannedhours   | msdyn_effort          |
| msdyn_project     | msdyn_remaininghours | msdyn_effortremaining |
| msdyn_project     | msdyn_scheduledend   | msdyn_finish          |
| msdyn_project     | msdyn_wbsduration    | msdyn_duration        |
| msdyn_projectteam | msdyn_assignedhours  | msdyn_effort          |
| msdyn_projectteam | msdyn_from           | msdyn_start           |
| msdyn_projectteam | msdyn_to             | msdyn_finish          |

Добавени са следните полета.

|   Entity          |   Логическо име                               |   Описание |
|-------------------|----------------------------------------------|---------------|
| msdyn_project     | msdyn_actualfeesales                         | Показва сбора на действителните такси за продажби по проекта. За използване само в Project Service Automation. |
| msdyn_project     | msdyn_actualmaterialcost                     | Показва сбора на действителната цена на материала по проекта. За използване само в Project Service Automation. |
| msdyn_project     | msdyn_actualmaterialsales                    | Показва сбора на действителните продажби на материал по проекта. За използване само в Project Service Automation. |
| msdyn_project     | msdyn_businesscase                           |                |
| msdyn_project     | msdyn_contractlineproject                    | Аспектите на договор, свързани с този проект. |
| msdyn_project     | msdyn_copyprojectcorrelationid               | Това е вътрешно поле на системата, използвано за **Копиране на проект**, свързано с идентификатора на корелация. За използване само в Project Service Automation. |
| msdyn_project     | msdyn_copyprojectsessionid                   | Това е вътрешно поле на системата, използвано за **Копиране на проект**, свързано с идентификатора на сесия. За използване само в Project Service Automation. |
| msdyn_project     | msdyn_globalrevisiontoken                    | Последно синхронизиране xRM Global Revision Token от услугата за планиране на проекта. |
| msdyn_project     | msdyn_msprojectdocument                      | Документът на Microsoft Project, който принадлежи към проекта. |
| msdyn_project     | msdyn_plannedmaterialcost                    | Сборът на планираната цена на материала по проекта. За използване само в Project Service Automation. |
| msdyn_project     | msdyn_plannedmaterialsales                   | Сборът на планираните продажби на материали по проекта. За използване само в Project Service Automation. |
| msdyn_project     | msdyn_program                                | Програмата, с която е свързан този проект. |
| msdyn_project     | msdyn_quotelineproject                       | Редът на оферта, свързан с този проект. |
| msdyn_project     | msdyn_replaylogheader                        | Заглавката на регистрационните файлове за повторно възпроизвеждане. |
| msdyn_project     | msdyn_schedulemode                           | Режимът на планиране по подразбиране, използван за всички задачи в проекта.  |
| msdyn_project     | msdyn_taskearlieststart                      | Най-ранната начална дата на всяка задача в проекта.  |
| msdyn_project     | msdyn_valuestatement                         |                |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Членът на екипа по проекта, от който е копиран този член на екипа по проекта. |
| msdyn_projectteam | msdyn_creategenericteammemberwithrequirement | Посочва дали да се създаде изискването за ресурс за новосъздаден общ член на екипа.  |
| msdyn_projectteam | msdyn_deletestatus                           | Състоянието на изтриване на члена на екипа, за да се проследи дали има изпратена заявка за изтриване до услугата за планиране на проекти и дали тя успешно е изпратила отговор в рамките на очаквания времеви прозорец. |
| msdyn_projectteam | msdyn_effortcompleted                        | Проследява усилията, положени от члена на екипа по заданието му. |
| msdyn_projectteam | msdyn_effortremaining                        | Проследява все още незавършени усилия, положени от члена на екипа по заданието му. |
| msdyn_projectteam | msdyn_markedfordeletiontimer                 | Периодът на изчакване от момента, в който членът на екипа изпрати заявка за изтриване до услугата за планиране на проекта, докато членът на екипа действително бъде изтрит в Microsoft Dataverse.|
| msdyn_projectteam | msdyn_markedfordeletiontimestamp             | Времевото клеймо за запис, когато заявката за изтриване на член на екипа е изпратена на услугата за планиране на проекти. |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Показва члена на екипа по проекта, от който е копиран този член на екипа по проекта.  |

## <a name="project-templates"></a>Шаблони на проекти

Project Operations не предоставя поддръжка за шаблони на проекти. Можете обаче да копирате голяма част от основната функционалност с помощта на [API за копиране на проекти](../project-management/dev-copy-project.md).

## <a name="desktop-add-in-support"></a>Поддръжка на добавки за настолен компютър

Поддръжката за добавката Microsoft Project Desktop няма да бъде налична в първите 2 фази на надстройката. Във фаза 3 клиентите, които имат проекти, по-големи от текущо поддържаните ограничения на Project for the Web, ще могат да използват добавката за настолен компютър.

## <a name="editing-resource-assignment-contours"></a>Редактиране на контури за присвояване на ресурси

Възможността за редактиране на контурите за присвояване на ресурси ще бъде налична, когато е налична фаза 2 на надстройката.

## <a name="billing-and-pricing"></a>Фактуриране и ценообразуване

Следните нови функции са добавени в Project Operations. Тези функции са адитивни по природа и не оказват влияние върху модела на данни на Project Service Automation.

- [Записване на използването на материали по проекти и проектни задачи](../material/material-usage-log.md)
- [Управление на подизпълнения](../pro/subcontracting/managing-subcontracts-overview.md)
- [Базирани на авансови плащания и капаро договори](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [Състояние и проверки за стойности по договор, които не трябва да се надвишават](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- [Фактуриране, базирано на задача](../pro/sales/mapping-projects-tasks-quote-line-sales.md)

## <a name="deprecated-components"></a>Отхвърлени компоненти

Следващите таблици документират всички остарели полета, които са преместени в решението за остарели компоненти след надграждане. За повече информация и връзка към решението вижте [отхвърлени компоненти между Dynamics 365 Project Service Automation 3x и Project Operations 4x](https://github.com/microsoft/Dynamics365-Project-Operations-PowerApps/tree/main/3x-4x-deprecated-solution).

### <a name="invoicedetail"></a>invoicedetail

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
|invoicedetail.msdyn_contractline    |

### <a name="msdyn_actual"></a>msdyn_actual

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_actual.msdyn_salescontractline                                                          |

### <a name="msdyn_characteristicreqforteammember"></a>msdyn_characteristicreqforteammember

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_characteristicreqforteammember.msdyn_characteristic                                     |
| msdyn_characteristicreqforteammember.msdyn_characteristicreqforteammemberid                   |
| msdyn_characteristicreqforteammember.msdyn_characteristictype                                 |
| msdyn_characteristicreqforteammember.msdyn_name                                               |
| msdyn_characteristicreqforteammember.msdyn_ratingvalue                                        |
| msdyn_characteristicreqforteammember.msdyn_resourcerequirementid                              |

### <a name="msdyn_contractlineinvoiceschedule"></a>msdyn_contractlineinvoiceschedule

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_contractlineinvoiceschedule.msdyn_contractline                                          |
| msdyn_contractlinescheduleofvalue.msdyn_contractline                                          |
 
### <a name="msdyn_dataexport"></a>msdyn_dataexport

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_dataexport.msdyn_dataexportid                                                           |
| msdyn_dataexport.msdyn_datatoken                                                              |
| msdyn_dataexport.msdyn_entityname                                                             |
| msdyn_dataexport.msdyn_exportedrecordcount                                                    |
| msdyn_dataexport.msdyn_exportstatus                                                           |
| msdyn_dataexport.msdyn_linkedentitydata                                                       |
| msdyn_dataexport.msdyn_name                                                                   |
| msdyn_dataexport.msdyn_pagingdata                                                             |

### <a name="msdyn_fact"></a>msdyn_fact

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_fact.msdyn_salescontractline                                                            |

### <a name="msdyn_findworkevent"></a>msdyn_findworkevent

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_findworkevent.msdyn_bookableresource                                                    |
| msdyn_findworkevent.msdyn_findworkeventid                                                     |
| msdyn_findworkevent.msdyn_name                                                                |
| msdyn_findworkevent.msdyn_timestamp                                                           |
| msdyn_findworkevent.msdyn_type                                                                |
| msdyn_findworkevent.msdyn_value                                                               |
| msdyn_findworkevent.msdyn_work                                                                |

### <a name="msdyn_invoicelinetransaction"></a>msdyn_invoicelinetransaction

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_invoicelinetransaction.msdyn_invoiceline                                                |
| msdyn_invoicelinetransaction.msdyn_salescontractline                                          |

### <a name="msdyn_journalline"></a>msdyn_journalline

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_journalline.msdyn_salescontractline                                                     |

### <a name="msdyn_opportunitylineresourcecategory"></a>msdyn_opportunitylineresourcecategory

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylineresourcecategory.msdyn_billingtype                                       |
| msdyn_opportunitylineresourcecategory.msdyn_description                                       |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylineresourcecategoryid                 |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylinetransactionclassification          |
| msdyn_opportunitylineresourcecategory.msdyn_resourcecategory                                  |

### <a name="msdyn_opportunitylinetransaction"></a>msdyn_opportunitylinetransaction

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransaction.msdyn_accountcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_accountingdate                                         |
| msdyn_opportunitylinetransaction.msdyn_accountvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_amount                                                 |
| msdyn_opportunitylinetransaction.msdyn_amount_base                                            |
| msdyn_opportunitylinetransaction.msdyn_amountmethod                                           |
| msdyn_opportunitylinetransaction.msdyn_basisamount                                            |
| msdyn_opportunitylinetransaction.msdyn_basisamount_base                                       |
| msdyn_opportunitylinetransaction.msdyn_basisprice                                             |
| msdyn_opportunitylinetransaction.msdyn_basisprice_base                                        |
| msdyn_opportunitylinetransaction.msdyn_basisquantity                                          |
| msdyn_opportunitylinetransaction.msdyn_billingtype                                            |
| msdyn_opportunitylinetransaction.msdyn_bookableresource                                       |
| msdyn_opportunitylinetransaction.msdyn_contactcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_contactvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_customertype                                           |
| msdyn_opportunitylinetransaction.msdyn_description                                            |
| msdyn_opportunitylinetransaction.msdyn_documentdate                                           |
| msdyn_opportunitylinetransaction.msdyn_enddatetime                                            |
| msdyn_opportunitylinetransaction.msdyn_exchangeratedate                                       |
| msdyn_opportunitylinetransaction.msdyn_opportunityline                                        |
| msdyn_opportunitylinetransaction.msdyn_opportunitylinetransactionid                           |
| msdyn_opportunitylinetransaction.msdyn_percent                                                |
| msdyn_opportunitylinetransaction.msdyn_price                                                  |
| msdyn_opportunitylinetransaction.msdyn_price_base                                             |
| msdyn_opportunitylinetransaction.msdyn_pricelist                                              |
| msdyn_opportunitylinetransaction.msdyn_product                                                |
| msdyn_opportunitylinetransaction.msdyn_project                                                |
| msdyn_opportunitylinetransaction.msdyn_quantity                                               |
| msdyn_opportunitylinetransaction.msdyn_resourcecategory                                       |
| msdyn_opportunitylinetransaction.msdyn_resourceorganizationalunitid                           |
| msdyn_opportunitylinetransaction.msdyn_startdatetime                                          |
| msdyn_opportunitylinetransaction.msdyn_task                                                   |
| msdyn_opportunitylinetransaction.msdyn_transactioncategory                                    |
| msdyn_opportunitylinetransaction.msdyn_transactionclassification                              |
| msdyn_opportunitylinetransaction.msdyn_transactiontypecode                                    |
| msdyn_opportunitylinetransaction.msdyn_unit                                                   |
| msdyn_opportunitylinetransaction.msdyn_unitschedule                                           |
| msdyn_opportunitylinetransaction.msdyn_vendortype                                             |

### <a name="msdyn_opportunitylinetransactioncategory"></a>msdyn_opportunitylinetransactioncategory

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactioncategory.msdyn_billingtype                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_description                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactioncategoryid           |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactionclassification       |
| msdyn_opportunitylinetransactioncategory.msdyn_transactioncategory                            |

### <a name="msdyn_opportunitylinetransactionclassificatio"></a>msdyn_opportunitylinetransactionclassificatio

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactionclassificatio.msdyn_billingtype                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_description                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_include                                   |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunityline                           |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunitylinetransactionclassificatioid |
| msdyn_opportunitylinetransactionclassificatio.msdyn_transactionclassification                 |

### <a name="msdyn_orderlineresourcecategory"></a>msdyn_orderlineresourcecategory

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlineresourcecategory.msdyn_contractline                                            |

### <a name="msdyn_orderlinetransaction"></a>msdyn_orderlinetransaction

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransaction.msdyn_salescontractline                                            |
| msdyn_orderlinetransactioncategory.msdyn_contractline                                         |

### <a name="msdyn_orderlinetransactionclassification"></a>msdyn_orderlinetransactionclassification

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransactionclassification.msdyn_contractline                                   |

### <a name="msdyn_project"></a>msdyn_project

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_project.msdyn_actualdurationminutes                                                     |
| msdyn_project.msdyn_actualhours                                                               |
| msdyn_project.msdyn_istemplate                                                                |
| msdyn_project.msdyn_plannedhours                                                              |
| msdyn_project.msdyn_projecttemplate                                                           |
| msdyn_project.msdyn_remaininghours                                                            |
| msdyn_project.msdyn_scheduleddurationminutes                                                  |
| msdyn_project.msdyn_scheduledend                                                              |
| msdyn_project.msdyn_stagename                                                                 |
| msdyn_project.msdyn_wbsduration                                                               |


### <a name="msdyn_projecttask"></a>msdyn_projecttask

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttask.msdyn_actualdurationminutes                                                 |
| msdyn_projecttask.msdyn_actualeffort                                                          |
| msdyn_projecttask.msdyn_aggregationdirection                                                  |
| msdyn_projecttask.msdyn_assignedresources                                                     |
| msdyn_projecttask.msdyn_assignedteammembers                                                   |
| msdyn_projecttask.msdyn_autoscheduling                                                        |
| msdyn_projecttask.msdyn_costestimatecontour                                                   |
| msdyn_projecttask.msdyn_effortcontour                                                         |
| msdyn_projecttask.msdyn_islinetask                                                            |
| msdyn_projecttask.msdyn_numberofresources                                                     |
| msdyn_projecttask.msdyn_remaininghours                                                        |
| msdyn_projecttask.msdyn_resourceutilization                                                   |
| msdyn_projecttask.msdyn_salesestimatecontour                                                  |
| msdyn_projecttask.msdyn_scheduledhours                                                        |
| msdyn_projecttask.msdyn_wbsid                                                                 |

### <a name="msdyn_projecttaskstatususer"></a>msdyn_projecttaskstatususer

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttaskstatususer.msdyn_bookableresource                                            |
| msdyn_projecttaskstatususer.msdyn_description                                                 |
| msdyn_projecttaskstatususer.msdyn_expectedcompletiondate                                      |
| msdyn_projecttaskstatususer.msdyn_expectedhourstocomplete                                     |
| msdyn_projecttaskstatususer.msdyn_iscompleted                                                 |
| msdyn_projecttaskstatususer.msdyn_name                                                        |
| msdyn_projecttaskstatususer.msdyn_percentcomplete                                             |
| msdyn_projecttaskstatususer.msdyn_projecttaskid                                               |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatusindicator                                  |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatususerid                                     |

### <a name="msdyn_projectteam"></a>msdyn_projectteam

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteam.msdyn_applicantcount                                                        |
| msdyn_projectteam.msdyn_applicantsavailable                                                   |
| msdyn_projectteam.msdyn_assignedhours                                                         |
| msdyn_projectteam.msdyn_description                                                           |
| msdyn_projectteam.msdyn_from                                                                  |
| msdyn_projectteam.msdyn_hoursrequested                                                        |
| msdyn_projectteam.msdyn_membershipstatus                                                      |
| msdyn_projectteam.msdyn_number                                                                |
| msdyn_projectteam.msdyn_to                                                                    |

### <a name="msdyn_projectteammembersignup"></a>msdyn_projectteammembersignup

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteammembersignup.msdyn_bookableresource                                          |
| msdyn_projectteammembersignup.msdyn_membershipstatus                                          |
| msdyn_projectteammembersignup.msdyn_name                                                      |
| msdyn_projectteammembersignup.msdyn_projectteammembersignupid                                 |
| msdyn_projectteammembersignup.msdyn_teammembership                                            |

### <a name="msdyn_projecttransactioncategory"></a>msdyn_projecttransactioncategory

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttransactioncategory.msdyn_billingtype                                            |
| msdyn_projecttransactioncategory.msdyn_name                                                   |
| msdyn_projecttransactioncategory.msdyn_project                                                |
| msdyn_projecttransactioncategory.msdyn_projecttransactioncategoryid                           |
| msdyn_projecttransactioncategory.msdyn_transactioncategory                                    |

### <a name="msdyn_quotelineinvoiceschedule"></a>msdyn_quotelineinvoiceschedule

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_quotelineinvoiceschedule.msdyn_quoteline                                                |
| msdyn_quotelineresourcecategory.msdyn_quoteline                                               |
| msdyn_quotelinescheduleofvalue.msdyn_quoteline                                                |
| msdyn_quotelinetransaction.msdyn_quoteline                                                    |
| msdyn_quotelinetransactioncategory.msdyn_quoteline                                            |
| msdyn_quotelinetransactionclassification.msdyn_quoteline                                      |

### <a name="msdyn_resourceassignment"></a>msdyn_resourceassignment

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_resourceassignment.msdyn_hours                                                          |
| msdyn_resourceassignment.msdyn_fromdate                                                       |
| msdyn_resourceassignment.msdyn_msprojectclientid                                              |
| msdyn_resourceassignment.msdyn_todate                                                         |
| msdyn_resourceassignmentdetail.msdyn_duration                                                 |
| msdyn_resourceassignmentdetail.msdyn_from                                                     |
| msdyn_resourceassignmentdetail.msdyn_name                                                     |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentdetailid                               |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentid                                     |

### <a name="salesorderdetail"></a>salesorderdetail

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| salesorderdetail.msdyn_quoteline                                                              |

