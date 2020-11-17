---
title: Синхронизирайте проектните задачи директно от Project Service Automation с Finance and Operations
description: Тази тема описва шаблона и основните задачи, които се използват за синхронизиране на прогнозни часове на задачи за проект директно от Microsoft Dynamics 365 Project Service Automation във Dynamics 365 Finance.
author: Yowelle
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 0383607a07def6c21562bf4b0893fe3ce3db6a04
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071802"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a>Синхронизирайте проектните задачи директно от Project Service Automation с Finance and Operations

[!include[banner](../includes/banner.md)]

Тази тема описва шаблона и основните задачи, които се използват за синхронизиране на прогнозни часове на задачи за проект директно от Dynamics 365 Project Service Automation във Dynamics 365 Finance.

> [!NOTE]
> - Интеграция на проектни задачи, категории транзакции, прогнози за часове, оценки на разходите и заключване на функционалността е налична във версия 8.0.
> - Ако използвате Enterprise Edition 7.3.0, след като инсталирате KB 4132657 и KB 4132660, ще можете да използвате шаблоните за интегриране на проектни задачи, категории на транзакционни транзакции, часови прогнози, прогнозни разходи и актуални данни и да конфигурирате заключване на функционалността. Ако трябва да нулирате счетоводните разпределения, препоръчваме да инсталирате и KB 4131710.
> - Интегрирането на действителни данни е достъпно от версия 8.0.1.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Поток от данни за Project Service Automation към Finance

Решението за интеграция на Project Service Automation to Finance използва функцията за интегриране на данни, за да синхронизира данните между копията на Project Service Automation и Finance. Шаблонът за интеграция, които се предлагат с функцията за интеграция на данни, позволяват потока от данни за задачи на проекта от Project Service Automation към Finance.

Следващата илюстрация показва как данните се синхронизират между Project Service Automation и Finance.

[![Поток от данни за интеграция на Project Service Automation с Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)

## <a name="template-and-task"></a>Шаблони и задача

За достъп до шаблона, в администраторски център на Microsoft Power Apps, изберете **Проекти** и след това в горния десен ъгъл изберете **Нов проект** , за да изберете публични шаблони.

Следният шаблон и основна задача се използват за синхронизиране на задачи на проекта от Project Service Automation към Finance:

- **Име на шаблона в Интегриране на данни:** Задачи на проект (PSA до Fin и Ops)
- **Име на задача в проекта:** Задачи на проекта

Преди да може да се случи синхронизиране на задачи на проект, трябва да синхронизирате договорите на проект и проектите.

## <a name="entity-set"></a>Набор от обекти

| Project Service Automation | Finance                             |
|----------------------------|-------------------------------------|
| Задачи от проекти              | Интеграционен обект за задача на проект |

## <a name="entity-flow"></a>Поток на обекта

Задачите по проект за часовете на проекта се управляват в Project Service Automation и се синхронизират с Finance като дейности на проект.

## <a name="prerequisites-and-mapping-setup"></a>Предпоставки и настройка на картографиране

Преди да може да се случи синхронизиране на задачи на проект, трябва да синхронизирате договорите на проект и проектите.

## <a name="power-query"></a>Power Query

Трябва да използвате Microsoft Power Query за Excel, за да филтрирате данни, ако това условие е изпълнено:

- Имате специфични за ресурсите записи в проектна задача.

Ако трябва да използвате Power Query, следвайте това указание:

- Шаблонът за проектни задачи (PSA до Fin и Ops) има филтър по подразбиране, който изключва специфични за ресурсите записи от проектна задача, като зададе филтъра на **IsLineTask** на **Невярно**. Ако създадете свой собствен шаблон, трябва да добавите този филтър.

## <a name="template-mapping-in-data-integration"></a>Съпоставяне на шаблони при интеграция на данни

Следващата илюстрация показва пример за съпоставяния на задача на шаблон при интеграция на данни. Картографирането показва информация за полето, която ще бъде синхронизирана от Project Service Automation към Finance.

[![Съпоставяне на шаблони](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)