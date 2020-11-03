---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 18, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 18, V3.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 04/27/2020
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
ms.openlocfilehash: 1d7ea200531dd24d56a829f879e3a2532a9b38dc
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071774"
---
# <a name="project-service-automation-update-release-18-v3"></a><span data-ttu-id="a043f-103">Project Service Automation, издание на актуализация 18, V3</span><span class="sxs-lookup"><span data-stu-id="a043f-103">Project Service Automation Update Release 18, V3</span></span>

<span data-ttu-id="a043f-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a043f-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="a043f-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="a043f-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="a043f-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="a043f-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="a043f-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения, за да инсталирате актуализацията.</span><span class="sxs-lookup"><span data-stu-id="a043f-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="a043f-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="a043f-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="a043f-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 18.</span><span class="sxs-lookup"><span data-stu-id="a043f-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 18.</span></span> <span data-ttu-id="a043f-110">Тази версия има номер на създаване V3.10.8.12 и е общо достъпна чрез самостоятелно актуализиране от април 2020 г.</span><span class="sxs-lookup"><span data-stu-id="a043f-110">This version has a build number of V3.10.8.12 and is generally available through a self-update in April 2020.</span></span>

## <a name="update-release-18"></a><span data-ttu-id="a043f-111">Издание на актуализация 18</span><span class="sxs-lookup"><span data-stu-id="a043f-111">Update Release 18</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="a043f-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="a043f-112">Bug fixes</span></span>

<span data-ttu-id="a043f-113">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="a043f-113">**Time and Expense**</span></span>

- <span data-ttu-id="a043f-114">Поправено: Потоците **Извикване** , **Заявка** и **Отмяна на одобрение** хвърлят изключения с неясни съобщения за грешки.</span><span class="sxs-lookup"><span data-stu-id="a043f-114">Fixed: **Recall** , **Request** , and **Cancel Approval** flows throw exceptions with unclear error messages.</span></span>
- <span data-ttu-id="a043f-115">Поправено: Когато **Отмяна на одобрение** не успее за разход, съответна грешка за изключение не се хвърля.</span><span class="sxs-lookup"><span data-stu-id="a043f-115">Fixed: When **Cancel Approval** fails for an expense, a relevant exception error is not thrown.</span></span>
- <span data-ttu-id="a043f-116">Поправено: Решетката за въвеждане на време неправилно обработва неработни дни в Австралия след превключването на лятното часово време (DST) през октомври.</span><span class="sxs-lookup"><span data-stu-id="a043f-116">Fixed: The Time Entry grid incorrectly handles non-working days in Australia after the daylight savings time (DST) switch in October.</span></span>
- <span data-ttu-id="a043f-117">Поправено: Неправилната логика по подразбиране предотвратява подаването на разходите.</span><span class="sxs-lookup"><span data-stu-id="a043f-117">Fixed: Incorrect defaulting logic prevents submission of expenses.</span></span>
- <span data-ttu-id="a043f-118">Поправено: Когато одобрението за времеви запис се провали, одобрението остава в състояние **В изчакване**.</span><span class="sxs-lookup"><span data-stu-id="a043f-118">Fixed: When time entry approval fails, the approval remains in a state of **Pending**.</span></span>
- <span data-ttu-id="a043f-119">Поправено: SQL грешки при групови одобрения (заключено/изтичане на времето).</span><span class="sxs-lookup"><span data-stu-id="a043f-119">Fixed: SQL Errors on bulk approvals (deadlock/timeout).</span></span>
- <span data-ttu-id="a043f-120">Поправено: Значителни проблеми с производителността в потребителското изживяване, причинени от актуализиране на членовете на екипа при одобряване на времеви записи.</span><span class="sxs-lookup"><span data-stu-id="a043f-120">Fixed: Significant performance issues in the user experience caused by updating team members while approving time entries.</span></span>

<span data-ttu-id="a043f-121">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="a043f-121">**Project Management**</span></span>

- <span data-ttu-id="a043f-122">Поправено: Известието за часовата зона е преместено от изгледа **Съгласуване** към основния формуляр **Проект**.</span><span class="sxs-lookup"><span data-stu-id="a043f-122">Fixed: Time zone notification moved from the **Reconciliation** view to the **Project** main form.</span></span>
- <span data-ttu-id="a043f-123">Поправено: Шаблонът на календара не се задава правилно по подразбиране, когато се отвори нов формуляр на проект.</span><span class="sxs-lookup"><span data-stu-id="a043f-123">Fixed: Calendar template is not correctly defaulting when a new project form opens.</span></span>
- <span data-ttu-id="a043f-124">Поправено: За браузъри, базирани на chromium, потребителите не могат лесно да избират предходни задачи, които да изтрият.</span><span class="sxs-lookup"><span data-stu-id="a043f-124">Fixed: For chromium-based browsers, users are unable to easily select predecessor tasks to delete.</span></span>
- <span data-ttu-id="a043f-125">Поправено: Създаване или копиране на **Проект от празен шаблон** извлича несвързани задания.</span><span class="sxs-lookup"><span data-stu-id="a043f-125">Fixed: Creating or copying **Project from Empty template** fetches unrelated assignments.</span></span>
- <span data-ttu-id="a043f-126">Поправено: В конкретни крайни случаи създаването на ново задание от мрежата на задачите води до създаване на дублирани записи.</span><span class="sxs-lookup"><span data-stu-id="a043f-126">Fixed: In specific edge cases, creating a new assignment from the task grid results in duplicate records being created.</span></span>
- <span data-ttu-id="a043f-127">Поправено: В ръчен режим потребителите не могат да актуализират началните дати на задачата да бъдат по-късни от текущата запаметена дата.</span><span class="sxs-lookup"><span data-stu-id="a043f-127">Fixed: In manual mode, users are unable to update task start dates to be later than the current date saved.</span></span>

<span data-ttu-id="a043f-128">**Управление на ресурси**</span><span class="sxs-lookup"><span data-stu-id="a043f-128">**Resource Management**</span></span>

- <span data-ttu-id="a043f-129">Поправено: Редът за междинна сума на изгледа **Съгласуване** неправилно изчислява отклонението на резервациите след удължаване на резервациите.</span><span class="sxs-lookup"><span data-stu-id="a043f-129">Fixed: **Reconciliation** view subtotal row incorrectly calculates bookings variance after extending bookings.</span></span>
- <span data-ttu-id="a043f-130">Поправено: Изгледът **Съгласуване** неправилно показва назначенията на ресурси, когато наличният ресурс има календар, който не съвпада с календара на проекта.</span><span class="sxs-lookup"><span data-stu-id="a043f-130">Fixed: **Reconciliation** view incorrectly displays resource assignments when the bookable resource has a calendar that does not match the project calendar.</span></span>

<span data-ttu-id="a043f-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="a043f-131">**Sales**</span></span>

- <span data-ttu-id="a043f-132">Поправено: Когато времевите записи се одобрят отново ( **Одобряване > Отмяна >** повторно одобряване) се създават дублирани действителни данни без възможност за таксуване.</span><span class="sxs-lookup"><span data-stu-id="a043f-132">Fixed: When time entries are re-approved ( **Approve > Cancel >** approve again), a duplicate non-chargeable actual is created.</span></span>
