---
title: Планиране на работата ви в Microsoft Project с помощта на добавката Project Service
description: Тази тема предоставя информация за това как да използвате добавката Microsoft Project за Microsoft Project Service.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 01/07/2021
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
ms.openlocfilehash: 1b1c9861f2a3fbb62b29ccad272dab28dc766439
ms.sourcegitcommit: 30242d7754bca300b594b0887eb4212d10bea1c4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/07/2022
ms.locfileid: "8727991"
---
# <a name="plan-your-work-in-microsoft-project-with-the-project-service-add-in"></a>Планиране на работата ви в Microsoft Project с помощта на добавката Project Service

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3x](../includes/cc-applies-to-psa-app-3x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ви улеснява при извършване на планирането на проекти, включително прогнози. Можете да определите работата, така че да са ясни разходите, усилията и стойността на продажбите при подаване на окончателното предложение.  

Можете да инсталирате [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] и да извършите работата по планирането в познатата среда на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]. Използвайте стабилните възможностите за планиране и управление на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и след това актуализирайте плана на проекта в Project Service Automation.  

> [!IMPORTANT]
> - За да използвате управлението на документи на SharePoint за съхранение на файловете на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] за проекти на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], администраторът на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] трябва да включи управлението на документи. 
> - [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] е съвместим само с [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.  

## <a name="download-and-install-the-add-in"></a>Изтеглете и инсталирайте добавката  
 Подгответе информацията за регистрация в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Тази информация ви е необходима, за да се свържете от [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] с [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

1.  От центъра за изтегляния изтеглете добавката за вашата поддържана версия на Project Service – [v2.X](/dynamics365/project-operations/psa/overview#guidance-for-earlier-versions-app-version-2x-or-1x) или [v 3.4+](https://www.microsoft.com/download/details.aspx?id=57956).  

2.  Изберете връзката за изтегляне.  

3.  Когато изтеглянето приключи, изберете **Да** за инсталиране на добавката.  

## <a name="configure-the-add-in"></a>Конфигуриране на добавката  

1. Отворете [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и изберете раздел **Project Service**.  

2. Изберете **Свързване**.  

3. Въведете информацията си за влизане и след това изберете **Вход**.  

   Вече можете да започнете да използвате добавката.  

## <a name="read-from-a-template"></a>Четене от шаблон  
 Четете от шаблон, който сте създали в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] и сте копирали в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], за да започнете да планирате своя проект. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Създаване на шаблон на проект (Project Service Automation)](../psa/create-project-template.md)  

1.  От раздела **Project Service** изберете **Четене** > **Шаблон на проект на Project Service Automation**.  

2.  Изберете шаблон на проект от списъка и след това изберете **Отвори**.  

    > [!NOTE]
    >  По подразбиране задачите, които са копирани от шаблона в проекта, са зададени като ръчно планирани.  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a>Присвояване на роли на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] на ресурси на проекти  

1.  Отворете проект и изберете лентата **Задача**.  

2. Изберете менюто **Диаграма на Гант** и след това изберете **Лист на ресурсите**.  

3. В листа на ресурсите, изберете падащото меню **Роля на ресурс в Project Service** и изберете роля в Project Service Automation.  

## <a name="staff-your-project-with-resources"></a>Осигурете ресурси за проекта си  

1.  От раздела Project Service изберете ред и изберете **Търсене на ресурси**.  

2.  На екрана **Резервиране на ресурс** изберете ресурса, който искате да използвате за проекта.  

3.  Изберете **Резервиране** и след това изберете **OK**.  

## <a name="publish-your-project"></a>Публикуване на вашия проект  
Когато приключи планирането на проекта, следващата стъпка е импортиране и публикуване на проекта в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

Проектът ще се импортира в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Прилагат се ценообразуването и процесът на генериране на екип. Отворете проекта в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], за да проверите, че са генерирани екипът, оценките на проекта и съставната структура на работата. В таблицата по-долу е показано къде да се намерят резултатите.


|              Microsoft Project                                                           |                      Project Service Automation                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Диаграма на Гант**   | Импортиране в екрана на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Съставна структура на работата**. |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Списък с ресурси** |   Импортиране в екрана на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Членове на екипа на проект**.   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Използване на употреба**    |    Импортира в екрана на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Оценки на проект**.     |

**За да импортирате и публикувате проекта**  
1. В раздела **Project Service** отидете на **Публикуване** > **Нов проект на Project Service Automation**.  

2. В диалоговия прозорец **Публикуване в нов проект в Project Service** въведете **Име на проект** и изберете **Клиент**.  

3. По желание изберете **Свързване на плана на проекта с Project Service Automation**, за да се свърже файлът на плана на проекта с Project Service Automation.  

4. Изберете **Публикуване**.  

   Свързването на файла на проекта с [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] прави файла на проекта главен и задава съставната структура на работата в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] като само за четене.  За да направите промени в плана на проекта, трябва да ги направите в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да ги публикувате като актуализации в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

## <a name="edit-a-project-thats-been-imported"></a>Редактиране на проект, който е импортиран  
 За да направите промени на план на проект, който е импортиран в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], имате две опции:  

- Отваряне на главния файл и редактиране в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

- Премахване на връзката на файла и редактиране директно в Project Service. По подразбиране проект, който е качен от [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], е заключен и може да се редактира само в проекта. За да редактирате файла в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], връзката на файла трябва да се премахне.  

### <a name="edit-in-pn_microsoft_project"></a>Редактиране в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]  

1. В главното меню отидете на **Project Service** > **Проекти**.  

2. От списъка с проекти отворете този, който сте създали в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. Изберете **Отвори в MS Project** от лентата. Така ще се отвори свързаният главен файл в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a>Премахване на връзката на файл и редактиране в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service  

1. В главното меню отидете на **Project Service** > **Проекти**.  

2. От списъка с проекти отворете този, който сте създали в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. Изберете **Премахни връзката с MS Project** от лентата.  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a>Качване на файл на проект в SharePoint или групи на Office  
 Можете да качите файла на проекта си в SharePoint и да го намерите под „Свързани документи” за проекта на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  Администраторът трябва да конфигурира управление на документи на SharePoint и да го включи за обекта на проекта. 

 Също така можете да качите файла на проекта на [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)], ако имате зададени групи на Office.

### <a name="upload-a-file-for-sharepoint"></a>Качване на файл за SharePoint  

1. В главното меню отидете на **Project Service** > **Качване**.  

2. Изберете **Към документи на проект в Project Service Automation**.  

3. В диалога **Разрешаване на отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** изберете **Да** или **Не**.  

   - Ако изберете **Да**, ще можете да изберете **Отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** в Project Service Automation, да стартирате [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да заредите файла на проекта от библиотеката с документи на SharePoint.  

   - Ако изберете **Не**, връзката за **Отворете в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** няма да работи.  

4. Файлът на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] може да се намери в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] под **Документи** за конкретния проект на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

### <a name="upload-a-file-for-office-groups"></a>Качване на файл за групи на Office  

1. В главното меню отидете на **Project Service** > **Качване**.  

2. Изберете **Към документи на проект в Project Service Automation**.  

3. В диалога **Разрешаване на отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** изберете **Да** или **Не**.  

   - Ако изберете **Да**, ще можете да изберете **Отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** в Project Service Automation, да стартирате [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да заредите файла на проекта от библиотеката с документи на SharePoint.  

   - Ако изберете **Не**, връзката за **Отворете в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** няма да работи.  

4. Файлът на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] може да се намери в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] под **Документи** за конкретния проект на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

## <a name="publish--your-project-as-a-template"></a>Публикуване на вашия проект като шаблон  
 Можете да запишете проекта си и да го използвате отново, като го запишете като шаблон на проект в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Шаблоните на проекти са планове на проекти за многократна употреба в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. За повече информация вижте [Създаване на шаблон за проект (Project Service Automation)](../psa/create-project-template.md). 

1. В раздела **Project Service** отидете на **Публикуване** > **Нов шаблон за проект на Project Service Automation**.  

2. В диалоговия прозорец **Публикуване в нов проект в шаблон на Project Service** въведете **Име на шаблона на проект**.  

3. По желание можете да изберете **Свързване на плана на проекта с Project Service Automation**, за да се свърже файлът на проекта с [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

4. Изберете **Публикуване**.  

Свързването на файла на проекта с [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] прави файла на проекта главен и задава съставната структура на работата в шаблона на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] само за четене.  За да направите промени в плана на проекта, трябва да ги направите в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да ги публикувате като актуализации в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].

## <a name="read-a-resource-loaded-schedule"></a>Четене на график, зареден с ресурс

Когато четете проект от Project Service Automation, календарът на ресурса не се синхронизира с настолния клиент. Ако има разлики в продължителността, усилията или края на задачата, вероятно причината е, че ресурсите и настолният клиент нямат един и същи календар с шаблон за работно време, приложен към проекта.


## <a name="data-synchronization"></a>Синхронизиране на данни
Таблиците в този раздел предоставят информация за синхронизирането на данните на обекта между Project Service Automation и добавката за настолни компютри на Microsoft Project.

### <a name="project-task-entity-table"></a>Таблица на обектите на проектната задача
Следващата таблица описва как данните на обекта на проектната задача се синхронизират между Project Service Automation и добавката за настолни компютри на Microsoft Project.

| **Обект** | **Поле** | **Microsoft Project към Project Service Automation** | **Project Service Automation към Microsoft Project** |
| --- | --- | --- | --- |
| Задача по проект | Краен срок | Синхронизиран | Несинхронизирано |
| Задача по проект | Очаквано усилие | Синхронизиран | Несинхронизирано |
| Задача по проект | ИД на клиент на MS Project | Синхронизиран | Несинхронизирано |
| Задача по проект | Родителска задача | Синхронизиран | Несинхронизирано |
| Задача по проект | Project | Синхронизиран | Несинхронизирано |
| Задача по проект | Задача от проект | Синхронизиран | Несинхронизирано |
| Задача по проект | Име на задача от проект | Синхронизиран | Несинхронизирано |
| Задача по проект | Ресурсна единица (отхвърлено във версия 3.0) | Синхронизиран | Несинхронизирано |
| Задача по проект | Планирано времетраене | Синхронизиран | Несинхронизирано |
| Задача по проект | Начална дата | Синхронизиран | Несинхронизирано |
| Задача по проект | ИД на ССР | Синхронизиран | Несинхронизирано |

### <a name="team-member-entity-table"></a>Таблица на обекта на член на екипа
Следващата таблица описва как данните на обект на член на екипа се синхронизират между Project Service Automation и Micros

| **Обект** | **Поле** | **Microsoft Project към Project Service Automation** | **Project Service Automation към Microsoft Project** |
| --- | --- | --- | --- |
| Член на екипа | ИД на клиент на MS Project | Синхронизиран | Несинхронизирано |
| Член на екипа | Име на позиция | Синхронизиран | Несинхронизирано |
| Член на екипа | проект | Синхронизиран | Синхронизиран |
| Член на екипа | Екип на проект | Синхронизиран | Синхронизиран |
| Член на екипа | Ресурсна единица | Несинхронизирано | Синхронизиран |
| Член на екипа | Роля | Несинхронизирано | Синхронизиран |
| Член на екипа | Работни часове | Несинхронизирано | Несинхронизирано |

### <a name="resource-assignment-entity-table"></a>Таблица на обекта за присвояване на ресурси
Следващата таблица описва как данните на Присвояване на ресурси се синхронизират между Project Service Automation и Micros

| **Обект** | **Поле** | **Microsoft Project към Project Service Automation** | **Project Service Automation към Microsoft Project** |
| --- | --- | --- | --- |
| Назначаване на ресурс | От дата | Синхронизиран | Несинхронизирано |
| Назначаване на ресурс | Часа | Синхронизиран | Несинхронизирано |
| Назначаване на ресурс | ИД на клиент на MS Project | Синхронизиран | Несинхронизирано |
| Назначаване на ресурс | Планирана работа | Синхронизиран | Несинхронизирано |
| Назначаване на ресурс | Project | Синхронизиран | Несинхронизирано |
| Назначаване на ресурс | Екип на проект | Синхронизиран | Несинхронизирано |
| Назначаване на ресурс | Назначаване на ресурс | Синхронизиран | Несинхронизирано |
| Назначаване на ресурс | Задача | Синхронизиран | Несинхронизирано |
| Назначаване на ресурс | Към днешна дата | Синхронизиран | Несинхронизирано |

### <a name="project-task-dependencies-entity-table"></a>Таблица на обектите на зависимост на проектната задача
Следващата таблица описва как данните на зависимост на проектната задача се синхронизират между Project Service Automation и Micros

| **Обект** | **Поле** | **Microsoft Project към Project Service Automation** | **Project Service Automation към Microsoft Project** |
| --- | --- | --- | --- |
| Зависимости на задачите от проекта | Зависимост на задачи от проект | Синхронизиран | Несинхронизирано |
| Зависимости на задачите от проекта | Тип на връзката | Синхронизиран | Несинхронизирано |
| Зависимости на задачите от проекта | Предшестваща задача | Синхронизиран | Несинхронизирано |
| Зависимости на задачите от проекта | Project | Синхронизиран | Несинхронизирано |
| Зависимости на задачите от проекта | Задача приемник | Синхронизиран | Несинхронизирано |

### <a name="additional-resources"></a>Допълнителни ресурси
 [Ръководство за мениджъри на проекти](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
