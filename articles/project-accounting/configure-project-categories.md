---
title: Конфигуриране на категории на проект
description: Тази тема предоставя информация за настройването на категориите на проект.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 84033182ce047d230724409eef9bc6afcaefd2b4
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071716"
---
# <a name="configure-project-categories"></a><span data-ttu-id="5c845-103">Конфигуриране на категории на проект</span><span class="sxs-lookup"><span data-stu-id="5c845-103">Configure project categories</span></span>

<span data-ttu-id="5c845-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="5c845-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="5c845-105">Project Operations предлага надеждни възможности за категоризиране на приходите и разходите по проекти.</span><span class="sxs-lookup"><span data-stu-id="5c845-105">Project Operations offers robust capabilities for categorizing revenue and expenses on projects.</span></span> <span data-ttu-id="5c845-106">Категориите предоставят възможност за отчитане и анализ на транзакции на проекти и задвижване на осчетоводяване в главната книга.</span><span class="sxs-lookup"><span data-stu-id="5c845-106">Categories provide the ability to report on and analyze project transactions, and drive posting to the general ledger.</span></span>

<span data-ttu-id="5c845-107">Следващата диаграма илюстрира връзката между категориите транзакции, споделените категории и категориите проекти.</span><span class="sxs-lookup"><span data-stu-id="5c845-107">The following diagram illustrates the correlation between transaction categories, shared categories, and project categories.</span></span> 

<span data-ttu-id="5c845-108">Категориите транзакции са основното групиране за транзакции по проекти.</span><span class="sxs-lookup"><span data-stu-id="5c845-108">Transaction categories are the basic grouping for project transactions.</span></span> <span data-ttu-id="5c845-109">В рамките на това групиране има набор от споделени категории, които могат да се споделят между приложения и модули.</span><span class="sxs-lookup"><span data-stu-id="5c845-109">Within that grouping, there is a set of shared categories that can be shared across applications and modules.</span></span> <span data-ttu-id="5c845-110">Още по-навътре в спецификите, категориите проекти са най-подробното ниво на категориите.</span><span class="sxs-lookup"><span data-stu-id="5c845-110">Getting even further into specifics, project categories are the most granular level of categories.</span></span> <span data-ttu-id="5c845-111">Категориите на проектите са специфични за юридическо лице, модул и приложение.</span><span class="sxs-lookup"><span data-stu-id="5c845-111">Project categories are specific to legal entity, module, and application.</span></span>

![Корелация между категориите транзакции, споделените категории и категориите проекти](media/project-categories.png)

## <a name="transaction-categories"></a><span data-ttu-id="5c845-113">Категории трансакция</span><span class="sxs-lookup"><span data-stu-id="5c845-113">Transaction categories</span></span>

<span data-ttu-id="5c845-114">Категориите на транзакциите представляват основното групиране за транзакции по проект и не са специфични за компанията или типа транзакция.</span><span class="sxs-lookup"><span data-stu-id="5c845-114">Transaction categories represent the basic grouping for project transactions and are not company or transaction type-specific.</span></span> <span data-ttu-id="5c845-115">Например Contoso Robotics използва категории за проектиране, пътуване, инсталиране и обслужване на транзакции, за да групира транзакции по проект.</span><span class="sxs-lookup"><span data-stu-id="5c845-115">For example, Contoso Robotics uses Design, Travel, Installation, and Service Transaction categories to group Project transactions.</span></span>

<span data-ttu-id="5c845-116">Категориите на транзакциите са дефинирани в модула Project Operations.</span><span class="sxs-lookup"><span data-stu-id="5c845-116">Transaction categories are defined in the Project Operations module.</span></span> 
1. <span data-ttu-id="5c845-117">Отидете на **Настройки** \> **Категории на трансакция** , за да отворите формуляра.</span><span class="sxs-lookup"><span data-stu-id="5c845-117">Go to **Settings** \> **Transaction Categories** to open the form.</span></span> 
2. <span data-ttu-id="5c845-118">Създайте нова категория транзакции, като изберете **Създаване** или като изберете **Импортиране от Excel**.</span><span class="sxs-lookup"><span data-stu-id="5c845-118">Create a new transaction category either by selecting **New** or by selecting **Import from Excel**.</span></span>

## <a name="shared-categories"></a><span data-ttu-id="5c845-119">Споделени категории</span><span class="sxs-lookup"><span data-stu-id="5c845-119">Shared categories</span></span>

<span data-ttu-id="5c845-120">Dynamics 365 използва концепцията за споделени категории, за да категоризира разходите в различни приложения, като например Dynamics 365 Finance, Dynamics 365 Supply Chain и Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="5c845-120">Dynamics 365 uses the Shared categories concept to categorize expenses in different applications, such as Dynamics 365 Finance, Dynamics 365 Supply Chain, and Dynamics 365 Project Operations.</span></span> <span data-ttu-id="5c845-121">За всяка създадена категория транзакции, Project Operations автоматично създава четири свързани споделени категории: Часове, Разходи, Такси и Артикул.</span><span class="sxs-lookup"><span data-stu-id="5c845-121">For each Transaction category created, Project Operations automatically creates four related Shared categories: Hours, Expense, Fees, and Item.</span></span> <span data-ttu-id="5c845-122">Можете да прегледате и коригирате споделените категории, като отидете на **Управление на проекти и счетоводство** \> **Настройка** \> **Категории** \> **Споделени категории**.</span><span class="sxs-lookup"><span data-stu-id="5c845-122">You can review and adjust the shared categories by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Shared Categories**.</span></span>

## <a name="project-categories"></a><span data-ttu-id="5c845-123">Категории на проект</span><span class="sxs-lookup"><span data-stu-id="5c845-123">Project categories</span></span>

<span data-ttu-id="5c845-124">Категориите на проекти представляват най-подробното ниво на конфигурация на категориите и трябва да бъдат конфигурирани отделно и за всяка компания от счетоводител на проекта.</span><span class="sxs-lookup"><span data-stu-id="5c845-124">Project categories represent most granular level of category configuration and must be configured separately, and for each company, by a Project accountant.</span></span>

1. <span data-ttu-id="5c845-125">Отидете на **Управление на проекти и счетоводство** \> **Настройка** \> **Категории** \> **Категории на проекти**.</span><span class="sxs-lookup"><span data-stu-id="5c845-125">Go to **Project Management and Accounting** \> **Setup** \> **Categories** \> **Project categories**.</span></span>
2. <span data-ttu-id="5c845-126">Изберете **Нова**.</span><span class="sxs-lookup"><span data-stu-id="5c845-126">Select **New**.</span></span>
3. <span data-ttu-id="5c845-127">Изберете **ИД на категория** от споделената категория, която създадохте в предишния раздел.</span><span class="sxs-lookup"><span data-stu-id="5c845-127">Select the **Category ID** of the Shared category you created in the previous section.</span></span> <span data-ttu-id="5c845-128">Project Operations позволява използването само на тези споделени категории, които са свързани с категории транзакции.</span><span class="sxs-lookup"><span data-stu-id="5c845-128">Project Operations allows using only those shared categories that are associated with transaction categories.</span></span>
4. <span data-ttu-id="5c845-129">Избор на категория на група.</span><span class="sxs-lookup"><span data-stu-id="5c845-129">Select a category group.</span></span>

## <a name="category-groups"></a><span data-ttu-id="5c845-130">Групи на категория</span><span class="sxs-lookup"><span data-stu-id="5c845-130">Category groups</span></span>

<span data-ttu-id="5c845-131">Групите категории се използват за споделяне на свойства, предимно публикуване на профили, между свързани категории на проекта.</span><span class="sxs-lookup"><span data-stu-id="5c845-131">Category groups are used to share properties, primarily posting profiles, between related Project categories.</span></span> <span data-ttu-id="5c845-132">Трябва да има поне една категория група за всеки тип транзакция и на всяка категория проект се присвоява група.</span><span class="sxs-lookup"><span data-stu-id="5c845-132">There must be at least one category group for each transaction type and each project category is assigned a group.</span></span>

<span data-ttu-id="5c845-133">Спецификациите за командироване в Project Operations се определят от правилата за профила на разходите и приходите на проекта, категориите проекти и групите категории.</span><span class="sxs-lookup"><span data-stu-id="5c845-133">The posting specifications in Project Operations are defined by the project cost and revenue profile rules, project categories, and category groups.</span></span> <span data-ttu-id="5c845-134">Можете да настроите групи категории, като отидете на **Управление на проекти и счетоводство** \> **Настройка** \> **Категории** \> **Групи по категории**.</span><span class="sxs-lookup"><span data-stu-id="5c845-134">You can set up category groups by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Category groups**.</span></span>
