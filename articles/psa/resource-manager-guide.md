---
title: Ръководство за мениджъри на ресурси
description: Ръководство за управлението на ресурси в Project Service
author: JohnPBurrows
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 4b9df18e7240450f01271b73eb6ea7e215be38c5
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5282815"
---
# <a name="resource-manager-guide-project-service"></a><span data-ttu-id="b13f9-103">Ръководство за мениджъри на ресурси (Project Service)</span><span class="sxs-lookup"><span data-stu-id="b13f9-103">Resource manager guide (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="b13f9-104">Възможностите на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] в [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] ви помагат да намерите най-подходящите ресурси в точното време за точния проект и да се уверите, че всички ресурси се използват ефективно.</span><span class="sxs-lookup"><span data-stu-id="b13f9-104">The [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] help you find the right resources at the right time for the right project and make sure all resources are utilized efficiently.</span></span>  
  
 <span data-ttu-id="b13f9-105">Разположете консултантите на компанията си ефективно и ефикасно чрез [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b13f9-105">Deploy your company’s consultants efficiently and effectively with the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> <span data-ttu-id="b13f9-106">Те ви предоставят инструментите, от които се нуждаете, за да планирате ресурси въз основа на изискванията и графиците на консултантски проекти и на уменията и наличността на своите консултанти.</span><span class="sxs-lookup"><span data-stu-id="b13f9-106">These provide you with the tools you need to schedule resources based on the requirements and schedules of consulting projects and on the skills and availability of your consultants.</span></span> <span data-ttu-id="b13f9-107">Можете бързо да намирате най-квалифицираните консултанти, които са налични за работа по проекти, и можете лесно да виждате как по-добре да ги планирате в хода на всеки проект.</span><span class="sxs-lookup"><span data-stu-id="b13f9-107">You can quickly find the most qualified consultants who are available to work on projects, and you can easily see how to better schedule them during the course of each project.</span></span>  
  
 <span data-ttu-id="b13f9-108">Планирането на ресурсите ви помага да направите следното:</span><span class="sxs-lookup"><span data-stu-id="b13f9-108">Resource scheduling helps you do the following:</span></span>  
  
- <span data-ttu-id="b13f9-109">Намиране на съответните ресурси за проекти въз основа на това доколко уменията и нивата им на професионална подготовка отговарят на изискванията за ресурси на проекта.</span><span class="sxs-lookup"><span data-stu-id="b13f9-109">Match resources to projects, based on how well their skills and proficiency levels match the project resource requirements.</span></span>  
  
- <span data-ttu-id="b13f9-110">Съпоставяне на графика на даден ресурс с календара на проекта въз основа на наличността и планираното неработно време.</span><span class="sxs-lookup"><span data-stu-id="b13f9-110">Match a resource’s schedule to a project calendar, based on their availability and scheduled time off.</span></span> <span data-ttu-id="b13f9-111">Цветово кодираният календар ви дава визуални сигнали за наличността на ресурсите.</span><span class="sxs-lookup"><span data-stu-id="b13f9-111">The color-coded calendar gives you visual cues about resource availability.</span></span>  
  
- <span data-ttu-id="b13f9-112">Преглеждане на капацитета на всеки консултант и да определяте как този капацитет се използва в момента.</span><span class="sxs-lookup"><span data-stu-id="b13f9-112">Review the capacity of each consultant and determine how that capacity is currently used.</span></span> <span data-ttu-id="b13f9-113">Това може да ви помогне да разберете кога даден консултант може да бъде твърде свободен или прекалено зает и дали работи на пълния си капацитет.</span><span class="sxs-lookup"><span data-stu-id="b13f9-113">This can help you find where a consultant might be under- or over-utilized, or if they’re working at capacity.</span></span>  
  
- <span data-ttu-id="b13f9-114">Присвояване на процент или определен брой часове от капацитета на един работник към даден проект.</span><span class="sxs-lookup"><span data-stu-id="b13f9-114">Assign a percentage or a specific number of hours for a worker’s capacity to a project.</span></span>  
  
- <span data-ttu-id="b13f9-115">Извършване на групови резервации на ресурси.</span><span class="sxs-lookup"><span data-stu-id="b13f9-115">Make group resource bookings.</span></span>  
  
- <span data-ttu-id="b13f9-116">Извършване на плаващи или твърди резервации на ресурси и преобразуване на плаващите часове във фиксирани с една стъпка.</span><span class="sxs-lookup"><span data-stu-id="b13f9-116">Soft book or hard book resources, and convert soft-booked hours into hard-booked hours in one step.</span></span>  
  
- <span data-ttu-id="b13f9-117">Автоматично формиране на екип по проекта въз основа на ресурси, дефинирани в съставната структура на работата за даден проект.</span><span class="sxs-lookup"><span data-stu-id="b13f9-117">Automatically form a project team based on resources defined in a work breakdown structure for a project.</span></span>  
  
- <span data-ttu-id="b13f9-118">Изпълняване на заявки за ресурси (резервиране, предложение, намиране на заместващи ресурси).</span><span class="sxs-lookup"><span data-stu-id="b13f9-118">Fulfill resource requests (book, propose, find substitute resources).</span></span>  
  
- <span data-ttu-id="b13f9-119">Присвояване на ресурси според централен модел (присвояване от мениджър на ресурса) или хибриден модел (присвояване от мениджър на ресурса и от други мениджъри).</span><span class="sxs-lookup"><span data-stu-id="b13f9-119">Assign resources according to a central (resource manager assigns) or hybrid model (resource manager and other managers can assign).</span></span> <span data-ttu-id="b13f9-120">За повече информация относно задаването на централен или хибриден модел на управление на ресурсите вижте [Конфигуриране на допълнителни настройки на параметри (Project Service)](../psa/configure-additional-parameters-settings.md).</span><span class="sxs-lookup"><span data-stu-id="b13f9-120">For more information about setting a central versus hybrid resource management model, see [Configure additional parameters settings (Project Service)](../psa/configure-additional-parameters-settings.md).</span></span>  
  
  <span data-ttu-id="b13f9-121">Можете да управлявате ресурсите ефективно за различните проекти и да гарантирате, че проектите са възложени на подходящ персонал.</span><span class="sxs-lookup"><span data-stu-id="b13f9-121">You can manage resources efficiently across projects and ensure that projects are staffed appropriately.</span></span> <span data-ttu-id="b13f9-122">Ще трябва да изпълните следните задачи:</span><span class="sxs-lookup"><span data-stu-id="b13f9-122">You’ll need to perform the following tasks:</span></span>  
  
- <span data-ttu-id="b13f9-123">[Управление на заявки за ресурси](../psa/manage-resource-requests.md).</span><span class="sxs-lookup"><span data-stu-id="b13f9-123">[Manage resource requests](../psa/manage-resource-requests.md).</span></span> <span data-ttu-id="b13f9-124">Съпоставяне на уменията и професионалната подготовка на вашите консултанти спрямо правилните проекти.</span><span class="sxs-lookup"><span data-stu-id="b13f9-124">Match the skills and proficiencies of your consultants to the right projects.</span></span>  
  
- <span data-ttu-id="b13f9-125">[Преглед за наличност на ресурси](../psa/view-resource-availability.md).</span><span class="sxs-lookup"><span data-stu-id="b13f9-125">[View resource availability](../psa/view-resource-availability.md).</span></span> <span data-ttu-id="b13f9-126">Проверете наличността на консултантите в календарен изглед.</span><span class="sxs-lookup"><span data-stu-id="b13f9-126">Check consultants’ availability in a calendar view.</span></span>  
  
- <span data-ttu-id="b13f9-127">[Преглед за използването на ресурси](../psa/view-resource-utilization.md).</span><span class="sxs-lookup"><span data-stu-id="b13f9-127">[View resource utilization](../psa/view-resource-utilization.md).</span></span> <span data-ttu-id="b13f9-128">Вижте процента от времето, в което вашите консултанти в момента са резервирани.</span><span class="sxs-lookup"><span data-stu-id="b13f9-128">See the percentage of time that your consultants are currently booked.</span></span>  
  
- <span data-ttu-id="b13f9-129">[Планиране на ресурси за проект](../psa/schedule-resources-project.md).</span><span class="sxs-lookup"><span data-stu-id="b13f9-129">[Schedule resources for a project](../psa/schedule-resources-project.md).</span></span> <span data-ttu-id="b13f9-130">Планирайте консултанти за проект.</span><span class="sxs-lookup"><span data-stu-id="b13f9-130">Schedule consultants for a project.</span></span>  
  
  <span data-ttu-id="b13f9-131">За повече информация за подаването за заявки за ресурси за отделни проекти вижте [Подаване на заявки за ресурси](../psa/submit-resource-requests.md).</span><span class="sxs-lookup"><span data-stu-id="b13f9-131">For more information about submitting resource requests for individual projects, see [Submit resource requests](../psa/submit-resource-requests.md).</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="b13f9-132">Вижте също</span><span class="sxs-lookup"><span data-stu-id="b13f9-132">See Also</span></span>  
 <span data-ttu-id="b13f9-133">[Преглед на Project Service](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="b13f9-133">[Overview of Project Service](../psa/overview.md) </span></span>  
 <span data-ttu-id="b13f9-134">[Ръководство на администратора](../psa/admin-guide.md) </span><span class="sxs-lookup"><span data-stu-id="b13f9-134">[Administrator Guide](../psa/admin-guide.md) </span></span>  
 <span data-ttu-id="b13f9-135">[Ръководство за мениджъри на акаунти](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="b13f9-135">[Account Manager Guiden](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="b13f9-136">[Ръководство за мениджъри на проекти](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="b13f9-136">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 [<span data-ttu-id="b13f9-137">Ръководство за време, разходи и сътрудничество</span><span class="sxs-lookup"><span data-stu-id="b13f9-137">Time, Expense, and Collaboration Guide</span></span>](../psa/time-expense-collaboration-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]