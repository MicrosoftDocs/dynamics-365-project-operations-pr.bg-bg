---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 26, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 26, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/12/2021
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
ms.openlocfilehash: 6aafe66fe8c63dc886455a36e93f32d4a581d5cc
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005553"
---
# <a name="project-service-automation-update-release-26-v3"></a><span data-ttu-id="95a23-103">Project Service Automation, издание на актуализация 26, V3</span><span class="sxs-lookup"><span data-stu-id="95a23-103">Project Service Automation Update Release 26, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="95a23-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="95a23-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="95a23-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="95a23-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="95a23-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="95a23-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="95a23-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="95a23-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="95a23-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="95a23-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="95a23-109">Тази тема изброява функциите и корекциите, които са нови или променени за актуализацията на Project Service Automation, издание 26, V3.</span><span class="sxs-lookup"><span data-stu-id="95a23-109">This topic lists the features and fixes that are new or changed for Project Service Automation Update Release 26, V3.</span></span> <span data-ttu-id="95a23-110">Тази версия има номер на компилация V3.10.44.59 и е общодостъпно чрез самостоятелна актуализация от декември 2020 г.</span><span class="sxs-lookup"><span data-stu-id="95a23-110">This version has a build number of V3.10.44.59 and is generally available through a self-update in December 2020.</span></span>

## <a name="update-release-26"></a><span data-ttu-id="95a23-111">Издание на актуализация 26</span><span class="sxs-lookup"><span data-stu-id="95a23-111">Update Release 26</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="95a23-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="95a23-112">Bug fixes</span></span>

<span data-ttu-id="95a23-113">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="95a23-113">**Time and Expense**</span></span>

<span data-ttu-id="95a23-114">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="95a23-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="95a23-115">Потребителите могат да променят задачата в запис за време, който е одобрен/подаден.</span><span class="sxs-lookup"><span data-stu-id="95a23-115">Users are able to change the task on a time entry that has been approved/submitted.</span></span>
- <span data-ttu-id="95a23-116">Грешка „Не е зададена препратка към обект“ при записване на запис за време.</span><span class="sxs-lookup"><span data-stu-id="95a23-116">"Object Reference Not Set" error when saving time entry.</span></span>
- <span data-ttu-id="95a23-117">Импортирането на запис за време от присвояване на ресурси създава записи за време с неправилни стойности на DateTime.</span><span class="sxs-lookup"><span data-stu-id="95a23-117">Time entry import from resource assignments creates time entries with the incorrect DateTime values.</span></span>
- <span data-ttu-id="95a23-118">Когато са инсталирани Project Service Automation и приложението Field Service, бутонът **Нов** се показва два пъти в командната лента за записи за време в приложението Field Service.</span><span class="sxs-lookup"><span data-stu-id="95a23-118">When Project Service Automation and the Field Service app are both installed, the **New** button is displaying twice on the command bar for time entries in the Field Service app.</span></span>
- <span data-ttu-id="95a23-119">Актуализациите на клетки **Разрешаване на единица** и **Опаковъчна единица** вече работят в мрежата **Оценки на разходи**.</span><span class="sxs-lookup"><span data-stu-id="95a23-119">**Allow Unit** and **Unit group** cells updates now work on the **Expense Estimates** grid.</span></span>
- <span data-ttu-id="95a23-120">Формулярът **Актуализиране на редактиране на запис за време** включва **Времева линия**.</span><span class="sxs-lookup"><span data-stu-id="95a23-120">**Update Time Entry Edit** form includes **Timeline**.</span></span>
- <span data-ttu-id="95a23-121">Одобрението на времето за несвързани с проекта записи за време блокира системата при търсене на роля на одобряващ на проект.</span><span class="sxs-lookup"><span data-stu-id="95a23-121">Time approval for non-project time entries blocks the system when searching for a project approver role.</span></span>

<span data-ttu-id="95a23-122">**Управление на ресурси**</span><span class="sxs-lookup"><span data-stu-id="95a23-122">**Resource Management**</span></span>

<span data-ttu-id="95a23-123">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="95a23-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="95a23-124">Добавена е проверка в добавката **PostProjectCreate**, за да проверява основно изискване, преди да създадете такова.</span><span class="sxs-lookup"><span data-stu-id="95a23-124">Added validation in the **PostProjectCreate** plug-in to check for a primary requirement before creating one.</span></span>
- <span data-ttu-id="95a23-125">Формулярът за бързо създаване **Член на екип на проект** връща изключение за нулева препратка, ако се премахнат полета от формуляра.</span><span class="sxs-lookup"><span data-stu-id="95a23-125">**Project Team Member** quick create form throws a null reference exception if fields are removed from the form.</span></span>
- <span data-ttu-id="95a23-126">Генерирането на изисквания за 12 часа в продължение на 1 година ще е неуспешно.</span><span class="sxs-lookup"><span data-stu-id="95a23-126">Generate requirements for 12 hours over 1 year will fail.</span></span>
- <span data-ttu-id="95a23-127">Подобрено съобщение за грешка за изключение за нулева препратка при създаване на изискване за ресурс.</span><span class="sxs-lookup"><span data-stu-id="95a23-127">Improved error message null reference exception during resource requirement creation.</span></span>

<span data-ttu-id="95a23-128">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="95a23-128">**Project Management**</span></span>

<span data-ttu-id="95a23-129">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="95a23-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="95a23-130">Подобрена проверка за справяне с изключение за нулева препратка, генерирано в добавката **PreProjectUpdate**.</span><span class="sxs-lookup"><span data-stu-id="95a23-130">Improved validation to address null reference exception generated in the **PreProjectUpdate** plug-in.</span></span>
- <span data-ttu-id="95a23-131">Проекти, публикувани от добавката за настолни компютри на Microsoft Project, изтриват неприсвоени задачи.</span><span class="sxs-lookup"><span data-stu-id="95a23-131">Projects published by the Microsoft Project desktop add-in delete unassigned assignments.</span></span>
- <span data-ttu-id="95a23-132">Добавена е нова проверка, когато препратката към проект на задача е невалидна поради изключение за нулева препратка в добавката **PreValidateProjectTaskUpdate**.</span><span class="sxs-lookup"><span data-stu-id="95a23-132">Added new validation when a task’s project reference is invalid due to null reference exception in **PreValidateProjectTaskUpdate** plug-in.</span></span>
- <span data-ttu-id="95a23-133">Мрежата на член на екипа не показва различни присвоявания в записа на члена на екипа.</span><span class="sxs-lookup"><span data-stu-id="95a23-133">Team Member grid does not show distinct assignments on the team member record.</span></span>
- <span data-ttu-id="95a23-134">Добавени са нови съобщения за проверка и грешки поради изключение за нулева препратка в добавката **PreProjectTaskDelete**.</span><span class="sxs-lookup"><span data-stu-id="95a23-134">Added new validation and error messages due to null reference exception in **PreProjectTaskDelete** plug-in.</span></span>

<span data-ttu-id="95a23-135">**Sales**</span><span class="sxs-lookup"><span data-stu-id="95a23-135">**Sales**</span></span>

<span data-ttu-id="95a23-136">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="95a23-136">The following issues have been fixed:</span></span>

- <span data-ttu-id="95a23-137">Когато избирате базиран на проект ред в оферта или договор, бутонът **Предложение** трябва да се вижда само при избор на базиран на продукт ред, свързан със съществуващ продукт.</span><span class="sxs-lookup"><span data-stu-id="95a23-137">When selecting a project-based line in quote or contract, the **Suggestion** button should only be visible when selecting a product-based line associated with an existing product.</span></span>
- <span data-ttu-id="95a23-138">Разделете привилегията **Create_Product** от привилегията **Create_ProjectContract**.</span><span class="sxs-lookup"><span data-stu-id="95a23-138">Split **Create_Product** privilege from **Create_ProjectContract** privilege.</span></span>
- <span data-ttu-id="95a23-139">Изтриването на ред за фактура води до грешка поради нулева препратка в **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span><span class="sxs-lookup"><span data-stu-id="95a23-139">Deleting an invoice line causes null reference failure on **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]