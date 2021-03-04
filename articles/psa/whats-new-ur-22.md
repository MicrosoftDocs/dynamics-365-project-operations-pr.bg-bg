---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 22, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 22, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 07/28/2020
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
ms.openlocfilehash: db4cbb9f9daadcb1911325f8bee987d5e480e1cf
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150970"
---
# <a name="project-service-automation-update-release-22-v3"></a><span data-ttu-id="521b8-103">Project Service Automation, издание на актуализация 22, V3</span><span class="sxs-lookup"><span data-stu-id="521b8-103">Project Service Automation Update Release 22, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="521b8-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="521b8-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="521b8-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="521b8-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="521b8-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="521b8-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="521b8-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="521b8-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="521b8-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="521b8-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="521b8-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 22.</span><span class="sxs-lookup"><span data-stu-id="521b8-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 22.</span></span> <span data-ttu-id="521b8-110">Тази версия има номер на компилацията V 3.10.33.48 и е общодостъпна чрез самоактуализация от юни 2020 г.</span><span class="sxs-lookup"><span data-stu-id="521b8-110">This version has a build number of V 3.10.33.48 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-22"></a><span data-ttu-id="521b8-111">Издание на актуализация 22</span><span class="sxs-lookup"><span data-stu-id="521b8-111">Update Release 22</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="521b8-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="521b8-112">Bug fixes</span></span>



<span data-ttu-id="521b8-113">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="521b8-113">**Time and Expense**</span></span>

<span data-ttu-id="521b8-114">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="521b8-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="521b8-115">**Записи за време** не се добавят автоматично в графика на записи за време след импортирането.</span><span class="sxs-lookup"><span data-stu-id="521b8-115">**Time entries** are not automatically added in the Time entries schedule after import.</span></span>
- <span data-ttu-id="521b8-116">Инструментът за избор на дата на мрежата на **Запис за време** не разпознава регионалните настройки на потребител.</span><span class="sxs-lookup"><span data-stu-id="521b8-116">The **Time Entry** grid date picker does not recognize a user's regional settings.</span></span>

<span data-ttu-id="521b8-117">**Управление на ресурси**</span><span class="sxs-lookup"><span data-stu-id="521b8-117">**Resource Management**</span></span>

<span data-ttu-id="521b8-118">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="521b8-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="521b8-119">В ръчен режим промените на контурите на **Присвояване на ресурс** не се разпознават, когато се генерират **изисквания за ресурс**.</span><span class="sxs-lookup"><span data-stu-id="521b8-119">In manual mode, changes to **Resource Assignment** contours are not recognized when generating **Resource Requirements**.</span></span>
- <span data-ttu-id="521b8-120">**Заявките за ресурси** не поддържат състояния на персонализирани заявки.</span><span class="sxs-lookup"><span data-stu-id="521b8-120">**Resource Requests** do not support custom request statuses.</span></span>

<span data-ttu-id="521b8-121">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="521b8-121">**Project Management**</span></span>

<span data-ttu-id="521b8-122">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="521b8-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="521b8-123">Използването на двукратно щракване върху EstimateGridControl няма да анализира правилно числата форматирани на нидерландски.</span><span class="sxs-lookup"><span data-stu-id="521b8-123">Using double-click on EstimateGridControl will not correctly parse Dutch format numbers.</span></span>
- <span data-ttu-id="521b8-124">Присвоените часове не се актуализират правилно, когато присвояванията се променят с помощта на добавката за клиент на настолен компютър на Microsoft Project.</span><span class="sxs-lookup"><span data-stu-id="521b8-124">Assigned hours do not update correctly when assignments are changed using the Microsoft Project desktop client add-in.</span></span>
- <span data-ttu-id="521b8-125">Подмрежите за проследяване и оценка на проект показват неправилен код на валутата на продажби, когато валутата на договора е различна от валутата на клиента и организацията е конфигурирана да показва кодове на валута вместо символи на валута.</span><span class="sxs-lookup"><span data-stu-id="521b8-125">Project Tracking and Estimates grids display incorrect sales currency code when contract currency is different than customer currency and organization is configured to display currency codes instead of currency symbols.</span></span>
- <span data-ttu-id="521b8-126">Крайната дата на член на екипа ще добави един ден, ако графикът на работното време е 24 часа на ден.</span><span class="sxs-lookup"><span data-stu-id="521b8-126">A Team member's finish date will add one day if the work hour schedule is 24-hours per day.</span></span>
- <span data-ttu-id="521b8-127">В графика на проекта добавянето на категория на трансакция към задача не задейства автоматично записване.</span><span class="sxs-lookup"><span data-stu-id="521b8-127">On the Project Schedule, adding a Transaction Category to a task does not trigger auto save.</span></span>
- <span data-ttu-id="521b8-128">Следната грешка се показва при добавяне на член на екипа към шаблона за проекта: „Изискванията за ресурс не могат да бъдат свързани с шаблони за проекти“.</span><span class="sxs-lookup"><span data-stu-id="521b8-128">The following error is displayed when adding a team member to the Project Template: "Resource requirements cannot be associated with project templates".</span></span> 
- <span data-ttu-id="521b8-129">Скриптът за правило на лента "msdyn.Approval.CanApproveOrReject" показва грешка при изчакване.</span><span class="sxs-lookup"><span data-stu-id="521b8-129">Ribbon rule script "msdyn.Approval.CanApproveOrReject" displays a timeout error.</span></span>

<span data-ttu-id="521b8-130">**Sales**</span><span class="sxs-lookup"><span data-stu-id="521b8-130">**Sales**</span></span>

<span data-ttu-id="521b8-131">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="521b8-131">The following issues have been fixed:</span></span>

- <span data-ttu-id="521b8-132">Съобщението за грешка при валидиране не се показва, когато „Ценова листа за себестойност” е избрано в справката на ценовата листа във формуляр/обект „Нова ценова листа на проект за оферта”.</span><span class="sxs-lookup"><span data-stu-id="521b8-132">Validation error message not displayed when a Cost Price List is selected in Price List lookup on 'New Quote Project Price List' form/entity.</span></span>
- <span data-ttu-id="521b8-133">Затварянето на офертата като спечелена не се придвижва към създадения договор, ако BPF, прикачен към офертата, е в последния етап.</span><span class="sxs-lookup"><span data-stu-id="521b8-133">Closing the quote as won does not navigate to the created contract if a BPF attached to the quote is in the final stage.</span></span>
- <span data-ttu-id="521b8-134">Обръщането на **Нефактурирани продажби** се свързва с първоначалната цена, когато се анулира запис за време.</span><span class="sxs-lookup"><span data-stu-id="521b8-134">Reversing **Unbilled Sales** is linked to original cost when a time entry is recalled.</span></span>
- <span data-ttu-id="521b8-135">След като изберете бутона **Потвърждение**, състоянието на фактурата не се променя на **Потвърдено**, докато фактурата не бъде обновена.</span><span class="sxs-lookup"><span data-stu-id="521b8-135">After selecting the **Confirm** button, the invoice status doesn't change to **Confirmed** unless the invoice is refreshed.</span></span>
