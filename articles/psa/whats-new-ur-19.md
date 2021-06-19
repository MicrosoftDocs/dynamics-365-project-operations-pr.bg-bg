---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 19, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 19, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 05/05/2020
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
ms.openlocfilehash: 7812bc41f32f9d4116c63990059f7dbc0351cf9e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006588"
---
# <a name="project-service-automation-update-release-19-v3"></a><span data-ttu-id="9c508-103">Project Service Automation, издание на актуализация 19, V3</span><span class="sxs-lookup"><span data-stu-id="9c508-103">Project Service Automation Update Release 19, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="9c508-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="9c508-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="9c508-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="9c508-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="9c508-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="9c508-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="9c508-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="9c508-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="9c508-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="9c508-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="9c508-109">Тази тема изброява функциите и корекциите, които са нови или променени за PSA V3, издание на актуализация 19.</span><span class="sxs-lookup"><span data-stu-id="9c508-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 19.</span></span> <span data-ttu-id="9c508-110">Тази версия има номер на компилацията V3.10.30.41 и е общодостъпна чрез самоактуализация от май 2020 г.</span><span class="sxs-lookup"><span data-stu-id="9c508-110">This version has a build number of V3.10.30.41 and is generally available through a self-update in May 2020.</span></span>

## <a name="update-release-19"></a><span data-ttu-id="9c508-111">Издание на актуализация 19</span><span class="sxs-lookup"><span data-stu-id="9c508-111">Update Release 19</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="9c508-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="9c508-112">Bug fixes</span></span>

<span data-ttu-id="9c508-113">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="9c508-113">**Time and Expense**</span></span>

<span data-ttu-id="9c508-114">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="9c508-114">The following issues have been fixed:</span></span> 

- <span data-ttu-id="9c508-115">Грешки, извлечени от импортирания на записи за време, не се извеждат правилно.</span><span class="sxs-lookup"><span data-stu-id="9c508-115">Errors derived from time entry imports are not surfaced correctly.</span></span>
- <span data-ttu-id="9c508-116">Мрежата за записи за време не поддържа поведението на полето **Само дата**.</span><span class="sxs-lookup"><span data-stu-id="9c508-116">Time Entry Grid does not support **Date Only** field behavior.</span></span>
- <span data-ttu-id="9c508-117">Ресурсите по проекти не могат да създават разход с проект.</span><span class="sxs-lookup"><span data-stu-id="9c508-117">Project Resources are unable to create an expense with a project.</span></span>

<span data-ttu-id="9c508-118">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="9c508-118">**Project Management**</span></span>

<span data-ttu-id="9c508-119">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="9c508-119">The following issues have been fixed:</span></span> 

-  <span data-ttu-id="9c508-120">Внукова задача води до неправилна оценка на усилията при изчислението за завършване (ОПЗ).</span><span class="sxs-lookup"><span data-stu-id="9c508-120">Grandchild task causes an incorrect effort estimate during the Completion (EAC) Calculation.</span></span>

<span data-ttu-id="9c508-121">**Sales**</span><span class="sxs-lookup"><span data-stu-id="9c508-121">**Sales**</span></span>

<span data-ttu-id="9c508-122">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="9c508-122">The following issues have been fixed:</span></span> 

- <span data-ttu-id="9c508-123">Действието **Преизчисляване** не работи с подробности за аспект на договор за разходи или подробности за ред на оферта.</span><span class="sxs-lookup"><span data-stu-id="9c508-123">The **Recalculate** action does not work with expense contract line details or quote line details.</span></span>
- <span data-ttu-id="9c508-124">**Актуализиране на цени** липсва за оценки на разходи.</span><span class="sxs-lookup"><span data-stu-id="9c508-124">**Update Prices** is missing for expense estimates.</span></span>
-  <span data-ttu-id="9c508-125">Клиентите не могат да избират персонализирани описания на състоянието на договора от страницата **Договор по проект**.</span><span class="sxs-lookup"><span data-stu-id="9c508-125">Customers are unable to select custom contract status reasons from the **Project Contract** page.</span></span>
- <span data-ttu-id="9c508-126">Клиентите се сблъскват с намалена производителност при създаване на персонализирана ценова листа от оферта.</span><span class="sxs-lookup"><span data-stu-id="9c508-126">Customers experience degraded performance when creating a custom price list from a quote.</span></span>
- <span data-ttu-id="9c508-127">Клиентите се сблъскват с несъответствие на стойностите по подразбиране за **единица** в страниците **Подробности за ред на оферта** и **Подробности за аспект на договор**.</span><span class="sxs-lookup"><span data-stu-id="9c508-127">Customers experience inconsistency with **unit** defaults on **Quote Line Details** and **Contract Line Details** pages.</span></span>
- <span data-ttu-id="9c508-128">Добавянето на елементи в категория на неплатими транзакции към платим аспект на договора няма да вземе предвид типа фактуриране **Неплатим** на категорията транзакции.</span><span class="sxs-lookup"><span data-stu-id="9c508-128">Adding non-chargeable transaction category items to a chargeable contract line will not respect the **Non-chargeable** billing type of the transaction category.</span></span>
- <span data-ttu-id="9c508-129">Клиентите не могат да използват новодобавените роли и категории в преди това създадени договори.</span><span class="sxs-lookup"><span data-stu-id="9c508-129">Customers can't use the newly added roles and category on previously created contracts.</span></span>
- <span data-ttu-id="9c508-130">Клиентите се сблъскват с намалена производителност Ненужно извличане в PreValidateProjectTeamMemberUpdate.cs</span><span class="sxs-lookup"><span data-stu-id="9c508-130">Customers experience degraded performance Unnecessary retrieve in PreValidateProjectTeamMemberUpdate.cs</span></span>
- <span data-ttu-id="9c508-131">Роли, настроени като неплатими в списъка **Категории ресурси**, трябва да се добавят към раздела **Платими роли** като **Неплатими** в аспекта на договора за проект.</span><span class="sxs-lookup"><span data-stu-id="9c508-131">Roles set up as non-chargeable in the **Resource Categories** list should be added to the **Chargeable Roles** tab as **Non0chargeable** on the contract line for a project.</span></span>
- <span data-ttu-id="9c508-132">Клиентите може да се сблъскат с намалена производителност при създаване на проект, тъй като **GetBookableResourceIdFromUser** извлича всички колони налични ресурси вместо само основния идентификатор.</span><span class="sxs-lookup"><span data-stu-id="9c508-132">Customers may experience degraded performance when creating a project because **GetBookableResourceIdFromUser** retrieves all columns of bookable resources instead of just the primary ID.</span></span>
- <span data-ttu-id="9c508-133">В обекта **TransactionType** липсва добавката за актуализиране преди валидиране, за да не позволява на потребителите да въвеждат **Units** и **UnitGroups**, които не са валидни за типовете транзакции.</span><span class="sxs-lookup"><span data-stu-id="9c508-133">**TransactionType** entity missing the pre-validation update plug-in to prevent users from entering **Units** and **UnitGroups** that are not valid for transaction types.</span></span>
- <span data-ttu-id="9c508-134">Стъпката **Премахване** не работи за импортиране на запис за време.</span><span class="sxs-lookup"><span data-stu-id="9c508-134">The **Remove** step does not work for time entry import.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]