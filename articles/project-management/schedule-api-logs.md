---
title: Регистрационни файлове за планиране на проекти
description: Тази статия предоставя информация и примери, които ще ви помогнат да използвате регистрационните файлове на Project Scheduling за проследяване на грешки, които са свързани с услугата Project Scheduling Service и APIs за планиране на проекти.
author: ruhercul
ms.date: 11/30/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: c57419642e90e4def01f2cd2474c9e82dc162b86
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923682"
---
# <a name="project-scheduling-logs"></a>Регистрационни файлове за планиране на проекти

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси/без складове, леко внедряване - фактуриране по проформа_, _Project for the Web_

Microsoft Dynamics 365 Project Operations използва [Project for the Web](https://support.microsoft.com/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5) като основна система за планиране. Вместо да използва стандартни интерфейси за програмиране на уеб приложения (API) на Microsoft Dataverse, Project Operations използва новите API за планиране на проекти за създаване, актуализиране и изтриване на задачи по проекти, присвоявания на ресурси, зависимости на задачи, кофи за проекти и членове на екипи по проекти. Въпреки това, когато операциите за създаване, актуализиране или изтриване се изпълняват програмно на обекти на съставна структура на работата (WBS), може да възникнат грешки. За проследяване на тези грешки и историята на операциите са въведени два нови административни журнала: **Набор от операции** и **Услуга за планиране на проекти (PSS)**. За достъп до тези регистрационни файлове отидете на **Настройки** \> **Интегриране на график**.

Следващата илюстрация показва модела на данни за регистрационните файлове на планирането на проекта.

![Модел на данните за дневниците за планиране на проекти.](media/LOGDATAMODEL.jpg)

## <a name="operation-set-log"></a>Регистър на набор от операции

Регистрационният файл на набор от операции проследява изпълнението на набор от операции, който се използва за изпълнение на една или много операции за създаване, актуализиране или изтриване в пакет на проекти, задачи на проекти, присвояване на ресурси, зависимости на задачи, кофи за проекти или членове на екипа на проекта. Полето **Операция в състояние** показва общото състояние на набора операции. Подробностите за полезния товар на набора от операции се записват в свързани записи с подробности за набор от операции.

### <a name="operation-set"></a>Набор от опции

Следната таблица показва полетата, които са свързани с обекта **Набор от операции**.

| Име на схема            | Описание                                                                                                  | DisplayName            |
|-----------------------|--------------------------------------------------------------------------------------------------------------|------------------------|
| msdyn_completedon     | Датата/часът на завършване или неуспех на набора от операции.                                                | CompletedOn            |
| msdyn_correlationid   | Стойността **correlationId** на заявката.                                                                  | CorrelationId          |
| msdyn_description     | Описанието на набора от операции.                                                                        | Описание            |
| msdyn_executedon      | Датата/часът, когато записът е стартиран.                                                                       | Изпълнено на            |
| msdyn_operationsetId  | Еднозначен идентификатор на екземпляри на обект.                                                                   | OperationSet           |
| msdyn_Project         | Проектът, свързан с набора от операции.                                                            | Project                |
| msdyn_projectid       | Стойността **projectId** на заявката.                                                                      | ProjectId (отхвърлено) |
| msdyn_projectName     | Неприложимо.                                                                                              | Неприложимо         |
| msdyn_PSSErrorLog     | Уникалният идентификатор на регистрационния файл за грешки на Project Scheduling Service, който е свързан с набора операции. | Регистрационен файл за грешки на PSS          |
| msdyn_PSSErrorLogName | Неприложимо.                                                                                              | Неприложимо         |
| msdyn_status          | Състоянието на набора от операции.                                                                             | Статус                 |
| msdyn_statusName      | Неприложимо.                                                                                              | Неприложимо         |
| msdyn_useraadid       | ИД на обект на Azure Active Directory (Azure AD) на потребителя, на когото принадлежи тази заявка.                     | UserAADID              |

### <a name="operation-set-detail"></a>Подробност за набор от операции

Следната таблица показва полетата, които са свързани с обекта **Подробност за набор от операции**.

| Име на схема                 | Описание                                                                                 | DisplayName           |
|----------------------------|---------------------------------------------------------------------------------------------|-----------------------|
| msdyn_cdspayload           | Сериализираните полета на Dataverse за заявката.                                            | CdsPayload            |
| msdyn_entityname           | Името на обекта за заявката.                                                     | EntityName            |
| msdyn_httpverb             | Методът на заявката.                                                                         | HTTPVerb (отхвърлено) |
| msdyn_httpverbName         | Неприложимо.                                                                             | Неприложимо        |
| msdyn_operationset         | Еднозначният идентификатор на набора от операции, към който принадлежи записът.                      | OperationSet          |
| msdyn_operationsetdetailId | Еднозначен идентификатор на екземпляри на обект.                                                  | Подробност за OperationSet   |
| msdyn_operationsetName     | Неприложимо.                                                                             | Неприложимо        |
| msdyn_operationtype        | Типът операция на подробността за набор от операции.                                             | OperationType         |
| msdyn_operationtypeName    | Неприложимо.                                                                             | Неприложимо        |
| msdyn_psspayload           | Сериализираните полета на Project Scheduling Service за заявката.                           | PssPayload            |
| msdyn_recordid             | Идентификаторът на записа на заявка.                                                       | ИД на запис             |
| msdyn_requestnumber        | Автоматично генериран номер, който идентифицира реда, в който са получени заявките. | Номер на заявка        |

## <a name="project-scheduling-service-error-logs"></a>Регистри на грешките на услугата за планиране на проекти

Регистрационните файлове за грешки на Project Scheduling Service улавят грешки, които възникват, когато Project Scheduling Service опита операция за **Записване** или **Отваряне**. Има три поддържани сценария, при които се генерират тези регистрационни файлове:

- Действията, инициирани от потребителя, са критично неуспешни (например присвояване не може да бъде създадено поради липсващи привилегии).
- Услугата за планиране на проекти не може програмно да създава, актуализира, изтрива или извършва каквато и да е друга каскадна операция върху обект.
- Потребителят изпитва грешки, когато запис не успее да се отвори (например, когато се отвори проект или се актуализира информацията на член на екипа).

### <a name="project-scheduling-service-log"></a>Регистър на услуга за планиране на проекти

В следващата таблица са показани полетата, които са включени в дневника на услугата за планиране на проекти.

| Име на схема          | Описание                                                                    | DisplayName    |
|---------------------|--------------------------------------------------------------------------------|----------------|
| msdyn_CallStack     | Стекът на повикванията на изключението.                                               | Стек на повикванията     |
| msdyn_correlationid | ИД на корелация на грешката.                                               | CorrelationId  |
| msdyn_errorcode     | Поле, което се използва за съхраняване на код за грешка на Dataverse или HTTP код за грешка. | Код на грешка     |
| msdyn_HelpLink      | Връзка към публичната документация за помощ.                                       | Връзка за помощ      |
| msdyn_log           | Дневникът от услугата за планиране на проекти.                                   | Регистрационен файл            |
| msdyn_project       | Проектът, свързан с регистрационния файл за грешка.                             | Project        |
| msdyn_projectName   | Името на проекта, ако полезният товар на набора операции ще бъде запазен. | Неприложимо |
| msdyn_psserrorlogId | Еднозначен идентификатор на екземпляри на обект.                                     | Регистрационен файл за грешки на PSS  |
| msdyn_SessionId     | ИД на сесия на проекта.                                                        | ИД на сесия     |

## <a name="error-log-cleanup"></a>Изчистване на регистрационен файл за грешки

По подразбиране както регистрационните файлове за грешки на Project Scheduling Service, така и регистрационният файл за набор от операции могат да се почистват на всеки 90 дни. Всички записи, които са по-стари от 90 дни, се изтриват. Въпреки това, чрез промяна на стойността на полето **msdyn_StateOperationSetAge** на страницата **Параметри на проекта**, администраторите могат да коригират диапазона на почистване, така че да е между 1 и 120 дни. Налични са няколко метода за промяна на тази стойност:

- Персонализирайте обекта **Параметър на проекта** чрез създаване на персонализирана страница и добавяне на полето **Възраст на набор от остарели операции**.
- Използвайте клиентски код, който използва [Комплект за разработка на софтуер WebApi (SDK)](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/updaterecord).
- Използвайте Service SDK код, който използва метода на Xrm SDK **updateRecord** (препратка към API на клиента) в управлявани от модел приложения. Power Apps включва описание и поддържани параметри за метода **updateRecord**.

    ```C#
    Xrm.WebApi.retrieveMultipleRecords('msdyn_projectparameter').then(function (response) {
        parameter = response.entities[0];
        var staleOperationValue = prompt("All records older than (x) days will be deleted, please enter X between 1 to 90 days", 1)
        var newData = {};
        newData.msdyn_projectparameterid = parameter.msdyn_projectparameterid;
        newData.msdyn_staleoperationsetage = parseInt(staleOperationValue);
        Xrm.WebApi.updateRecord("msdyn_projectparameter", parameter.msdyn_projectparameterid, newData).then(
            function success(result) {
                console.log("Project Parameter: Stale Operation Expiry is set to: " + newData.msdyn_staleoperationsetage);
                // perform operations on record update
                Xrm.WebApi.retrieveMultipleRecords('msdyn_projectparameter')
                .then(function (response2) { console.log("Confirmed Project Parameter: Stale Operation Expiry is set to: " + response2.entities[0].msdyn_staleoperationsetage) });
            },
            function (error) {
                console.log("Failed to Update Project Ednpoint with error: " + error.message);
            // handle error conditions
            }
        );
    });
    ```
