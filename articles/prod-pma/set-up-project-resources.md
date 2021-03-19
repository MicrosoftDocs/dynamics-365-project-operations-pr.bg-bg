---
title: Настройване на ресурси на проект
description: Тази тема предоставя информация за настройване или заявяване на ресурси по проект.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0bf146c3bfb2fd558c471d8a9e980834cb1b87df
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288726"
---
# <a name="set-up-project-resources"></a><span data-ttu-id="b269e-103">Настройване на ресурси на проект</span><span class="sxs-lookup"><span data-stu-id="b269e-103">Set up project resources</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="b269e-104">Трябва да настроите календар и да го свържете със служител или работник.</span><span class="sxs-lookup"><span data-stu-id="b269e-104">You must set up a calendar and associate it with an employee or a worker.</span></span> <span data-ttu-id="b269e-105">Календарът се използва за планиране на проекта и работното време на ресурсите, които са запазени за проекта.</span><span class="sxs-lookup"><span data-stu-id="b269e-105">The calendar is used to schedule the project and the working time of the resources that are reserved for the project.</span></span> <span data-ttu-id="b269e-106">По време на настройката на календара мениджърите на проекти могат да направят изравняване на ресурсите като част от оптимизацията на ресурсите.</span><span class="sxs-lookup"><span data-stu-id="b269e-106">During calendar setup, project managers can do resource leveling as part of resource optimization.</span></span> <span data-ttu-id="b269e-107">Въз основа на календарния график могат да се поставят ограничения върху ресурсите.</span><span class="sxs-lookup"><span data-stu-id="b269e-107">Based on the calendar schedule, restrictions can be put on resources.</span></span> <span data-ttu-id="b269e-108">Можете да настроите календар на страницата **Календари**.</span><span class="sxs-lookup"><span data-stu-id="b269e-108">You can set up a calendar on the **Calendars** page.</span></span>

<span data-ttu-id="b269e-109">Когато настройвате работник като ресурс на проект, можете да избирате от работници, които работят във фирмата, за която настройвате ресурси.</span><span class="sxs-lookup"><span data-stu-id="b269e-109">When you set up a worker as a project resource, you can select from workers who work in the company that you're setting up resources for.</span></span> <span data-ttu-id="b269e-110">Като алтернатива можете да изберете работници от други компании във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="b269e-110">Alternatively, you can select workers from other companies in your organization.</span></span> <span data-ttu-id="b269e-111">Тези работници са известни като вътрешнофирмени ресурси.</span><span class="sxs-lookup"><span data-stu-id="b269e-111">These workers are known as intercompany resources.</span></span>

<span data-ttu-id="b269e-112">Следващите процедури обясняват как да настроите работник като ресурс за проект във вашата компания и как да настроите ресурс за вътрешнофирмен проект.</span><span class="sxs-lookup"><span data-stu-id="b269e-112">The following procedures explain how to set up a worker as a project resource in your company and how to set up an intercompany project resource.</span></span>

## <a name="set-up-a-worker-as-a-project-resource"></a><span data-ttu-id="b269e-113">Настройте работник като ресурс на проекта</span><span class="sxs-lookup"><span data-stu-id="b269e-113">Set up a worker as a project resource</span></span>

1. <span data-ttu-id="b269e-114">На страницата **Работници** в **Работници** списък, изберете работника, който добавяте като ресурс на проект, и отворете работния запис.</span><span class="sxs-lookup"><span data-stu-id="b269e-114">On the **Workers** page, in the **Workers** list, select the worker that you're adding as a project resource, and open the worker record.</span></span>
2. <span data-ttu-id="b269e-115">В екрана за действие изберете **Проект** &gt; **Настройки** &gt; **Настройка на проекта**.</span><span class="sxs-lookup"><span data-stu-id="b269e-115">On the Action Pane, select **Project** &gt; **Setup** &gt; **Project setup**.</span></span>
3. <span data-ttu-id="b269e-116">Изберете календар и след това затворете страницата.</span><span class="sxs-lookup"><span data-stu-id="b269e-116">Select a calendar, and then close the page.</span></span>

<span data-ttu-id="b269e-117">Можете също така да посочите проекти по подразбиране за ресурс като вид предварително задание.</span><span class="sxs-lookup"><span data-stu-id="b269e-117">You can also specify default projects for a resource as a type of pre-assignment.</span></span> <span data-ttu-id="b269e-118">Предварителните задания могат да се използват, когато мениджърът на ресурси или мениджърът на проекти знаят по кои проекти ще работи ресурсът предварително.</span><span class="sxs-lookup"><span data-stu-id="b269e-118">Pre-assignments can be used when the resource manager or project manager knows which projects the resource will be working on in advance.</span></span> <span data-ttu-id="b269e-119">Предварителните задания също могат да се основават на искането на спонсор на проект или клиент.</span><span class="sxs-lookup"><span data-stu-id="b269e-119">Pre-assignments can also be based on the request of a project sponsor or customer.</span></span> <span data-ttu-id="b269e-120">За да зададете предварително проект, на страницата **Възлагане на проекти** в раздела **Проекти** в списъка **Оставащи проекти** изберете подходящия проект.</span><span class="sxs-lookup"><span data-stu-id="b269e-120">To pre-assign a project, on the **Assign projects** page, on the **Projects** tab, in the **Remaining projects** list, select the appropriate project.</span></span>

## <a name="set-up-an-intercompany-resource"></a><span data-ttu-id="b269e-121">Настройте вътрешнофирмен ресурс</span><span class="sxs-lookup"><span data-stu-id="b269e-121">Set up an intercompany resource</span></span>

<span data-ttu-id="b269e-122">Когато настройвате работник като вътрешнофирмен ресурс, трябва да завършите настройката както във фирмата за заеми, така и във фирмата за заеми.</span><span class="sxs-lookup"><span data-stu-id="b269e-122">When you set up a worker as an intercompany resource, you must complete the setup in both the lending company and the borrowing company.</span></span>

### <a name="in-the-lending-company"></a><span data-ttu-id="b269e-123">В кредитиращата компания</span><span class="sxs-lookup"><span data-stu-id="b269e-123">In the lending company</span></span>

1. <span data-ttu-id="b269e-124">Във „Finance“ проверете дали е избрана фирмата-заемодател и след това завършете процедурата в предишния раздел „Настройване на работник като ресурс на проекта“.</span><span class="sxs-lookup"><span data-stu-id="b269e-124">In Finance, verify that the lending company is selected, and then complete the procedure in the previous section, "Set up a worker as a project resource."</span></span>
2. <span data-ttu-id="b269e-125">На страницата **Междуфирмено осчетоводяване** изберете **Ново**.</span><span class="sxs-lookup"><span data-stu-id="b269e-125">On the **Intercompany accounting** page, select **New**.</span></span>
3. <span data-ttu-id="b269e-126">В полето **ИД на юридическо лице**, изберете кредитиращата компания.</span><span class="sxs-lookup"><span data-stu-id="b269e-126">In the **Legal entity ID** field, select the lending company.</span></span> <span data-ttu-id="b269e-127">Попълнете останалите полетата, както е подходящо, и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="b269e-127">Fill in the remaining fields as appropriate, and then select **Save**.</span></span>
4. <span data-ttu-id="b269e-128">На страницата **Цена на прехвърляне** изберете **Нов**.</span><span class="sxs-lookup"><span data-stu-id="b269e-128">On the **Transfer price** page, select **New**.</span></span>
5. <span data-ttu-id="b269e-129">В полето **Кредитирано юридическо лице** изберете съответната компания.</span><span class="sxs-lookup"><span data-stu-id="b269e-129">In the **Borrowing legal entity** field, select the appropriate company.</span></span>
6. <span data-ttu-id="b269e-130">За да заемете на заемащата фирма само ресурса, който сте създали в началото на този раздел, в полето **Ресурс**, изберете името на ресурса, който сте създали.</span><span class="sxs-lookup"><span data-stu-id="b269e-130">To lend the borrowing company only the resource that you created at the beginning of this section, in the **Resource** field, select the name of the resource that you created.</span></span> <span data-ttu-id="b269e-131">За да направите всички ресурси в заемащата компания достъпни за заемащата компания, оставете полето **Ресурс** празно.</span><span class="sxs-lookup"><span data-stu-id="b269e-131">To make all resources in the lending company available to the borrowing company, leave the **Resource** field blank.</span></span>
7. <span data-ttu-id="b269e-132">На страницата **Управление на проекти и счетоводни параметри** в раздела **Междуфирмени**, задайте опцията **Активирайте вътрешнофирменото планиране на ресурси и разписания** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="b269e-132">On the **Project management and accounting parameters** page, on the **Intercompany** tab, set the **Enable intercompany resource scheduling and timesheets** option to **Yes**.</span></span>

### <a name="in-the-borrowing-company"></a><span data-ttu-id="b269e-133">В кредитираната компания</span><span class="sxs-lookup"><span data-stu-id="b269e-133">In the borrowing company</span></span>

- <span data-ttu-id="b269e-134">На страницата **Списък с ресурси** във филтъра за търсене въведете името на ресурса, който сте създали за фирмата заемодател, за да проверите дали името е включено в списъка с ресурси за компанията заемодател.</span><span class="sxs-lookup"><span data-stu-id="b269e-134">On the **Resources list** page, in the search filter, enter the name of the resource that you created for the lending company, to verify that the name is included in the resource list for the borrowing company.</span></span>

## <a name="request-project-resources"></a><span data-ttu-id="b269e-135">Заявяване на ресурси по проекти</span><span class="sxs-lookup"><span data-stu-id="b269e-135">Request project resources</span></span>
<span data-ttu-id="b269e-136">Функционалността за планиране на ресурси на проекти само нека нека мениджърите на ресурси разпределят персонал ресурси по ангажименти или проекти.</span><span class="sxs-lookup"><span data-stu-id="b269e-136">The functionality for project resource scheduling only lets resource managers distribute staffed resources on engagements or projects.</span></span> <span data-ttu-id="b269e-137">За да активирате тази функционалност, изпълнете следните задачи или проверете дали са изпълнени:</span><span class="sxs-lookup"><span data-stu-id="b269e-137">To enable this functionality, complete the following tasks, or verify that they have been completed:</span></span>

- <span data-ttu-id="b269e-138">Настройте числови последователности.</span><span class="sxs-lookup"><span data-stu-id="b269e-138">Set up number sequences.</span></span>
- <span data-ttu-id="b269e-139">Настройте работни потоци за управление на проекти и счетоводство.</span><span class="sxs-lookup"><span data-stu-id="b269e-139">Set up project management and accounting workflows.</span></span>
- <span data-ttu-id="b269e-140">Активирайте работните потоци на заявки за ресурси.</span><span class="sxs-lookup"><span data-stu-id="b269e-140">Enable resource request workflows.</span></span>

<span data-ttu-id="b269e-141">След като приключите предходните задачи, можете да изпълните следните задачи, както ви е необходимо:</span><span class="sxs-lookup"><span data-stu-id="b269e-141">After the preceding tasks have been completed, you can complete the following tasks as you require:</span></span>

- <span data-ttu-id="b269e-142">Създайте заявка за ресурс от персонализиран ресурс с персонална резервация.</span><span class="sxs-lookup"><span data-stu-id="b269e-142">Create a resource request from a soft-booked staffed resource.</span></span>
- <span data-ttu-id="b269e-143">Заявки за наблюдение на ресурси.</span><span class="sxs-lookup"><span data-stu-id="b269e-143">Monitor resource requests.</span></span>
- <span data-ttu-id="b269e-144">Изпълнете заявки за ресурси.</span><span class="sxs-lookup"><span data-stu-id="b269e-144">Fulfill resource requests.</span></span>
- <span data-ttu-id="b269e-145">Поискайте ресурс с персонал от ССР.</span><span class="sxs-lookup"><span data-stu-id="b269e-145">Request a staffed resource from a WBS.</span></span>
- <span data-ttu-id="b269e-146">Резервирайте ресурси за проект, без да имате заявка за персонал.</span><span class="sxs-lookup"><span data-stu-id="b269e-146">Book resources to a project without having a request for a staffed resource.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]