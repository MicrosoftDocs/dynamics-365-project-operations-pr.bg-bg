---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 26, V3
ms.openlocfilehash: 849e7288ee91d3e9360c0b03f6b8b37ff29338e7
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/25/2020
ms.locfileid: "4643250"
---
<a name="project-service-automation-update-release-26-v3"></a><span data-ttu-id="91b85-102">Project Service Automation, издание на актуализация 26, V3</span><span class="sxs-lookup"><span data-stu-id="91b85-102">Project Service Automation Update Release 26, V3</span></span>
================================================

<span data-ttu-id="91b85-103">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="91b85-103">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="91b85-104">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="91b85-104">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="91b85-105">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="91b85-105">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="91b85-106">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="91b85-106">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="91b85-107">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="91b85-107">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="91b85-108">Тази тема изброява функциите и корекциите, които са нови или променени за актуализацията на Project Service Automation, издание 26, V3.</span><span class="sxs-lookup"><span data-stu-id="91b85-108">This topic lists the features and fixes that are new or changed for Project Service Automation Update Release 26, V3.</span></span> <span data-ttu-id="91b85-109">Тази версия има номер на компилация V3.10.44.59 и е общодостъпно чрез самостоятелна актуализация от декември 2020 г.</span><span class="sxs-lookup"><span data-stu-id="91b85-109">This version has a build number of V3.10.44.59 and is generally available through a self-update in December 2020.</span></span>

<a name="update-release-26"></a><span data-ttu-id="91b85-110">Издание на актуализация 26</span><span class="sxs-lookup"><span data-stu-id="91b85-110">Update Release 26</span></span>
-----------------

### <a name="bug-fixes"></a><span data-ttu-id="91b85-111">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="91b85-111">Bug fixes</span></span>

<span data-ttu-id="91b85-112">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="91b85-112">**Time and Expense**</span></span>

<span data-ttu-id="91b85-113">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="91b85-113">The following issues have been fixed:</span></span>

-   <span data-ttu-id="91b85-114">Потребителите могат да променят задачата в запис за време, който е одобрен/подаден.</span><span class="sxs-lookup"><span data-stu-id="91b85-114">Users are able to change the task on a time entry that has been approved/submitted.</span></span>

-   <span data-ttu-id="91b85-115">Грешка „Не е зададена препратка към обект“ при записване на запис за време.</span><span class="sxs-lookup"><span data-stu-id="91b85-115">"Object Reference Not Set" error when saving time entry.</span></span>

-   <span data-ttu-id="91b85-116">Импортирането на запис за време от присвояване на ресурси създава записи за време с неправилни стойности на DateTime.</span><span class="sxs-lookup"><span data-stu-id="91b85-116">Time entry import from resource assignments creates time entries with the incorrect DateTime values.</span></span>

-   <span data-ttu-id="91b85-117">Когато са инсталирани Project Service Automation и приложението Field Service, бутонът **Нов** се показва два пъти в командната лента за записи за време в приложението Field Service.</span><span class="sxs-lookup"><span data-stu-id="91b85-117">When Project Service Automation and the Field Service app are both installed, the **New** button is displaying twice on the command bar for time entries in the Field Service app.</span></span>

-   <span data-ttu-id="91b85-118">Актуализациите на клетки **Разрешаване на единица** и **Опаковъчна единица** вече работят в мрежата **Оценки на разходи**.</span><span class="sxs-lookup"><span data-stu-id="91b85-118">**Allow Unit** and **Unit group** cells updates now work on the **Expense Estimates** grid.</span></span>

-   <span data-ttu-id="91b85-119">Формулярът **Актуализиране на редактиране на запис за време** включва **Времева линия**.</span><span class="sxs-lookup"><span data-stu-id="91b85-119">**Update Time Entry Edit** form includes **Timeline**.</span></span>

-   <span data-ttu-id="91b85-120">Одобрението на времето за несвързани с проекта записи за време блокира системата при търсене на роля на одобряващ на проект.</span><span class="sxs-lookup"><span data-stu-id="91b85-120">Time approval for non-project time entries blocks the system when searching for a project approver role.</span></span>

<span data-ttu-id="91b85-121">**Управление на ресурси**</span><span class="sxs-lookup"><span data-stu-id="91b85-121">**Resource Management**</span></span>

<span data-ttu-id="91b85-122">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="91b85-122">The following issues have been fixed:</span></span>

-   <span data-ttu-id="91b85-123">Добавена е проверка в добавката **PostProjectCreate**, за да проверява основно изискване, преди да създадете такова.</span><span class="sxs-lookup"><span data-stu-id="91b85-123">Added validation in the **PostProjectCreate** plug-in to check for a primary requirement before creating one.</span></span>

-   <span data-ttu-id="91b85-124">Формулярът за бързо създаване **Член на екип на проект** връща изключение за нулева препратка, ако се премахнат полета от формуляра.</span><span class="sxs-lookup"><span data-stu-id="91b85-124">**Project Team Member** quick create form throws a null reference exception if fields are removed from the form.</span></span>

-   <span data-ttu-id="91b85-125">Генерирането на изисквания за 12 часа в продължение на 1 година ще е неуспешно.</span><span class="sxs-lookup"><span data-stu-id="91b85-125">Generate requirements for 12 hours over 1 year will fail.</span></span>

-   <span data-ttu-id="91b85-126">Подобрено съобщение за грешка за изключение за нулева препратка при създаване на изискване за ресурс.</span><span class="sxs-lookup"><span data-stu-id="91b85-126">Improved error message null reference exception during resource requirement creation.</span></span>

<span data-ttu-id="91b85-127">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="91b85-127">**Project Management**</span></span>

<span data-ttu-id="91b85-128">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="91b85-128">The following issues have been fixed:</span></span>

-   <span data-ttu-id="91b85-129">Подобрена проверка за справяне с изключение за нулева препратка, генерирано в добавката **PreProjectUpdate**.</span><span class="sxs-lookup"><span data-stu-id="91b85-129">Improved validation to address null reference exception generated in the **PreProjectUpdate** plug-in.</span></span>

-   <span data-ttu-id="91b85-130">Проекти, публикувани от добавката за настолни компютри на Microsoft Project, изтриват неприсвоени задачи.</span><span class="sxs-lookup"><span data-stu-id="91b85-130">Projects published by the Microsoft Project desktop add-in delete unassigned assignments.</span></span>

-   <span data-ttu-id="91b85-131">Добавена е нова проверка, когато препратката към проект на задача е невалидна поради изключение за нулева препратка в добавката **PreValidateProjectTaskUpdate**.</span><span class="sxs-lookup"><span data-stu-id="91b85-131">Added new validation when a task’s project reference is invalid due to null reference exception in **PreValidateProjectTaskUpdate** plug-in.</span></span>

-   <span data-ttu-id="91b85-132">Мрежата на член на екипа не показва различни присвоявания в записа на члена на екипа.</span><span class="sxs-lookup"><span data-stu-id="91b85-132">Team Member grid does not show distinct assignments on the team member record.</span></span>

-   <span data-ttu-id="91b85-133">Добавени са нови съобщения за проверка и грешки поради изключение за нулева препратка в добавката **PreProjectTaskDelete**.</span><span class="sxs-lookup"><span data-stu-id="91b85-133">Added new validation and error messages due to null reference exception in **PreProjectTaskDelete** plug-in.</span></span>

<span data-ttu-id="91b85-134">**Sales**</span><span class="sxs-lookup"><span data-stu-id="91b85-134">**Sales**</span></span>

<span data-ttu-id="91b85-135">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="91b85-135">The following issues have been fixed:</span></span>

-   <span data-ttu-id="91b85-136">Когато избирате базиран на проект ред в оферта или договор, бутонът **Предложение** трябва да се вижда само при избор на базиран на продукт ред, свързан със съществуващ продукт.</span><span class="sxs-lookup"><span data-stu-id="91b85-136">When selecting a project-based line in quote or contract, the **Suggestion** button should only be visible when selecting a product-based line associated with an existing product.</span></span>

-   <span data-ttu-id="91b85-137">Разделете привилегията **Create_Product** от привилегията **Create_ProjectContract**.</span><span class="sxs-lookup"><span data-stu-id="91b85-137">Split **Create_Product** privilege from **Create_ProjectContract** privilege.</span></span>

-   <span data-ttu-id="91b85-138">Изтриването на ред за фактура води до грешка поради нулева препратка в **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span><span class="sxs-lookup"><span data-stu-id="91b85-138">Deleting an invoice line causes null reference failure on **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span></span>
