---
title: Използване на добавката за Project Service за планиране на работата в Microsoft Project | MicrosoftDocs
description: Тази тема предоставя информация за това как да добавите, конфигурирате и използвате добавката Microsoft Project за Microsoft Project Service.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
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
ms.openlocfilehash: e85b3e0e13bb48aeb9eeb111c2f782f4d62505a7
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014508"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a>Използвайте добавката Project Service Automation за планиране на работата в Microsoft Project

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ви улеснява при извършване на планирането на проекти, включително прогнози. Можете да определите работата, така че да са ясни разходите, усилията и стойността на продажбите при подаване на окончателното предложение.  

 Сега можете да инсталирате [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] и да извършите работата по планирането в познатата среда на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]. Използвайте стабилните възможностите за планиране и управление на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и след това актуализирайте плана на проекта в Project Service Automation.  

> [!IMPORTANT]
> - За да използвате управлението на документи на SharePoint за съхранение на файловете на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] за проекти на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], администраторът на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] трябва да включи управлението на документи. 
> - [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] е съвместим само с [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.  

## <a name="download-and-install-the-add-in"></a>Изтеглете и инсталирайте добавката  
 Подгответе информацията за регистрация в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Тази информация ви е необходима, за да се свържете от [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] с [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

1.  От центъра за изтегляния изтеглете добавката за вашата поддържана версия на Project Service – [v2.X](https://go.microsoft.com/fwlink/?linkid=828268) или [v 3.4+](https://www.microsoft.com/download/details.aspx?id=57956).  

2.  Щракнете върху връзката за изтегляне.  

3.  Когато изтеглянето приключи, щракнете върху **Да** за инсталиране на добавката.  

## <a name="configure-the-add-in"></a>Конфигуриране на добавката  

1. Отворете [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и щракнете върху раздел **Project Service**.  

2. Щракнете върху **свързване**.  

3. Въведете информацията си за влизане и след това щракнете върху **Влизане**.  

   Вече можете да започнете да използвате добавката.  

## <a name="read-from-a-template"></a>Четене от шаблон  
 Четете от шаблон, който сте създали в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] и сте копирали в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], за да започнете да планирате своя проект. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Създаване на шаблон на проект (Project Service Automation)](../psa/create-project-template.md)  

1.  От раздела **Project Service** щракнете върху **Четене** > **Шаблон на проект на Project Service Automation**.  

2.  Изберете шаблон на проект от списъка и след това щракнете върху **Отвори**.  

    > [!NOTE]
    >  По подразбиране задачите, които са копирани от шаблона в проекта, са зададени като ръчно планирани.  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a>Присвояване на роли на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] на ресурси на проекти  

1.  Отворете проект и щракнете върху лентата **Задача**.  

2.  Щракнете върху менюто **Диаграма на Гант** и след това изберете **Лист на ресурсите**.  

3.  В листа на ресурсите, щракнете върху падащото меню **Роля на ресурс в Project Service** и изберете роля в Project Service Automation.  

## <a name="staff-your-project-with-resources"></a>Осигурете ресурси за проекта си  

1.  От раздела Project Service изберете ред и щракнете върху **Търсене на ресурси**.  

2.  На екрана **Резервиране на ресурс** изберете ресурса, който искате да използвате за проекта.  

3.  Щракнете върху **Резервирай** и след това щракнете върху **OK**.  

## <a name="publish-your-project"></a>Публикуване на вашия проект  
Когато приключи планирането на проекта, следващата стъпка е импортиране и публикуване на проекта в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

Проектът ще се импортира в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Прилагат се ценообразуването и процесът на генериране на екип. Отворете проекта в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], за да проверите, че са генерирани екипът, оценките на проекта и съставната структура на работата. В таблицата по-долу е показано къде да се намерят резултатите:


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Диаграма на Гант**   | Импортиране в екрана на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Съставна структура на работата**. |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Списък с ресурси** |   Импортиране в екрана на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Членове на екипа на проект**.   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Използване на употреба**    |    Импортира в екрана на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Оценки на проект**.     |

**За да импортирате и публикувате проекта**  
1. От раздела **Project Service** щракнете върху **Публикуване** > **Нов проект на Project Service Automation**.  

2. На диалоговия прозорец **Публикуване в нов проект в Project Service** въведете **Име на проект** и изберете **Клиент**.  

3. По желание проверете **Свързване на плана на проекта с Project Service Automation**, за да се свърже файлът на плана на проекта с Project Service Automation.  

4. Щракнете върху **Публикуване**.  

   Свързването на файла на проекта с [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] прави файла на проекта главен и задава съставната структура на работата в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] като само за четене.  За да направите промени в плана на проекта, трябва да ги направите в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да ги публикувате като актуализации в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

## <a name="edit-a-project-thats-been-imported"></a>Редактиране на проект, който е импортиран  
 За да направите промени на план на проект, който е импортиран в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], имате две опции:  

- Отваряне на главния файл и редактиране в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

- Премахване на връзката на файла и редактиране директно в Project Service. По подразбиране проект, който е качен от [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], е заключен и може да се редактира само в проекта. За да редактирате файла в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], връзката на файла трябва да се премахне.  

### <a name="edit-in-pn_microsoft_project"></a>Редактиране в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]  

1. От главното меню щракнете върху **Project Service** > **Проекти**.  

2. От списъка с проекти отворете този, който сте създали в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. Щракнете върху **Отвори в MS Project** от лентата. Така ще се отвори свързаният главен файл в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a>Премахване на връзката на файл и редактиране в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service  

1. От главното меню щракнете върху **Project Service** > **Проекти**.  

2. От списъка с проекти отворете този, който сте създали в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. Щракнете върху **Премахни връзката с MS Project** от лентата.  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a>Качване на файл на проект в SharePoint или групи на Office  
 Можете да качите файла на проекта си в SharePoint и да го намерите под „Свързани документи” за проекта на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  Администраторът трябва да конфигурира управление на документи на SharePoint и да го включи за обекта на проекта. 

 Също така можете да качите файла на проекта на [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)], ако имате зададени групи на Office.

### <a name="upload-a-file-for-sharepoint"></a>Качване на файл за SharePoint  

1. От главното меню щракнете върху **Project Service** > **Качване**.  

2. Изберете **Към документи на проект в Project Service Automation**.  

3. В диалоговия прозорец **Разрешаване на отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** изберете **Да** или **Не**.  

   - Ако щракнете върху **Да**, ще можете да изберете бутона **Отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** в Project Service Automation, да стартирате [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да заредите файла на проекта от библиотеката с документи на SharePoint.  

   - Ако щракнете върху **Не**, връзката за бутона **Отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** няма да работи.  

4. Файлът на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] може да се намери в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] под **Документи** за конкретния проект на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

### <a name="upload-a-file-for-office-groups"></a>Качване на файл за групи на Office  

1. От главното меню щракнете върху **Project Service** > **Качване**.  

2. Изберете **Към документи на проект в Project Service Automation**.  

3. В диалоговия прозорец **Разрешаване на отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** изберете **Да** или **Не**.  

   - Ако щракнете върху **Да**, ще можете да изберете бутона **Отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** в Project Service Automation, да стартирате [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да заредите файла на проекта от библиотеката с документи на SharePoint.  

   - Ако щракнете върху **Не**, връзката за бутона **Отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** няма да работи.  

4. Файлът на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] може да се намери в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] под **Документи** за конкретния проект на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

## <a name="publish--your-project-as-a-template"></a>Публикуване на вашия проект като шаблон  
 Можете да запишете проекта си и да го използвате отново, като го запишете като шаблон на проект в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  Шаблоните на проекти са планове на проекти за многократна употреба в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Създаване на шаблон на проект (Project Service Automation)](../psa/create-project-template.md)  

1. От раздела **Project Service** щракнете върху **Публикуване** > **Нов шаблон на проект на Project Service Automation**.  

2. На диалоговия прозорец **Публикуване в нов проект в шаблон на Project Service** въведете **Име на шаблона на проект**.  

3. По желание проверете **Свързване на плана на проекта с Project Service Automation**, за да се свърже файлът на проекта с [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

4. Щракнете върху **Публикуване**.  

Свързването на файла на проекта с [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] прави файла на проекта главен и задава съставната структура на работата в шаблона на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] само за четене.  За да направите промени в плана на проекта, трябва да ги направите в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да ги публикувате като актуализации в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].

## <a name="read-a-resource-loaded-schedule"></a>Четене на график, зареден с ресурс

Когато четете проект от Project Service Automation, календарът на ресурса не се синхронизира с настолния клиент. Ако има разлики в продължителността, усилията или края на задачата, вероятно причината е, че ресурсите и настолният клиент нямат един и същи календар с шаблон за работно време, приложен към проекта.


## <a name="data-synchronization"></a>Синхронизиране на данни

Следващата таблица описва как данните се синхронизират между Project Service Automation и добавката за настолни компютри на Microsoft Project.

| **Обект** | **Поле** | **Microsoft Project към Project Service Automation** | **Project Service Automation към Microsoft Project** |
| --- | --- | --- | --- |
| Задача по проект | Краен срок | ● | - |
| Задача по проект | Очаквано усилие | ● | - |
| Задача по проект | ИД на клиент на MS Project | ● | - |
| Задача по проект | Родителска задача | ● | - |
| Задача по проект | Project | ● | - |
| Задача по проект | Задача от проект | ● | - |
| Задача по проект | Име на задача от проект | ● | - |
| Задача по проект | Ресурсна единица (отхвърлено във версия 3.0) | ● | - |
| Задача по проект | Планирано времетраене | ● | - |
| Задача по проект | Начална дата | ● | - |
| Задача по проект | ИД на ССР | ● | - |

| **Обект** | **Поле** | **Microsoft Project към Project Service Automation** | **Project Service Automation към Microsoft Project** |
| --- | --- | --- | --- |
| Член на екипа | ИД на клиент на MS Project | ● | - |
| Член на екипа | Име на позиция | ● | - |
| Член на екипа | проект | ● | ● |
| Член на екипа | Екип на проект | ● | ● |
| Член на екипа | Ресурсна единица | - | ● |
| Член на екипа | Роля | - | ● |
| Член на екипа | Работни часове | Несинхронизирани | Несинхронизирани |

| **Обект** | **Поле** | **Microsoft Project към Project Service Automation** | **Project Service Automation към Microsoft Project** |
| --- | --- | --- | --- |
| Назначаване на ресурс | От дата | ● | - |
| Назначаване на ресурс | Часа | ● | - |
| Назначаване на ресурс | ИД на клиент на MS Project | ● | - |
| Назначаване на ресурс | Планирана работа | ● | - |
| Назначаване на ресурс | Project | ● | - |
| Назначаване на ресурс | Екип на проект | ● | - |
| Назначаване на ресурс | Назначаване на ресурс | ● | - |
| Назначаване на ресурс | Задача | ● | - |
| Назначаване на ресурс | До дата | ● | - |

| **Обект** | **Поле** | **Microsoft Project към Project Service Automation** | **Project Service Automation към Microsoft Project** |
| --- | --- | --- | --- |
| Зависимости на задачите от проекта | Зависимост на задачи от проект | ● | - |
| Зависимости на задачите от проекта | Тип на връзката | ● | - |
| Зависимости на задачите от проекта | Предшестваща задача | ● | - |
| Зависимости на задачите от проекта | Project | ● | - |
| Зависимости на задачите от проекта | Задача приемник | ● | - |

### <a name="see-also"></a>Вижте също  
 [Ръководство за мениджъри на проекти](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]