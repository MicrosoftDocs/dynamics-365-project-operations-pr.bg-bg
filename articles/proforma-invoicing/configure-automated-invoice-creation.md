---
title: Конфигуриране на автоматично създаване на фактура
description: Тази тема предоставя информация за горещо за конфигуриране на системата за автоматично генериране на фактури.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 764fd4568619e4f5676ee3cbf7fce14ffb069548
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898113"
---
# <a name="configure-automated-invoice-creation"></a><span data-ttu-id="a65ee-103">Конфигуриране на автоматично създаване на фактура</span><span class="sxs-lookup"><span data-stu-id="a65ee-103">Configure automated invoice creation</span></span>

<span data-ttu-id="a65ee-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="a65ee-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a65ee-105">Изпълнете следните стъпки, за да конфигурирате автоматизирана фактура, изпълнявана в операции на проекта.</span><span class="sxs-lookup"><span data-stu-id="a65ee-105">Complete the following steps to configure an automated invoice run in Project operations.</span></span>

1. <span data-ttu-id="a65ee-106">Отидете в **Настройки** \> **Пакетни задания**.</span><span class="sxs-lookup"><span data-stu-id="a65ee-106">Go to **Settings** \> **Batch jobs**.</span></span>
2. <span data-ttu-id="a65ee-107">Създайте пакетно задание и го наименувайте **Създаване на фактури в Project Operations**.</span><span class="sxs-lookup"><span data-stu-id="a65ee-107">Create a batch job, and name it **Project operations create invoices**.</span></span> <span data-ttu-id="a65ee-108">Името на пакетното задание трябва да включва термина „създаване на фактури“.</span><span class="sxs-lookup"><span data-stu-id="a65ee-108">The name of the batch job must include the term "create invoices."</span></span>
3. <span data-ttu-id="a65ee-109">В полето **Тип задание** изберете **Няма**.</span><span class="sxs-lookup"><span data-stu-id="a65ee-109">In the **Job type** field, select **None**.</span></span> <span data-ttu-id="a65ee-110">По подразбиране опциите **Честота дневно** и **Е активно** са зададени на **Да**.</span><span class="sxs-lookup"><span data-stu-id="a65ee-110">By default, the **Frequency Daily** and **Is Active** options are set to **Yes**.</span></span>
4. <span data-ttu-id="a65ee-111">Изберете **Стартиране на работен поток**.</span><span class="sxs-lookup"><span data-stu-id="a65ee-111">Select **Run Workflow**.</span></span> <span data-ttu-id="a65ee-112">В диалоговия прозорец **Търсене на запис** ще видите три работни процеса:</span><span class="sxs-lookup"><span data-stu-id="a65ee-112">In the **Look Up Record** dialog box, you will see three workflows:</span></span>

    - <span data-ttu-id="a65ee-113">ProcessRunCaller</span><span class="sxs-lookup"><span data-stu-id="a65ee-113">ProcessRunCaller</span></span>
    - <span data-ttu-id="a65ee-114">ProcessRunner</span><span class="sxs-lookup"><span data-stu-id="a65ee-114">ProcessRunner</span></span>
    - <span data-ttu-id="a65ee-115">UpdateRoleUtilization</span><span class="sxs-lookup"><span data-stu-id="a65ee-115">UpdateRoleUtilization</span></span>

5. <span data-ttu-id="a65ee-116">Изберете **ProcessRunCaller** и след това **Добавяне**.</span><span class="sxs-lookup"><span data-stu-id="a65ee-116">Select **ProcessRunCaller**, and then select **Add**.</span></span>
6. <span data-ttu-id="a65ee-117">В следващия диалогов прозорец изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="a65ee-117">In the next dialog box, select **OK**.</span></span> <span data-ttu-id="a65ee-118">Работен поток **Заспиване** е последван от работен поток **Обработване**.</span><span class="sxs-lookup"><span data-stu-id="a65ee-118">A **Sleep** workflow is followed by a **Process** workflow.</span></span>

    <span data-ttu-id="a65ee-119">Можете също да изберете **ProcessRunner** в стъпка 5.</span><span class="sxs-lookup"><span data-stu-id="a65ee-119">You can also select **ProcessRunner** in step 5.</span></span> <span data-ttu-id="a65ee-120">След това, когато изберете **OK**, работният поток **Обработка** е последван от работен поток **Заспиване**.</span><span class="sxs-lookup"><span data-stu-id="a65ee-120">Then, when you select **OK**, a **Process** workflow is followed by a **Sleep** workflow.</span></span>

<span data-ttu-id="a65ee-121">Работните потоци **ProcessRunCaller** и **ProcessRunner** създават фактури.</span><span class="sxs-lookup"><span data-stu-id="a65ee-121">The **ProcessRunCaller** and **ProcessRunner** workflows create invoices.</span></span> <span data-ttu-id="a65ee-122">**ProcessRunCaller** извиква **ProcessRunner**.</span><span class="sxs-lookup"><span data-stu-id="a65ee-122">**ProcessRunCaller** calls **ProcessRunner**.</span></span> <span data-ttu-id="a65ee-123">**ProcessRunner** е работният поток, който всъщност създава фактурите.</span><span class="sxs-lookup"><span data-stu-id="a65ee-123">**ProcessRunner** is the workflow that actually creates the invoices.</span></span> <span data-ttu-id="a65ee-124">Той преминава през всички редове на договора, за които трябва да бъдат създадени фактури, и създава фактури за тези редове.</span><span class="sxs-lookup"><span data-stu-id="a65ee-124">It goes through all the contract lines that invoices must be created for, and it creates invoices for those lines.</span></span> <span data-ttu-id="a65ee-125">За да определи редовете на договора, за които трябва да бъдат създадени фактури, заданието търси в датите на изпълнение на фактурите за редовете на договора.</span><span class="sxs-lookup"><span data-stu-id="a65ee-125">To determine the contract lines that invoices must be created for, the job looks at invoice run dates for the contract lines.</span></span> <span data-ttu-id="a65ee-126">Ако редове на договор, които принадлежат към един договор, имат една и съща дата на изпълнение на фактура, транзакциите се комбинират в една фактура, която има два реда.</span><span class="sxs-lookup"><span data-stu-id="a65ee-126">If contract lines that belong to one contract have the same invoice run date, the transactions are combined into one invoice that has two invoice lines.</span></span> <span data-ttu-id="a65ee-127">Ако няма транзакции, за които да бъдат създадени фактури, заданието пропуска създаването на фактури.</span><span class="sxs-lookup"><span data-stu-id="a65ee-127">If there are no transactions to create invoices for, the job skips invoice creation.</span></span>

<span data-ttu-id="a65ee-128">След като **ProcessRunner** завърши изпълнението на цикъла, той извиква **ProcessRunCaller**, дава крайния час, и се затваря.</span><span class="sxs-lookup"><span data-stu-id="a65ee-128">After **ProcessRunner** has finished running, it calls **ProcessRunCaller**, provides the end time, and is closed.</span></span> <span data-ttu-id="a65ee-129">**ProcessRunCaller** след това стартира таймер, който работи в продължение на 24 часа от посочения краен час.</span><span class="sxs-lookup"><span data-stu-id="a65ee-129">**ProcessRunCaller** then starts a timer that runs for 24 hours from the specified end time.</span></span> <span data-ttu-id="a65ee-130">В края на таймера **ProcessRunCaller** се затваря.</span><span class="sxs-lookup"><span data-stu-id="a65ee-130">At the end of the timer, **ProcessRunCaller** is closed.</span></span>

<span data-ttu-id="a65ee-131">Заданието за пакетно обработване за създаване на фактури е повтарящо се задание.</span><span class="sxs-lookup"><span data-stu-id="a65ee-131">The batch process job for creating invoices is a recurrent job.</span></span> <span data-ttu-id="a65ee-132">Ако това пакетно обработване се изпълнява много пъти, се създават няколко екземпляра на заданието и причиняват грешки.</span><span class="sxs-lookup"><span data-stu-id="a65ee-132">If this batch process is run many times, multiple instances of the job are created and cause errors.</span></span> <span data-ttu-id="a65ee-133">Затова трябва да стартирате пакетното обработване само един път и трябва да го рестартирате само ако спре да работи.</span><span class="sxs-lookup"><span data-stu-id="a65ee-133">Therefore, you should start the batch process only one time, and you should restart it only if it stops running.</span></span>

> [!NOTE]
> <span data-ttu-id="a65ee-134">Партидното фактуриране се изпълнява само за линиите на договор за проект, които са конфигурирани от графици за фактури.</span><span class="sxs-lookup"><span data-stu-id="a65ee-134">Batch invoicing only runs for project contract lines that are configured by invoice schedules.</span></span> <span data-ttu-id="a65ee-135">Аспекти на договор с метод на фактуриране по фиксирана цена трябва да имат конфигурирани контролни точки.</span><span class="sxs-lookup"><span data-stu-id="a65ee-135">A contract line with a fixed price billing method must have milestones configured.</span></span> <span data-ttu-id="a65ee-136">Аспекти на договор по проект с метод на фактуриране по време и материали ще се нуждаят от зададен график за фактуриране, базиран на дата.</span><span class="sxs-lookup"><span data-stu-id="a65ee-136">A project contract line with a time and material billing method will need a date-based invoice schedule set up.</span></span> <span data-ttu-id="a65ee-137">Същото се отнася и за аспекти на договор, базирани на проект.</span><span class="sxs-lookup"><span data-stu-id="a65ee-137">The same applies to a project-based contract line.</span></span>     
