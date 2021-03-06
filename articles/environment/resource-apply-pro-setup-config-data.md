---
title: Настройка и прилагане на конфигурационни данни в Common Data Service за Project Operations
description: Тази тема предоставя информация за настройка и прилагане на конфигурационни данни в Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d99ab4c7b2ebf6ba56b86a3e0151036c6247e484
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948750"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service-for-project-operations"></a>Настройка и прилагане на конфигурационни данни в Common Data Service за Project Operations

_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_

## <a name="install-setup-and-configuration-data"></a>Първоначална настройка и данни за конфигурация

1. Изтеглете, деблокирайте и разархивирайте [Пакет за данни за настройка и конфигуриране](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).
2. Придвижете се до разархивираната папка и стартирайте изпълнимия файл, *DataMigrationUtility*.
3. На страница 1 на Common Data Service Съветник за миграция на конфигурация (CMT), изберете **Импортиране на данни** и след това изберете **Продължение**.

![Мигриране на конфигурация](./media/1ConfigurationMigration.png)

4. На страница 2 от съветника за CMT изберете **Office 365** като **Тип на внедряване**.
5. Изберете квадратчета за отметка **Показване на списък с наличните организации** и **Показване на напреднали**.
6. Изберете региона на вашия наемател, въведете вашите идентификационни данни и изберете **Вход**.

![Вход в конфигурация](./media/2ConfigurationSignin.png)

7. На страница 3 от списъка с организации на наемателя изберете организацията, в която искате да импортирате демонстрационните данни, и изберете **Вход**.
8. На страница 4 изберете zip файла, *SampleSetupAndConfigData* от разопакованата папка.

![Избор на Zip файл](./media/3ZipFile.png)

![Избор на файл](./media/4SelectAFile.png)

9. След като изберете zip файла, изберете **Импортиране на данни**.

![Импортиране на данни](./media/5ImportData.png)

10. Импортирането ще продължи приблизително две-десет минути в зависимост от скоростта на вашата мрежа. След като импортирането завърши, излезте от съветника за CMT. 
11. Проверете вашата организация за данни в следните 19 обекта:

  - Валута
  - Организационна единица
  - Контакт
  - Данъчна група
  - Клиентска група
  - Единица
  - Опаковъчна единица
  - Ценова листа
  - Ценова листа на параметър на проекта
  - Честота на фактура
  - Категория налични ресурси
  - Категория на трансакция
  - Категория на разхода
  - Цена на роля
  - Цена на категория транзакция
  - Характеристика
  - Наличен ресурс
  - Асоциация на категория налични ресурси
  - Характеристика на наличен ресурс

![Пълно импортиране](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a>Актуализиране на конфигурациите на Project Operations

1. Навигиране до средата на CE. Можете да я намерите, като отворите [Административен център на Power Platform](https://admin.powerplatform.microsoft.com/environments), изберете среда и след това изберете **Отворена среда**. 

![Отваряне на средата](./media/7OpenEnvironment.png)

2. Отидете на **Проекти** > **Ресурси** и след това изберете **Създаване**, за да създадете резервируем ресурс за вашия потребител.

![Налични ресурси](./media/8BookableResources.png)

3. На раздела **Общи** изберете своя администратор. Уверете се, че часовата зона съвпада с тази, в която се намирате. 

![Нов наличен ресурс](./media/9NewBookableResource.png)

4. В раздела **Планиране** в полето **Фирма** изберете фирмата **USPM** и след това изберете **Записване**. 

![Раздел за планиране](./media/10SchedulingTab.png)

5. Изберете раздела **Работни часове**.  

![Работно време](./media/11WorkHours.png)

6. Щракнете двукратно върху която и да е стойност в календара и изберете **редактиране** > **Всички събития от поредицата**. 

![Работен календар](./media/12WorkCalendar.png)

7. Сменете работното време на осем (8) работен ден, маркирайте почивните дни като неработни дни и се уверете, че часовата зона съвпада с вашата. 
8. Изберете **Записване и затваряне**.

![Актуализиране на календар](./media/13UpdateCalendar.png)

9. Отидете на **Настройки** > **Шаблони на календара** и изберете **Създаване**.
 
 ![Шаблони на календар](./media/14CalendarTemplates.png)
 
 10. Въведете име, изберете ресурса на шаблона, който сте създали, и след това изберете **Записване**. 
 
 ![Записване на Шаблон на календар](./media/15SaveCalendarTemplate.png)
 
 11. Отидете на **Параметри** и щракнете двукратно върху записа. 
 
 ![Параметри на проекта](./media/16ProjectParameters.png)
 
12. Актуализирайте следните полета:

 - **Фирма по подразбиране**: USPM
 - **Организационна единица по подразбиране**: Contoso Robotics Global
 - **Честота на фактурите**: Седми и последен ден
 - **Шаблон за работен час**: Преминете към шаблона, който сте създали.

13. Изберете **Записване**. 

![Актуализирани параметри на проекта](./media/17UpdatedProjectParameters.png)
