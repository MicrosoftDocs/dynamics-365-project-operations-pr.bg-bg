---
title: Заявки за пътуване
description: Тази тема предоставя информация относно заявките за пътуване.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 46a678ac4486c99f11d74dbac07dedd08364cb2f
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4123725"
---
# <a name="travel-requisitions"></a><span data-ttu-id="cd7cf-103">Заявки за пътуване</span><span class="sxs-lookup"><span data-stu-id="cd7cf-103">Travel requisitions</span></span>

<span data-ttu-id="cd7cf-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="cd7cf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="cd7cf-105">В заявката за пътуване са посочени разходите, които ще бъдат направени за целите на пътуването.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-105">A travel requisition lists the expenses that will be incurred for the purpose of travel.</span></span> <span data-ttu-id="cd7cf-106">Заявка за пътуване се представя за преглед и може да се използва за оторизиране на разходи.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-106">A travel requisition is submitted for review and can be used to authorize expenses.</span></span>

<span data-ttu-id="cd7cf-107">Може да се наложи да подадете заявка за пътуване, преди да понесете някакви разходи, които са начислени на организацията.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-107">You may be required to submit a travel requisition before you incur any expense that is charged to the organization.</span></span> <span data-ttu-id="cd7cf-108">Това изискване се прилага, независимо дали начислявате разходи по корпоративна кредитна карта, харчите пари в брой, получени от аванс в брой, или правите разходи от джоба, които ще бъдат възстановени от организацията.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-108">This requirement applies, regardless of whether you charge expenses to a corporate credit card, spend cash that you received from a cash advance, or incur out-of-pocket expenses that will be reimbursed by the organization.</span></span>

<span data-ttu-id="cd7cf-109">Реквизициите за пътуване и политиките могат да се използват за подпомагане на управлението на разходите на организацията.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-109">Travel requisitions and policies can be used to help manage organization expenditures.</span></span> <span data-ttu-id="cd7cf-110">Например, ако вашата организация работи по проект с фиксирана цена, който изисква пътуване, пътните разходи на членовете на екипа на проекта трябва да се поберат в бюджета на проекта.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-110">For example, if your organization is working on a fixed-price project that requires travel, the travel expenses of the project's team members must fit within the project budget.</span></span> <span data-ttu-id="cd7cf-111">Като изисква пътните разходи да бъдат одобрени преди да бъдат направени, организацията може да помогне да се гарантира, че проектът остава в рамките на бюджета.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-111">By requiring that travel expenses be approved before they are incurred, the organization can help make sure that the project remains within budget.</span></span>

## <a name="configuration"></a><span data-ttu-id="cd7cf-112">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="cd7cf-112">Configuration</span></span> 

<span data-ttu-id="cd7cf-113">Изискванията за пътуване могат да бъдат конфигурирани като „задължителни“, като се активира параметърът „Преупълномощаването на пътуването е задължително“ в параметрите за управление на разходите.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-113">Travel Requisitions can be configured as "mandatory" by enabling the "Pre-authorization of travel is mandatory" parameter in Expense Management Parameters.</span></span> 

## <a name="create-and-submit-a-travel-requisition"></a><span data-ttu-id="cd7cf-114">Създайте и изпратете заявка за пътуване</span><span class="sxs-lookup"><span data-stu-id="cd7cf-114">Create and submit a travel requisition</span></span>

1. <span data-ttu-id="cd7cf-115">Отидете на **Моите разходи: Заявка за пътуване** и изберете **Нова заявка за пътуване**.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-115">Go to **My expenses: Travel Requisition**, and select **New travel Requisition**.</span></span>
2. <span data-ttu-id="cd7cf-116">Въведете цел и дестинация за заявката.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-116">Enter a purpose and destination for the requisition.</span></span>
3. <span data-ttu-id="cd7cf-117">В полето **Описание на пътуването**, въведете допълнителна информация.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-117">In the  **Travel description** field, enter any additional information.</span></span> 
4. <span data-ttu-id="cd7cf-118">За всеки от очакваните разходи, като полет, хранене или автомобил под наем, създайте разходна позиция.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-118">For each of the expected expenses, such as Flight, meals, or car rental, create an expense line item.</span></span> <span data-ttu-id="cd7cf-119">Включете прогнозната дата, прогнозната сума и валутата за всеки разход.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-119">Include the estimated date, estimated amount, and the currency for each expense.</span></span> 
5. <span data-ttu-id="cd7cf-120">Когато приключите с добавянето на очакваните разходи, изберете **Запазете**.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-120">When you have finished adding the expected expenses, select **Save**.</span></span>
6. <span data-ttu-id="cd7cf-121">Когато сте готови да подадете заявката за пътуване, изберете **Работен поток** > **Подаване**.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-121">When you are ready to submit the travel requisition, select **Workflow** > **Submit**.</span></span>

<span data-ttu-id="cd7cf-122">Можете да видите вашите одобрени заявки за пътуване под **Моите разходи: Заявка за пътуване**.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-122">You can view your approved travel requisitions under **My Expenses: Travel Requisition**.</span></span> 

## <a name="view-available-travel-requisitions"></a><span data-ttu-id="cd7cf-123">Вижте наличните заявки за пътуване</span><span class="sxs-lookup"><span data-stu-id="cd7cf-123">View available travel requisitions</span></span>

<span data-ttu-id="cd7cf-124">Можете да видите всички свои заявки за пътуване под **Моите разходи: Заявка за пътуване**.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-124">You can view all of your travel requisitions under **My Expenses: Travel Requisitions**.</span></span>

## <a name="approve-travel-requisitions"></a><span data-ttu-id="cd7cf-125">Одобряване на заявки за пътуване</span><span class="sxs-lookup"><span data-stu-id="cd7cf-125">Approve travel requisitions</span></span>

<span data-ttu-id="cd7cf-126">Изберете заявката за пътуване, която искате да одобрите, и след това изберете **Работен поток** > **Одобряване**.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-126">Select the travel requisition that you want to approve, and then select **Workflow** > **Approve**.</span></span>  

## <a name="submit-an-expense-report-using-your-approved-travel-requisition"></a><span data-ttu-id="cd7cf-127">Изпратете отчет за разходите, като използвате одобрената заявка за пътуване</span><span class="sxs-lookup"><span data-stu-id="cd7cf-127">Submit an expense report using your approved travel requisition</span></span>

1. <span data-ttu-id="cd7cf-128">Създайте нов отчет за разходите и в заглавието на отчета за разходите и от списъка с одобрени заявки за пътуване изберете **Карта за заявка за пътуване**.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-128">Create a new expense report and in the expense report header, and from the list of approved travel requisitions, select **Map to Travel requisition**.</span></span>
2. <span data-ttu-id="cd7cf-129">Полето **Сума за заявка за пътуване** се актуализира автоматично в заглавката на отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-129">The **Travel requisition amount** field is automatically updated in the expense report header.</span></span>
3. <span data-ttu-id="cd7cf-130">Добавете всички разходи, направени за пътуването.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-130">Add each expense incurred for the trip.</span></span> <span data-ttu-id="cd7cf-131">Ако полето **Предварително удостоверено** е активирано, съгласуваната сума и разрешената сума за конкретната категория разходи ще бъдат актуализирани.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-131">If the **Pre-authorized** field is enabled, the reconciled amount and authorized amount for the specific expense category will be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="cd7cf-132">Когато съпоставяте отчет за разходите с одобрена заявка за пътуване, сумата на транзакцията не може да бъде по-голяма от разрешената сума.</span><span class="sxs-lookup"><span data-stu-id="cd7cf-132">When you map an expense report to an approved travel requisition, the transaction amount can't be greater than the authorized amount.</span></span> 
