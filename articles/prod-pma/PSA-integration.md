---
title: Общ преглед на Project Service Automation
description: Тази тема предоставя информация за решението за интеграция на Dynamics 365 Project Service Automation в Dynamics 365 Finance.
author: ruhercul
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: ruhercul
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 5ca459b99881b612e4656be112c8a2e420b4196e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005868"
---
# <a name="project-service-automation-overview"></a>Общ преглед на Project Service Automation

[!include[banner](../includes/banner.md)]
[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Решението за интеграция на Project Service Automation в Finance използва функцията за интегриране на данни, за да синхронизира данните между екземплярите на Dynamics 365 Finance и Dynamics 365 Project Service Automation чрез Common Data Service. Шаблони за интеграция, които се предлагат с функцията за интеграция на данни, позволяват потока от проекти, договори на проект и аспекти на договор по проект, контролни точки на проект, задачи по проект, категории на трансакция на разходи, прогнози за часове, и прогнози за разходи прогнозни разходи за проекти от Project Service Automation към Finance.

> [!NOTE]
> - Ако използвате версия 7.3.0, трябва да инсталирате KB 4074835. След това ще можете да интегрирате проекти с фиксирана цена.
> - Ако използвате версия 7.3.0 и пренасяте транзакции с такси от Project Service Automation, трябва да инсталирате KB 4345320, за да включите тези такси във фактурата на проекта.
> - Ако използвате версия 8.0, ще можете да използвате интеграция на проектни задачи, категории транзакции, прогнози за часове, оценки на разходите и заключване на функционалността.
> - Ако използвате версия 8.0.1 или по-нова, ще можете да синхронизирате актуални данни.

Преди да можете да интегрирате Project Service Automation Finance, трябва да конфигурирате параметрите за интеграция на Project Service Automation. За повече информация вижте [Параметри на интеграция на Project Service Automation](PSA-parameters.md).

Това решение за интеграция позволява директна синхронизация в следните сценарии:

- Поддържайте договорите за проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.
- Създаване на проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.
- Поддържайте аспекти на договор за проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.
- Поддържайте контролни точки на аспекти на договор за проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.
- Поддържайте задачи на проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.
- Поддържайте категории на трансакции на разход във Finance и ги синхронизирайте директно от Finance в Project Service Automation.
- Създавайте прогнозни часове в проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.
- Създавайте прогнозни разходи на проекти в Project Service Automation и ги синхронизирайте директно от Project Service Automation към Finance.
- Създайте действителни данни за времето, разходите и таксите на проект в Project Service Automation и създайте транзакции на проекти в дневника за интеграция на Project Service Automation, така че те да могат да бъдат публикувани във Finance.

## <a name="data-synchronization"></a>Синхронизиране на данни

Следващата илюстрация показва как данните се синхронизират като част от интеграцията между Project Service Automation и Finance.

> [!NOTE]
> Понастоящем не са налични всички шаблони. Шаблоните ще бъдат пуснати, когато бъдат завършени.

[![Интеграция на Project Service Automation с Finance](./media/PSA-integration.png)](./media/PSA-integration.png)

## <a name="system-requirements-for-finance"></a>Системни изисквания за финанси

За да използвате решението за интегриране на Project Service Automation за финансиране, трябва да инсталирате Enterprise Edition 7.3 с актуализация на платформа 12 или по-нова.

## <a name="system-requirements-for-project-service-automation"></a>Системни изисквания за Project Service Automation

За да използвате решението за интегриране на Project Service Automation за финансиране, трябва да инсталирате следните компоненти:

- Dynamics 365 Project Service Automation версия 9.0.0.0 или по-нова
- Решение за перспектива за пари за Dynamics 365 Sales, версия 1.14.0.0 (v14) или по-нова версия
- Решение за Project Service Automation към Finance за Dynamics 365 Project Service Automation версия 1.0.0.0 или по-нова

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a>Инсталирайте решението за интеграция на Project Service Automation във Finance във вашия екземпляр на Project Service Automation

Изтеглете решението за интеграция на Project Service Automation във Finance от [Център за изтегляне на Microsoft](https://www.microsoft.com/download/details.aspx?id=57016) и следвайте инструкциите, приложени към решението.


[!INCLUDE[footer-include](../includes/footer-banner.md)]