---
title: График на разходите за разследване на Федералните награди
description: Тази тема предоставя информация за Графика на разходите за разследване на Федералните награди.
author: velofog
ms.date: 04/2/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: PSNProjSEFAinquiry
audience: Application User
ms.devlang: ''
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.tgt_pltfrm: ''
ms.custom: ''
ms.search.region: Global
ms.search.industry: public sector
ms.author: andchoi
ms.search.validFrom: 2020-4-01
ms.dyn365.ops.version: 10.0.11
ms.openlocfilehash: a16b0fb097124e26da09e220a1239cd6df303f98
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010053"
---
# <a name="schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="08218-103">График на разходите за разследване на Федералните награди</span><span class="sxs-lookup"><span data-stu-id="08218-103">Schedule of Expenditures of Federal Awards inquiry</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="08218-104">Според Службата за управление и бюджет Circular A-133 агенциите, които получават федерални средства, подлежат на изисквания за одит, които са известни и като единични одити.</span><span class="sxs-lookup"><span data-stu-id="08218-104">According to Office of Management and Budget Circular A-133, agencies that receive federal funds are subject to audit requirements, which are also known as single audits.</span></span> <span data-ttu-id="08218-105">Процесът на одита се използва за периодично докладване на приходите и разходите на федералните безвъзмездни средства.</span><span class="sxs-lookup"><span data-stu-id="08218-105">The audit process is used to report on the revenues and expenditures of federal grants on a recurring basis.</span></span> <span data-ttu-id="08218-106">Част от доклада за единния одит включва График на разходите на Федералните награди (SEFA).</span><span class="sxs-lookup"><span data-stu-id="08218-106">Part of the single audit report includes the Schedule of Expenditures of Federal Awards (SEFA).</span></span>

<span data-ttu-id="08218-107">Графикът на разходите за разследване на Федералните награди включва заглавието и номера на Федералната битова помощ (CFDA), номера на безвъзмездните средства, годината на отпускане, името на федералната агенция, която предоставя средствата, и името на пропуска чрез субект.</span><span class="sxs-lookup"><span data-stu-id="08218-107">The Schedule of Expenditures of Federal Awards inquiry includes the Catalog of Federal Domestic Assistance (CFDA) title and number, the grant number, the year of the grant, the name of the federal agency that provides the funds, and the name of the pass-through entity.</span></span> <span data-ttu-id="08218-108">Запитването е за определен период.</span><span class="sxs-lookup"><span data-stu-id="08218-108">The inquiry is for a specific period.</span></span> <span data-ttu-id="08218-109">Обикновено този период е същият като периода на финансовия отчет, който е финансова година.</span><span class="sxs-lookup"><span data-stu-id="08218-109">Typically, that period is the same as the financial statement period, which is a fiscal year.</span></span>

<span data-ttu-id="08218-110">Запитването включва безвъзмездни средства, които имат прогнозни дати в избрания период от време.</span><span class="sxs-lookup"><span data-stu-id="08218-110">The inquiry includes grants that have projection dates in the selected date range.</span></span> <span data-ttu-id="08218-111">Колоната **Грантодателска агенция** на запитването показва клиента на безвъзмездната финансова помощ или, за прехвърляне на безвъзмездна помощ, агенцията на дарителя.</span><span class="sxs-lookup"><span data-stu-id="08218-111">The **Grantor agency** column of the inquiry shows the grant customer or, for a pass-through grant, the grantor agency.</span></span> <span data-ttu-id="08218-112">За безвъзмездна финансова помощ, **Предавателна агенция** колоната показва клиента на безвъзмездната финансова помощ.</span><span class="sxs-lookup"><span data-stu-id="08218-112">For a pass-through grant, the **Pass-through agency** column shows the grant customer.</span></span> <span data-ttu-id="08218-113">Ако стипендията не е безвъзмездна финансова помощ, колоната **Предавателна агенция** е празна.</span><span class="sxs-lookup"><span data-stu-id="08218-113">If the grant isn't a pass-through grant, the **Pass-through agency** column is blank.</span></span>

## <a name="set-up-the-cfda-clusters"></a><span data-ttu-id="08218-114">Настройване на CFDA клъстери</span><span class="sxs-lookup"><span data-stu-id="08218-114">Set up the CFDA clusters</span></span>

<span data-ttu-id="08218-115">Трябва да настроите клъстерите CFDA, които могат да бъдат свързани с номера на CFDA в списъка с разходите за разследване на Федералните награди.</span><span class="sxs-lookup"><span data-stu-id="08218-115">You must set up the CFDA clusters that can be associated with CFDA numbers in the Schedule of Expenditures of Federal Awards inquiry.</span></span>

1. <span data-ttu-id="08218-116">Отидете на **Управление на проекти и счетоводство \> Настройка \> Безвъзмездни средства \> Каталог на федералните клъстери за домашна помощ**.</span><span class="sxs-lookup"><span data-stu-id="08218-116">Go to **Project management and accounting \> Setup \> Grants \> Catalog of Federal Domestic Assistance clusters**.</span></span>
2. <span data-ttu-id="08218-117">Изберете **Създаване**, за да създадете CFDA клъстер.</span><span class="sxs-lookup"><span data-stu-id="08218-117">Select **New** to create a CFDA cluster.</span></span>
3. <span data-ttu-id="08218-118">Въведете име на клъстера.</span><span class="sxs-lookup"><span data-stu-id="08218-118">Enter the cluster name.</span></span>
4. <span data-ttu-id="08218-119">Изберете **Записване**, за да запишете промените си.</span><span class="sxs-lookup"><span data-stu-id="08218-119">Select **Save** to save your changes.</span></span>

## <a name="set-up-cfda-numbers"></a><span data-ttu-id="08218-120">Настройте CFDA номера</span><span class="sxs-lookup"><span data-stu-id="08218-120">Set up CFDA numbers</span></span>

<span data-ttu-id="08218-121">Трябва да настроите CFDA номера, които могат да бъдат добавени към стипендии и включени в списъка с разходите за разследване на Федералните награди.</span><span class="sxs-lookup"><span data-stu-id="08218-121">You must set up CFDA numbers that can be added to grants and included in the Schedule of Expenditures of Federal Awards inquiry.</span></span>

1. <span data-ttu-id="08218-122">Отидете на **Управление на проекти и счетоводство \> Настройка \> Безвъзмездни средства \> Каталог на федералните номера за домашна помощ**.</span><span class="sxs-lookup"><span data-stu-id="08218-122">Go to **Project management and accounting \> Setup \> Grants \> Catalog of Federal Domestic Assistance numbers**.</span></span>
2. <span data-ttu-id="08218-123">Изберете **Създаване**, за да създадете CFDA номер.</span><span class="sxs-lookup"><span data-stu-id="08218-123">Select **New** to create a CFDA number.</span></span>
3. <span data-ttu-id="08218-124">В колоната **Номер** въведете CFDA номера.</span><span class="sxs-lookup"><span data-stu-id="08218-124">In the **Number** column, enter the CFDA number.</span></span>
4. <span data-ttu-id="08218-125">Натиснете клавиша **Tab**.</span><span class="sxs-lookup"><span data-stu-id="08218-125">Press the **Tab** key.</span></span>
5. <span data-ttu-id="08218-126">В колоната **Описание** въведете CFDA заглавие.</span><span class="sxs-lookup"><span data-stu-id="08218-126">In the **Description** column, enter the CFDA title.</span></span>
6. <span data-ttu-id="08218-127">Натиснете клавиша **Tab**.</span><span class="sxs-lookup"><span data-stu-id="08218-127">Press the **Tab** key.</span></span>
7. <span data-ttu-id="08218-128">По избор: В полето **Програмен клъстер** добавете съответния CFDA клъстер.</span><span class="sxs-lookup"><span data-stu-id="08218-128">Optional: In the **Program cluster** field, add the appropriate CFDA cluster.</span></span>
8. <span data-ttu-id="08218-129">Изберете **Записване**, за да запишете промените си.</span><span class="sxs-lookup"><span data-stu-id="08218-129">Select **Save** to save your changes.</span></span>

## <a name="set-up-grants-to-report-for-the-schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="08218-130">Създайте безвъзмездни средства за отчитане за График на разходите за разследване на Федералните награди</span><span class="sxs-lookup"><span data-stu-id="08218-130">Set up grants to report for the Schedule of Expenditures of Federal Awards inquiry</span></span>

1. <span data-ttu-id="08218-131">Отидете на **Управление на проекти и счетоводство \> Безвъзмездни средства \> Безвъзмездни средства** и изберете съществуващ грант.</span><span class="sxs-lookup"><span data-stu-id="08218-131">Go to **Project management and accounting \> Grants \> Grants**, and select an existing grant.</span></span>
2. <span data-ttu-id="08218-132">На FastTab **Настройка** в полето **Каталог на федералната домашна помощ** задайте номера на CFDA.</span><span class="sxs-lookup"><span data-stu-id="08218-132">On the **Setup** FastTab, in the **Catalog of Federal Domestic Assistance** field, assign the CFDA number.</span></span> <span data-ttu-id="08218-133">Номерът на CFDA в безвъзмездните средства определя клъстера на CFDA за докладване.</span><span class="sxs-lookup"><span data-stu-id="08218-133">The CFDA number on the grant determines the CFDA cluster for reporting.</span></span>
3. <span data-ttu-id="08218-134">На FastTab **Информация за връзка** въведете информацията за концедента, като изпълните следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="08218-134">On **Contact information** FastTab, enter the grantor information by following these steps:</span></span>

    1. <span data-ttu-id="08218-135">В полето **Предоставяне на клиент** въведете клиента, който отговаря за безвъзмездните средства.</span><span class="sxs-lookup"><span data-stu-id="08218-135">In the **Grant customer** field, enter the customer who is responsible for the grant.</span></span> <span data-ttu-id="08218-136">За съществуваща субсидия тази информация може вече да е въведена.</span><span class="sxs-lookup"><span data-stu-id="08218-136">For an existing grant, this information might already be entered.</span></span>
    2. <span data-ttu-id="08218-137">Посочете дали клиентът на безвъзмездни средства е финансиращият.</span><span class="sxs-lookup"><span data-stu-id="08218-137">Indicate whether the grant customer is the funder.</span></span> <span data-ttu-id="08218-138">Ако клиентът на безвъзмездни средства е финансиращият, оставете **Преминаване** квадратчето е изчистено.</span><span class="sxs-lookup"><span data-stu-id="08218-138">If the grant customer is the funder, leave the **Pass-through** check box cleared.</span></span> <span data-ttu-id="08218-139">Ако друг клиент е финансиращ и клиентът на безвъзмездната финансова помощ отговаря за харченето и проследяването на парите, изберете **Преминаване** отметка.</span><span class="sxs-lookup"><span data-stu-id="08218-139">If another customer is the funder, and the grant customer is responsible for spending and tracking the money, select the **Pass-through** check box.</span></span>

4. <span data-ttu-id="08218-140">Ако сте избрали **Преминаване** в предишната стъпка в **Грантодателска агенция** поле, въведете клиента, предоставил безвъзмездните средства.</span><span class="sxs-lookup"><span data-stu-id="08218-140">If you selected the **Pass-through** check box in the previous step, in the **Grantor agency** field, enter the customer who provided the grant.</span></span> <span data-ttu-id="08218-141">Дарителската агенция и клиентът на субсидията не могат да бъдат един и същ клиент.</span><span class="sxs-lookup"><span data-stu-id="08218-141">The grantor agency and the grant customer can't be the same customer.</span></span>

<span data-ttu-id="08218-142">Ето пример за безвъзмездна финансова помощ:</span><span class="sxs-lookup"><span data-stu-id="08218-142">Here is an example of a pass-through grant:</span></span>

<span data-ttu-id="08218-143">Федералното правителство финансира инфраструктурен проект за държава.</span><span class="sxs-lookup"><span data-stu-id="08218-143">The federal government funded an infrastructure project for a state.</span></span> <span data-ttu-id="08218-144">Федералното правителство даде парите на държавата да ги похарчи.</span><span class="sxs-lookup"><span data-stu-id="08218-144">The federal government gave the money to the state to spend.</span></span> <span data-ttu-id="08218-145">В този случай федералното правителство е дарителската агенция, а държавата е клиентът на безвъзмездната финансова помощ.</span><span class="sxs-lookup"><span data-stu-id="08218-145">In this case, the federal government is the grantor agency, and the state is the grant customer.</span></span>

> [!NOTE] 
> <span data-ttu-id="08218-146">Когато включите функцията за първи път, първоначалните номера на CFDA ще бъдат въведени чрез използване на съществуващите номера на безвъзмездни средства.</span><span class="sxs-lookup"><span data-stu-id="08218-146">When you first turn on the feature, initial CFDA numbers will be entered by using the existing numbers on grants.</span></span>

## <a name="exclude-grants-from-sefa-reporting-based-on-the-grant-type"></a><span data-ttu-id="08218-147">Изключете безвъзмездните средства от отчитането на SEFA въз основа на вида на безвъзмездните средства</span><span class="sxs-lookup"><span data-stu-id="08218-147">Exclude grants from SEFA reporting based on the grant type</span></span>

1. <span data-ttu-id="08218-148">Отидете на **Управление на проекти и счетоводство \> Настройка \> Безвъзмездни средства \> Видове безвъзмездни средства**.</span><span class="sxs-lookup"><span data-stu-id="08218-148">Go to **Project management and accounting \> Setup \> Grants \> Grant types**.</span></span>
2. <span data-ttu-id="08218-149">На FastTab **Информация по подразбиране** изберете квадратчето за отметка **Изключете от списъка с разходите на Федералните награди**.</span><span class="sxs-lookup"><span data-stu-id="08218-149">On the **Default information** FastTab, select the **Exclude from Schedule of Expenditures of Federal Awards** check box.</span></span>
3. <span data-ttu-id="08218-150">Изберете **Записване**, за да запишете промените си.</span><span class="sxs-lookup"><span data-stu-id="08218-150">Select **Save** to save your changes.</span></span>

## <a name="run-the-schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="08218-151">Изпълнете График на разходите за разследване на Федералните награди</span><span class="sxs-lookup"><span data-stu-id="08218-151">Run the Schedule of Expenditures of Federal Awards inquiry</span></span>

1. <span data-ttu-id="08218-152">Отидете на **Управление на проекти и счетоводство \> Запитвания и доклади \> Запитване за безвъзмездна помощ \> График на разходите за федерални награди**.</span><span class="sxs-lookup"><span data-stu-id="08218-152">Go to **Project management and accounting \> Inquiries and reports \> Grant inquiry \> Schedule of Expenditures of Federal Awards**.</span></span>
2. <span data-ttu-id="08218-153">В секцията **Параметри** изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="08218-153">In the **Parameters** section, follow these steps:</span></span>

    1. <span data-ttu-id="08218-154">В полето **Интервал от дати** изберете кода за интервала от време.</span><span class="sxs-lookup"><span data-stu-id="08218-154">In the **Date interval** field, select the code for the date interval.</span></span> <span data-ttu-id="08218-155">Като алтернатива, в **Дата От** и **Дата До** полета, дефинирайте интервала за дата.</span><span class="sxs-lookup"><span data-stu-id="08218-155">Alternatively, in the **From date** and **To date** fields, define the date interval.</span></span>
    2. <span data-ttu-id="08218-156">По избор: За да включите само фактурирани транзакции като приходи в запитването, задайте **Включете само фактурирани приходи** опция на **Да**.</span><span class="sxs-lookup"><span data-stu-id="08218-156">Optional: To include only billed transactions as revenue in the inquiry, set the **Include only billed revenues** option to **Yes**.</span></span>

## <a name="columns"></a><span data-ttu-id="08218-157">Колони</span><span class="sxs-lookup"><span data-stu-id="08218-157">Columns</span></span>

<span data-ttu-id="08218-158">Графикът на разходите за разследване на Федералните награди включва следните колони:</span><span class="sxs-lookup"><span data-stu-id="08218-158">The Schedule of Expenditures of Federal Awards inquiry includes the following columns:</span></span>

- <span data-ttu-id="08218-159">Каталог на името на клъстера на Федералната домашна помощ</span><span class="sxs-lookup"><span data-stu-id="08218-159">Catalog of Federal Domestic Assistance cluster name</span></span>
- <span data-ttu-id="08218-160">Грантодателска агенция</span><span class="sxs-lookup"><span data-stu-id="08218-160">Grantor agency</span></span>
- <span data-ttu-id="08218-161">Агенция за преминаване</span><span class="sxs-lookup"><span data-stu-id="08218-161">Pass-through agency</span></span>
- <span data-ttu-id="08218-162">Име на дарение</span><span class="sxs-lookup"><span data-stu-id="08218-162">Grant name</span></span>
- <span data-ttu-id="08218-163">ИД на дарение</span><span class="sxs-lookup"><span data-stu-id="08218-163">Grant ID</span></span>
- <span data-ttu-id="08218-164">ИД на кандидатура за дарение</span><span class="sxs-lookup"><span data-stu-id="08218-164">Grant application ID</span></span>
- <span data-ttu-id="08218-165">Каталог на Федералната домашна помощ</span><span class="sxs-lookup"><span data-stu-id="08218-165">Catalog of Federal Domestic Assistance</span></span>
- <span data-ttu-id="08218-166">Разписки</span><span class="sxs-lookup"><span data-stu-id="08218-166">Receipts</span></span>
- <span data-ttu-id="08218-167">Разходи</span><span class="sxs-lookup"><span data-stu-id="08218-167">Expenditures</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]