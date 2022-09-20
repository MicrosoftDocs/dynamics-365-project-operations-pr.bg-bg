---
title: Промени на функции от Project Service Automation до Project Operations
description: Тази статия предоставя общ преглед на промените на функциите от Project Service Automation в Dynamics 365 Project Operations.
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

Надстройката от Dynamics 365 Project Service Automation до Dynamics 365 Project Operations Lite ще бъде доставена в три фази. Тази статия предоставя информация за основните промени, които можете да очаквате да видите, когато надстройката завърши.

| Ъпгрейд доставка | Фаза 1 <br>(януари 2022 г.) | Фаза 2 <br>(ноември 2022 г.) | Фаза 3  |
|------------------|------------------------|---------------------------|---------------------------|
| Няма зависимост от структурата на разбивката на работата (WBS) за проекти. | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| WBS е включена в поддържаните понастоящем граници на Project Operations. | &nbsp; | :heavy_check_mark: | :heavy_check_mark: |
| WBS извън поддържаните в момента граници на Project Operations, включително поддръжка за настолен клиент на Project. | &nbsp; | &nbsp; | :heavy_check_mark: |

## <a name="project-management"></a>Управление на проекти

Най-значимите промени в потребителския опит ще бъдат в областта на планирането на проекти. Project Operations приема нов модерен опит за управление на структура на разбивка на работата (WBS) чрез ливъридж на възможностите за планиране, предоставени от [Project for the Web](https://support.microsoft.com/en-us/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5).

## <a name="differences-in-the-scheduling-experience"></a>Разлики в изживяването при планиране

Следната таблица обобщава разликите в планирането между автоматизацията на услугата на проекта и операциите по проекта.

|  Планиране     |   Project Operations   |   PSA   |
|-----------------|------------------------|---------|
| Шаблони за проекти - Възможност за дефиниране и прилагане на шаблони за проекти при създаване на проект  |  &nbsp;    | :heavy_check_mark: |
| Проект работа разбивка структура (WBS) интеграция с настолен клиент   |    &nbsp;  | :heavy_check_mark: |
| Ограничения - Започнете не по-рано от, завърши не по-късно от  | :heavy_check_mark: |   &nbsp;  |
| Етапни цели - Задачи с нулева продължителност   | :heavy_check_mark:  |  &nbsp;  |
| Задачите, задвижвани с ресурси, ще зачитат наличието на присвоени ресурси   | :heavy_check_mark: |  &nbsp;    |
| Редактиране поетапно във времето - Редактиране на планове и работа на дневна база   |   &nbsp;  | :heavy_check_mark: |
| Автоматично/ръчно планиране - Използвайте двигателя за планиране на проекта за автоматично или ръчно планиране на задачи |  &nbsp; | :heavy_check_mark:  |
| Редактиране на големи проекти директно в потребителския интерфейс: Няма ограничение за размера на плановете, които могат да се редактират  | 500 ограничение на задачите  | :heavy_check_mark:       |
| Процентът е завършен - Маркирайте напредъка на задачата   | :heavy_check_mark:  |  &nbsp;  |
| [Режими](../project-management/scheduling-modes.md) на график на проекта - Дефиниране на проекта като фиксирани единици, фиксирани усилия или фиксирана продължителност | :heavy_check_mark: | &nbsp; |
| Хронология - Изграждане и персонализиране на изгледа на времевата скала, за да визуализирате подробности за графика и да комуникирате със заинтересованите страни. | :heavy_check_mark:  | &nbsp; |
| Задачи, задвижвани от усилията - Планиране на поддръжка на двигатели за планиране на задача като задвижвани усилия  | :heavy_check_mark:  | &nbsp; |
| **Диалогов прозорец за информация** за задачите - Запазване на подробностите за задачите с помощта на диалогов прозорец | :heavy_check_mark:  |  &nbsp;  |
| Плъзгане и пускане - Задачи с няколко избора и модифициране на позицията им на WBS | :heavy_check_mark: | &nbsp;  |
| Гъвкави постоянни изгледи - Дефиниране на по-гранулирани изгледи на атрибутите на задачите   | :heavy_check_mark:  | &nbsp; |
| Сортиране и филтриране на WBS  | :heavy_check_mark:  | &nbsp; |
| Дъски изглед за доставка на проекти, които не са водопади  | :heavy_check_mark:   | &nbsp; |
| Изглед на времевата скала - Интерактивна диаграма на Гант, използвана за визуализиране и редактиране на WBS   | :heavy_check_mark:  | &nbsp; |
| Клавишни комбинации - Използвайте клавишни комбинации за често срещани операции, като от тире или вмъкване  | :heavy_check_mark:  |  &nbsp; |
| Отмяна на няколко нива - Извършване на анализ на какво-ако, за да се разбере напълно въздействието на промените чрез обръщане и повторно приложение на цял набор от операции | :heavy_check_mark: | &nbsp; |
| Cut/Copy/Paste - Съвместна работа по разработване на график чрез копиране и поставяне на подробности за графика между приложенията  | :heavy_check_mark: | &nbsp; |
| Контролни списъци за задачи - Добавяне на до 20 елемента от контролния списък към задача   | :heavy_check_mark: | &nbsp; |

## <a name="project-planning"></a>Планиране на проект

Страницата на **проекта** в Project Operations има значителен брой разлики в сравнение със страницата на **проекта** в Project Service Automation.

Следните действия са премахнати от **страницата "Проекти** " като част от надстройката фаза 1:

  - **Отвори в MS Project**
  - **Създаване на шаблон**
  - **Премахни връзката от MS Project**

Страницата на **проекта** в Project Operations включва следните нови раздели.

- **Оценки на материал**
- **Настройка на фактуриране на задача**

Разделът **Състояние** е премахнат и **полето Състояние** сега е в **раздела Резюме** с режима на планиране на проекта.

   ![Актуализации на страницата на проекта.](media/projectform.png)

Разделът **График** е преименуван в **раздела Задача** и разполага с новия опит за планиране на проекти с Project за уеб.

   ![Раздел "Нови задачи по проекта".](media/tasktab.png)

## <a name="scheduling-modes"></a>Методи на планиране

Project Operations въведе нова функция, [Режими](../project-management/scheduling-modes.md) на планиране. Всички съществуващи проекти на Project Service Automation ще по подразбиране фиксирана **продължителност** в операциите на проекта. Обаче по подразбиране за нови проекти може да се управлява, като отидете **на Настройки** > **параметри** > **·** > **параметър график режим**.

   ![Настройки на параметрите на проекта за режим График.](media/projectparameter.png)

## <a name="project-planning-limits"></a>Лимити за планиране на проекти

Project Operations разчита на Project за уеб за всички операции по планиране на проекти. Проект за уеб управлява структурата на разбивка на работата с помощта на ограниченията в следващата таблица.

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

## <a name="project-planning-extensibility-and-development"></a>Разширяемост и разработване на планиране на проекти

След надграждане до Project Operations, трябва да използвате API за планиране на проекти за изпълнение на създаване, актуализиране и изтриване на операции на следните обекти:

|   Име на обекта           |   Логическо име на обект       |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Задача по проект            | msdyn_projecttask           |
| Зависимост на задачи от проект | msdyn_projecttaskdependency |
| Назначаване на ресурс     | msdyn_resourceassignment    |
| Набор на проекта          | msdyn_projectbucket         |
| Член на екипа на проект     | msdyn_projectteam           |

Ако в момента имате персонализации, които включват тези обекти, вижте [Използване на API за график на проекта за извършване на операции с обекти](../project-management/schedule-api-preview.md) за планиране за насоки за внедряване.

## <a name="data-model-changes"></a>Промени в модела на данните

Като част от Фаза 1 на надстройване има промени в модела на данните. Тези промени са преди всичко промени на полета на съществуващи обекти. Във Фаза 1 обектите, **msydn_project** и **msdyn_projectteam** са рефракториране на персонализациите. 

> [!IMPORTANT]
> Този раздел ще се актуализира с допълнителни обекти, тъй като бъдещите фази на надстройване са завършени.

Следните полета са заменени с нови полета.

|   Entity          |   Старо логично име   |   Ново логично име    |
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
| msdyn_project     | msdyn_actualfeesales                         | Показва съвкупната сума на действителните продажби на такси по проекта. За използване само в "Автоматизация на услугата за проекти". |
| msdyn_project     | msdyn_actualmaterialcost                     | Показва сумарния съвкуп на действителните материални разходи по проекта. За използване само в "Автоматизация на услугата за проекти". |
| msdyn_project     | msdyn_actualmaterialsales                    | Показва съвкупната сума на действителните продажби на материали по проекта. За използване само в "Автоматизация на услугата за проекти". |
| msdyn_project     | msdyn_businesscase                           |                |
| msdyn_project     | msdyn_contractlineproject                    | Редът от договора, свързан с този проект. |
| msdyn_project     | msdyn_copyprojectcorrelationid               | Това е вътрешно системно поле, което се използва за **Копиране на проект**, свързано с идентификатора на корелация. За използване само в "Автоматизация на услугата за проекти". |
| msdyn_project     | msdyn_copyprojectsessionid                   | Това е вътрешно системно поле, използвано за **Копиране на проект**, свързано с идентификатора на сесията. За използване само в "Автоматизация на услугата за проекти". |
| msdyn_project     | msdyn_globalrevisiontoken                    | Последно синхронизиране на xRM глобален маркер за ревизия от услугата за планиране на проекти. |
| msdyn_project     | msdyn_msprojectdocument                      | Документът на Microsoft Project, който принадлежи на проекта. |
| msdyn_project     | msdyn_plannedmaterialcost                    | Съвкупната сума на планираните материални разходи по проекта. За използване само в "Автоматизация на услугата за проекти". |
| msdyn_project     | msdyn_plannedmaterialsales                   | Съвкупната сума на планираните продажби на материали по проекта. За използване само в "Автоматизация на услугата за проекти". |
| msdyn_project     | msdyn_program                                | Програмата, с която е свързан този проект. |
| msdyn_project     | msdyn_quotelineproject                       | Редът "Оферта", свързан с този проект. |
| msdyn_project     | msdyn_replaylogheader                        | Заглавката за регистрационните файлове за повторения. |
| msdyn_project     | msdyn_schedulemode                           | Режимът на планиране по подразбиране, използван за всички задачи по проекта.  |
| msdyn_project     | msdyn_taskearlieststart                      | Най-ранната начална дата на всяка задача в проекта.  |
| msdyn_project     | msdyn_valuestatement                         |                |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Членът на екипа на проекта, от който е копиран този член на екипа по проекта. |
| msdyn_projectteam | msdyn_creategenericteammemberwithrequirement | Показва дали да създадете изискването за ресурс за новосъздаен генеричен член на екипа.  |
| msdyn_projectteam | msdyn_deletestatus                           | Състоянието на изтриване на члена на екипа за проследяване, ако има заявка за изтриване, изпратена до услугата за планиране на проекта, и дали тя успешно изпраща отговор обратно в рамките на прозореца на очакваното време. |
| msdyn_projectteam | msdyn_effortcompleted                        | Проследява усилията, осъществени от члена на екипа по техните задачи. |
| msdyn_projectteam | msdyn_effortremaining                        | Проследява усилието, което предстои да бъде завършено от члена на екипа по техните задачи. |
| msdyn_projectteam | msdyn_markedfordeletiontimer                 | Периодът на изчакване, считано от момента, в който членът на екипа изпрати искане за изтриване до услугата за планиране на проекта, докато членът на екипа действително бъде изтрит на Microsoft Dataverse.|
| msdyn_projectteam | msdyn_markedfordeletiontimestamp             | Клеймото за запис, когато членът на екипа изтрие заявката се изпраща на услугата за планиране на проекта. |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Показва члена на екипа по проекта, от който е копиран този член на екипа по проекта.  |

## <a name="project-templates"></a>Шаблони на проекти

Project Operations не предоставя поддръжка за шаблони за проекти. Можете обаче да копирате голяма част от основната функционалност с използването на API за копиране на [проекта](../project-management/dev-copy-project.md).

## <a name="desktop-add-in-support"></a>Поддръжка на добавка на работния плот

Поддръжката на добавката "Работен плот на Microsoft Project" няма да бъде налична през първите 2 фази на надстройването. Във фаза 3 клиентите, които имат проекти, по-големи от поддържаните в момента граници на Project for the Web, ще могат да използват добавката за работния плот.

## <a name="editing-resource-assignment-contours"></a>Редактиране на контури за присвояване на ресурси

Възможността за редактиране на контури за присвояване на ресурси ще бъде налична, когато фаза 2 на надстройване е налична.

## <a name="billing-and-pricing"></a>Фактуриране и ценообразуване

Следните нови функции са добавени в Project Operations. Тези функции са адитивни по характер и не оказват въздействие върху модела на данни за автоматизация на услугата за проекти.

- [Записване на използването на материали по проекти и проектни задачи](../material/material-usage-log.md)
- [Управление на подизпълнители](../pro/subcontracting/managing-subcontracts-overview.md)
- [Базирани на авансови плащания и капаро договори](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [Състояние и валидации, които не надвишават договора](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- [Таксуване въз основа на задача](../pro/sales/mapping-projects-tasks-quote-line-sales.md)

## <a name="deprecated-components"></a>Амортизирани компоненти

Следващите таблици документират всички амортирани полета, които се преместват в амортизираното решение компоненти пост надстройка. За повече информация и връзка към решението вижте [Dynamics 365 Project Service Automation 3x към Project Operations 4x амортирани компоненти](https://github.com/microsoft/Dynamics365-Project-Operations-PowerApps/tree/main/3x-4x-deprecated-solution).

### <a name="invoicedetail"></a>фактуриранаетаил

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
|invoicedetail.msdyn_contractline    |

### <a name="msdyn_actual"></a>msdyn_actual

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_actual.msdyn_продажбиизпълнител                                                          |

### <a name="msdyn_characteristicreqforteammember"></a>msdyn_characteristicreqforteammember

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_characteristicreqforteammember.msdyn_характеристика                                     |
| msdyn_characteristicreqforteammember.msdyn_характеристикарекфортеамеберид                   |
| msdyn_characteristicreqforteammember.msdyn_характерен тип                                 |
| msdyn_characteristicreqforteammember.msdyn_име                                               |
| msdyn_characteristicreqforteammember.msdyn_оценкавастойка                                        |
| msdyn_characteristicreqforteammember.msdyn_resourcerementid                              |

### <a name="msdyn_contractlineinvoiceschedule"></a>msdyn_contractlineinvoiceschedule

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_contractlineinvoiceschedule.msdyn_контрактлайн                                          |
| msdyn_contractlinescheduleofvalue.msdyn_контрактлайн                                          |
 
### <a name="msdyn_dataexport"></a>msdyn_dataexport

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_dataexport.msdyn_dataекспортид                                                           |
| msdyn_dataexport.msdyn_datatoken                                                              |
| msdyn_dataexport.msdyn_име на обект                                                             |
| msdyn_dataexport.msdyn_изнесенорезордкаунт                                                    |
| msdyn_dataexport.msdyn_износстатус                                                           |
| msdyn_dataexport.msdyn_данни за обвързаност                                                       |
| msdyn_dataexport.msdyn_име                                                                   |
| msdyn_dataexport.msdyn_пагингдата                                                             |

### <a name="msdyn_fact"></a>msdyn_fact

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_fact.msdyn_продажбиизпълнител                                                            |

### <a name="msdyn_findworkevent"></a>msdyn_findworkevent

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_findworkevent.msdyn_резервирай ресурс                                                    |
| msdyn_findworkevent.msdyn_намериработавентен                                                     |
| msdyn_findworkevent.msdyn_име                                                                |
| msdyn_findworkevent.msdyn_клеймо                                                           |
| msdyn_findworkevent.msdyn_type                                                                |
| msdyn_findworkevent.msdyn_стойност                                                               |
| msdyn_findworkevent.msdyn_работа                                                                |

### <a name="msdyn_invoicelinetransaction"></a>msdyn_invoicelinetransaction

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_invoicelinetransaction.msdyn_фактура линия                                                |
| msdyn_invoicelinetransaction.msdyn_продажбиизпълнител                                          |

### <a name="msdyn_journalline"></a>msdyn_journalline

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_journalline.msdyn_продажбиизпълнител                                                     |

### <a name="msdyn_opportunitylineresourcecategory"></a>msdyn_opportunitylineresourcecategory

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylineresourcecategory.msdyn_тип фактуриране                                       |
| msdyn_opportunitylineresourcecategory.msdyn_описание                                       |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylineresourcecategoryid                 |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylineтрансакциякласификация          |
| msdyn_opportunitylineresourcecategory.msdyn_ресурен категория                                  |

### <a name="msdyn_opportunitylinetransaction"></a>msdyn_opportunitylinetransaction

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransaction.msdyn_акаунтcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_счетоводна дата                                         |
| msdyn_opportunitylinetransaction.msdyn_акаунтвендор                                          |
| msdyn_opportunitylinetransaction.msdyn_сума                                                 |
| msdyn_opportunitylinetransaction.msdyn_сума_база                                            |
| msdyn_opportunitylinetransaction.msdyn_сумаметод                                           |
| msdyn_opportunitylinetransaction.msdyn_базиста                                            |
| msdyn_opportunitylinetransaction.msdyn_базисаmount_база                                       |
| msdyn_opportunitylinetransaction.msdyn_базацена                                             |
| msdyn_opportunitylinetransaction.msdyn_базацена_база                                        |
| msdyn_opportunitylinetransaction.msdyn_основаквантитет                                          |
| msdyn_opportunitylinetransaction.msdyn_тип фактуриране                                            |
| msdyn_opportunitylinetransaction.msdyn_резервирай ресурс                                       |
| msdyn_opportunitylinetransaction.msdyn_контакт обичай                                        |
| msdyn_opportunitylinetransaction.msdyn_контактвендор                                          |
| msdyn_opportunitylinetransaction.msdyn_клиентски тип                                           |
| msdyn_opportunitylinetransaction.msdyn_описание                                            |
| msdyn_opportunitylinetransaction.msdyn_документ                                           |
| msdyn_opportunitylinetransaction.msdyn_крайвреме                                            |
| msdyn_opportunitylinetransaction.msdyn_обменен дата                                       |
| msdyn_opportunitylinetransaction.msdyn_възможност линия                                        |
| msdyn_opportunitylinetransaction.msdyn_възможностлинтрансакцияid                           |
| msdyn_opportunitylinetransaction.msdyn_процента                                                |
| msdyn_opportunitylinetransaction.msdyn_цена                                                  |
| msdyn_opportunitylinetransaction.msdyn_цена_база                                             |
| msdyn_opportunitylinetransaction.msdyn_ценова листа                                              |
| msdyn_opportunitylinetransaction.msdyn_продукт                                                |
| msdyn_opportunitylinetransaction.msdyn_проект                                                |
| msdyn_opportunitylinetransaction.msdyn_количество                                               |
| msdyn_opportunitylinetransaction.msdyn_ресурен категория                                       |
| msdyn_opportunitylinetransaction.msdyn_ресурсорганизационна унитиди                           |
| msdyn_opportunitylinetransaction.msdyn_стартдатайм                                          |
| msdyn_opportunitylinetransaction.msdyn_задача                                                   |
| msdyn_opportunitylinetransaction.msdyn_транзакциякатегория                                    |
| msdyn_opportunitylinetransaction.msdyn_класификация на транзакциите                              |
| msdyn_opportunitylinetransaction.msdyn_трансакционен типкод                                    |
| msdyn_opportunitylinetransaction.msdyn_единица                                                   |
| msdyn_opportunitylinetransaction.msdyn_модул                                           |
| msdyn_opportunitylinetransaction.msdyn_доставчик тип                                             |

### <a name="msdyn_opportunitylinetransactioncategory"></a>msdyn_opportunitylinetransactioncategory

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactioncategory.msdyn_тип фактуриране                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_описание                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylineтрансакциякатегорид           |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylineтрансакциякласификация       |
| msdyn_opportunitylinetransactioncategory.msdyn_транзакциякатегория                            |

### <a name="msdyn_opportunitylinetransactionclassificatio"></a>msdyn_opportunitylinetransactionclassificatio

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactionclassificatio.msdyn_тип фактуриране                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_описание                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_включвам                                   |
| msdyn_opportunitylinetransactionclassificatio.msdyn_възможност линия                           |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunitylinetransactionкласификатиоид |
| msdyn_opportunitylinetransactionclassificatio.msdyn_класификация на транзакциите                 |

### <a name="msdyn_orderlineresourcecategory"></a>msdyn_orderlineresourcecategory

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlineresourcecategory.msdyn_контрактлайн                                            |

### <a name="msdyn_orderlinetransaction"></a>msdyn_orderlinetransaction

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransaction.msdyn_продажбиизпълнител                                            |
| msdyn_orderlinetransactioncategory.msdyn_контрактлайн                                         |

### <a name="msdyn_orderlinetransactionclassification"></a>msdyn_orderlinetransactionclassification

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransactionclassification.msdyn_контрактлайн                                   |

### <a name="msdyn_project"></a>msdyn_project

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_project.msdyn_действителнадействиеминути                                                     |
| msdyn_project.msdyn_действителничаса                                                               |
| msdyn_project.msdyn_istemplate                                                                |
| msdyn_project.msdyn_планираничаса                                                              |
| msdyn_project.msdyn_проектмплит                                                           |
| msdyn_project.msdyn_оставащичаса                                                            |
| msdyn_project.msdyn_графикдуриране минути                                                  |
| msdyn_project.msdyn_планирано                                                              |
| msdyn_project.msdyn_стагенаме                                                                 |
| msdyn_project.msdyn_wbsдюрация                                                               |


### <a name="msdyn_projecttask"></a>msdyn_projecttask

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttask.msdyn_действителнадействиеминути                                                 |
| msdyn_projecttask.msdyn_действителенусиленост                                                          |
| msdyn_projecttask.msdyn_агрегиращапосока                                                  |
| msdyn_projecttask.msdyn_присвоени ресурси                                                     |
| msdyn_projecttask.msdyn_присвоеничленки                                                   |
| msdyn_projecttask.msdyn_автосрочване                                                        |
| msdyn_projecttask.msdyn_costestimateконтур                                                   |
| msdyn_projecttask.msdyn_усилиеконтур                                                         |
| msdyn_projecttask.msdyn_islinetask                                                            |
| msdyn_projecttask.msdyn_numberofresources                                                     |
| msdyn_projecttask.msdyn_оставащичаса                                                        |
| msdyn_projecttask.msdyn_ресурсоизточник                                                   |
| msdyn_projecttask.msdyn_оценка на продажбитеконтур                                                  |
| msdyn_projecttask.msdyn_графикхумори                                                        |
| msdyn_projecttask.msdyn_wbsid                                                                 |

### <a name="msdyn_projecttaskstatususer"></a>msdyn_projecttaskstatususer

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttaskstatususer.msdyn_резервирай ресурс                                            |
| msdyn_projecttaskstatususer.msdyn_описание                                                 |
| msdyn_projecttaskstatususer.msdyn_очакванадовършване                                      |
| msdyn_projecttaskstatususer.msdyn_очакванчастдовършване                                     |
| msdyn_projecttaskstatususer.msdyn_е завършен                                                 |
| msdyn_projecttaskstatususer.msdyn_име                                                        |
| msdyn_projecttaskstatususer.msdyn_процентпълен                                             |
| msdyn_projecttaskstatususer.msdyn_проекттаскид                                               |
| msdyn_projecttaskstatususer.msdyn_проект задачитактусинатор                                  |
| msdyn_projecttaskstatususer.msdyn_проект задачиtatususerid                                     |

### <a name="msdyn_projectteam"></a>msdyn_projectteam

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteam.msdyn_кандидатско ниво                                                        |
| msdyn_projectteam.msdyn_кандидати на разположение                                                   |
| msdyn_projectteam.msdyn_присвоеначаса                                                         |
| msdyn_projectteam.msdyn_описание                                                           |
| msdyn_projectteam.msdyn_от                                                                  |
| msdyn_projectteam.msdyn_часарекордирани                                                        |
| msdyn_projectteam.msdyn_членствастатус                                                      |
| msdyn_projectteam.msdyn_номер                                                                |
| msdyn_projectteam.msdyn_to                                                                    |

### <a name="msdyn_projectteammembersignup"></a>msdyn_projectteammembersignup

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteammembersignup.msdyn_резервирай ресурс                                          |
| msdyn_projectteammembersignup.msdyn_членствостатус                                          |
| msdyn_projectteammembersignup.msdyn_име                                                      |
| msdyn_projectteammembersignup.msdyn_projectteamмембърсигналупид                                 |
| msdyn_projectteammembersignup.msdyn_екипчленство                                            |

### <a name="msdyn_projecttransactioncategory"></a>msdyn_projecttransactioncategory

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttransactioncategory.msdyn_тип фактуриране                                            |
| msdyn_projecttransactioncategory.msdyn_име                                                   |
| msdyn_projecttransactioncategory.msdyn_проект                                                |
| msdyn_projecttransactioncategory.msdyn_проекттрансакциякатегорид                           |
| msdyn_projecttransactioncategory.msdyn_транзакциякатегория                                    |

### <a name="msdyn_quotelineinvoiceschedule"></a>msdyn_quotelineinvoiceschedule

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_quotelineinvoiceschedule.msdyn_цитатлайн                                                |
| msdyn_quotelineresourcecategory.msdyn_цитатлайн                                               |
| msdyn_quotelinescheduleofvalue.msdyn_цитатлайн                                                |
| msdyn_quotelinetransaction.msdyn_цитатлайн                                                    |
| msdyn_quotelinetransactioncategory.msdyn_цитатлайн                                            |
| msdyn_quotelinetransactionclassification.msdyn_цитатлайн                                      |

### <a name="msdyn_resourceassignment"></a>msdyn_resourceassignment

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_resourceassignment.msdyn_часове                                                          |
| msdyn_resourceassignment.msdyn_от дата                                                       |
| msdyn_resourceassignment.msdyn_msпроектклиентиден                                              |
| msdyn_resourceassignment.msdyn_todate                                                         |
| msdyn_resourceassignmentdetail.msdyn_продължителност                                                 |
| msdyn_resourceassignmentdetail.msdyn_от                                                     |
| msdyn_resourceassignmentdetail.msdyn_име                                                     |
| msdyn_resourceassignmentdetail.msdyn_ресурсзадача подробно                               |
| msdyn_resourceassignmentdetail.msdyn_resourcesignmentid                                     |

### <a name="salesorderdetail"></a>търговецдетайл

| Полета                                                    |
|-----------------------------------------------------------------------------------------------|
| salesorderdetail.msdyn_quoteline                                                              |

