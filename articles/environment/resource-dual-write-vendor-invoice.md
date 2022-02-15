---
title: Интегриране на фактуриране на доставчик
description: Тази тема предоставя информация за интегриране на фактуриране на доставчик в Project Operations.
author: sigitac
ms.date: 04/27/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 538a2694591f1d0d368ee0ffeed9bdf12cb47420c3d0571f75185fe433f23436
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/06/2021
ms.locfileid: "6986478"
---
# <a name="vendor-invoice-integration"></a>Интегриране на фактуриране на доставчик

_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_

Свързано с проекти осигуряване в Dynamics 365 Project Operations може да бъде записано, като отидете на **Задължения** > **Фактури** > **Чакащи фактури на доставчици** и използвате документ за изчакваща фактура на доставчик. За повече информация вижте [Закупете нескладовите материали, като използвате изчакваща фактура на доставчика](../procurement/pending-vendor-invoices.md).

> [!IMPORTANT]
> Преди да използвате функциите, описани в тази тема, прегледайте и приложете необходимите конфигурации. За повече информация вижте [Разрешаване на нескладовите материали и изчакващи фактура на доставчика](../procurement/configure-materials-nonstocked.md).

В Project Operations фактурите на доставчици, свързани с проекта, се публикуват, като се използват специални правила за осчетоводяване:

- Свързаните с проекта разходи (включително невъзстановими данъци) не се осчетоводяват веднага в сметката за разходите по проекта в главната книга. Вместо това цената се осчетоводява в **Сметка за интеграция на поръчки**. Този акаунт е конфигуриран в **Управление на проекти и счетоводство** > **Настройка** > **Управление на проекти и счетоводни параметри** в **Project Operations върху Dynamics 365 Customer engagement**.
- Двойното писане синхронизира данните за фактурите на доставчика с Microsoft Dataverse, като се използват следните таблични карти:

     - **Обект за експортиране на фактура на доставчик на проект за Project Operations (msdyn_projectvendorinvoices)**: Тази таблична карта синхронизира информацията за заглавието на фактура на доставчика. В Dataverse се синхронизират се само фактури на доставчици с поне един ред, който съдържа идентификатор на проект.
     - **Обект за експортиране на ред на фактура на доставчик на проект за Project Operations (msdyn_projectvendorinvoicelines)**: Тази таблична карта синхронизира информацията за заглавието на ред на фактура на доставчика. В Dataverse се синхронизират се само редове, които съдържат идентификатор на проект.

     > [!NOTE]
     > Подробности за фактура на доставчика в Dataverse не могат да се редактират.

Данъчен вторичен журнал, вторичен журнал на доставчик и други финансови осчетоводявания се записват, както е приложимо в Dynamics 365 Finance към момента на публикуване на фактура на доставчик.

![Интегриране на фактуриране на доставчик.](media/DW7VendorInvoice.png)

Когато записите се записват в обект **Фактура на продавач** в Dataverse, започва автоматизиран процес на одобрение на записите. Ако е необходимо, състоянието на автоматизирания процес на одобрение може да бъде прегледано чрез Dataverse, като отидете на **Разширени настройки** > **Система** > **Системни задачи**. След като одобрението приключи, системата създава записи на класа на транзакция на материал в обекта **Действителни данни**.

След това действителните факти, свързани с материали, се обработват с помощта на картата на таблица с двойно записване **Действителни данни за интеграция на Project Operations (msdyn_actuals)**. За повече информация вижте [Прогнозни оценки и действителни данни](resource-dual-write-estimates-actuals.md).

Периодичният процес **Импортиране от постановка** създава редове на журнал за интеграция на Project Operations, свързани с отчета на доставчик. Акаунтът за компенсиране е по подразбиране акаунтът за интегриране на осигуряването. Когато се публикува журнал за интегриране, салдо по сметка се изчиства за транзакцията на фактура на доставчик и сумата на реда се премества в сметката за разходи по проекта. Създават се също трансакции на вторичен журнал за целите на фактурирането и признаването на приходите.