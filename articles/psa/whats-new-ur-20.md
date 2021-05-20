---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 20, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation, издание на актуализация 20, V3
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 06/12/2020
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
ms.openlocfilehash: 124dad5438f9489d1ddbc952cecaee977b6b7f01
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949081"
---
# <a name="project-service-automation-update-release-20-v3"></a><span data-ttu-id="91a5a-103">Project Service Automation, издание на актуализация 20, V3</span><span class="sxs-lookup"><span data-stu-id="91a5a-103">Project Service Automation Update Release 20, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="91a5a-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="91a5a-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="91a5a-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="91a5a-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="91a5a-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="91a5a-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="91a5a-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="91a5a-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="91a5a-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="91a5a-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="91a5a-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 20.</span><span class="sxs-lookup"><span data-stu-id="91a5a-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 20.</span></span> <span data-ttu-id="91a5a-110">Тази версия има номер на компилацията V 3.10.31.37 и е общодостъпна чрез самоактуализация от юни 2020 г.</span><span class="sxs-lookup"><span data-stu-id="91a5a-110">This version has a build number of V 3.10.31.37 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-20"></a><span data-ttu-id="91a5a-111">Издание на актуализация 20</span><span class="sxs-lookup"><span data-stu-id="91a5a-111">Update Release 20</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="91a5a-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="91a5a-112">Bug fixes</span></span>

<span data-ttu-id="91a5a-113">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="91a5a-113">**Project Management**</span></span>

<span data-ttu-id="91a5a-114">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="91a5a-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="91a5a-115">Импортирането на членове на екипа на проект с метод за разпределение, който изисква часове, води до неясно съобщение за грешка, когато указаните часове са нула.</span><span class="sxs-lookup"><span data-stu-id="91a5a-115">Importing project team members with an allocation method that requires hours results in an unclear error message when the specified hours are zero.</span></span>
- <span data-ttu-id="91a5a-116">Потребителите получават неправилна грешка, когато са въведени максимален брой знаци в полето **Описание** за задача от проект.</span><span class="sxs-lookup"><span data-stu-id="91a5a-116">Users receive an incorrect error when the maximum number of characters have been entered into the **Description** field for a project task.</span></span>
- <span data-ttu-id="91a5a-117">Страницата **Изтегляне на добавката Microsoft Dynamics 365 Project Service Automation** пренасочва към страницата за изтегляне на английски език, когато езиковите настройки на потребителя са настроени на японски.</span><span class="sxs-lookup"><span data-stu-id="91a5a-117">The **Microsoft Dynamics 365 Project Service Automation add-in download** page redirects to the English download page when the user’s language settings are set to Japanese.</span></span>
- <span data-ttu-id="91a5a-118">Когато възникне грешка в сървъра, етикетът за синхронизация на раздела **График** на формуляра **Проекти** понякога остава.</span><span class="sxs-lookup"><span data-stu-id="91a5a-118">When a server error occurs, the synchronization label on the **Schedule** tab of the **Projects** form sometimes remains.</span></span>
- <span data-ttu-id="91a5a-119">Към сървъра се изпращат излишни актуализации на задача при промяна на задача.</span><span class="sxs-lookup"><span data-stu-id="91a5a-119">Redundant task updates are being sent to the server when a task is modified.</span></span>

<span data-ttu-id="91a5a-120">**Sales**</span><span class="sxs-lookup"><span data-stu-id="91a5a-120">**Sales**</span></span>

<span data-ttu-id="91a5a-121">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="91a5a-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="91a5a-122">Във формуляра **Договор** двукратното щракване върху **Създаване на фактура** създава две фактури за един запис на действителни данни.</span><span class="sxs-lookup"><span data-stu-id="91a5a-122">On the **Contract** form, double-clicking **Create Invoice** creates two invoices for a single actuals record.</span></span>
- <span data-ttu-id="91a5a-123">В Internet Explorer 11 потребителите не могат да създават записи за разходи.</span><span class="sxs-lookup"><span data-stu-id="91a5a-123">In Internet Explorer 11, users are unable to create expense entries.</span></span>
- <span data-ttu-id="91a5a-124">Сторнирането на разходи и сторнирането на действителни данни за нефактурирани продажби не са свързани.</span><span class="sxs-lookup"><span data-stu-id="91a5a-124">Reversal of Cost and reversal of Unbilled Sales Actuals are not linked.</span></span>
- <span data-ttu-id="91a5a-125">Бутонът **Обновяване на действителните данни** във формуляра **Проект** не обновява **Действителни часове за задача**.</span><span class="sxs-lookup"><span data-stu-id="91a5a-125">The **Refresh Actuals** button on the **Project** form does not refresh **Task Actual Hours**.</span></span>
- <span data-ttu-id="91a5a-126">Добавката **PreValidateProjectTeamMemberCreate** може да създава дублирани общи налични ресурси, когато атрибутът **msdyn_isgenericresourceprojectscoped** е зададен на **False**.</span><span class="sxs-lookup"><span data-stu-id="91a5a-126">The **PreValidateProjectTeamMemberCreate** plug-in can create duplicate generic bookable resources when the attribute **msdyn_isgenericresourceprojectscoped** is set to **False**.</span></span>
- <span data-ttu-id="91a5a-127">**Преизчисляване** изчиства платимите разходи от подробностите за ред на базирана на продукти оферта и подробностите за аспект на договор.</span><span class="sxs-lookup"><span data-stu-id="91a5a-127">**Recalculate** clears chargeable costs of product-based quote line details and contract line details.</span></span>
- <span data-ttu-id="91a5a-128">В конкретни сценарии добавката **PostEstimateLineUpdate** показва грешка на изключение за нулева препратка.</span><span class="sxs-lookup"><span data-stu-id="91a5a-128">In specific scenarios, the **PostEstimateLineUpdate** plug-in displays a null teference exception error.</span></span>
- <span data-ttu-id="91a5a-129">Продължителността на времевата фаза в **Таблица за анализ на рентабилността** не съвпада с продължителността на разходите в подробностите за реда на офертата с фиксирана цена.</span><span class="sxs-lookup"><span data-stu-id="91a5a-129">Time phase duration on the **Profitability Analysis Chart** does not match duration of the costs in the fixed-price quote line detail of the quote.</span></span>
- <span data-ttu-id="91a5a-130">Стойностите по подразбиране на единиците и опаковъчните единици не са правилни за категориите разходи във формулярите **Подробности за аспект на договор** и **Подробности за ред на оферта**.</span><span class="sxs-lookup"><span data-stu-id="91a5a-130">Unit and unit group values do not default correctly for expense categories on the **Contract Line Details** and **Quote Line Details** forms.</span></span>
- <span data-ttu-id="91a5a-131">Списъците **Себестойност на организационна единица** разрешават припокривания в ефективността на датите.</span><span class="sxs-lookup"><span data-stu-id="91a5a-131">**Org Unit Cost Price** lists permit overlaps in the date effectivity.</span></span>
- <span data-ttu-id="91a5a-132">Потребителите нямат право да променят **OrgUnit**, когато типът поръчка не е базирана на работа, тъй като ще доведе до грешка на изключение за нулева препратка.</span><span class="sxs-lookup"><span data-stu-id="91a5a-132">Users are not permitted to change the **OrgUnit** when the order type is not work-based because it will lead to a null reference exception error.</span></span>
- <span data-ttu-id="91a5a-133">При опит за навигиране от формуляра **Подробности за ред на оферта** обратно към раздела **Оферта** формулярът се обновява и се показва разделът **Обобщение**.</span><span class="sxs-lookup"><span data-stu-id="91a5a-133">When attempting to navigate from the **Quote Line Details** form, back to the **Quote** tab, the form refreshes and displays the **Summary** tab.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]