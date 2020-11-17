---
title: Синхронизирайте категориите разходи за проекти между Finance and Operations и Project Service Automation
description: Тази тема описва шаблон и основните задачи, които се използват за синхронизиране на категории на разход по проект между Microsoft Dynamics 365 Finance и Dynamics 365 Project Service Automation.
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
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: ed7ca3c85d3f99b7eefe10f4ddec822b9aeb1684
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071959"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a>Синхронизирайте категориите разходи за проекти между Finance and Operations и Project Service Automation

[!include[banner](../includes/banner.md)]

Тази тема описва шаблон и основните задачи, които се използват за синхронизиране на категории на разход по проект между Dynamics 365 Finance и Dynamics 365 Project Service Automation.

> [!NOTE]
> - Интеграция на проектни задачи, категории транзакции, прогнози за часове, оценки на разходите и заключване на функционалността е налична във версия 8.0.
> - Интегрирането на действителни данни е достъпно от версия 8.0.1.
> - Ако използвате Enterprise Edition 7.3.0, след като инсталирате KB 4132657 и KB 4132660, ще можете да използвате шаблоните за интегриране на проектни задачи, категории на транзакционни транзакции, часови прогнози, прогнозни разходи и актуални данни и да конфигурирате заключване на функционалността. Ако трябва да нулирате счетоводните разпределения, препоръчваме да инсталирате и KB 4131710.

## <a name="data-flow-for-project-service-automation-and-finance"></a>Поток от данни за Project Service Automation и Finance

Решението за интеграция на Project Service Automation и Finance използва функцията за интегриране на данни, за да синхронизира данните между копията на Project Service Automation и Finance. Шаблоните за интеграция, които се предлагат с функцията за интеграция на данни, позволяват потока от данни за категории на трансакция на прогнозни часови прогнози на проекта и прогнозни разходи за проекти между Project Service Automation и Finance.

Ако категориите проектни разходи са усвоени във Finance, интеграционният поток е първо от Finance към Project Service Automation. Идентификационните идентификатори на категориите на разходите по проекта след това се актуализират чрез синхронизиране от Project Service Automation към Finance.

Ако категориите проектни разходи са усвоени в Project Service Automation, интеграционният поток е първо от Project Service Automation към Finance. Категориите на проектите вече трябва да бъдат конфигурирани във Finance преди синхронизирането от Project Service Automation. След това синхронизирайте от Finance обратно към Project Service Automation и след това от Project Service Automation към Finance отново. По този начин помагате да гарантирате, че категориите са свързани и че не се създават дубликати.

> [!NOTE]
> Обикновено категориите разходи за проекти се усвояват във Finance. Ако обаче не са или ако категориите разходи вече са създадени в Project Service Automation, първо трябва да синхронизирате с помощта на шаблона за категории транзакции на категории на проекта (PSA към Fin и Ops). След това синхронизирайте, като използвате шаблона за категории транзакции на проекта (Fin и Ops към PSA). След това трябва да стартирате синхронизирането от Project Service Automation към Finance още веднъж.
>
> Ако първо синхронизирате от Project Service Automation, трябва да бъдат изпълнени следните изисквания във Finance, преди да се стартира синхронизацията:
>
> - Споделената категория, която съответства на категорията на проекта, която е настроена в Project Service Automation, трябва да съществува и трябва да бъде активирана и за двете **Проект** и **Разход**.
> - За всяко юридическо лице по финанси, с което трябва да се интегрира, трябва да съществуват следните категории проекти:
>
>     - **Категория на проекта** съществува. 
>     - **Използвайте в разходи** е активирано.
>     - **Активен в журнала** е активирано.
>     - **Тип транзакция** е зададено на **Разход**.

Следващата илюстрация показва как данните се синхронизират между Project Service Automation и Finance.

[![Поток от данни за интеграция на Project Service Automation с Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a>Синхронизиране на категория на разход по проекта между Finance и Project Service Automation

### <a name="template-and-task"></a>Шаблони и задача

За достъп до шаблона, в администраторски център на Microsoft Power Apps, изберете **Проекти** и след това в горния десен ъгъл изберете **Нов проект** , за да изберете публични шаблони.

Следният шаблон и основните задачи се използват за синхронизиране на категории на разходи на проекта от Finance към Project Service Automation:

- **Име на шаблона в Интегриране на данни:** Категории на трансакция на разходи по проект (Fin и Ops към PSA)
- **Име на задачата в проекта:** Синхронизирайте категории с PSA

### <a name="entity-set"></a>Набор от обекти

| Finance                           | Project Service Automation |
|-----------------------------------|----------------------------|
| Интеграционен обект за категории | Категории трансакция     |

### <a name="entity-flow"></a>Поток на обекта

Категориите на разходи на проекта се управляват във Finance и се синхронизират с Project Service Automation като категории на трансакция.

### <a name="power-query"></a>Power Query

Когато синхронизирате с Project Service Automation, трябва да използвате Microsoft Power Query за Excel, за да зададете типа на таксуване в категорията на транзакциите. Категориите на транзакционните категории на проекта (Fin и Ops към PSA) предоставят колона и картографиране по подразбиране. Ако създадете свой собствен шаблон, трябва да добавите тази условна колона в Power Query. Следвайте тези стъпки.

1. Щракнете върху стрелката, за да отворите задачата за картографиране на категорията на разходите за проекта в шаблона за категории на транзакции за проект (Fin и Ops към PSA).
2. Щракнете върху връзката **Разширени заявки и филтриране** , за да отворите Power Query.
2. Изберете **Добавете условна колона**.
3. Въведете име за новата колона, като например **BillingType**.
4. Въведете следното условие: **ако CATEGORYID не е равно на нула, тогава 19235001, в противен случай е нула**.
5. Щракнете върху **OK** на колоната.
6. Не забравяйте да картографирате тази нова колона на страницата за картографиране.

Следващата илюстрация показва пример за съпоставяне на задача на шаблон при интеграция на данни. Картографирането показва информация за полето, която ще бъде синхронизирана от Finance в Project Service Automation.

[![Съпоставяне на шаблон за категория на разход по проекта и Project Service Automation](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a>Синхронизиране на категория на разход по проекта между Finance и Project Service Automation

### <a name="template-and-task"></a>Шаблони и задача

Следният шаблон и основните задачи се използват за синхронизиране на категории на разходи на проекта от Project Service Automation към Finance:

- **Име на шаблона в Интегриране на данни:** Категории на трансакция на разходи по проект (PSA към Fin и Ops)
- **Име на задачата в проекта:** Синхронизирайте категории с Fin Ops

### <a name="entity-set"></a>Набор от обекти

| Project Service Automation | Finance                           |
|----------------------------|-----------------------------------|
| Категории трансакция     | Интеграционен обект за категории |

### <a name="entity-flow"></a>Поток на обекта

Категориите на разходи на проекта се управляват във Finance и се синхронизират с Project Service Automation като категории на трансакция. Обратната синхронизация с актуализации на Finance в категорията ба проект във Finance с ИД на интеграция от Project Service Automation.

### <a name="template-mapping-in-data-integration"></a>Съпоставяне на шаблони при интеграция на данни

Следващата илюстрация показва пример за съпоставяне на задача на шаблон при интеграция на данни.

> [!NOTE]
> Картографирането показва информация за полето, която ще бъде синхронизирана от Project Service Automation към Finance.

[![Съпоставяне на Project Service Automation с шаблон на Finance](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)