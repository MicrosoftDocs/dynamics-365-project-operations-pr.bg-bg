---
title: Настройте работни потоци за управление на разходите
description: Можете да настроите процес на работен поток, който се използва за преглед и одобряване на документи за пътуване и разходи.
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
ms.openlocfilehash: dfc5945f32bb8d4073fc31499979ba279fef66a4
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896538"
---
# <a name="set-up-workflows-for-expense-management"></a><span data-ttu-id="f07a3-103">Настройте работни потоци за управление на разходите</span><span class="sxs-lookup"><span data-stu-id="f07a3-103">Set up workflows for Expense management</span></span>

<span data-ttu-id="f07a3-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="f07a3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f07a3-105">Можете да настроите процес на работен поток за преглед и одобряване на документи за пътуване и разходи.</span><span class="sxs-lookup"><span data-stu-id="f07a3-105">You can set up a workflow process to review and approve travel and expense documents.</span></span> <span data-ttu-id="f07a3-106">Можете да дефинирате работни потоци за отчети за разходите, заявки за пътуване и искания за авансови плащания.</span><span class="sxs-lookup"><span data-stu-id="f07a3-106">You can define workflows for expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="f07a3-107">Работният процес представлява бизнес процес и определя начина, по който документът протича през системата.</span><span class="sxs-lookup"><span data-stu-id="f07a3-107">A workflow represents a business process and defines how a document flows through the system.</span></span> <span data-ttu-id="f07a3-108">Работният процес също така посочва кой трябва да изпълни задача или да одобри документ.</span><span class="sxs-lookup"><span data-stu-id="f07a3-108">The workflow also indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="f07a3-109">Има няколко предимства от използването на системата за работен поток във вашата организация:</span><span class="sxs-lookup"><span data-stu-id="f07a3-109">There are several benefits of using the workflow system in your organization:</span></span>

- <span data-ttu-id="f07a3-110">**Последователни процеси**: Можете да дефинирате процеса на одобрение за конкретни документи, като заявки за покупка и отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="f07a3-110">**Consistent processes**: You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="f07a3-111">Използването на системата на работния процес помага да се гарантира, че документите се обработват и одобряват по последователен и ефективен начин.</span><span class="sxs-lookup"><span data-stu-id="f07a3-111">Using the workflow system helps ensure that documents are processed and approved in a consistent and efficient manner.</span></span>
- <span data-ttu-id="f07a3-112">**Видимост на процеса**: Можете да проследявате метриките на състоянието, историята и производителността на конкретен екземпляр на работния поток.</span><span class="sxs-lookup"><span data-stu-id="f07a3-112">**Process visibility**: You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="f07a3-113">Това ви помага да определите дали трябва да се правят промени в работния процес, за да се подобри ефективността.</span><span class="sxs-lookup"><span data-stu-id="f07a3-113">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>
- <span data-ttu-id="f07a3-114">**Централизиран работен списък**: Потребителите могат да преглеждат централизиран работен списък, за да видят задачите на работния процес и одобренията, които са им възложени.</span><span class="sxs-lookup"><span data-stu-id="f07a3-114">**Centralized work list**: Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

## <a name="workflow-types"></a><span data-ttu-id="f07a3-115">Типове работен поток</span><span class="sxs-lookup"><span data-stu-id="f07a3-115">Workflow types</span></span>

<span data-ttu-id="f07a3-116">Следващата таблица изброява видовете работни потоци, в които можете да създавате **Управление на разходите**.</span><span class="sxs-lookup"><span data-stu-id="f07a3-116">The following table lists the types of workflows that you can create in **Expense Management**.</span></span>


|              <span data-ttu-id="f07a3-117"><strong>Тип</strong></span><span class="sxs-lookup"><span data-stu-id="f07a3-117"><strong>Type</strong></span></span>              |                   <span data-ttu-id="f07a3-118"><strong>Използвайте този тип за</strong></span><span class="sxs-lookup"><span data-stu-id="f07a3-118"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|   <span data-ttu-id="f07a3-119"><strong>Автоматично одобряване на отчети за разходи</strong></span><span class="sxs-lookup"><span data-stu-id="f07a3-119"><strong>Expense report auto approval</strong></span></span> |            <span data-ttu-id="f07a3-120">Създайте работни потоци за одобрение за отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="f07a3-120">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="f07a3-121"><strong>Автоматично публикуване на отчети за разходи</strong></span><span class="sxs-lookup"><span data-stu-id="f07a3-121"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="f07a3-122">Създайте работни потоци за автоматично одобрение за отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="f07a3-122">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="f07a3-123"><strong>Елемент на ред за разходи</strong></span><span class="sxs-lookup"><span data-stu-id="f07a3-123"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="f07a3-124">Създайте работни потоци за одобрение за елементи от ред и отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="f07a3-124">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="f07a3-125"><strong>Автоматично осчетоводяване на елемент на ред за разходи</strong></span><span class="sxs-lookup"><span data-stu-id="f07a3-125"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="f07a3-126">Създайте работни потоци за автоматично одобрение за елементи от ред и отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="f07a3-126">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="f07a3-127"><strong>Заявка за пътуване</strong></span><span class="sxs-lookup"><span data-stu-id="f07a3-127"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="f07a3-128">Създайте работни процеси за одобрение за заявки за пътуване.</span><span class="sxs-lookup"><span data-stu-id="f07a3-128">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="f07a3-129"><strong>Заявка за аванс в брой</strong></span><span class="sxs-lookup"><span data-stu-id="f07a3-129"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="f07a3-130">Създайте работни потоци за одобрение за заявки за авансови плащания.</span><span class="sxs-lookup"><span data-stu-id="f07a3-130">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="f07a3-131"><strong>Възстановяване на данък ДДС</strong></span><span class="sxs-lookup"><span data-stu-id="f07a3-131"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="f07a3-132">Създайте работни потоци за одобрение за възстановяване на данък върху добавената стойност (ДДС).</span><span class="sxs-lookup"><span data-stu-id="f07a3-132">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |