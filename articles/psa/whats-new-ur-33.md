---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 33, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 33, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/30/2021
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
ms.openlocfilehash: 2c96e4abd484bb66285421baaad82ead9589bbe9
ms.sourcegitcommit: be5beba71ee9770c0083b4fe5cc89e7ec6b741b8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334503"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-33-v3"></a><span data-ttu-id="a4e2a-103">Какво е новото или промененото в Project Service Automation, издание на актуализация 33, V3</span><span class="sxs-lookup"><span data-stu-id="a4e2a-103">What's new or changed in Project Service Automation Update Release 33, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="a4e2a-104">С удоволствие обявяваме най-новата актуализация за приложението Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="a4e2a-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="a4e2a-106">Съвместим е с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="a4e2a-107">За да актуализирате до тази версия, посетете страницата на центъра за администриране за решенията на Dynamics 365 Online и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="a4e2a-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="a4e2a-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="a4e2a-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 33.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 33.</span></span> <span data-ttu-id="a4e2a-110">Тази версия има номер на компилация V3.10.54.98 и обикновено се предлага чрез самообновяване през юли 2021 г.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-110">This version has a build number of V3.10.54.98 and is generally available through a self-update in July 2021.</span></span>

## <a name="update-release-33"></a><span data-ttu-id="a4e2a-111">Издание на актуализация 33</span><span class="sxs-lookup"><span data-stu-id="a4e2a-111">Update Release 33</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="a4e2a-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="a4e2a-112">Bug fixes</span></span>

<span data-ttu-id="a4e2a-113">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="a4e2a-113">**Time and Expense**</span></span>

<span data-ttu-id="a4e2a-114">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="a4e2a-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="a4e2a-115">Две заключени полета, **msdyn_description** и **msdyn_externaldescription** могат да се редактират след подаване.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-115">Two locked fields, **msdyn_description** and **msdyn_externaldescription** are editable after submission.</span></span>
- <span data-ttu-id="a4e2a-116">Съобщение за грешка се появява, ако се създаде разход, който не е свързан с проект.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-116">An error message occurs if an expense is created that isn't related to a project.</span></span>
- <span data-ttu-id="a4e2a-117">Когато се създаде запис на време, ролята на ресурса по подразбиране е неактивна роля.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-117">When a time entry is created, the resource role defaults to an inactive role.</span></span>
- <span data-ttu-id="a4e2a-118">Счетоводни записи, свързани с извикан и изтрит разход, не се изтриват.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-118">Journal lines associated with a recalled and deleted expense aren't deleted.</span></span>
- <span data-ttu-id="a4e2a-119">Във **Въвеждане на време Бързо създаване на формуляр**, актуализирайте **Списък на проектните задачи** изглед, за да промените датата, показана по подразбиране, на началната дата на задачата.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-119">On the **Time entry Quick Create Form**, update the **Project Task List** view to change the date displayed by default to the start date of the task.</span></span>
- <span data-ttu-id="a4e2a-120">Когато създавате запис на време от раздел **Свързани** за наличния ресурс, записът за време е създаден неправилно за влезлия потребител вместо за родителския наличен ресурс.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-120">When you create a time entry from the **Related** tab of the bookable resource, the time entry is incorrectly created for the signed-in user instead of the parent bookable resource.</span></span>
- <span data-ttu-id="a4e2a-121">Новите полета се добавят към **Групово одобрение MDD** диалогов прозорец.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-121">New fields are added to the **Bulk approval MDD** dialog box.</span></span>

<span data-ttu-id="a4e2a-122">**Планиране на проект**</span><span class="sxs-lookup"><span data-stu-id="a4e2a-122">**Project planning**</span></span>

<span data-ttu-id="a4e2a-123">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="a4e2a-123">The following issues have been fixed:</span></span>
- <span data-ttu-id="a4e2a-124">Бавна производителност на създаване на проекти, когато се прилагат шаблони за работно време на проекта със сложни календари.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-124">Slow project creation performance when project work hour templates are applied with complex calendars.</span></span>
- <span data-ttu-id="a4e2a-125">Когато началната дата е по-голяма от крайната дата, в шаблона на проекта за копиране се появява грешка поради разлики във времевия компонент на всяко поле.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-125">When the start date is greater than the end date, an error displays on the copy project template because of differences in the time component of each field.</span></span>

<span data-ttu-id="a4e2a-126">**Управление на ресурси**</span><span class="sxs-lookup"><span data-stu-id="a4e2a-126">**Resource management**</span></span>

<span data-ttu-id="a4e2a-127">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="a4e2a-127">The following issues have been fixed:</span></span>
- <span data-ttu-id="a4e2a-128">Неправилен параметър се използва в заявката за използване на ресурса и XML води до неправилни резултати от филтъра на мрежа **Използване на ресурсите**.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-128">An incorrect parameter is used in the resource utilization query and the XML leads to incorrect filter results on the **Resource Utilization** grid.</span></span>
- <span data-ttu-id="a4e2a-129">Потвърждението **Удължете резервациите** показва неправилна крайна дата за резервации.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-129">The **Extend Bookings** confirmation displays incorrect end date for bookings.</span></span>

<span data-ttu-id="a4e2a-130">**Продажби**</span><span class="sxs-lookup"><span data-stu-id="a4e2a-130">**Sales**</span></span>

<span data-ttu-id="a4e2a-131">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="a4e2a-131">The following issues have been fixed:</span></span>
- <span data-ttu-id="a4e2a-132">Възниква съобщение за грешка, ако се създаде цена на категория с липсващи стойности.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-132">An error message occurs if a category price is created with missing values.</span></span>
- <span data-ttu-id="a4e2a-133">Възниква съобщение за грешка, ако крайният етап на договора е създаден без ред за поръчка.</span><span class="sxs-lookup"><span data-stu-id="a4e2a-133">An error message occurs if a contract line milestone is created without an order line.</span></span>
