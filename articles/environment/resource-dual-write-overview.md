---
title: Интеграция на двойно записване на Project Operations
description: Тази тема предоставя преглед на интеграцията с двойно писане на Project Operations.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ce4f7bf8185e6f3f942df14d30d7b8d0a3e4444a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998668"
---
# <a name="project-operations-dual-write-integration-overview"></a><span data-ttu-id="9b90c-103">Общ преглед на интеграция на двойно записване на Project Operations</span><span class="sxs-lookup"><span data-stu-id="9b90c-103">Project Operations dual-write integration overview</span></span>

<span data-ttu-id="9b90c-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="9b90c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="9b90c-105">Project Operations използва [възможности за двойно писане](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) за синхронизиране на данни между Microsoft Dataverse и Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="9b90c-105">Project Operations uses [dual-write capabilities](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) to synchronize data across Microsoft Dataverse and Dynamics 365 Finance.</span></span>

<span data-ttu-id="9b90c-106">Следващата илюстрация показва как данните се синхронизират като част от тази интеграция между Dataverse и Finance.</span><span class="sxs-lookup"><span data-stu-id="9b90c-106">The following illustration shows how data is synchronized as part of this integration between Dataverse and Finance.</span></span>

![Преглед на потоците от данни за Project Operations](./media/ProjectOperationsFlows.jpg)

<span data-ttu-id="9b90c-108">Project Operations на Dataverse осигурява модерен потребителски интерфейс (UI) и лесна разширяемост без код/малко код с помощта на възможности на Power Platform.</span><span class="sxs-lookup"><span data-stu-id="9b90c-108">Project Operations on Dataverse provides a modern user interface (UI) and easy no-code/low-code extensibility using Power Platform capabilities.</span></span> <span data-ttu-id="9b90c-109">Мениджърите на проекти, мениджърите на ресурси, членовете на екипа на проекта и други лица от фронт офиса изпълняват своите дейности в Project Operations на Dataverse.</span><span class="sxs-lookup"><span data-stu-id="9b90c-109">Project managers, Resource managers, Project team members, and other front-office personas, perform their activities in Project Operations on Dataverse.</span></span>

<span data-ttu-id="9b90c-110">Project Operations във Finance предоставя подкрепа за счетоводство на проекти и признаване на приходи.</span><span class="sxs-lookup"><span data-stu-id="9b90c-110">Project Operations in Finance provides project accounting and revenue recognition support.</span></span> <span data-ttu-id="9b90c-111">Project Operations се включва във финансовата рамка във Finance за изчисляване на данък върху продажбите, валутни курсове, отчитане на финансовите измерения и др.</span><span class="sxs-lookup"><span data-stu-id="9b90c-111">Project Operations plugs in to the financial framework in Finance for sales tax calculation, currency exchange rates, financial dimension reporting, and more.</span></span> <span data-ttu-id="9b90c-112">Опитът на счетоводителя по проекта се базира предимно на Finance.</span><span class="sxs-lookup"><span data-stu-id="9b90c-112">The Project accountant experiences are mostly based in Finance.</span></span>

<span data-ttu-id="9b90c-113">Интеграцията на Project Operations се състои от следната интеграция на компоненти:</span><span class="sxs-lookup"><span data-stu-id="9b90c-113">Project Operations integration consists of the following component integration:</span></span>


- [<span data-ttu-id="9b90c-114">Интегриране на данни за настройка и конфигурация на Project Operations</span><span class="sxs-lookup"><span data-stu-id="9b90c-114">Project Operations setup and configuration data integration</span></span>](resource-dual-write-setup-integration.md) 
- [<span data-ttu-id="9b90c-115">Проектни оценки и действителни данни</span><span class="sxs-lookup"><span data-stu-id="9b90c-115">Project estimates and actuals</span></span>](resource-dual-write-estimates-actuals.md)
- [<span data-ttu-id="9b90c-116">Фактури по проект</span><span class="sxs-lookup"><span data-stu-id="9b90c-116">Project invoices</span></span>](resource-dual-write-project-invoice.md)
- [<span data-ttu-id="9b90c-117">Управление на разходите</span><span class="sxs-lookup"><span data-stu-id="9b90c-117">Expense management</span></span>](resource-dual-write-expense.md)
- [<span data-ttu-id="9b90c-118">Фактура от доставчик</span><span class="sxs-lookup"><span data-stu-id="9b90c-118">Vendor invoice</span></span>](resource-dual-write-vendor-invoice.md)
