---
title: Прогнози за разноски
description: Тази тема предоставя информация за определяне или оценка на разходи, базирани на проекти.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2afe4ff2f84fc5426c409e6314da73b11a4de281
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907878"
---
# <a name="expense-estimates"></a><span data-ttu-id="cdc0b-103">Прогнози за разноски</span><span class="sxs-lookup"><span data-stu-id="cdc0b-103">Expense estimates</span></span>
<span data-ttu-id="cdc0b-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="cdc0b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cdc0b-105">Заедно с дефинирането на базирани на ресурси оценки, Dynamics 365 Project Operations позволява на мениджърите на проекти да определят разходите, базирани на проекта, за всеки проект.</span><span class="sxs-lookup"><span data-stu-id="cdc0b-105">Along with defining resource-based estimates, Dynamics 365 Project Operations allows Project managers to define project-based expenses for each project.</span></span> <span data-ttu-id="cdc0b-106">Всяка разходна позиция може да бъде свързана с конкретна проектна задача или категория разходи.</span><span class="sxs-lookup"><span data-stu-id="cdc0b-106">Each expense item can be associated with a specific project task or expense category.</span></span> <span data-ttu-id="cdc0b-107">Категориите на разходите обикновено се определят на организационно ниво.</span><span class="sxs-lookup"><span data-stu-id="cdc0b-107">Expense categories are typically defined at the organizational level.</span></span> <span data-ttu-id="cdc0b-108">Ценообразуването за всяка категория разходи обикновено се определя в следната йерархия:</span><span class="sxs-lookup"><span data-stu-id="cdc0b-108">Pricing for each expense category is typically defined in the following hierarchy:</span></span>

- <span data-ttu-id="cdc0b-109">Организация</span><span class="sxs-lookup"><span data-stu-id="cdc0b-109">Organization</span></span>
- <span data-ttu-id="cdc0b-110">Клиент</span><span class="sxs-lookup"><span data-stu-id="cdc0b-110">Customer</span></span>
- <span data-ttu-id="cdc0b-111">Оферта/договор</span><span class="sxs-lookup"><span data-stu-id="cdc0b-111">Quote/contract</span></span>

<span data-ttu-id="cdc0b-112">Изпълнете следните стъпки, за да видите, добавите или изтриете разходи за проект.</span><span class="sxs-lookup"><span data-stu-id="cdc0b-112">Complete the following steps to view, add, or delete a project expense.</span></span>

1. <span data-ttu-id="cdc0b-113">Отидете на **Проекти** и изберете проекта, по който искате да работите.</span><span class="sxs-lookup"><span data-stu-id="cdc0b-113">Go to **Projects**, and select the project you want to work on.</span></span>
2. <span data-ttu-id="cdc0b-114">Изберете раздела **Оценки на проекти** и вижте списъка с разходите по проекта.</span><span class="sxs-lookup"><span data-stu-id="cdc0b-114">Select the **Project Estimates** tab and view the list of project expenses.</span></span>
3. <span data-ttu-id="cdc0b-115">Изберете **Нови разходи** за да добавите разход.</span><span class="sxs-lookup"><span data-stu-id="cdc0b-115">Select **New Expense** to add an expense.</span></span> <span data-ttu-id="cdc0b-116">Или изберете разход за изтриване и след това изберете **Изтриване на разходите**.</span><span class="sxs-lookup"><span data-stu-id="cdc0b-116">Or, select an expense to delete, and then select **Delete Expense**.</span></span>

<span data-ttu-id="cdc0b-117">Следните атрибути са дефинирани за всяка разходна позиция:</span><span class="sxs-lookup"><span data-stu-id="cdc0b-117">The following attributes are defined for each expense line item:</span></span>

- <span data-ttu-id="cdc0b-118">**Категория**: Общите групи, използвани за описване на всички разходи, направени по даден проект.</span><span class="sxs-lookup"><span data-stu-id="cdc0b-118">**Category**: The common groupings used to describe all expenses incurred on a project.</span></span>
- <span data-ttu-id="cdc0b-119">**Начална дата**: Датата, на която се очаква да бъдат направени разходите.</span><span class="sxs-lookup"><span data-stu-id="cdc0b-119">**Start Date**: The date when the expense is forecasted to be incurred.</span></span>
- <span data-ttu-id="cdc0b-120">**Количество**: Очакваният брой разходни позиции за конкретна категория.</span><span class="sxs-lookup"><span data-stu-id="cdc0b-120">**Quantity**: The estimated number of expense items for a specific category.</span></span>
- <span data-ttu-id="cdc0b-121">**Единична себестойност**: Единичната цена, използвана за изчисляване на разходите.</span><span class="sxs-lookup"><span data-stu-id="cdc0b-121">**Unit Cost Price**: The unit price used to calculate to cost of the expense.</span></span>
- <span data-ttu-id="cdc0b-122">**Единична цена на продажба**: Единичната цена, използвана за изчисляване на цените за продажба на разходите.</span><span class="sxs-lookup"><span data-stu-id="cdc0b-122">**Unit Sales Price**: The unit price used to calculate the sale prices of the expense.</span></span>

