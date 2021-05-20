---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 23, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 23, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 08/25/2020
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
ms.openlocfilehash: f90c0d2168b261cf1b6ef10374f282274ea61af5
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948946"
---
# <a name="project-service-automation-update-release-23-v3"></a><span data-ttu-id="a1fef-103">Project Service Automation, издание на актуализация 23, V3</span><span class="sxs-lookup"><span data-stu-id="a1fef-103">Project Service Automation Update Release 23, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="a1fef-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a1fef-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="a1fef-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="a1fef-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="a1fef-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="a1fef-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="a1fef-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="a1fef-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="a1fef-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="a1fef-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="a1fef-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 23.</span><span class="sxs-lookup"><span data-stu-id="a1fef-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 23.</span></span> <span data-ttu-id="a1fef-110">Тази версия е с номер на компилация V 3.10.34.30 и е общодостъпна за самостоятелно актуализиране от август 2020.</span><span class="sxs-lookup"><span data-stu-id="a1fef-110">This version has a build number of V 3.10.34.30 and is generally available through a self-update in August 2020.</span></span>

## <a name="update-release-23"></a><span data-ttu-id="a1fef-111">Издание на актуализация 23</span><span class="sxs-lookup"><span data-stu-id="a1fef-111">Update Release 23</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="a1fef-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="a1fef-112">Bug fixes</span></span>

<span data-ttu-id="a1fef-113">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="a1fef-113">**Time and Expense**</span></span>

<span data-ttu-id="a1fef-114">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="a1fef-114">The following issues have been fixed:</span></span>
- <span data-ttu-id="a1fef-115">Обработвайте случай на ръба в **Изтриване на член на екипа по проекта**, за да предоставите смислено изключение.</span><span class="sxs-lookup"><span data-stu-id="a1fef-115">Handle edge case in **Project Team Member Delete** to provide a meaningful exception.</span></span>
- <span data-ttu-id="a1fef-116">Импортирането на задание води до празен екран за премахване.</span><span class="sxs-lookup"><span data-stu-id="a1fef-116">Assignment import results in a blank remove screen.</span></span>

<span data-ttu-id="a1fef-117">**Управление на ресурси**</span><span class="sxs-lookup"><span data-stu-id="a1fef-117">**Resource Management**</span></span>

<span data-ttu-id="a1fef-118">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="a1fef-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="a1fef-119">**Ресурсна карта на мрежата за използване на ресурсите** показва неправилни данни, когато времевата скала е повече от пет дни.</span><span class="sxs-lookup"><span data-stu-id="a1fef-119">The **Resource utilization grid resource card** shows incorrect data when the time scale is more than five days.</span></span>
- <span data-ttu-id="a1fef-120">Когато клиентите създават наличен ресурс, приставката периодично не успява автоматично да добави ресурса към група на Microsoft Office 365.</span><span class="sxs-lookup"><span data-stu-id="a1fef-120">When customers create a bookable resource, the plug-in intermittently fails to automatically add the resource to a Microsoft Office 365 group.</span></span>
- <span data-ttu-id="a1fef-121">Изгледът **Съгласуване** показва ръчни контури неправилно в изгледа **Седмица** или **Месец**.</span><span class="sxs-lookup"><span data-stu-id="a1fef-121">**Reconciliation** view displays manual contours incorrectly in the **Week** or **Month** view.</span></span>

<span data-ttu-id="a1fef-122">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="a1fef-122">**Project Management**</span></span>

<span data-ttu-id="a1fef-123">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="a1fef-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="a1fef-124">Прекомерен брой обекти **RetrieveMultiple за потребителски настройки** причиняват влошена производителност за одобрение на проекти и други операции.</span><span class="sxs-lookup"><span data-stu-id="a1fef-124">An excessive number of **RetrieveMultiple for usersettings** entities are causing degraded performance for project approvals and other operations.</span></span>
- <span data-ttu-id="a1fef-125">Търсенето на ресурси в мрежата **Планиране на задачите** е ограничено до показване само на петима членове на екипа от екипа на проекта</span><span class="sxs-lookup"><span data-stu-id="a1fef-125">The **Task Planning** grid resource lookup is limited to only show up to five team members from the project team.</span></span> 
- <span data-ttu-id="a1fef-126">Търсенето на ресурс в мрежата **Планиране на задачите** не филтрира неактивни ресурси.</span><span class="sxs-lookup"><span data-stu-id="a1fef-126">The **Task Planning** grid resource lookup does not filter inactive resources.</span></span>
- <span data-ttu-id="a1fef-127">Ръчният режим не работи, както се очаква в структурата на разбивка на работата по планирането на проекта.</span><span class="sxs-lookup"><span data-stu-id="a1fef-127">Manual mode is not working as expected in the project planning work breakdown structure.</span></span>
- <span data-ttu-id="a1fef-128">Мрежата **Планиране на задачите** показва **Неактивни категории транзакции**.</span><span class="sxs-lookup"><span data-stu-id="a1fef-128">The **Task Planning** grid shows **Inactive Transaction Categories**.</span></span>
- <span data-ttu-id="a1fef-129">Мрежата **Възлагане на ресурси** закръгля неправилно, когато задача има множество задания.</span><span class="sxs-lookup"><span data-stu-id="a1fef-129">The **Resource Assignment** grid rounds incorrectly when a task has multiple assignments.</span></span>
- <span data-ttu-id="a1fef-130">Стойностите на закръгляването са различни между планираните разходи и действителните разходи за една задача.</span><span class="sxs-lookup"><span data-stu-id="a1fef-130">Rounding values are different between planned cost and actual cost for a single task.</span></span>

<span data-ttu-id="a1fef-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="a1fef-131">**Sales**</span></span>

<span data-ttu-id="a1fef-132">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="a1fef-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="a1fef-133">Двойното щракване върху **Извличане на всички категории транзакции** създава множество редове.</span><span class="sxs-lookup"><span data-stu-id="a1fef-133">**Fetch All Transaction Categories** double-click creates multiple lines.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]