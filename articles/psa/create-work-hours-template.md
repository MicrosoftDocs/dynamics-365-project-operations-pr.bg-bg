---
title: Създаване на шаблон за работно време
description: Тази тема описва как се създава шаблон за работно време в Project Service.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 105e3cb2ef7b904e96dc21013906e0b7444e3b88
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997183"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="3be9f-103">Създаване на шаблон за работно време (Project Service)</span><span class="sxs-lookup"><span data-stu-id="3be9f-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="3be9f-104">За да създадете и управлявате проект, трябва да приложите шаблон към календара към проекта.</span><span class="sxs-lookup"><span data-stu-id="3be9f-104">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="3be9f-105">Шаблонът на календара дефинира следните атрибути на проекта:</span><span class="sxs-lookup"><span data-stu-id="3be9f-105">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="3be9f-106">Работно време, включително начален и краен час</span><span class="sxs-lookup"><span data-stu-id="3be9f-106">Working hours, including start and end time</span></span>
- <span data-ttu-id="3be9f-107">Работни дни</span><span class="sxs-lookup"><span data-stu-id="3be9f-107">Working days</span></span>
- <span data-ttu-id="3be9f-108">Календарни изключения като неработни дни</span><span class="sxs-lookup"><span data-stu-id="3be9f-108">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="3be9f-109">Шаблонът на календара, който се прилага към проект, е копие на шаблона на календара, дефиниран в настройките на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="3be9f-109">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="3be9f-110">Ако промените шаблона на календара, тези промени не се разпространяват в работното време на проекта.</span><span class="sxs-lookup"><span data-stu-id="3be9f-110">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="3be9f-111">За да промените работното време на проекта, трябва да се приложи нов шаблон.</span><span class="sxs-lookup"><span data-stu-id="3be9f-111">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="3be9f-112">За да създадете шаблон за календар за вашата организация, има две ключови изисквания:</span><span class="sxs-lookup"><span data-stu-id="3be9f-112">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="3be9f-113">Определете желаното работно време на шаблона, като използвате нов или съществуващ резервируем ресурс.</span><span class="sxs-lookup"><span data-stu-id="3be9f-113">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="3be9f-114">Създайте нов шаблон за календар и свържете шаблона с резервируемия ресурс.</span><span class="sxs-lookup"><span data-stu-id="3be9f-114">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="3be9f-115">**Определете работните часове на шаблона**</span><span class="sxs-lookup"><span data-stu-id="3be9f-115">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="3be9f-116">Отидете на **Ресурси** \> **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="3be9f-116">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="3be9f-117">Създайте нов ресурс за справка в шаблона на календара или изберете съществуващ ресурс.</span><span class="sxs-lookup"><span data-stu-id="3be9f-117">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="3be9f-118">Изберете раздела **Работни часове** в раздела на ресурса и попълнете инструкциите в [Задайте работно време за ресурс](/dynamics365/field-service/set-work-hours-resource.md) за да конфигурирате правилата на календара.</span><span class="sxs-lookup"><span data-stu-id="3be9f-118">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](/dynamics365/field-service/set-work-hours-resource.md) to configure the calendar rules.</span></span>

<span data-ttu-id="3be9f-119">**Създаване на нов шаблон за календар**</span><span class="sxs-lookup"><span data-stu-id="3be9f-119">**Create a new calendar template**</span></span>

1. <span data-ttu-id="3be9f-120">Отидете на **Настройки** \> **Шаблон на календар**.</span><span class="sxs-lookup"><span data-stu-id="3be9f-120">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="3be9f-121">Изберете **Създаване** и въведете име, описание и ресурс на шаблон.</span><span class="sxs-lookup"><span data-stu-id="3be9f-121">Select **New**, and enter a name, description, and template resource.</span></span>


> [!NOTE]
> <span data-ttu-id="3be9f-122">Когато ресурс е посочен в шаблон на календар, копие от календара на ресурса се свързва с шаблона на календара.</span><span class="sxs-lookup"><span data-stu-id="3be9f-122">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="3be9f-123">Ако работните часове на копирания шаблон се променят, тези промени няма да се разпространят в шаблона на календара.</span><span class="sxs-lookup"><span data-stu-id="3be9f-123">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>


### <a name="see-also"></a><span data-ttu-id="3be9f-124">Вижте също</span><span class="sxs-lookup"><span data-stu-id="3be9f-124">See Also</span></span>  
 [<span data-ttu-id="3be9f-125">Настройване на ресурси</span><span class="sxs-lookup"><span data-stu-id="3be9f-125">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
