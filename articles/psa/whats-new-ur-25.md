---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 25, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 25, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 10/26/2020
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
ms.openlocfilehash: 30822ec64b31e110202a587dd941bdff60116712
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280430"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-25-v3"></a><span data-ttu-id="8f873-103">Какво е новото или промененото в Project Service Automation, издание на актуализация 25, V3</span><span class="sxs-lookup"><span data-stu-id="8f873-103">What's new or changed in Project Service Automation Update Release 25, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="8f873-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="8f873-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="8f873-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="8f873-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="8f873-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="8f873-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="8f873-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="8f873-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="8f873-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="8f873-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="8f873-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 25. Тази версия е с номер на компилация V 3.10.43.76 и е общодостъпна чрез самостоятелна актуализация от октомври 2020 г.</span><span class="sxs-lookup"><span data-stu-id="8f873-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 25 This version has a build number of V 3.10.43.76 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-25"></a><span data-ttu-id="8f873-110">Издание на актуализация 25</span><span class="sxs-lookup"><span data-stu-id="8f873-110">Update Release 25</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="8f873-111">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="8f873-111">Bug fixes</span></span>

<span data-ttu-id="8f873-112">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="8f873-112">**Time and Expense**</span></span>

<span data-ttu-id="8f873-113">Следният проблем е коригиран:</span><span class="sxs-lookup"><span data-stu-id="8f873-113">The following issue has been fixed:</span></span>

- <span data-ttu-id="8f873-114">Диаграма на запис за време, показваща допълнителни данни въз основа на извличане на твърде голям интервал.</span><span class="sxs-lookup"><span data-stu-id="8f873-114">Time entry chart showing additional data based on too large of an interval being retrieved.</span></span>

<span data-ttu-id="8f873-115">**Управление на ресурси**</span><span class="sxs-lookup"><span data-stu-id="8f873-115">**Resource Management**</span></span>

<span data-ttu-id="8f873-116">Следният проблем е коригиран:</span><span class="sxs-lookup"><span data-stu-id="8f873-116">The following issue has been fixed:</span></span>

- <span data-ttu-id="8f873-117">Добавен код на Package Deployer, за да пропуснете импортирането на корекция на Universal Resource Scheduling, ако съществува корекция с по-висока версия.</span><span class="sxs-lookup"><span data-stu-id="8f873-117">Added package deployer code to skip the Universal Resource Scheduling patch import if a higher version patch already exists.</span></span>

<span data-ttu-id="8f873-118">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="8f873-118">**Project Management**</span></span>

<span data-ttu-id="8f873-119">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="8f873-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="8f873-120">Коригирано закръгляване и несъответствия в обменния курс, водещи до неправилни планирани разходи в мрежата за проследяване на проекта.</span><span class="sxs-lookup"><span data-stu-id="8f873-120">Corrected rounding and exchange rate discrepancies resulting in incorrect planned cost in the project tracking grid.</span></span>
- <span data-ttu-id="8f873-121">Поддържат възможността за показване на две или повече мрежи за реагиране във формуляра **Проект**.</span><span class="sxs-lookup"><span data-stu-id="8f873-121">Support the ability to display two or more react grids on the **Project** form.</span></span>
- <span data-ttu-id="8f873-122">Предоставено валидиране за адресиране на възможността за присвояване на задача след крайната дата на календара, което води до неуспешно присвояване на ресурс.</span><span class="sxs-lookup"><span data-stu-id="8f873-122">Provided validation to address the ability to assign a task past the calendar end date, which results in a failed resource assignment.</span></span>
- <span data-ttu-id="8f873-123">Подобрена обработка на грешки за адресиране на изключение с нулева препратка, генерирано от следното:</span><span class="sxs-lookup"><span data-stu-id="8f873-123">Improved error handling to address Null Reference Exception generated from the following:</span></span>

    - <span data-ttu-id="8f873-124">Добавка **PreValidateProjectTeamMemberCreate**</span><span class="sxs-lookup"><span data-stu-id="8f873-124">**PreValidateProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="8f873-125">**PreValidateProjectTaskCreate**, когато се създава задача по проект без свързан проект</span><span class="sxs-lookup"><span data-stu-id="8f873-125">**PreValidateProjectTaskCreate** when a project task is created without an associated project</span></span>
    - <span data-ttu-id="8f873-126">Добавка **PreProjectTeamMemberCreate**</span><span class="sxs-lookup"><span data-stu-id="8f873-126">**PreProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="8f873-127">Добавка **PostProjectTeamMemberDelete**</span><span class="sxs-lookup"><span data-stu-id="8f873-127">**PostProjectTeamMemberDelete** plug-in</span></span>
    - <span data-ttu-id="8f873-128">Добавка **PreValidateProjectTaskDelete**</span><span class="sxs-lookup"><span data-stu-id="8f873-128">**PreValidateProjectTaskDelete** plug-in</span></span>

<span data-ttu-id="8f873-129">**Sales**</span><span class="sxs-lookup"><span data-stu-id="8f873-129">**Sales**</span></span>

<span data-ttu-id="8f873-130">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="8f873-130">The following issues have been fixed:</span></span>

- <span data-ttu-id="8f873-131">Подобрена обработка на грешки за адресиране на изключения с нулева препратка, генерирани от **Копиране на проект: Оценява управлението на HelperResource**.</span><span class="sxs-lookup"><span data-stu-id="8f873-131">Improved error handling to address Null Reference Exceptions generated from **Copy Project: Estimates HelperResource Management**.</span></span>
- <span data-ttu-id="8f873-132">**Не е готово за фактуриране** на **Натрупване за фактуриране на време и материали** не изчиства състоянието на фактуриране.</span><span class="sxs-lookup"><span data-stu-id="8f873-132">**Not ready to Invoice** on a **Time and Material Billing Backlog** doesn't clear the billing status.</span></span>
- <span data-ttu-id="8f873-133">Коригирани са бутоните с погрешни етикети **Цени** в раздела **Цена на роля** и **Елементи от каталог**.</span><span class="sxs-lookup"><span data-stu-id="8f873-133">Corrected mislabeled **Prices** buttons on the **Role Price** and **Catalog Items** tab.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]