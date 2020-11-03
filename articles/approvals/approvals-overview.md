---
title: Общ преглед на одобренията
description: Тази тема предоставя информация за работа с одобрения в Project Operations.
author: stsporen
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 37994422e9146765076fdbb77f5c763b4f1d0802
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071680"
---
# <a name="approvals-overview"></a><span data-ttu-id="d06fa-103">Общ преглед на одобренията</span><span class="sxs-lookup"><span data-stu-id="d06fa-103">Approvals overview</span></span>

<span data-ttu-id="d06fa-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="d06fa-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d06fa-105">Представянията за време и разходи се движат през работния процес на одобрение.</span><span class="sxs-lookup"><span data-stu-id="d06fa-105">Time and Expense submissions move through an approval workflow.</span></span> <span data-ttu-id="d06fa-106">След като записите бъдат одобрени, транзакциите се записват в действителност или времето се записва в графика.</span><span class="sxs-lookup"><span data-stu-id="d06fa-106">After the entries are approved, transactions are recorded in actuals or time is booked in the schedule.</span></span>

## <a name="approvals-workflow"></a><span data-ttu-id="d06fa-107">Работен поток на одобрения</span><span class="sxs-lookup"><span data-stu-id="d06fa-107">Approvals workflow</span></span>
<span data-ttu-id="d06fa-108">Когато създавате и изпращате запис за време или разходи, се създава запис за одобрение.</span><span class="sxs-lookup"><span data-stu-id="d06fa-108">When you create and submit a time or expense entry, an approval entry is created.</span></span> <span data-ttu-id="d06fa-109">Одобряващият проекта или вашият мениджър преглеждат и одобряват вашето участие.</span><span class="sxs-lookup"><span data-stu-id="d06fa-109">The Project approver or your manager reviews and approves your entry.</span></span> <span data-ttu-id="d06fa-110">Ако записът е свързан с проект, когато бъде одобрен, действителните ще бъдат създадени.</span><span class="sxs-lookup"><span data-stu-id="d06fa-110">If the entry is related to a project, when it's approved, the actuals will be created.</span></span> <span data-ttu-id="d06fa-111">Това позволява проследяване на разходите и фактурирането.</span><span class="sxs-lookup"><span data-stu-id="d06fa-111">This allows the cost and billing to be tracked.</span></span> 

## <a name="approve-an-entry"></a><span data-ttu-id="d06fa-112">Одобрете запис</span><span class="sxs-lookup"><span data-stu-id="d06fa-112">Approve an entry</span></span>
<span data-ttu-id="d06fa-113">Формулярът **Одобрения** ви позволява да превключвате между различни изгледи, така че да можете да преглеждате различните видове одобрения.</span><span class="sxs-lookup"><span data-stu-id="d06fa-113">The **Approvals** form allows you to switch between different views so that you can view the different types of approvals.</span></span>
  
1. <span data-ttu-id="d06fa-114">Отидете на формуляра **Одобрения** и изберете **Разходи** , **Време** или **Извиквания**.</span><span class="sxs-lookup"><span data-stu-id="d06fa-114">Go to the **Approvals** form and select **Expenses** , **Time** , or **Recalls**.</span></span>
2. <span data-ttu-id="d06fa-115">Прегледайте всяко одобрение и изберете тези, които искате да одобрите.</span><span class="sxs-lookup"><span data-stu-id="d06fa-115">Review each approval, and select the ones you want to approve.</span></span>
3. <span data-ttu-id="d06fa-116">Изберете **Одобрете** , за да одобрите избраните записи.</span><span class="sxs-lookup"><span data-stu-id="d06fa-116">Select **Approve** to approve the selected entries.</span></span>
<span data-ttu-id="d06fa-117">Системата ще обработи тези записи и ще създаде факти или резервация.</span><span class="sxs-lookup"><span data-stu-id="d06fa-117">The system will process these entries and create actuals or a booking.</span></span>

## <a name="reject-an-entry"></a><span data-ttu-id="d06fa-118">Отхвърлете запис</span><span class="sxs-lookup"><span data-stu-id="d06fa-118">Reject an entry</span></span>
<span data-ttu-id="d06fa-119">Като одобряващ проекта, може да се наложи да изпратите запис обратно на потребител за корекция.</span><span class="sxs-lookup"><span data-stu-id="d06fa-119">As the Project approver, you may have to send an entry back to a user for correction.</span></span>
  
1. <span data-ttu-id="d06fa-120">Отидете на формуляра **Одобрения** и изберете записа, който да отхвърлите.</span><span class="sxs-lookup"><span data-stu-id="d06fa-120">Go to the **Approvals** form and select the entry to reject.</span></span> 
2. <span data-ttu-id="d06fa-121">Изберете **Отхвърлете**.</span><span class="sxs-lookup"><span data-stu-id="d06fa-121">Select **Reject**.</span></span>
3. <span data-ttu-id="d06fa-122">По избор - Добавете коментар в диалога **Коментари за отхвърляне** , за да информира потребителя защо записът се отхвърля.</span><span class="sxs-lookup"><span data-stu-id="d06fa-122">Optional - Add a comment in the **Rejection Comments** dialog to inform the user why the entry is being rejected.</span></span>
4. <span data-ttu-id="d06fa-123">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="d06fa-123">Select **OK**.</span></span> <span data-ttu-id="d06fa-124">Записът ще бъде върнат на потребителя.</span><span class="sxs-lookup"><span data-stu-id="d06fa-124">The entry will be returned to the user.</span></span>
  
## <a name="recall-entries"></a><span data-ttu-id="d06fa-125">Оттегляне на записи</span><span class="sxs-lookup"><span data-stu-id="d06fa-125">Recall entries</span></span>
<span data-ttu-id="d06fa-126">В даден момент може да се наложи да извикате подаден запис.</span><span class="sxs-lookup"><span data-stu-id="d06fa-126">At some point, you might need to recall a submitted entry.</span></span> <span data-ttu-id="d06fa-127">Ако записът не е одобрен, той ще бъде върнат незабавно.</span><span class="sxs-lookup"><span data-stu-id="d06fa-127">If the entry has not been approved, it will be returned immediately.</span></span> <span data-ttu-id="d06fa-128">Одобреното вписване обаче може да има съществено въздействие.</span><span class="sxs-lookup"><span data-stu-id="d06fa-128">An approved entry however, may have a material impact.</span></span> <span data-ttu-id="d06fa-129">Одобрителят на проекта е длъжен да одобри изтеглянето, за да обърне транзакцията в Действителни данни.</span><span class="sxs-lookup"><span data-stu-id="d06fa-129">The Project approver is required to approve the recall in order to reverse the transaction in Actuals.</span></span>

## <a name="specify-project-approvers"></a><span data-ttu-id="d06fa-130">Указване на одобряващи на проект</span><span class="sxs-lookup"><span data-stu-id="d06fa-130">Specify Project approvers</span></span>
<span data-ttu-id="d06fa-131">Всеки проект има определен брой членове на проектния екип.</span><span class="sxs-lookup"><span data-stu-id="d06fa-131">Each project has a number of project team members.</span></span> <span data-ttu-id="d06fa-132">Можете да посочите кои членове на екипа са и одобряващи проекти.</span><span class="sxs-lookup"><span data-stu-id="d06fa-132">You can specify which team members are also Project approvers.</span></span>

1. <span data-ttu-id="d06fa-133">Отидете на формуляра **Проекти** и отворете проекта от списъка.</span><span class="sxs-lookup"><span data-stu-id="d06fa-133">Go to the **Projects** form and open the project from the list.</span></span>
2. <span data-ttu-id="d06fa-134">На раздела **Екип** изберете члена на екипа, който ще бъде одобряващ проект, и след това изберете **редактиране**.</span><span class="sxs-lookup"><span data-stu-id="d06fa-134">On the **Team** tab, select the team member who will be a Project approver and then select **Edit**.</span></span>
3. <span data-ttu-id="d06fa-135">Задайте полето **Одобряващ проект** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="d06fa-135">Set the **Project Approver** field to **Yes**.</span></span>
4. <span data-ttu-id="d06fa-136">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="d06fa-136">Select **Save**.</span></span>
5. <span data-ttu-id="d06fa-137">Повторете стъпки 2 - 4, за да добавите допълнителни одобряващи на проект.</span><span class="sxs-lookup"><span data-stu-id="d06fa-137">Repeat steps 2-4 to add additional Project approvers.</span></span>

## <a name="configure-the-users-manager"></a><span data-ttu-id="d06fa-138">Конфигурирайте мениджъра на потребителя</span><span class="sxs-lookup"><span data-stu-id="d06fa-138">Configure the user's manager</span></span>

1. <span data-ttu-id="d06fa-139">Отидете в **Настройки** > **Защита** > **Потребители**.</span><span class="sxs-lookup"><span data-stu-id="d06fa-139">Go to **Settings** > **Security** > **Users**.</span></span>
2. <span data-ttu-id="d06fa-140">Изберете потребителя, на когото назначавате мениджър, и в областта **Информация за организацията** изберете мениджъра от списъка.</span><span class="sxs-lookup"><span data-stu-id="d06fa-140">Select the user to whom you are assigning a manager and in the **Organization Information** area, select the manager from the list.</span></span> 
3. <span data-ttu-id="d06fa-141">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="d06fa-141">Select **Save**.</span></span>


