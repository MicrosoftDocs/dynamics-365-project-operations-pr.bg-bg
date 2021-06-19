---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 32, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 32, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/01/2021
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
ms.openlocfilehash: 11bf451ef4f24e2301ffde4f86a556a8a4fe30b0
ms.sourcegitcommit: 886102894244887d72e5a6213071e8d8a52c9d48
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/01/2021
ms.locfileid: "6129653"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-32-v3"></a><span data-ttu-id="17178-103">Какво е новото или промененото в Project Service Automation, издание на актуализация 32, V3</span><span class="sxs-lookup"><span data-stu-id="17178-103">What's new or changed in Project Service Automation Update Release 32, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="17178-104">С удоволствие обявяваме най-новата актуализация за приложението Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="17178-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="17178-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="17178-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="17178-106">Съвместим е с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="17178-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="17178-107">За да актуализирате до тази версия, посетете страницата на центъра за администриране за решенията на Dynamics 365 Online и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="17178-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="17178-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="17178-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="17178-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 32.</span><span class="sxs-lookup"><span data-stu-id="17178-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 32.</span></span> <span data-ttu-id="17178-110">Тази версия има номер на компилация V3.10.53.108 и е общодостъпна чрез самостоятелна актуализиция през юни 2021 г.</span><span class="sxs-lookup"><span data-stu-id="17178-110">This version has a build number of V3.10.53.108 and is generally available through a self-update in June 2021.</span></span>

## <a name="update-release-32"></a><span data-ttu-id="17178-111">Издание на актуализация 32</span><span class="sxs-lookup"><span data-stu-id="17178-111">Update Release 32</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="17178-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="17178-112">Bug fixes</span></span>

#### <a name="general"></a><span data-ttu-id="17178-113">Обща информация</span><span class="sxs-lookup"><span data-stu-id="17178-113">General</span></span>

- <span data-ttu-id="17178-114">Когато основната надстройка е неуспешна, трябва да се блокират само основните входни точки на приложението, за да се гарантира, че споделените обекти все още са достъпни.</span><span class="sxs-lookup"><span data-stu-id="17178-114">When a major upgrade fails, only the main application entry points should be blocked, to ensure that shared entities are still accessible.</span></span>

#### <a name="time-and-expense"></a><span data-ttu-id="17178-115">Време и разход</span><span class="sxs-lookup"><span data-stu-id="17178-115">Time and Expense</span></span>

<span data-ttu-id="17178-116">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="17178-116">The following issues have been fixed:</span></span>

- <span data-ttu-id="17178-117">**TimeEntriesImportFromResourceAssignment** не поддържа началното и крайното време на контурното делене на присвояването на ресурси.</span><span class="sxs-lookup"><span data-stu-id="17178-117">**TimeEntriesImportFromResourceAssignment** doesn't maintain the start and end times of the resource assignment contour slice.</span></span>
- <span data-ttu-id="17178-118">Когато изберете **Отваряне на запис** в мрежата **Запис за време**, може да не успеете да изберете други формуляри.</span><span class="sxs-lookup"><span data-stu-id="17178-118">When you select **Open Entry** on the **Time Entry** grid, you might be prevented from selecting other forms.</span></span>
- <span data-ttu-id="17178-119">Докато импортирате присвоявания към записи за време, заявката за клиентски код може да генерира дълъг URL адрес, който да направи заявката неуспешна.</span><span class="sxs-lookup"><span data-stu-id="17178-119">While you import assignments to time entries, the client code query could generate a long URL that fails the query.</span></span>
- <span data-ttu-id="17178-120">В мрежата **Запис за време** след изтриване на стойност от клетка, фокусът не остава в мрежата.</span><span class="sxs-lookup"><span data-stu-id="17178-120">In the **Time Entry** grid, after a value is deleted from a cell, the focus doesn't remain in the grid.</span></span>
- <span data-ttu-id="17178-121">Бутонът **Отхвърляне** е премахнат от изгледа **Обработка на одобрения** за новите одобрения.</span><span class="sxs-lookup"><span data-stu-id="17178-121">The **Reject** button has been removed from the **Processing approvals** view for modern approvals.</span></span>
- <span data-ttu-id="17178-122">Стабилността и ефективността на груповото одобрение на записи за време се влияят от блокировки и неуспешно обработване по подходящ начин на персонализации, които са свързани с обекта **Запис за време**.</span><span class="sxs-lookup"><span data-stu-id="17178-122">The stability and performance of time entry bulk approval are affected by deadlocks and a failure to appropriately handle customizations that are related to the **Time Entry** entity.</span></span>

#### <a name="project-planning"></a><span data-ttu-id="17178-123">Планиране на проект</span><span class="sxs-lookup"><span data-stu-id="17178-123">Project Planning</span></span>

- <span data-ttu-id="17178-124">Изключение с нулева препратка се генерира, когато актуализирате проект, който има нулева стойност в полето **Единица, сключваща договора**.</span><span class="sxs-lookup"><span data-stu-id="17178-124">A null reference exception is generated when you update a project that has a null value in the **Contracting Unit** field.</span></span>
- <span data-ttu-id="17178-125">**Обновяване на общите суми по проекта** неправилно изчислява оставащите разходи и оставащите продажби по даден проект.</span><span class="sxs-lookup"><span data-stu-id="17178-125">**Refresh Project Totals** incorrectly calculates the remaining cost and remaining sales on a project.</span></span>
- <span data-ttu-id="17178-126">Излишните изчисления на цените засягат производителността, свързана с актуализации на контурите за присвояване на ресурси.</span><span class="sxs-lookup"><span data-stu-id="17178-126">Redundant pricing calculations affect performance that is related to updates on resource assignment contours.</span></span>

#### <a name="resource-management"></a><span data-ttu-id="17178-127">Управление на ресурс</span><span class="sxs-lookup"><span data-stu-id="17178-127">Resource Management</span></span>

<span data-ttu-id="17178-128">Следният проблем е коригиран:</span><span class="sxs-lookup"><span data-stu-id="17178-128">The following issue has been fixed:</span></span>

- <span data-ttu-id="17178-129">Когато производителността в календара на наличен ресурс е повече от 1, Project Service Automation неправилно разпознава производителността като 0 (нула).</span><span class="sxs-lookup"><span data-stu-id="17178-129">When a bookable resource's calendar capacity is more than 1, Project Service Automation incorrectly recognizes the capacity as 0 (zero).</span></span> <span data-ttu-id="17178-130">Следователно в изгледа на графика възниква безкраен цикъл.</span><span class="sxs-lookup"><span data-stu-id="17178-130">Therefore, an infinite loop occurs in the schedule view.</span></span>

#### <a name="sales"></a><span data-ttu-id="17178-131">Продажби</span><span class="sxs-lookup"><span data-stu-id="17178-131">Sales</span></span>

<span data-ttu-id="17178-132">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="17178-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="17178-133">Когато се създава счетоводен запис, който има персонализиран тип трансакция, възниква следното изключение за нулева препратка: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span><span class="sxs-lookup"><span data-stu-id="17178-133">When a journal line is created that has a custom transaction type, the following null reference exception occurs: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span></span>
- <span data-ttu-id="17178-134">Роли и категории, които са дезактивирани, преди копиране на оферта, не трябва да се добавят към платими роли и категории на наскоро копираната оферта.</span><span class="sxs-lookup"><span data-stu-id="17178-134">Roles and categories that are inactivated before a quotation is copied should not be added to chargeable roles and categories of the newly copied quotation.</span></span>
- <span data-ttu-id="17178-135">Датата на документа и счетоводната дата не са съгласувани с началната дата, посочена в подробностите за ред на фактура, които се създават директно в чернова на фактура.</span><span class="sxs-lookup"><span data-stu-id="17178-135">The document date and accounting date aren't aligned with the start date that is provided on an invoice line detail that is created directly on a draft invoice.</span></span>
- <span data-ttu-id="17178-136">Изключенията с нулеви препратки се генерират в сценарии, свързани с дезактивиране на роли и категории, преди да се копира офертата.</span><span class="sxs-lookup"><span data-stu-id="17178-136">Null reference exceptions are generated in scenarios that are related to inactivation of roles and categories before a quotation is copied.</span></span>
- <span data-ttu-id="17178-137">Действието **Актуализиране на цени** на страницата **Проекти** не актуализира оценките на разходите и материалите.</span><span class="sxs-lookup"><span data-stu-id="17178-137">The **Update Prices** action on the **Projects** page doesn't update expense estimates and material estimates.</span></span>
