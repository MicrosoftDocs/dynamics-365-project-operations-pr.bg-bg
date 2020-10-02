---
title: Отчети за разходи и множество одобряващи
description: Тази тема предоставя информация за отчетите за разходите, които изискват одобрение от повече от едно лице.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 818092dd631d07cc0a7d63c9eec51eeff4f67ffe
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897078"
---
# <a name="expense-reports-and-multiple-approvers"></a><span data-ttu-id="6c454-103">Отчети за разходи и множество одобряващи</span><span class="sxs-lookup"><span data-stu-id="6c454-103">Expense reports and multiple approvers</span></span>

<span data-ttu-id="6c454-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="6c454-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="6c454-105">В зависимост от политиките за одобрение на разходите на вашата организация може да се наложи повече от едно лице да одобри представен отчет за разходите.</span><span class="sxs-lookup"><span data-stu-id="6c454-105">Depending on your organization's expense approval policies, more than one person might have to approve a submitted expense report.</span></span> <span data-ttu-id="6c454-106">Когато настройвате процеса на работния поток за одобрение на отчета за разходите, можете да добавите елементи на работния поток, които включват задачи или стъпки за един или повече одобряващи отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="6c454-106">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="6c454-107">Например може да изискате всички отчети за разходите да бъдат одобрени от двама отделни души, мениджъра на служителя, който е представил отчета, и координатора на задълженията по сметките.</span><span class="sxs-lookup"><span data-stu-id="6c454-107">For example, you might require that all expense reports be approved by two separate people, the manager of the employee who submitted the report and the Accounts payable coordinator.</span></span>

<span data-ttu-id="6c454-108">Ако решите да изисквате множество одобряващи отчети за разходите, можете да добавите елементи на работния поток по всеки от следните начини:</span><span class="sxs-lookup"><span data-stu-id="6c454-108">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="6c454-109">Добавете един елемент за одобрение, който има една стъпка.</span><span class="sxs-lookup"><span data-stu-id="6c454-109">Add one approval element that has one step.</span></span> <span data-ttu-id="6c454-110">Например, стъпката може да изисква отчет за разходите да бъде присвоен на група потребители и да бъде одобрен от 50 процента от членовете на групата потребители.</span><span class="sxs-lookup"><span data-stu-id="6c454-110">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="6c454-111">Добавете един елемент за одобрение, който има няколко стъпки.</span><span class="sxs-lookup"><span data-stu-id="6c454-111">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="6c454-112">Например елементът за одобрение може да има следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="6c454-112">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="6c454-113">Управителят на служителя, подал отчета за разходите, го одобрява.</span><span class="sxs-lookup"><span data-stu-id="6c454-113">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="6c454-114">Служителят по задълженията проверява разписките и елементите на отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="6c454-114">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="6c454-115">Собственикът на бюджета одобрява отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="6c454-115">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="6c454-116">Добавете множество елементи за одобрение, всеки от които има една стъпка.</span><span class="sxs-lookup"><span data-stu-id="6c454-116">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="6c454-117">Например можете да добавите отделен елемент за одобрение за всяка от следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="6c454-117">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="6c454-118">Мениджърът на служителя одобрява отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="6c454-118">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="6c454-119">Собственикът на бюджета одобрява отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="6c454-119">The budget owner approves the expense report.</span></span>
