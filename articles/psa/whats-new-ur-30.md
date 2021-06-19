---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 30, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 30, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/01/2021
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
ms.openlocfilehash: 3b6b7dba9c2a22587d27006b9972c950fbb454f2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010413"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-30-v3"></a><span data-ttu-id="b2ba5-103">Какво е новото или промененото в Project Service Automation, издание на актуализация 30, V3</span><span class="sxs-lookup"><span data-stu-id="b2ba5-103">What's new or changed in Project Service Automation Update Release 30, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="b2ba5-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="b2ba5-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="b2ba5-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="b2ba5-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="b2ba5-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution.md).</span><span class="sxs-lookup"><span data-stu-id="b2ba5-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution.md).</span></span>

<span data-ttu-id="b2ba5-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 30.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 30.</span></span> <span data-ttu-id="b2ba5-110">Тази версия има номер на създаване V3.10.51.61 и е общо достъпна чрез самостоятелно актуализиране от април 2021 г.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-110">This version has a build number of V3.10.51.61 and is generally available through a self-update in April 2021.</span></span>

## <a name="update-release-30"></a><span data-ttu-id="b2ba5-111">Издание на актуализация 30</span><span class="sxs-lookup"><span data-stu-id="b2ba5-111">Update Release 30</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="b2ba5-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="b2ba5-112">Bug fixes</span></span>

<span data-ttu-id="b2ba5-113">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="b2ba5-113">**Time and Expense**</span></span>

<span data-ttu-id="b2ba5-114">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="b2ba5-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="b2ba5-115">Възниква грешка, когато създавате и записвате запис за време на страницата **Бързо създаване**, ако полето **Роля** е премахнато.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-115">An error occurs when you create and save a time entry on the **Quick Create** page if the **Role** field is removed.</span></span>
- <span data-ttu-id="b2ba5-116">Филтърът за въвеждане на време прилага грешен оператор на филтъра.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-116">The Time Entry filter applies the wrong filter operator.</span></span>
- <span data-ttu-id="b2ba5-117">Копираните разписания не се показват автоматично, когато изберете **Седмица на копиране** на контрола за въвеждане на време.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-117">Copied timesheets aren't automatically displayed when you select **Copy Week** on the time entry control.</span></span>

<span data-ttu-id="b2ba5-118">**Управление на ресурси**</span><span class="sxs-lookup"><span data-stu-id="b2ba5-118">**Resource Management**</span></span>

<span data-ttu-id="b2ba5-119">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="b2ba5-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="b2ba5-120">Когато удължите резервацията, състоянието на резервацията, присвоено на твърдата резервация, е неправилно.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-120">When you extend a booking, the booking status assigned to the hard booking is incorrect.</span></span> <span data-ttu-id="b2ba5-121">Удължаването на резервацията зачита състоянието на резервацията, определено като **Ангажиран** в метаданните за настройка на резервацията.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-121">Extending a booking respects the booking status defined as **Committed** in the booking setup metadata.</span></span>
- <span data-ttu-id="b2ba5-122">Когато не е посочено валидно състояние на резервацията, съобщението за грешка не е локализирано правилно.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-122">When a valid booking status isn't specified, the error message is not correctly localized.</span></span>

<span data-ttu-id="b2ba5-123">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="b2ba5-123">**Project Management**</span></span>

<span data-ttu-id="b2ba5-124">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="b2ba5-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="b2ba5-125">Проектите не могат да се създават в една валута и да включват свързани задачи в друга валута.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-125">Projects can't be created in one currency and include related tasks in another currency.</span></span>

<span data-ttu-id="b2ba5-126">**Продажби**</span><span class="sxs-lookup"><span data-stu-id="b2ba5-126">**Sales**</span></span>

<span data-ttu-id="b2ba5-127">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="b2ba5-127">The following issues have been fixed:</span></span>

- <span data-ttu-id="b2ba5-128">Когато се копира ценова листа, цените не се актуализират.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-128">When a price list is copied, prices aren't updated.</span></span>
- <span data-ttu-id="b2ba5-129">Затварянето на оферта като спечелена не е успешно, когато детайлът на разходите има стойност за произход.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-129">Closing a quote as won fails when the cost detail has a value for origin.</span></span>
- <span data-ttu-id="b2ba5-130">В обекта **Задача на проекта** **Очаквани разходи** е преименувано на **Планирани разходи (база)**.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-130">On the **Project Task** entity, **Estimated Cost** has been renamed to **Planned Cost (Base)**.</span></span>
- <span data-ttu-id="b2ba5-131">При създаване или изтриване на фактури се генерира изключение с нулева препратка.</span><span class="sxs-lookup"><span data-stu-id="b2ba5-131">A null reference exception is generated when invoices are created or deleted.</span></span>
