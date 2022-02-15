---
title: Интегриране на фактуриране по проект
description: Тази тема предоставя информация за интеграция на двойно записване на Project Operations за фактуриране на клиенти.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 37549080d76e3bffd7cb002aee8e3c46b9eeb18e3cec915cd971881b69747534
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/06/2021
ms.locfileid: "6993228"
---
# <a name="project-invoice-integration"></a>Интегриране на фактуриране по проект

Тази тема предоставя информация за интеграция на двойно записване на Project Operations за фактуриране на клиенти.

В Project Operations мениджърът на проекта управлява натрупването на фактури по проекта и създава проформа фактура за клиента в Microsoft Dataverse. Въз основа на тази проформа фактура, чиновникът по сметките или счетоводителят на проекта създава фактура, ориентирана към клиента. Интеграцията с двойно записване гарантира, че данните за проформа фактурата са синхронизирани с приложения на Finance and Operations. След като се публикува фактура, ориентирана към клиентите, системата актуализира съответните фактически проекти в Dataverse със счетоводната подробност. Следващата графика предоставя концептуален преглед на тази интеграция на високо ниво.

   ![Интегриране на фактуриране по проект.](./media/DW5Invoicing.png)

След като ръководителят на проекта потвърди проформа фактурата в Dataverse, информацията за заглавката на проформа фактура се синхронизира с приложения на Finance and Operations, използващи карта на таблицата с двойно писане, **Предложение за фактура по проект V2 (фактури)**. Това е еднопосочна интеграция от Dataverse в приложения на Finance and Operations. Създаване или изтриване на предложения за фактури по проекта директно в приложения на Finance and Operations не се поддържа.

Потвърждение на фактура в Dataverse също задейства бизнес логиката за създаване на записи, свързани с фактуриране в обекта **Действителни данни**. Тези записи се синхронизират с приложения на Finance and Operations, използващи таблица с двойно записване **Действителни данни за интеграция на Project Operations (msdyn\_actuals)**. За повече информация вижте [Прогнозни оценки и действителни данни](resource-dual-write-estimates-actuals.md). 

Редовете за предложения за фактури по проекта се създават чрез периодичния процес, **Поставяне на формуляр за импортиране**. Този процес се основава на подробностите за действителните фактурирани продажби в таблицата **Реални постановки**. За повече информация вижте [Управлявайте предложения за фактури по проекта](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 