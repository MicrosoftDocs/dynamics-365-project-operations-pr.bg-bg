---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 16, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 16, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/18/2020
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
ms.openlocfilehash: 5d4851ed27028117d25efb0610c25a5aac9c8b70
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006768"
---
# <a name="project-service-automation-update-release-16-v3"></a><span data-ttu-id="7a52e-103">Project Service Automation, издание на актуализация 16, V3</span><span class="sxs-lookup"><span data-stu-id="7a52e-103">Project Service Automation Update Release 16, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="7a52e-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="7a52e-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="7a52e-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="7a52e-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="7a52e-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="7a52e-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="7a52e-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения, за да инсталирате актуализацията.</span><span class="sxs-lookup"><span data-stu-id="7a52e-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="7a52e-108">За повече информация вижте: [Инсталиране, актуализиране на предпочитано решение](/dynamics365/project-service/upgrade-psa-home-page).</span><span class="sxs-lookup"><span data-stu-id="7a52e-108">For more information, see [Install, Update a Preferred Solution](/dynamics365/project-service/upgrade-psa-home-page).</span></span>
<span data-ttu-id="7a52e-109">Тази тема изброява функциите и корекциите, които са нови или променени за PSA V3, издание на актуализация 16.</span><span class="sxs-lookup"><span data-stu-id="7a52e-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 16.</span></span> <span data-ttu-id="7a52e-110">Тази версия е с номер на компилация V3.10.6.34 и е общодостъпна за самостоятелно актуализиране от януари 2020 г.</span><span class="sxs-lookup"><span data-stu-id="7a52e-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in January 2020.</span></span>


## <a name="update-release-16"></a><span data-ttu-id="7a52e-111">Издание на актуализация 16</span><span class="sxs-lookup"><span data-stu-id="7a52e-111">Update Release 16</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="7a52e-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="7a52e-112">Bug fixes</span></span>

-   <span data-ttu-id="7a52e-113">Време и разход</span><span class="sxs-lookup"><span data-stu-id="7a52e-113">Time and Expense</span></span>

    -   <span data-ttu-id="7a52e-114">Поправено: Потребителите, които се опитват да изпратят изтритите записи за време и разходи за одобрения, вече ще получават съответните съобщения за грешки.</span><span class="sxs-lookup"><span data-stu-id="7a52e-114">Fixed: Users attempting to submit deleted time and expense entries for approvals will now receive relevant error messages.</span></span>

-   <span data-ttu-id="7a52e-115">Управление на проекти</span><span class="sxs-lookup"><span data-stu-id="7a52e-115">Project Management</span></span>

    -   <span data-ttu-id="7a52e-116">Поправено: Ресурсовите единици, определени за членовете на екипа в шаблоните, се спазват, когато шаблоните се прилагат към нов проект.</span><span class="sxs-lookup"><span data-stu-id="7a52e-116">Fixed: The resourcing units defined for team members in templates are respected with the templates are applied to a new project.</span></span>

    -   <span data-ttu-id="7a52e-117">Поправено: Подобрено управление на преназначаването на собствеността върху записи.</span><span class="sxs-lookup"><span data-stu-id="7a52e-117">Fixed: Improved handling of the re-assignment of record ownership.</span></span>

    -   <span data-ttu-id="7a52e-118">Поправено: Проектите, които са в процес на копиране, няма да бъдат позволени да бъдат копирани, докато всички операции по копиране не приключат.</span><span class="sxs-lookup"><span data-stu-id="7a52e-118">Fixed: Projects that are in the process of being copied will not be permitted to copied until all copy operations are complete.</span></span>

-   <span data-ttu-id="7a52e-119">Управление на ресурс</span><span class="sxs-lookup"><span data-stu-id="7a52e-119">Resource Management</span></span>

    -   <span data-ttu-id="7a52e-120">Поправено: Удължаването на резервациите сега се справя правилно с кратки срокове и вече не създава нула часа за удължени резервации.</span><span class="sxs-lookup"><span data-stu-id="7a52e-120">Fixed: Extend bookings now handles short durations correctly and no longer creates zero hours for extended bookings.</span></span>

    -   <span data-ttu-id="7a52e-121">Фиксирано: Изгледът за съгласуване се показва, когато часовата зона на проекта е +5:30 GMT и времето на потребителя е различно.</span><span class="sxs-lookup"><span data-stu-id="7a52e-121">Fixed: The reconciliation view now renders when the project time zone is +5:30 GMT and the user’s time aone is different.</span></span>

-   <span data-ttu-id="7a52e-122">Sales</span><span class="sxs-lookup"><span data-stu-id="7a52e-122">Sales</span></span>

    -   <span data-ttu-id="7a52e-123">Поправено: Когато проект, нанесен в аспекти на договор, е премахнат и нов проект е нанесен, реалните записи на новия проект не се преоценяват въз основа на правилата за фактуриране и ценообразуване, определени в договорената линия.</span><span class="sxs-lookup"><span data-stu-id="7a52e-123">Fixed: When a project mapped to a contract line is removed and a new project is mapped, the actual records on the new project were not getting re-evaluated based on the billing and pricing rules defined on the contract line.</span></span> <span data-ttu-id="7a52e-124">Това е поправено в тази версия.</span><span class="sxs-lookup"><span data-stu-id="7a52e-124">This has been fixed in this release.</span></span> <span data-ttu-id="7a52e-125">Ценообразуването и действителните записи на новонанесения проект ще бъдат променени и създадени отново правилно въз основа на правилата за ценообразуване и фактуриране на договора.</span><span class="sxs-lookup"><span data-stu-id="7a52e-125">Pricing and actual records on the newly mapped project will get reversed and re-created correctly based on the pricing and billing rules of the contract line.</span></span> <span data-ttu-id="7a52e-126">Действителните записи на неописания проект също ще бъдат преоценявани и създадени отново като следствие.</span><span class="sxs-lookup"><span data-stu-id="7a52e-126">The actual records of the un-mapped project will also get re-evaluated and re-created as a consequence.</span></span>

    -   <span data-ttu-id="7a52e-127">Поправено: Добавено е допълнително валидиране към полето **Количество** на реда с прогноза, за да се гарантира, че нулевите стойности не се запазват.</span><span class="sxs-lookup"><span data-stu-id="7a52e-127">Fixed: Additional validation has been added to an estimate line’s **Amount** field to ensure that null values are not persisted.</span></span>

    -   <span data-ttu-id="7a52e-128">Поправено: Когато актуализациите са актуализирани за даден проект, към основния формуляр на проекта е добавен бутон за опресняване, за да могат потребителите отново да синхронизират актуалните данни.</span><span class="sxs-lookup"><span data-stu-id="7a52e-128">Fixed: When actuals have been updated on a project, a refresh button has been added to the project main form to allow users to re-sync the actuals.</span></span>

    -   <span data-ttu-id="7a52e-129">Фиксирано: Когато потребителите надстроят от 2.X до 3.X, проекти с NULL стойност за името на проекта ще бъдат разрешени.</span><span class="sxs-lookup"><span data-stu-id="7a52e-129">Fixed: When users upgrade from 2.X to 3.X, projects with a NULL value for project name will be permitted.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]