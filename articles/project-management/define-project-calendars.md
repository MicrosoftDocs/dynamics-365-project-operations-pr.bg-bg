---
title: Определяне на календари на проекти
description: Тази тема предоставя информация за това как да приложите шаблон на календар към проект за проследяване на графика на проекта.
author: ruhercul
ms.date: 02/05/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 0d1a2c4bd2d4022bbf79afcef79170eb482e6418
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998983"
---
# <a name="define-project-calendars"></a><span data-ttu-id="8f5f5-103">Определяне на календари на проекти</span><span class="sxs-lookup"><span data-stu-id="8f5f5-103">Define project calendars</span></span>

<span data-ttu-id="8f5f5-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="8f5f5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8f5f5-105">За да създадете и управлявате проект, трябва да приложите шаблон към календара към проекта.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-105">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="8f5f5-106">Шаблонът на календара дефинира следните атрибути на проекта:</span><span class="sxs-lookup"><span data-stu-id="8f5f5-106">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="8f5f5-107">Работно време, включително начален и краен час</span><span class="sxs-lookup"><span data-stu-id="8f5f5-107">Working hours, including start and end time</span></span>
- <span data-ttu-id="8f5f5-108">Работни дни</span><span class="sxs-lookup"><span data-stu-id="8f5f5-108">Working days</span></span>
- <span data-ttu-id="8f5f5-109">Календарни изключения като неработни дни</span><span class="sxs-lookup"><span data-stu-id="8f5f5-109">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="8f5f5-110">Шаблонът на календара, който се прилага към проект, е копие на шаблона на календара, дефиниран в настройките на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-110">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="8f5f5-111">Ако промените шаблона на календара, тези промени не се разпространяват в работното време на проекта.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-111">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="8f5f5-112">За да промените работното време на проекта, трябва да се приложи нов шаблон.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-112">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="8f5f5-113">За да създадете шаблон за календар за вашата организация, има две ключови изисквания:</span><span class="sxs-lookup"><span data-stu-id="8f5f5-113">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="8f5f5-114">Определете желаното работно време на шаблона, като използвате нов или съществуващ резервируем ресурс.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-114">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="8f5f5-115">Създайте нов шаблон за календар и свържете шаблона с резервируемия ресурс.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-115">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="8f5f5-116">**Определете работните часове на шаблона**</span><span class="sxs-lookup"><span data-stu-id="8f5f5-116">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="8f5f5-117">Отидете на **Ресурси** \> **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-117">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="8f5f5-118">Създайте нов ресурс за справка в шаблона на календара или изберете съществуващ ресурс.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-118">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="8f5f5-119">Изберете раздела **Работни часове** в раздела на ресурса и попълнете инструкциите в [Задайте работно време за ресурс](/dynamics365/field-service/set-work-hours-resource.md) за да конфигурирате правилата на календара.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-119">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](/dynamics365/field-service/set-work-hours-resource.md) to configure the calendar rules.</span></span>

<span data-ttu-id="8f5f5-120">**Създаване на нов шаблон за календар**</span><span class="sxs-lookup"><span data-stu-id="8f5f5-120">**Create a new calendar template**</span></span>

1. <span data-ttu-id="8f5f5-121">Отидете на **Настройки** \> **Шаблон на календар**.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-121">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="8f5f5-122">Изберете **Създаване** и въведете име, описание и ресурс на шаблон.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-122">Select **New**, and enter a name, description, and template resource.</span></span>

> [!NOTE]
> <span data-ttu-id="8f5f5-123">Когато ресурс е посочен в шаблон на календар, копие от календара на ресурса се свързва с шаблона на календара.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-123">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="8f5f5-124">Ако работните часове на копирания шаблон се променят, тези промени няма да се разпространят в шаблона на календара.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-124">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>

<span data-ttu-id="8f5f5-125">Сега можете да свържете работния шаблон с шаблон на календар на проект.</span><span class="sxs-lookup"><span data-stu-id="8f5f5-125">You can now associate the work template with a project calendar template.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]

