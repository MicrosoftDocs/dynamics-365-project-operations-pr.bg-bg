---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 21, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 21, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 06/19/2020
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
ms.openlocfilehash: 69b592db7456bf11c2e933256569d726056d1a32
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280610"
---
# <a name="project-service-automation-update-release-21-v3"></a><span data-ttu-id="8cba5-103">Project Service Automation, издание на актуализация 21, V3</span><span class="sxs-lookup"><span data-stu-id="8cba5-103">Project Service Automation Update Release 21, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="8cba5-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="8cba5-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="8cba5-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="8cba5-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="8cba5-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="8cba5-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="8cba5-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="8cba5-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="8cba5-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="8cba5-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="8cba5-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 21.</span><span class="sxs-lookup"><span data-stu-id="8cba5-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 21.</span></span> <span data-ttu-id="8cba5-110">Тази версия има номер на компилацията V 3.10.32.50 и е общодостъпна чрез самоактуализация от юни 2020 г.</span><span class="sxs-lookup"><span data-stu-id="8cba5-110">This version has a build number of V 3.10.32.50 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-21"></a><span data-ttu-id="8cba5-111">Издание на актуализация 21</span><span class="sxs-lookup"><span data-stu-id="8cba5-111">Update Release 21</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="8cba5-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="8cba5-112">Bug fixes</span></span>

<span data-ttu-id="8cba5-113">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="8cba5-113">**Time and Expense**</span></span>

<span data-ttu-id="8cba5-114">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="8cba5-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="8cba5-115">При хостинг на **контролата за мрежа на запис за време** в таблата мрежата не използва пълната ширина на контейнера на мрежата на таблото.</span><span class="sxs-lookup"><span data-stu-id="8cba5-115">When hosting the **Time Entry Grid Control** in Dashboards, the grid does not utilize the full width of the dashboard grid container.</span></span>
- <span data-ttu-id="8cba5-116">За конкретни часови зони контролата на мрежата **Запис за време** не показва записи.</span><span class="sxs-lookup"><span data-stu-id="8cba5-116">For specific time zones, the **Time Entry** grid control does not display records.</span></span>
- <span data-ttu-id="8cba5-117">Записите за време, които са след 21:00 ч., се показват в грешния ден.</span><span class="sxs-lookup"><span data-stu-id="8cba5-117">Time entries that are after 9:00 PM appear on the wrong day.</span></span>
- <span data-ttu-id="8cba5-118">Потребителите не могат да подават разходи, ако категорията на разход **Необходима е разписка за разход** няма стойност.</span><span class="sxs-lookup"><span data-stu-id="8cba5-118">Users are unable to submit expenses if the expense category, **Expense receipt required** has no value.</span></span>

<span data-ttu-id="8cba5-119">**Управление на ресурси**</span><span class="sxs-lookup"><span data-stu-id="8cba5-119">**Resource Management**</span></span>

<span data-ttu-id="8cba5-120">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="8cba5-120">The following issues have been fixed:</span></span>

- <span data-ttu-id="8cba5-121">Неактивните резервации се показват в изгледа **Съгласуване**.</span><span class="sxs-lookup"><span data-stu-id="8cba5-121">Inactive bookings are displayed in the **Reconciliation** view.</span></span>
- <span data-ttu-id="8cba5-122">Изпълнението на общите ресурси няма валидиране, за да се гарантира, че съществува валидно състояние на резервация.</span><span class="sxs-lookup"><span data-stu-id="8cba5-122">Generic resource fulfillment was missing validation to ensure that a valid booking status exists.</span></span>

<span data-ttu-id="8cba5-123">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="8cba5-123">**Project Management**</span></span>

<span data-ttu-id="8cba5-124">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="8cba5-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="8cba5-125">Мрежите на формуляра **Проект** (**Присвояване на ресурс**, **Задача**, изглед **Съгласуване**, **Оценки на разходи**) остават редактируеми дори когато проектът не е активен.</span><span class="sxs-lookup"><span data-stu-id="8cba5-125">The **Project** form grids (**Resource Assignment**, **Task**, **Reconciliation** view, **Expense Estimates**) remain editable even when a project is not active.</span></span>
- <span data-ttu-id="8cba5-126">Дублиращите се клиенти не могат да се обединяват с клиенти, които са свързани с потвърдени договори по проект.</span><span class="sxs-lookup"><span data-stu-id="8cba5-126">Duplicate customers can't be merged with customers that are linked to confirmed project contracts.</span></span>
- <span data-ttu-id="8cba5-127">Когато се добави ресурс, който няма валиден календар, системата не връща лесно за използване съобщение за грешка.</span><span class="sxs-lookup"><span data-stu-id="8cba5-127">When a resource who does not have a valid calendar is added, the system does not return a user friendly-error message.</span></span>
- <span data-ttu-id="8cba5-128">Бутонът **Добавяне на задача** на мрежата на задача е активиран, когато проектът е свързан с **добавка на Microsoft Project**.</span><span class="sxs-lookup"><span data-stu-id="8cba5-128">The **Add Task** button on the task grid is enabled when the project is linked to **Microsoft Project add-in**.</span></span>
- <span data-ttu-id="8cba5-129">Усилието нараства неконтролируемо, когато задача с категория е присвоена към ресурс с роля, за която е определена себестойност.</span><span class="sxs-lookup"><span data-stu-id="8cba5-129">Effort grows uncontrollably when a task with a category is assigned to a resource with a role for which there is a cost price defined.</span></span>

<span data-ttu-id="8cba5-130">**Sales**</span><span class="sxs-lookup"><span data-stu-id="8cba5-130">**Sales**</span></span>

<span data-ttu-id="8cba5-131">Направени са следните подобрения:</span><span class="sxs-lookup"><span data-stu-id="8cba5-131">The following enhancements have been made:</span></span>

- <span data-ttu-id="8cba5-132">**Честота на фактура** и **Начало на фактуриране** са преместени в раздела **График на фактура**.</span><span class="sxs-lookup"><span data-stu-id="8cba5-132">**Invoice Frequency** and **Billing Start** have been moved to the **Invoice Schedule** tab.</span></span>

<span data-ttu-id="8cba5-133">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="8cba5-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="8cba5-134">**Обща цена на продажби** е нула (0) за **Категория**, въпреки че **Роля** е с обща цена на продажби, която не е нула.</span><span class="sxs-lookup"><span data-stu-id="8cba5-134">**Total Sales Price** is zero (0) for **Category** even though **Role** has a total sales price that is not zero.</span></span>
- <span data-ttu-id="8cba5-135">Клиентите не могат да променят стойността на полето **Състояние на фактура** на **Готово за фактуриране**, когато друг персонализиран процес актуализира допълнително поле.</span><span class="sxs-lookup"><span data-stu-id="8cba5-135">Customers can't change the value of the **Invoice Status** field to **Ready for invoicing** when another customized process is updating an additional field.</span></span>
- <span data-ttu-id="8cba5-136">Бутонът **Обновяване на редове на фактура** може да създаде няколко дублирани реда, ако се избере няколко пъти.</span><span class="sxs-lookup"><span data-stu-id="8cba5-136">The **Refresh Invoice Lines** button can create multiple duplicated lines if it is repeatedly selected.</span></span>
- <span data-ttu-id="8cba5-137">Бутонът **Актуализиране на цени** не работи в подмрежата **Цени на роля** във формуляра **Бърз преглед**.</span><span class="sxs-lookup"><span data-stu-id="8cba5-137">The **Update Prices** button doesn't work on the **Role Prices** subgrid in the **Quick View** form.</span></span>
- <span data-ttu-id="8cba5-138">Логиката **Резолюция на ценова листа за продажби** неправилно обработва часовите зони, което води до неправилен избор на ценови листи.</span><span class="sxs-lookup"><span data-stu-id="8cba5-138">The **Sales Price List Resolution** logic improperly handles time zones, resulting in the incorrect selection of price lists.</span></span>
- <span data-ttu-id="8cba5-139">**Обща действителна стойност** на проекта може да се намали с частична сума след одобрение на еднократен запис.</span><span class="sxs-lookup"><span data-stu-id="8cba5-139">A project’s **Total Actual Cost** can be off by a fractional amount after a single time entry is approved.</span></span>
- <span data-ttu-id="8cba5-140">Логиката **Резолюция на цена** не предоставя лесно за използване съобщение за грешка, ако **Извлечена RolePrice** няма стойности в полетата **„Основна единица”** и **„Цена в основна единица”**.</span><span class="sxs-lookup"><span data-stu-id="8cba5-140">The **Price Resolution** logic does not provide a user-friendly error message if **Retrieved RolePrice** doesn't have values in **'Primary Unit'** and **'Price In Primary Unit'** fields.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]