---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 14, V3
description: Тази тема предоставя информация за новостите в актуализацията на Project Service Automation, издание 14, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/29/2020
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
ms.openlocfilehash: b811bf7ccfb626e6944801dffa943d2afab0c5e8
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4124805"
---
# <a name="project-service-automation-update-release-14-v3"></a><span data-ttu-id="c8e36-103">Project Service Automation, издание на актуализация 14, V3</span><span class="sxs-lookup"><span data-stu-id="c8e36-103">Project Service Automation Update Release 14, V3</span></span>
<span data-ttu-id="c8e36-104">С удоволствие съобщаваме за най-новата актуализация за приложението Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="c8e36-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="c8e36-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="c8e36-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="c8e36-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="c8e36-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="c8e36-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online и отидете на страницата с решения, за да инсталирате актуализацията.</span><span class="sxs-lookup"><span data-stu-id="c8e36-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="c8e36-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="c8e36-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="c8e36-109">Тази тема изброява функциите и корекциите, които са нови или променени за PSA V3, издание на актуализация 14.</span><span class="sxs-lookup"><span data-stu-id="c8e36-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 14.</span></span> <span data-ttu-id="c8e36-110">Тази версия е с номер на компилация V3.10.4.21 и е достъпна по следния график:</span><span class="sxs-lookup"><span data-stu-id="c8e36-110">This version has a build number of V3.10.4.21 and is available on the following schedule:</span></span>

- <span data-ttu-id="c8e36-111">**Общодостъпна (самостоятелно актуализиране):** януари 2020 г.</span><span class="sxs-lookup"><span data-stu-id="c8e36-111">**General availability (self-update):** January 2020</span></span>
- <span data-ttu-id="c8e36-112">**Автоматична актуализация:** февруари 2020 г.</span><span class="sxs-lookup"><span data-stu-id="c8e36-112">**Auto-update:** February 2020</span></span>

## <a name="update-release-14"></a><span data-ttu-id="c8e36-113">Издание на актуализация 14</span><span class="sxs-lookup"><span data-stu-id="c8e36-113">Update Release 14</span></span>

### <a name="enhancements"></a><span data-ttu-id="c8e36-114">Подобрения</span><span class="sxs-lookup"><span data-stu-id="c8e36-114">Enhancements</span></span>

- <span data-ttu-id="c8e36-115">Sales</span><span class="sxs-lookup"><span data-stu-id="c8e36-115">Sales</span></span>

     - <span data-ttu-id="c8e36-116">Стойностите на персонализирани полета от **Подробности за ред на оферта** се копират в **Подробности за аспекти на договор по проект**, когато офертата се актуализира до **Затворена като спечелена**.</span><span class="sxs-lookup"><span data-stu-id="c8e36-116">Custom field values from **Quote Line Details** are copied to **Project Contract Line Details** when a quote is updated to **Closed as won**.</span></span>
     - <span data-ttu-id="c8e36-117">Потвърдени проекти могат да бъдат **Затворени като загубени**.</span><span class="sxs-lookup"><span data-stu-id="c8e36-117">Confirmed projects can be **Closed as lost**.</span></span>

- <span data-ttu-id="c8e36-118">Управление на ресурс</span><span class="sxs-lookup"><span data-stu-id="c8e36-118">Resource Management</span></span>

     - <span data-ttu-id="c8e36-119">При удължаване на резервации, потребителите ще бъдат подканени с диалогов прозорец за потвърждение да обобщят резултатите от резервациите и да предоставят връзка за поддръжка на резервациите.</span><span class="sxs-lookup"><span data-stu-id="c8e36-119">When extending bookings, users will be prompted with a confirmation dialog box to summarize booking results and provide a link to Maintain Bookings.</span></span>


### <a name="bug-fixes"></a><span data-ttu-id="c8e36-120">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="c8e36-120">Bug fixes</span></span>

- <span data-ttu-id="c8e36-121">Време и разход</span><span class="sxs-lookup"><span data-stu-id="c8e36-121">Time and Expense</span></span>

     - <span data-ttu-id="c8e36-122">Поправено: Подобрено потребителско изживяване, когато потребителят не е избрал записи, които да бъдат коригирани.</span><span class="sxs-lookup"><span data-stu-id="c8e36-122">Fixed: Improved the user experience when the user has not selected any entries to be corrected.</span></span>

- <span data-ttu-id="c8e36-123">Управление на ресурс</span><span class="sxs-lookup"><span data-stu-id="c8e36-123">Resource Management</span></span>

     - <span data-ttu-id="c8e36-124">Поправено: Резервирането на ресурс няколко пъти препълва името на наличния ресурс.</span><span class="sxs-lookup"><span data-stu-id="c8e36-124">Fixed: Booking a resource multiple times overflows the name of the bookable resource.</span></span>

- <span data-ttu-id="c8e36-125">Sales</span><span class="sxs-lookup"><span data-stu-id="c8e36-125">Sales</span></span>

     - <span data-ttu-id="c8e36-126">Поправено: Общата продажна цена не се изчислява, докато потребителят не въведе и себестойност за оценка на разходите по проект.</span><span class="sxs-lookup"><span data-stu-id="c8e36-126">Fixed: The total sales price is not calculated until the user also inputs a cost price for expense estimates on a project.</span></span>
     - <span data-ttu-id="c8e36-127">Поправено: Затварянето на оферта като **Спечелена** е неуспешно, ако свързаният договор по проект не е в състояние **Чернова**.</span><span class="sxs-lookup"><span data-stu-id="c8e36-127">Fixed: Closing a quote as **Won** fails if the associated project contract is not in a **Draft** state.</span></span>

