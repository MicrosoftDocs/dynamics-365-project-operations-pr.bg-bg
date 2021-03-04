---
title: Прилагане на демонстрационни данни за настройка и конфигурация – олекотено
description: Тази тема предоставя информация за това как да приложите демонстрационни данни за настройка конфигурационни в Project Operations.
author: sigitac
manager: Annbe
ms.date: 01/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 762b0cf317d442565a033f56033a53a5b5cc435c
ms.sourcegitcommit: b4298ca4729643c1040ef35dde8c67f829461ce7
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/29/2021
ms.locfileid: "5089106"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a>Прилагане на демонстрационни данни за настройка и конфигурация за Project Operations – олекотено 

_**Леко внедряване – фактуриране на сделка към проформа_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a>Предварителни изисквания

Преди да започнете конфигурацията, трябва да имате среда на Common Data Service (CDS), осигурена за Dynamics 365 Project Operations.


## <a name="instructions"></a>Инструкции

1. Изтеглете [Пакет с основни данни](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip). 
2. Придвижете се до папката *ProjOpsDemoDataSetupAndMaster - Integrated CMT* и стартирайте изпълнимия файл *DataMigrationUtility*.
3. На страница 1 на Common Data Service Съветник за миграция на конфигурация (CMT), изберете **Импортиране на данни** и след това изберете **Продължение**.

    ![Мигриране на конфигурация](./media/1ConfigurationMigration.png)

4. На страница 2 от съветника за CMT изберете **Microsoft 365** като **Тип на внедряване**.
5. Изберете квадратчета за отметка **Показване на списък с наличните организации** и **Показване на напреднали**.
6. Изберете региона на вашия наемател, въведете вашите идентификационни данни и след това изберете **Вход**.

   ![Вход в конфигурация](./media/2ConfigurationSignin.png)

7. На страница 3 от списъка с организации на клиента изберете организацията, в която искате да импортирате демонстрационните данни, и изберете **Вход**.
8. На страница 4 изберете zip файла *MasterAndSetupData* от разопакованата папка *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.

   ![Zip файл](./media/3ZipFile.png)

   ![Избор на файл](./media/4SelectAFile.png)

9. След като изберете zip файла, изберете **Импортиране на данни**.

   ![Импортиране на данни](./media/5ImportData.png)

10. Импортирането ще продължи приблизително две-десет минути в зависимост от скоростта на вашата мрежа. След като завърши, излезте от съветника за CMT. 
11. Проверете вашата организация за данни в следните 20 обекта:

    -   Валута
    -   Клиент
    -   Организационна единица
    -   Контакт
    -   Единица
    -   Опаковъчна единица
    -   Ценова листа
    -   Ценова листа на параметър на проекта 
    -   Честота на фактура
    -   Категория налични ресурси
    -   Категория на трансакция
    -   Категория на разхода
    -   Цена на роля
    -   Цена на категория транзакция
    -   Характеристика
    -   Наличен ресурс
    -   Асоциация на категория налични ресурси
    -   Характеристика на наличен ресурс

    ![Пълно импортиране](./media/6CompleteImport.png)
