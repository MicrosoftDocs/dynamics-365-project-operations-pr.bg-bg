---
title: Настройване на работни потоци за управление на разходите
description: Можете да настроите процес на работен поток за преглед и одобряване на документи за пътуване и разходи.
author: ShylaThompson
manager: AnnBe
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 36ab1edc4769013684fa9248e6c5eac025637bbd
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271610"
---
# <a name="set-up-expense-management-workflows"></a><span data-ttu-id="1fbb5-103">Настройване на работни потоци за управление на разходите</span><span class="sxs-lookup"><span data-stu-id="1fbb5-103">Set up Expense management workflows</span></span>

<span data-ttu-id="1fbb5-104">Можете да настроите процес на работен поток, който се използва за преглед и одобряване на документи за пътуване и разходи.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-104">You can set up a workflow process that is used to review and approve travel and expense documents.</span></span> <span data-ttu-id="1fbb5-105">Документите, за които работните потоци могат да бъдат определени, включват отчети за разходите, заявки за пътуване и искания за авансови плащания.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-105">The documents for which workflows can be defined include expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="1fbb5-106">Работният процес представлява бизнес процес.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-106">A workflow represents a business process.</span></span> <span data-ttu-id="1fbb5-107">Той определя как даден документ протича през системата и указва кой трябва да изпълни задача или да одобри документ.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-107">It defines how a document flows through the system and indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="1fbb5-108">Има няколко предимства от използването на системата за работен поток във вашата организация:</span><span class="sxs-lookup"><span data-stu-id="1fbb5-108">There are several benefits of using the workflow system in your organization:</span></span>

-   <span data-ttu-id="1fbb5-109">**Последователни процеси** – Можете да дефинирате процеса на одобрение за конкретни документи, като заявки за покупка и отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-109">**Consistent processes** — You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="1fbb5-110">Използването на системата на работния процес помага да се гарантира, че документите се обработват и одобряват по последователен и ефективен начин.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-110">Using the workflow system helps to ensure that documents are processed and approved in a consistent and efficient manner.</span></span>

-   <span data-ttu-id="1fbb5-111">Видимост на процеса – Можете да проследявате метриките на състоянието, историята и производителността на конкретен екземпляр на работния поток.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-111">Process visibility — You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="1fbb5-112">Това ви помага да определите дали трябва да се правят промени в работния процес, за да се подобри ефективността.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-112">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>

-   <span data-ttu-id="1fbb5-113">Централизиран работен списък – Потребителите могат да преглеждат централизиран работен списък, за да видят задачите на работния процес и одобренията, които са им възложени.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-113">Centralized work list — Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

<span data-ttu-id="1fbb5-114">**Типовете на работни потоци, които можете да създавате**</span><span class="sxs-lookup"><span data-stu-id="1fbb5-114">**The types of workflows you can create**</span></span>

<span data-ttu-id="1fbb5-115">Следващата таблица изброява видовете работни потоци, в които можете да създавате **Разходи**.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-115">The following table lists the types of workflows that you can create in **Expense**.</span></span>


|              <span data-ttu-id="1fbb5-116"><strong>Тип</strong></span><span class="sxs-lookup"><span data-stu-id="1fbb5-116"><strong>Type</strong></span></span>              |                   <span data-ttu-id="1fbb5-117"><strong>Използвайте този тип за</strong></span><span class="sxs-lookup"><span data-stu-id="1fbb5-117"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|         <span data-ttu-id="1fbb5-118"><strong>Отчет за разходите</strong></span><span class="sxs-lookup"><span data-stu-id="1fbb5-118"><strong>Expense report</strong></span></span>         |            <span data-ttu-id="1fbb5-119">Създайте работни потоци за одобрение за отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-119">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="1fbb5-120"><strong>Автоматично публикуване на отчети за разходи</strong></span><span class="sxs-lookup"><span data-stu-id="1fbb5-120"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="1fbb5-121">Създайте работни потоци за автоматично одобрение за отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-121">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="1fbb5-122"><strong>Елемент на ред за разходи</strong></span><span class="sxs-lookup"><span data-stu-id="1fbb5-122"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="1fbb5-123">Създайте работни потоци за одобрение за елементи от ред и отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-123">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="1fbb5-124"><strong>Автоматично осчетоводяване на елемент на ред за разходи</strong></span><span class="sxs-lookup"><span data-stu-id="1fbb5-124"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="1fbb5-125">Създайте работни потоци за автоматично одобрение за елементи от ред и отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-125">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="1fbb5-126"><strong>Заявка за пътуване</strong></span><span class="sxs-lookup"><span data-stu-id="1fbb5-126"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="1fbb5-127">Създайте работни процеси за одобрение за заявки за пътуване.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-127">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="1fbb5-128"><strong>Заявка за аванс в брой</strong></span><span class="sxs-lookup"><span data-stu-id="1fbb5-128"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="1fbb5-129">Създайте работни потоци за одобрение за заявки за авансови плащания.</span><span class="sxs-lookup"><span data-stu-id="1fbb5-129">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="1fbb5-130"><strong>Възстановяване на данък ДДС</strong></span><span class="sxs-lookup"><span data-stu-id="1fbb5-130"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="1fbb5-131">Създайте работни потоци за одобрение за възстановяване на данък върху добавената стойност (ДДС).</span><span class="sxs-lookup"><span data-stu-id="1fbb5-131">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |



[!INCLUDE[footer-include](../includes/footer-banner.md)]