---
title: Работен поток за управление на разходите
description: Тази тема обяснява как можете да използвате системата за работен поток в Microsoft Dynamics 365 Finance, за да настроите процес на преглед на отчетите за разходи в управлението на разходите.
author: ShylaThompson
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 51ac2712f62d5c5d85b21c0ea929517ccb893bca
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005193"
---
# <a name="expense-management-workflow"></a><span data-ttu-id="0487b-103">Работен поток за управление на разходите</span><span class="sxs-lookup"><span data-stu-id="0487b-103">Expense management workflow</span></span>

<span data-ttu-id="0487b-104">Можете да използвате системата за работен поток, за да настроите процес на преглед на отчетите за разходи в управлението на разходите.</span><span class="sxs-lookup"><span data-stu-id="0487b-104">You can use the workflow system to set up a review process for expense reports in Expense management.</span></span> <span data-ttu-id="0487b-105">Можете да настроите работен поток, който използва следните критерии, за да определи кой одобрява отчетите за разходите:</span><span class="sxs-lookup"><span data-stu-id="0487b-105">You can set up a workflow that uses the following criteria to determine who approves expense reports:</span></span>

- <span data-ttu-id="0487b-106">Йерархия на отчитане на служителите и предварително дефинирани ограничения за одобрение</span><span class="sxs-lookup"><span data-stu-id="0487b-106">The employee reporting hierarchy and predefined approval limits</span></span>
- <span data-ttu-id="0487b-107">Одобрение на няколко нива, което поддържа временни одобряващи и окончателен одобряващ</span><span class="sxs-lookup"><span data-stu-id="0487b-107">Multi-level approval that supports interim approvers and a final approver</span></span>
- <span data-ttu-id="0487b-108">Финансови измерения и отговорност на проекта</span><span class="sxs-lookup"><span data-stu-id="0487b-108">Financial dimensions and project responsibility</span></span>
- <span data-ttu-id="0487b-109">Присвояване на конкретни потребители или потребителски групи</span><span class="sxs-lookup"><span data-stu-id="0487b-109">Assignment to specific users or user groups</span></span>

<span data-ttu-id="0487b-110">Одобренията на работния поток могат да бъдат създадени за отчети за разходи, заявки за пътуване, аванси в брой и възстановяване на данък върху добавената стойност (ДДС).</span><span class="sxs-lookup"><span data-stu-id="0487b-110">Workflow approvals can be created for expense reports, travel requisitions, cash advances, and value-added tax (VAT) recovery.</span></span>

<span data-ttu-id="0487b-111">**Пример**</span><span class="sxs-lookup"><span data-stu-id="0487b-111">**Example**</span></span>

<span data-ttu-id="0487b-112">Следващият процес е пример за работния процес за управление на разходите за отчет за разходите.</span><span class="sxs-lookup"><span data-stu-id="0487b-112">The following process is an example of the expense management workflow for an expense report.</span></span>

1. <span data-ttu-id="0487b-113">Служител създава и запазва отчет за разходите.</span><span class="sxs-lookup"><span data-stu-id="0487b-113">An employee creates and saves an expense report.</span></span>
2. <span data-ttu-id="0487b-114">Служителят подава отчета за разходите за одобрение.</span><span class="sxs-lookup"><span data-stu-id="0487b-114">The employee submits the expense report for approval.</span></span> <span data-ttu-id="0487b-115">Одобряващият се идентифицира въз основа на правилата, дефинирани при настройката на работния поток.</span><span class="sxs-lookup"><span data-stu-id="0487b-115">The approver is identified based on the rules that were defined when the workflow was set up.</span></span>
3. <span data-ttu-id="0487b-116">Одобряващият получава уведомление, че отчет за разходите е готов за одобрение.</span><span class="sxs-lookup"><span data-stu-id="0487b-116">The approver receives a notification that an expense report is ready for approval.</span></span> <span data-ttu-id="0487b-117">Одобряващият преглежда отчета за разходите и проверява дали са изпълнени следните условия:</span><span class="sxs-lookup"><span data-stu-id="0487b-117">The approver reviews the expense report and verifies that the following conditions are met:</span></span>

    - <span data-ttu-id="0487b-118">Разходите не нарушават никакви политики за разходи.</span><span class="sxs-lookup"><span data-stu-id="0487b-118">The expenses don't violate any expense policies.</span></span> <span data-ttu-id="0487b-119">Ако даден разход нарушава политика, одобряващият проверява дали отчетът за разходите включва валидна обосновка за бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0487b-119">If an expense violates a policy, the approver verifies that the expense report includes a valid business justification.</span></span>
    - <span data-ttu-id="0487b-120">Електронните разписки са приложени към отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="0487b-120">Electronic receipts are attached to the expense report.</span></span>

4. <span data-ttu-id="0487b-121">Одобряващият одобрява отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="0487b-121">The approver approves the expense report.</span></span>
5. <span data-ttu-id="0487b-122">Отчетът за разходите се възлага на координатора на задълженията за осчетоводяване.</span><span class="sxs-lookup"><span data-stu-id="0487b-122">The expense report is assigned to the Accounts payable coordinator for posting.</span></span>
6. <span data-ttu-id="0487b-123">Настъпва една от следните стъпки в зависимост от това дали е конфигурирано автоматично публикуване:</span><span class="sxs-lookup"><span data-stu-id="0487b-123">One of the following steps occurs, depending on whether automatic posting is configured:</span></span>

    - <span data-ttu-id="0487b-124">Ако е конфигурирано автоматично осчетоводяване, отчетът за разходите се обработва за плащане и се актуализира състоянието на отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="0487b-124">If automatic posting is configured, the expense report is processed for payment, and the status of the expense report is updated.</span></span>
    - <span data-ttu-id="0487b-125">Ако автоматичното осчетоводяване не е конфигурирано, координаторът на задълженията по сметките проверява дали са подадени всички оригинални разписки и че разписките са съобразени с разходите в отчета за разходите.</span><span class="sxs-lookup"><span data-stu-id="0487b-125">If automatic posting isn't configured, the Accounts payable coordinator verifies that all original receipts have been submitted, and that the receipts are aligned with the expenses on the expense report.</span></span> <span data-ttu-id="0487b-126">Всички данъчни кодове, които са въведени в отчета за разходите, също трябва да бъдат проверени като правилни.</span><span class="sxs-lookup"><span data-stu-id="0487b-126">All tax codes that are entered on the expense report must also be verified as correct.</span></span>

<span data-ttu-id="0487b-127">След като тези изисквания бъдат проверени, отчетът за разходите се публикува.</span><span class="sxs-lookup"><span data-stu-id="0487b-127">After these requirements are verified, the expense report is posted.</span></span>

<span data-ttu-id="0487b-128">След осчетоводяването на отчета за разходите се разрешава плащане за отчета за разходите и на служителя се възстановяват разходите.</span><span class="sxs-lookup"><span data-stu-id="0487b-128">After the expense report is posted, payment is authorized for the expense report, and the employee is reimbursed.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]