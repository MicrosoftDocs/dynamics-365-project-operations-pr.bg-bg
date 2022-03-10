---
title: Интеграция на двойно записване на Project Operations
description: Тази тема предоставя преглед на интеграцията с двойно писане на Project Operations.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.custom: intro-internal
ms.openlocfilehash: b65c40e8aaa9524c1c634738dadd23f21e86e2ec095c47bc849467c8806addbc
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/06/2021
ms.locfileid: "7007898"
---
# <a name="project-operations-dual-write-integration-overview"></a>Общ преглед на интеграция на двойно записване на Project Operations

_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_

Project Operations използва [възможности за двойно писане](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) за синхронизиране на данни между Microsoft Dataverse и Dynamics 365 Finance.

Следващата илюстрация показва как данните се синхронизират като част от тази интеграция между Dataverse и Finance.

![Преглед на потоците от данни за Project Operations.](./media/ProjectOperationsFlows.jpg)

Project Operations на Dataverse осигурява модерен потребителски интерфейс (UI) и лесна разширяемост без код/малко код с помощта на възможности на Power Platform. Мениджърите на проекти, мениджърите на ресурси, членовете на екипа на проекта и други лица от фронт офиса изпълняват своите дейности в Project Operations на Dataverse.

Project Operations във Finance предоставя подкрепа за счетоводство на проекти и признаване на приходи. Project Operations се включва във финансовата рамка във Finance за изчисляване на данък върху продажбите, валутни курсове, отчитане на финансовите измерения и др. Опитът на счетоводителя по проекта се базира предимно на Finance.

Интеграцията на Project Operations се състои от следната интеграция на компоненти:


- [Интегриране на данни за настройка и конфигурация на Project Operations](resource-dual-write-setup-integration.md) 
- [Проектни оценки и действителни данни](resource-dual-write-estimates-actuals.md)
- [Фактури по проект](resource-dual-write-project-invoice.md)
- [Управление на разходите](resource-dual-write-expense.md)
- [Фактура от доставчик](resource-dual-write-vendor-invoice.md)
