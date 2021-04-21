---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 29, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 29, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/22/2021
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
ms.openlocfilehash: 0e1ff0db42adb8b991b26dca1585bd603b2e2276
ms.sourcegitcommit: f57408d6637f670b920d7ce95f8ace8eb1963093
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/17/2021
ms.locfileid: "5664630"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-29-v3"></a><span data-ttu-id="1aa17-103">Какво е новото или промененото в Project Service Automation, издание на актуализация 29, V3</span><span class="sxs-lookup"><span data-stu-id="1aa17-103">What's new or changed in Project Service Automation Update Release 29, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="1aa17-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="1aa17-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="1aa17-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="1aa17-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="1aa17-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="1aa17-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="1aa17-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="1aa17-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="1aa17-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="1aa17-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="1aa17-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 29.</span><span class="sxs-lookup"><span data-stu-id="1aa17-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 29.</span></span> <span data-ttu-id="1aa17-110">Тази версия има номер на компилация V3.10.47.7 и е общодостъпно чрез самостоятелна актуализация от февруари 2021 г.</span><span class="sxs-lookup"><span data-stu-id="1aa17-110">This version has a build number of V3.10.47.7 and is generally available through a self-update in February 2021.</span></span>

## <a name="update-release-29"></a><span data-ttu-id="1aa17-111">Издание на актуализация 29</span><span class="sxs-lookup"><span data-stu-id="1aa17-111">Update Release 29</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="1aa17-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="1aa17-112">Bug fixes</span></span>

<span data-ttu-id="1aa17-113">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="1aa17-113">**Time and Expense**</span></span>

<span data-ttu-id="1aa17-114">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="1aa17-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="1aa17-115">Потребителите не могат да видят работното време, регистрирано в неработни дни в мрежата за въвеждане на време.</span><span class="sxs-lookup"><span data-stu-id="1aa17-115">Users can't see working hours logged on non-working days in the time entry grid.</span></span>
- <span data-ttu-id="1aa17-116">Одобрените записи за разходи могат да бъдат редактирани в мрежата.</span><span class="sxs-lookup"><span data-stu-id="1aa17-116">Approved expense entries can be edited on the grid.</span></span>

<span data-ttu-id="1aa17-117">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="1aa17-117">**Project Management**</span></span>

<span data-ttu-id="1aa17-118">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="1aa17-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="1aa17-119">Липсваща логика за валидиране, за да се гарантира, че часовете за усилие за присвояване на ресурси не могат да бъдат отрицателни.</span><span class="sxs-lookup"><span data-stu-id="1aa17-119">Missing validation logic to ensure resource assignment effort hours can't be negative.</span></span>
- <span data-ttu-id="1aa17-120">Персонализираното действие **AssignResourcesForTask** актуализира всички полета вместо само променените полета.</span><span class="sxs-lookup"><span data-stu-id="1aa17-120">The custom action, **AssignResourcesForTask** updates all fields instead of only changed fields.</span></span>
- <span data-ttu-id="1aa17-121">Когато копирате проект в среда с приставки или работни потоци, които са регистрирани в събитието **CreateProject**, атрибутът **msdyn_bulkgenerationstatus** не се актуализира, ако **CopyWBSToProject** се проваля.</span><span class="sxs-lookup"><span data-stu-id="1aa17-121">When copying a project in an environment with plug-ins or workflows that are registered on the **CreateProject** event, the **msdyn_bulkgenerationstatus** attribute isn't updated if the **CopyWBSToProject** fails.</span></span>
- <span data-ttu-id="1aa17-122">Когато разширите календара на проекта, работните дни не се сортират във възходящ ред, което води до неуспех на някои актуализации на проектни задачи.</span><span class="sxs-lookup"><span data-stu-id="1aa17-122">When you expand the project calendar, the working days aren't sorted in ascending order causing some project task updates to fail.</span></span>
- <span data-ttu-id="1aa17-123">Промяната на мениджъра на проекти в съществуващ проект задейства логиката по подразбиране на организационната единица.</span><span class="sxs-lookup"><span data-stu-id="1aa17-123">Changing the Project Manager on an existing project triggers the organizational unit defaulting logic.</span></span>

<span data-ttu-id="1aa17-124">**Продажби**</span><span class="sxs-lookup"><span data-stu-id="1aa17-124">**Sales**</span></span>

<span data-ttu-id="1aa17-125">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="1aa17-125">The following issues have been fixed:</span></span>

- <span data-ttu-id="1aa17-126">Разделът **Изпълнение на договора** на страницата **Договор** се проваля безшумно по време на инициализация, когато не са налице редове на договора.</span><span class="sxs-lookup"><span data-stu-id="1aa17-126">The **Contract Performance** tab on the **Contract** page fails silently during initialization when no contract lines are present.</span></span>
