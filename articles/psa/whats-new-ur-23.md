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
ms.openlocfilehash: 07f1a274914d7e641ddf2fd42f377dce1da7f815
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131105"
---
# <a name="project-service-automation-update-release-23-v3"></a><span data-ttu-id="9385a-103">Project Service Automation, издание на актуализация 23, V3</span><span class="sxs-lookup"><span data-stu-id="9385a-103">Project Service Automation Update Release 23, V3</span></span>

<span data-ttu-id="9385a-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="9385a-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="9385a-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="9385a-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="9385a-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="9385a-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="9385a-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="9385a-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="9385a-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="9385a-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="9385a-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 23.</span><span class="sxs-lookup"><span data-stu-id="9385a-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 23.</span></span> <span data-ttu-id="9385a-110">Тази версия е с номер на компилация V 3.10.34.30 и е общодостъпна за самостоятелно актуализиране от август 2020.</span><span class="sxs-lookup"><span data-stu-id="9385a-110">This version has a build number of V 3.10.34.30 and is generally available through a self-update in August 2020.</span></span>

## <a name="update-release-23"></a><span data-ttu-id="9385a-111">Издание на актуализация 23</span><span class="sxs-lookup"><span data-stu-id="9385a-111">Update Release 23</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="9385a-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="9385a-112">Bug fixes</span></span>

<span data-ttu-id="9385a-113">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="9385a-113">**Time and Expense**</span></span>

<span data-ttu-id="9385a-114">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="9385a-114">The following issues have been fixed:</span></span>
- <span data-ttu-id="9385a-115">Обработвайте случай на ръба в **Изтриване на член на екипа по проекта**, за да предоставите смислено изключение.</span><span class="sxs-lookup"><span data-stu-id="9385a-115">Handle edge case in **Project Team Member Delete** to provide a meaningful exception.</span></span>
- <span data-ttu-id="9385a-116">Импортирането на задание води до празен екран за премахване.</span><span class="sxs-lookup"><span data-stu-id="9385a-116">Assignment import results in a blank remove screen.</span></span>

<span data-ttu-id="9385a-117">**Управление на ресурси**</span><span class="sxs-lookup"><span data-stu-id="9385a-117">**Resource Management**</span></span>

<span data-ttu-id="9385a-118">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="9385a-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="9385a-119">**Ресурсна карта на мрежата за използване на ресурсите** показва неправилни данни, когато времевата скала е повече от пет дни.</span><span class="sxs-lookup"><span data-stu-id="9385a-119">The **Resource utilization grid resource card** shows incorrect data when the time scale is more than five days.</span></span>
- <span data-ttu-id="9385a-120">Когато клиентите създават наличен ресурс, приставката периодично не успява автоматично да добави ресурса към група на Microsoft Office 365.</span><span class="sxs-lookup"><span data-stu-id="9385a-120">When customers create a bookable resource, the plug-in intermittently fails to automatically add the resource to a Microsoft Office 365 group.</span></span>
- <span data-ttu-id="9385a-121">Изгледът **Съгласуване** показва ръчни контури неправилно в изгледа **Седмица** или **Месец**.</span><span class="sxs-lookup"><span data-stu-id="9385a-121">**Reconciliation** view displays manual contours incorrectly in the **Week** or **Month** view.</span></span>

<span data-ttu-id="9385a-122">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="9385a-122">**Project Management**</span></span>

<span data-ttu-id="9385a-123">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="9385a-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="9385a-124">Прекомерен брой обекти **RetrieveMultiple за потребителски настройки** причиняват влошена производителност за одобрение на проекти и други операции.</span><span class="sxs-lookup"><span data-stu-id="9385a-124">An excessive number of **RetrieveMultiple for usersettings** entities are causing degraded performance for project approvals and other operations.</span></span>
- <span data-ttu-id="9385a-125">Търсенето на ресурси в мрежата **Планиране на задачите** е ограничено до показване само на петима членове на екипа от екипа на проекта</span><span class="sxs-lookup"><span data-stu-id="9385a-125">The **Task Planning** grid resource lookup is limited to only show up to five team members from the project team.</span></span> 
- <span data-ttu-id="9385a-126">Търсенето на ресурс в мрежата **Планиране на задачите** не филтрира неактивни ресурси.</span><span class="sxs-lookup"><span data-stu-id="9385a-126">The **Task Planning** grid resource lookup does not filter inactive resources.</span></span>
- <span data-ttu-id="9385a-127">Ръчният режим не работи, както се очаква в структурата на разбивка на работата по планирането на проекта.</span><span class="sxs-lookup"><span data-stu-id="9385a-127">Manual mode is not working as expected in the project planning work breakdown structure.</span></span>
- <span data-ttu-id="9385a-128">Мрежата **Планиране на задачите** показва **Неактивни категории транзакции**.</span><span class="sxs-lookup"><span data-stu-id="9385a-128">The **Task Planning** grid shows **Inactive Transaction Categories**.</span></span>
- <span data-ttu-id="9385a-129">Мрежата **Възлагане на ресурси** закръгля неправилно, когато задача има множество задания.</span><span class="sxs-lookup"><span data-stu-id="9385a-129">The **Resource Assignment** grid rounds incorrectly when a task has multiple assignments.</span></span>
- <span data-ttu-id="9385a-130">Стойностите на закръгляването са различни между планираните разходи и действителните разходи за една задача.</span><span class="sxs-lookup"><span data-stu-id="9385a-130">Rounding values are different between planned cost and actual cost for a single task.</span></span>

<span data-ttu-id="9385a-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="9385a-131">**Sales**</span></span>

<span data-ttu-id="9385a-132">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="9385a-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="9385a-133">Двойното щракване върху **Извличане на всички категории транзакции** създава множество редове.</span><span class="sxs-lookup"><span data-stu-id="9385a-133">**Fetch All Transaction Categories** double-click creates multiple lines.</span></span>
