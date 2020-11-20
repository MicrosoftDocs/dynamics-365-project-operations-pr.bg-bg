---
title: Стойности по подразбиране за финансово измерение
description: Тази тема предоставя информация за това как да настроите финансовите измерения по подразбиране.
author: sigitac
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: aa6771ba5346fd4133b82c3e670badfa7655299f
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131870"
---
# <a name="financial-dimension-defaults"></a><span data-ttu-id="bdc9c-103">Стойности по подразбиране за финансово измерение</span><span class="sxs-lookup"><span data-stu-id="bdc9c-103">Financial dimension defaults</span></span>

<span data-ttu-id="bdc9c-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="bdc9c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="bdc9c-105">Dynamics 365 Project Operations използва рамката [Финансови измерения](https://docs.microsoft.com/dynamics365/finance/general-ledger/financial-dimensions) в Dynamics 365 Finance за предоставяне на допълнителни аналитични данни за транзакции в подкнигата и общата счетоводна книга.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-105">Dynamics 365 Project Operations uses the [Financial dimensions](https://docs.microsoft.com/dynamics365/finance/general-ledger/financial-dimensions) framework in Dynamics 365 Finance to provide additional insights on project subledger and general ledger transactions.</span></span>

<span data-ttu-id="bdc9c-106">Финансовите измерения по подразбиране могат да се зададат за клиент, източник на финансиране на проекта, контролна точка, аспекти на договор по проект или проект.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-106">Default financial dimensions can be set on a customer, project funding source, milestone, project contract line, or project.</span></span>

## <a name="define-default-financial-dimensions-for-a-customer"></a><span data-ttu-id="bdc9c-107">Определяне на финансовите измерения по подразбиране за клиент</span><span class="sxs-lookup"><span data-stu-id="bdc9c-107">Define default financial dimensions for a customer</span></span>

<span data-ttu-id="bdc9c-108">По подразбиране клиентските измерения са посочени във Finance.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-108">Customer dimension defaults are specified in Finance.</span></span> <span data-ttu-id="bdc9c-109">Изпълнете следните стъпки, за да настроите измерения по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-109">Complete the following steps to set dimension defaults.</span></span>

1. <span data-ttu-id="bdc9c-110">Отидете на **Вземания** > **Клиенти** > **Всички клиенти**.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-110">Go to **Accounts receivable** > **Customers** > **All customers**.</span></span>
2. <span data-ttu-id="bdc9c-111">На страницата **Клиенти**, в раздела **Финансови измерения** задайте стойностите на финансовите измерения за конкретния клиент.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-111">On the **Customers** page, on the **Financial dimensions** tab, set the financial dimension values for specific customer.</span></span>

## <a name="define-default-financial-dimensions-for-project-contracts"></a><span data-ttu-id="bdc9c-112">Определяне на финансовите измерения за договори по проект</span><span class="sxs-lookup"><span data-stu-id="bdc9c-112">Define default financial dimensions for project contracts</span></span>

<span data-ttu-id="bdc9c-113">Договорите по проект се създават и поддържат в Common Data Service (CDS).</span><span class="sxs-lookup"><span data-stu-id="bdc9c-113">Project contracts are created and maintained in Common Data Service (CDS).</span></span> <span data-ttu-id="bdc9c-114">Счетоводните атрибути за договорите по проект са зададени в модула **Управление на проекти и счетоводство** във Finance.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-114">Accounting attributes for project contracts are set in the **Project management and accounting** module in Finance.</span></span>

### <a name="set-financial-dimensions-for-a-project-funding-source"></a><span data-ttu-id="bdc9c-115">Задайте финансови измерения за източник на финансиране на проект</span><span class="sxs-lookup"><span data-stu-id="bdc9c-115">Set financial dimensions for a project funding source</span></span>

1. <span data-ttu-id="bdc9c-116">Отидете на **Управление на проекти и счетоводство** > **Проекти** > **Договори по проекти**.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-116">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="bdc9c-117">Изберете записа, който искате да актуализирате, и в раздела **Договор по проект** изберете **Показване на счетоводство по подразбиране**.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-117">Select the record you want to update, and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="bdc9c-118">Разгънете **Свързана информация** и изберете раздела **Източници на финансиране**.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-118">Expand **Related information** and select the **Funding sources** tab.</span></span>
4. <span data-ttu-id="bdc9c-119">Задайте стойности по подразбиране за финансово измерение.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-119">Set the financial dimension defaults.</span></span> <span data-ttu-id="bdc9c-120">Обърнете внимание, че финансовите измерения по подразбиране са от акаунта на клиента.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-120">Notice that the financial dimensions default from the customer account.</span></span>

### <a name="set-financial-dimensions-for-a-project-contract-line"></a><span data-ttu-id="bdc9c-121">Задаване на финансови измерения за аспекти на договор по проект</span><span class="sxs-lookup"><span data-stu-id="bdc9c-121">Set financial dimensions for a project contract line</span></span>

1. <span data-ttu-id="bdc9c-122">Отидете на **Управление на проекти и счетоводство** > **Проекти** > **Договори по проекти**.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-122">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="bdc9c-123">Изберете записа, който искате да актуализирате, и в раздела **Договор по проект** изберете **Показване на счетоводство по подразбиране**.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-123">Select the record you want to update and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="bdc9c-124">Разгънете **Свързана информация** и изберете раздела **Аспекти на договор**.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-124">Expand **Related information** and select the **Contract lines** tab.</span></span>
4. <span data-ttu-id="bdc9c-125">Задайте стойности по подразбиране за финансово измерение.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-125">Set the financial dimension defaults.</span></span> <span data-ttu-id="bdc9c-126">Финансовите измерения по подразбиране са приложими и могат да се използват само с аспекти на договор с фиксирана цена (контролна точка).</span><span class="sxs-lookup"><span data-stu-id="bdc9c-126">The financial dimension defaults are applicable and can be used only with Fixed price (milestone) contract lines.</span></span>

<span data-ttu-id="bdc9c-127">Тези стойности по подразбиране се използват за свързани трансакции по акаунт на проект и редове на фактури.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-127">These defaults are used on related project on-account transactions and invoice lines.</span></span>

## <a name="define-default-financial-dimensions-for-projects"></a><span data-ttu-id="bdc9c-128">Определяне на финансовите измерения за проекти</span><span class="sxs-lookup"><span data-stu-id="bdc9c-128">Define default financial dimensions for projects</span></span>

<span data-ttu-id="bdc9c-129">Проектите се създават и поддържат в CDS.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-129">Projects are created and maintained in CDS.</span></span> <span data-ttu-id="bdc9c-130">Счетоводните атрибути за проектите са зададени в модула **Управление на проекти и счетоводство** във Finance.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-130">Accounting attributes for projects are set in the **Project management and accounting** module in Finance.</span></span>

1. <span data-ttu-id="bdc9c-131">Отидете на **Управление на проекти и счетоводство** > **Проекти** > **Всички проекти**.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-131">Go to **Project management and accounting** > **Projects** > **All projects**.</span></span>
2. <span data-ttu-id="bdc9c-132">Изберете записа, който искате да актуализирате, и в раздела **Проект** изберете **Показване на счетоводство по подразбиране**.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-132">Select the record that you want to update and on the **Project** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="bdc9c-133">Разгънете **Свързана информация** и изберете раздела **Настройка**.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-133">Expand **Related information** and select the **Setup** tab.</span></span>
4. <span data-ttu-id="bdc9c-134">Задайте стойности по подразбиране за финансово измерение.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-134">Set the financial dimension defaults.</span></span> <span data-ttu-id="bdc9c-135">Обърнете внимание, че финансовите измерения по подразбиране са от акаунта на клиента.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-135">Notice that financial dimensions default from the customer account.</span></span> <span data-ttu-id="bdc9c-136">Ако проектът е свързан с аспекти на договор с множество клиенти на договор по проект, основният клиент се използва за финансови измерения по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-136">If the project is associated with a contract line with multiple project contract customers, the primary customer is used to default financial dimensions.</span></span>

<span data-ttu-id="bdc9c-137">Финансовите измерения по подразбиране на проекта се използват за задаване на стойности по подразбиране за счетоводен запис за трансакции за време, разход и такса в **журнала за интеграция на Project Operations** и в свързаните редове на фактура по проект.</span><span class="sxs-lookup"><span data-stu-id="bdc9c-137">Project default financial dimensions are used to set journal line defaults for time, expense, and fee transactions in the **Project Operations Integration Journal** and on related project invoice lines.</span></span>
