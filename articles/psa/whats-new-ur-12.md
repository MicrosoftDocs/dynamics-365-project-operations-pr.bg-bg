---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 12, V3
description: Тази тема предоставя информация за новостите в актуализацията на Project Service Automation, издание 12, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: fc92a5dcc111688159f9be5b2839b7c040404a3b
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4119945"
---
# <a name="project-service-automation-update-release-12-v3"></a><span data-ttu-id="191bc-103">Project Service Automation, издание на актуализация 12, V3</span><span class="sxs-lookup"><span data-stu-id="191bc-103">Project Service Automation Update Release 12, V3</span></span>
<span data-ttu-id="191bc-104">С удоволствие съобщаваме за най-новата актуализация за приложението Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="191bc-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="191bc-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="191bc-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="191bc-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="191bc-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="191bc-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online и отидете на страницата с решения, за да инсталирате актуализацията.</span><span class="sxs-lookup"><span data-stu-id="191bc-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="191bc-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="191bc-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="191bc-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 12.</span><span class="sxs-lookup"><span data-stu-id="191bc-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 12.</span></span> <span data-ttu-id="191bc-110">Тази версия е с номер на компилация V3.10.2.34 и е общодостъпна за самостоятелно актуализиране от октомври 2019 г.</span><span class="sxs-lookup"><span data-stu-id="191bc-110">This version has a build number of V3.10.2.34 and is generally available through a self-update in October 2019.</span></span>

## <a name="update-release-12"></a><span data-ttu-id="191bc-111">Издание на актуализация 12</span><span class="sxs-lookup"><span data-stu-id="191bc-111">Update Release 12</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="191bc-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="191bc-112">Bug fixes</span></span>

- <span data-ttu-id="191bc-113">Време и разход</span><span class="sxs-lookup"><span data-stu-id="191bc-113">Time and Expense</span></span>

    - <span data-ttu-id="191bc-114">Поправено: Съобщенията за грешки при запис за време са актуализирани с по-подходящ контекст.</span><span class="sxs-lookup"><span data-stu-id="191bc-114">Fixed: Time entry error messaging has been updated with more relevant context.</span></span>
    - <span data-ttu-id="191bc-115">Поправено: Мрежата и графикът на записите за време правилно показват вертикалната лента за превъртане, когато е необходимо.</span><span class="sxs-lookup"><span data-stu-id="191bc-115">Fixed: Time entry grid and schedule correctly displays the vertical scrollbar when required.</span></span>
    - <span data-ttu-id="191bc-116">Поправено: Подадени записи за разход и време могат да се одобряват.</span><span class="sxs-lookup"><span data-stu-id="191bc-116">Fixed: Submitted expense and time entries can be approved.</span></span>
    - <span data-ttu-id="191bc-117">Поправено: Съобщението в диалоговия прозорец за потвърждение на отмяна на одобрение е коригиран, така че да отразява състоянието на одобрението при промяна от **Одобрено** на **Подадено**.</span><span class="sxs-lookup"><span data-stu-id="191bc-117">Fixed: Cancel approval confirmation dialog message has been corrected to reflect the status of the approval when changed from **Approved** to **Submitted**.</span></span>
    - <span data-ttu-id="191bc-118">Поправено: Полетата **Цена**, **Единица** и **Количество** вече са заключени в записа на разход след одобрението му.</span><span class="sxs-lookup"><span data-stu-id="191bc-118">Fixed: **Price**, **Unit**, and **Quantity** fields are now locked on the Expense record after it is has been approved.</span></span>

- <span data-ttu-id="191bc-119">Управление на проекти</span><span class="sxs-lookup"><span data-stu-id="191bc-119">Project Management</span></span>

    - <span data-ttu-id="191bc-120">Поправено: Действието **Създаване** в основния формуляр **Член на екипа** е премахнато.</span><span class="sxs-lookup"><span data-stu-id="191bc-120">Fixed: **New** action on **Team member** main form has been removed.</span></span>
    - <span data-ttu-id="191bc-121">Поправено: Присвояванията на ресурси са актуализирани, за да отчитат грешки при неточно закръгляване, които водят до промяна на крайната дата на задача.</span><span class="sxs-lookup"><span data-stu-id="191bc-121">Fixed: Resource assignments have been updated to account for inaccurate rounding errors, which lead to a shift in a task’s end date.</span></span>
    - <span data-ttu-id="191bc-122">Поправено: В мрежата на задачата уместните грешки от страна на сървъра се извеждат за потребителя.</span><span class="sxs-lookup"><span data-stu-id="191bc-122">Fixed: In the task grid, relevant server-side errors will be surfaced to the user.</span></span>
    - <span data-ttu-id="191bc-123">Поправено: Името на члена на екипа вече се рендира в инструмента за избор на хора вместо името на позицията.</span><span class="sxs-lookup"><span data-stu-id="191bc-123">Fixed: The team member’s name now renders in the task people picker instead of the position name.</span></span>

- <span data-ttu-id="191bc-124">Управление на ресурс</span><span class="sxs-lookup"><span data-stu-id="191bc-124">Resource Management</span></span>

    - <span data-ttu-id="191bc-125">Поправено: Подробностите за изискване за ресурс за проекти, създадени от шаблон, вече използват календара на проекта.</span><span class="sxs-lookup"><span data-stu-id="191bc-125">Fixed: Resource requirement details for projects created from a template now use the project calendar.</span></span>
    - <span data-ttu-id="191bc-126">Поправено: Уменията и компетенциите по подразбиране вече са от главни данни за роля до изискването за ресурс, създадено за тази роля.</span><span class="sxs-lookup"><span data-stu-id="191bc-126">Fixed: Skills and competencies now default from role master data to the resource requirement created for that role.</span></span>

- <span data-ttu-id="191bc-127">Sales</span><span class="sxs-lookup"><span data-stu-id="191bc-127">Sales</span></span>

    - <span data-ttu-id="191bc-128">Поправено: Открити са дублирани ИД на обекти в основния формуляр **Договор**.</span><span class="sxs-lookup"><span data-stu-id="191bc-128">Fixed: Duplicate object IDs found on the **Contract main** form.</span></span>
    - <span data-ttu-id="191bc-129">Поправено: Логиката е актуализирана, за да се вижда раздела **Анализ на оферта**, така че да показва настройката на метаданните на раздела.</span><span class="sxs-lookup"><span data-stu-id="191bc-129">Fixed: Logic has been updated to make the **Quote Analysis** tab visible so that it displays the metadata setup of the tab.</span></span>
    - <span data-ttu-id="191bc-130">Поправено: Датата на осчетоводяване на действителния запис сега идва от датата на записа за време/разход, а не от датата на одобрението.</span><span class="sxs-lookup"><span data-stu-id="191bc-130">Fixed: Accounting date on the actual record now comes from the date of the time/expense entry date and not the date of the approval.</span></span>
