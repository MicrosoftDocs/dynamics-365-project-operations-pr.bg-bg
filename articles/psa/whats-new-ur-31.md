---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 31, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 31, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/26/2021
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
ms.openlocfilehash: a595c0a129ac35d3416984e57908e73e1eaef2fd
ms.sourcegitcommit: 6e1498502461e86cff722ccaf8795ff11c7c47ad
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2021
ms.locfileid: "5945522"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-31-v3"></a><span data-ttu-id="b8187-103">Какво е новото или промененото в Project Service Automation, издание на актуализация 31, V3</span><span class="sxs-lookup"><span data-stu-id="b8187-103">What's new or changed in Project Service Automation Update Release 31, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="b8187-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="b8187-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="b8187-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="b8187-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="b8187-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="b8187-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="b8187-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="b8187-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="b8187-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="b8187-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="b8187-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 31.</span><span class="sxs-lookup"><span data-stu-id="b8187-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 31.</span></span> <span data-ttu-id="b8187-110">Тази версия има номер на компилацията V3.10.52.77 и е общодостъпна чрез самоактуализация от май 2021 г.</span><span class="sxs-lookup"><span data-stu-id="b8187-110">This version has a build number of V3.10.52.77 and is generally available through a self-update in May 2021.</span></span>

## <a name="update-release-31"></a><span data-ttu-id="b8187-111">Издание на актуализация 31</span><span class="sxs-lookup"><span data-stu-id="b8187-111">Update Release 31</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="b8187-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="b8187-112">Bug fixes</span></span>

<span data-ttu-id="b8187-113">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="b8187-113">**Time and Expense**</span></span>

<span data-ttu-id="b8187-114">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="b8187-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="b8187-115">Командни бутони за контрол на въвеждане на време на страницата **Наличен ресурс** бяха объркващи.</span><span class="sxs-lookup"><span data-stu-id="b8187-115">Time entry control command buttons on the **Bookable Resource** page were confusing.</span></span>
- <span data-ttu-id="b8187-116">Изключено е изключение за нулева препратка в **Project.SetTrackingFields** при одобряване на запис на време.</span><span class="sxs-lookup"><span data-stu-id="b8187-116">A null reference exception was generated in **Project.SetTrackingFields** when approving a time entry.</span></span>

<span data-ttu-id="b8187-117">**Управление на ресурси**</span><span class="sxs-lookup"><span data-stu-id="b8187-117">**Resource Management**</span></span>

<span data-ttu-id="b8187-118">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="b8187-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="b8187-119">**Създайте член на екипа** не показва правилно настройката на метаданните за настройка на резервация за **Статус на ангажираност по подразбиране**.</span><span class="sxs-lookup"><span data-stu-id="b8187-119">**Create Team Member** doesn't correctly display the booking setup metadata setting for **Default Booking Committed Status**.</span></span>
- <span data-ttu-id="b8187-120">При надстройка от PSA 1.X до 3.X, процесът на надстройка е неуспешен в **UpgradeResourceRequirements**.</span><span class="sxs-lookup"><span data-stu-id="b8187-120">When upgrading from PSA 1.X to 3.X, the upgrade process fails at **UpgradeResourceRequirements**.</span></span>


<span data-ttu-id="b8187-121">**Продажби**</span><span class="sxs-lookup"><span data-stu-id="b8187-121">**Sales**</span></span>

<span data-ttu-id="b8187-122">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="b8187-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="b8187-123">Действителните приходи преобразуват сумите във валутата на проекта в мрежата за проследяване.</span><span class="sxs-lookup"><span data-stu-id="b8187-123">Actual revenue converts the amounts to the project currency in the tracking grid.</span></span>
- <span data-ttu-id="b8187-124">Валутата по подразбиране е неясна при създаване на редове на дневници, редове за котировки и линии на договори в сценарии, при които основната валута на организацията се различава от валутата на проекта.</span><span class="sxs-lookup"><span data-stu-id="b8187-124">The currency default is unclear when creating journal lines, quote lines, and contract lines in scenarios where an organization's base currency differs from the project currency.</span></span>
- <span data-ttu-id="b8187-125">Заявката **Изчаква валидиране на дневника за корекция** не се филтрира по проект.</span><span class="sxs-lookup"><span data-stu-id="b8187-125">**Pending correction journal validation** query doesn't filter by project.</span></span>
- <span data-ttu-id="b8187-126">Останалите продажби се изчисляват неправилно за даден проект.</span><span class="sxs-lookup"><span data-stu-id="b8187-126">Remaining sales are calculated incorrectly on a project.</span></span>
- <span data-ttu-id="b8187-127">Котировките, базирани на контакт, се провалят, когато са създадени без ценова листа.</span><span class="sxs-lookup"><span data-stu-id="b8187-127">Quotes based on a contact fail when they are created without a price list.</span></span>
- <span data-ttu-id="b8187-128">Когато изберете, не се показва въртящо устройство за обработка **Потвърдете фактурата**.</span><span class="sxs-lookup"><span data-stu-id="b8187-128">No processing spinner is shown when you select **Confirm Invoice**.</span></span>
- <span data-ttu-id="b8187-129">Когато изберете, не се показва въртящо устройство за обработка **Създаване на фактура**.</span><span class="sxs-lookup"><span data-stu-id="b8187-129">No processing spinner is shown when you select **Create Invoice**.</span></span>
- <span data-ttu-id="b8187-130">Затварянето на оферта като загубена не отменя резервациите.</span><span class="sxs-lookup"><span data-stu-id="b8187-130">Closing a quote as lost doesn't cancel the bookings.</span></span>







