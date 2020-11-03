---
title: Множество одобряващи за отчет за разходите
description: Тази тема предоставя информация за отчетите за разходите, които изискват одобрение от множество хора.
author: saraschi2
manager: AnnBe
ms.date: 02/23/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvExpensesReportList
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: ce24b156a268f9f5aada35f9314d2d9c6607200b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071976"
---
# <a name="multiple-approvers-on-an-expense-report"></a><span data-ttu-id="bde2d-103">Множество одобряващи за отчет за разходите</span><span class="sxs-lookup"><span data-stu-id="bde2d-103">Multiple approvers on an expense report</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="bde2d-104">В зависимост от политиките за одобрение на разходите на вашата организация може да се наложи повече от едно лице да одобри отчет за разходите, подаден от служител.</span><span class="sxs-lookup"><span data-stu-id="bde2d-104">Depending on your organization's expense approval policies, more than one person might have to approve an expense report that is submitted by an employee.</span></span> <span data-ttu-id="bde2d-105">Когато настройвате процеса на работния поток за одобрение на отчета за разходите, можете да добавите елементи на работния поток, които включват задачи или стъпки за един или повече одобряващи отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="bde2d-105">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="bde2d-106">Например може да изискате всички отчети за разходите да бъдат одобрени първо от мениджъра на служителя, който е представил отчета, и след това от координатора на задълженията по сметките.</span><span class="sxs-lookup"><span data-stu-id="bde2d-106">For example, you might require that all expense reports be approved first by the manager of the employee who submitted the report and then by the Accounts payable coordinator.</span></span>

<span data-ttu-id="bde2d-107">Ако решите да изисквате множество одобряващи отчети за разходите, можете да добавите елементи на работния поток по всеки от следните начини:</span><span class="sxs-lookup"><span data-stu-id="bde2d-107">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="bde2d-108">Добавете един елемент за одобрение, който има една стъпка.</span><span class="sxs-lookup"><span data-stu-id="bde2d-108">Add one approval element that has one step.</span></span> <span data-ttu-id="bde2d-109">Например, стъпката може да изисква отчет за разходите да бъде присвоен на група потребители и да бъде одобрен от 50 процента от членовете на групата потребители.</span><span class="sxs-lookup"><span data-stu-id="bde2d-109">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="bde2d-110">Добавете един елемент за одобрение, който има няколко стъпки.</span><span class="sxs-lookup"><span data-stu-id="bde2d-110">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="bde2d-111">Например елементът за одобрение може да има следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="bde2d-111">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="bde2d-112">Управителят на служителя, подал отчета за разходите, го одобрява.</span><span class="sxs-lookup"><span data-stu-id="bde2d-112">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="bde2d-113">Служителят по задълженията проверява разписките и елементите на отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="bde2d-113">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="bde2d-114">Собственикът на бюджета одобрява отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="bde2d-114">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="bde2d-115">Добавете множество елементи за одобрение, всеки от които има една стъпка.</span><span class="sxs-lookup"><span data-stu-id="bde2d-115">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="bde2d-116">Например можете да добавите отделен елемент за одобрение за всяка от следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="bde2d-116">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="bde2d-117">Мениджърът на служителя одобрява отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="bde2d-117">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="bde2d-118">Собственикът на бюджета одобрява отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="bde2d-118">The budget owner approves the expense report.</span></span>
