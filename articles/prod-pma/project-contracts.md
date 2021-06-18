---
title: Договори по проект
description: Тази тема предоставя примери за проектни договори, които можете да създадете за различни видове проекти и източници на финансиране, както и как можете да управлявате договори и да фактурирате клиенти на проекти.
author: Yowelle
ms.date: 11/03/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectContractsListPage, ProjProjectsListPage
audience: Application User, IT Pro
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: a794ec38ac07c1418f9e95b741941a83492bb3d5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999748"
---
# <a name="project-contracts"></a><span data-ttu-id="0c655-103">Договори по проект</span><span class="sxs-lookup"><span data-stu-id="0c655-103">Project contracts</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="0c655-104">Тази статия предоставя примери за проектни договори, които можете да създадете за различни видове проекти и източници на финансиране, както и как можете да управлявате договори и да фактурирате клиенти на проекти.</span><span class="sxs-lookup"><span data-stu-id="0c655-104">This article provides examples of the project contracts that you can create for various types of projects and funding sources, and how you can manage contracts and invoice project customers.</span></span>

<span data-ttu-id="0c655-105">Типът проект, който създавате за договор за проект, определя метода, който се използва за фактуриране на клиентите на проекта.</span><span class="sxs-lookup"><span data-stu-id="0c655-105">The type of project that you create for a project contract determines the method that is used to invoice project customers.</span></span> <span data-ttu-id="0c655-106">Можете да промените договор за проект и свързания проект, но не можете да промените типа на проекта.</span><span class="sxs-lookup"><span data-stu-id="0c655-106">You can change a project contract and the related project, but you can't change the project type.</span></span> 

<span data-ttu-id="0c655-107">Използвайки договор за проект, можете да фактурирате един или повече проекти едновременно.</span><span class="sxs-lookup"><span data-stu-id="0c655-107">By using a project contract, you can invoice one or more projects at the same time.</span></span> <span data-ttu-id="0c655-108">Договорът за проект също помага да се гарантира последователна процедура за фактуриране за всеки подпроект в структурата на проекта.</span><span class="sxs-lookup"><span data-stu-id="0c655-108">The project contract also helps guarantee a consistent invoicing procedure for every subproject in a project structure.</span></span> 

<span data-ttu-id="0c655-109">Всеки проект, който ще бъде фактуриран, трябва да бъде свързан с договор за проект.</span><span class="sxs-lookup"><span data-stu-id="0c655-109">Every project that will be invoiced must be associated with a project contract.</span></span> <span data-ttu-id="0c655-110">Настройките за договор за проект се прилагат за всички проекти и подпроекти, които са свързани с този договор за проект.</span><span class="sxs-lookup"><span data-stu-id="0c655-110">The settings for a project contract apply to all projects and subprojects that are associated with that project contract.</span></span> 

<span data-ttu-id="0c655-111">Договорът за проект може да посочи един или повече източници на финансиране.</span><span class="sxs-lookup"><span data-stu-id="0c655-111">A project contract can specify one or more sources of funding.</span></span> <span data-ttu-id="0c655-112">Следователно можете да разделите фактурирането между множество финансиращи, да зададете лимити за финансиране, така че източниците на финансиране да не бъдат таксувани повече от определена сума, и да конфигурирате правилата за финансиране за начисляване на разходи.</span><span class="sxs-lookup"><span data-stu-id="0c655-112">Therefore, you can split the billing among multiple funders, set up funding limits so that funding sources are not billed more than a specified amount, and configure funding rules for charging expenditures.</span></span>

## <a name="funding-for-project-contracts"></a><span data-ttu-id="0c655-113">Финансиране по договори за проекти</span><span class="sxs-lookup"><span data-stu-id="0c655-113">Funding for project contracts</span></span>
<span data-ttu-id="0c655-114">Някои договори за проекти посочват, че множество страни споделят отговорността за финансиране на разходите по проекта.</span><span class="sxs-lookup"><span data-stu-id="0c655-114">Some project contracts specify that multiple parties share the responsibility for funding the project costs.</span></span> <span data-ttu-id="0c655-115">Ето някои примери:</span><span class="sxs-lookup"><span data-stu-id="0c655-115">Here are some examples:</span></span>

-   <span data-ttu-id="0c655-116">Голям клиент, който има множество подразделения, иска финансирането на даден проект да бъде разделено по подразделения.</span><span class="sxs-lookup"><span data-stu-id="0c655-116">A large customer that has multiple divisions requests that funding of a project be split by division.</span></span>
-   <span data-ttu-id="0c655-117">Вашата компания споделя разходите за голям проект с външна организация.</span><span class="sxs-lookup"><span data-stu-id="0c655-117">Your company shares the costs of a large project with an external organization.</span></span>
-   <span data-ttu-id="0c655-118">Пътен проект е съфинансиран от две общини.</span><span class="sxs-lookup"><span data-stu-id="0c655-118">A  road project is co-funded by two municipalities.</span></span>
-   <span data-ttu-id="0c655-119">Проект за мост се финансира от държавна субсидия и частна корпорация.</span><span class="sxs-lookup"><span data-stu-id="0c655-119">A bridge project is funded by a government grant and a private corporation.</span></span>

<span data-ttu-id="0c655-120">В Dynamics 365 Finance можете да разделите таксуването за една транзакция или цял проект между множество клиенти, безвъзмездни средства или организации.</span><span class="sxs-lookup"><span data-stu-id="0c655-120">In Dynamics 365 Finance, you can split the billing for a single transaction or an entire project among multiple customers, grants, or organizations.</span></span> 

<span data-ttu-id="0c655-121">При проекти, които имат множество финансиращи организации, всички страни, които допринасят за финансирането на разширен проект за финансиране, се наричат източници на финансиране.</span><span class="sxs-lookup"><span data-stu-id="0c655-121">In projects that have multiple funders, all parties that contribute to the funding of an advanced funding project are called funding sources.</span></span> <span data-ttu-id="0c655-122">След като клиент, организация или безвъзмездна финансова помощ е дефиниран като източник на финансиране, той може да бъде присвоен на едно или повече правила за финансиране.</span><span class="sxs-lookup"><span data-stu-id="0c655-122">After a customer, organization, or grant is defined as a funding source, it can be assigned to one or more funding rules.</span></span> <span data-ttu-id="0c655-123">Правилата за финансиране съдържат критерии, които определят как таксите се разпределят към различните източници на финансиране за даден проект.</span><span class="sxs-lookup"><span data-stu-id="0c655-123">Funding rules contain the criteria that determines how charges are allocated to the various funding sources for a project.</span></span> 

<span data-ttu-id="0c655-124">Тъй като наличните артикули, като тези, които се появяват в заявките за покупка и поръчките за покупка, не могат да бъдат разделени, сумата на разходите не може да бъде разделена между множество източници на финансиране по време на разпределението.</span><span class="sxs-lookup"><span data-stu-id="0c655-124">Because stocked items, such as those that appear on purchase requisitions and purchase orders, can't be split, the cost amount can't be split among multiple funding sources at the time of distribution.</span></span> <span data-ttu-id="0c655-125">Следователно стойността на източника на финансиране остава 0 (нула), докато не бъде осчетоводена емисията на инвентара.</span><span class="sxs-lookup"><span data-stu-id="0c655-125">Therefore, the funding source value remains 0 (zero) until the inventory issue is posted.</span></span> <span data-ttu-id="0c655-126">Когато се публикува броят на инвентара, сумата на разходите се разпределя съгласно правилата за разпределение на сметките за проекта.</span><span class="sxs-lookup"><span data-stu-id="0c655-126">When the inventory issue is posted, the cost amount is distributed according to the account distribution rules for the project.</span></span>

<span data-ttu-id="0c655-127">Ето няколко стъпки, които можете да предприемете, за да улесните разделянето на фактурите между множество източници на финансиране:</span><span class="sxs-lookup"><span data-stu-id="0c655-127">Here are some steps that you can take to make it easier to split the billing among multiple funding sources:</span></span>

-   <span data-ttu-id="0c655-128">Посочете, че всички транзакции, които са въведени за проект, използват същата валута на продажби като договора за проект.</span><span class="sxs-lookup"><span data-stu-id="0c655-128">Specify that all transactions that are entered for a project use the same sales currency as the project contract.</span></span>
-   <span data-ttu-id="0c655-129">Настройте лимити за финансиране, така че източникът на финансиране да не бъде фактуриран повече от определена сума за даден проект.</span><span class="sxs-lookup"><span data-stu-id="0c655-129">Set up funding limits, so that a funding source isn't invoiced more than a specified amount toward a project.</span></span>
-   <span data-ttu-id="0c655-130">Конфигурирайте правила за финансиране и лимити за финансиране за всеки работник, артикул, категория, категория група и тип транзакция (или за всички видове транзакции).</span><span class="sxs-lookup"><span data-stu-id="0c655-130">Configure funding rules and funding limits for each worker, item, category, category group, and transaction type (or for all transaction types).</span></span>
-   <span data-ttu-id="0c655-131">Изберете незадължителни начална и крайна дата, за да определите периода, в който всяко правило за финансиране е валидно.</span><span class="sxs-lookup"><span data-stu-id="0c655-131">Select optional start and end dates to define the period when each funding rule is valid.</span></span>
-   <span data-ttu-id="0c655-132">Посочете процента, за който отговаря всеки източник на финансиране.</span><span class="sxs-lookup"><span data-stu-id="0c655-132">Specify the percentage that each funding source is responsible for.</span></span>
-   <span data-ttu-id="0c655-133">Посочете кой източник на финансиране е отговорен за закръгляване на разликите, причинени от изчисленията на разпределението на финансирането.</span><span class="sxs-lookup"><span data-stu-id="0c655-133">Specify which funding source is responsible for rounding differences that are caused by funding allocation calculations.</span></span>
-   <span data-ttu-id="0c655-134">Създайте правила, които определят как разходите по проекта се фактурират на външни клиенти и се начисляват на вътрешни организации.</span><span class="sxs-lookup"><span data-stu-id="0c655-134">Set up rules that determine how project costs are invoiced to external customers and charged to internal organizations.</span></span>
-   <span data-ttu-id="0c655-135">Записвайте транзакциите в задържана сметка за финансиране, докато не бъде получено допълнително финансиране или докато не решите да поемете вътрешно разходите.</span><span class="sxs-lookup"><span data-stu-id="0c655-135">Record transactions in an on-hold funding account until additional funding can be obtained, or until you decide to bear the costs internally.</span></span>

<span data-ttu-id="0c655-136">За да се определи коя данъчна група да се свърже с транзакция, проектът се търси за присвояване на данъчна група.</span><span class="sxs-lookup"><span data-stu-id="0c655-136">To determine which tax group to associate with a transaction, the project is searched for a tax group assignment.</span></span> <span data-ttu-id="0c655-137">Ако на ниво проект не е направено възлагане на данъчна група, проектният договор се търси.</span><span class="sxs-lookup"><span data-stu-id="0c655-137">If no tax group assignment has been made at the project level, the project contract is searched.</span></span>

### <a name="example-multiple-funding-sources-simple"></a><span data-ttu-id="0c655-138">Пример: Множество източници на финансиране (прости)</span><span class="sxs-lookup"><span data-stu-id="0c655-138">Example: Multiple funding sources (simple)</span></span>

<span data-ttu-id="0c655-139">Следващата таблица предоставя сценарии за управление на разпределението на финансирането между множество източници на финансиране.</span><span class="sxs-lookup"><span data-stu-id="0c655-139">The following table provides scenarios for managing funding allocation among multiple funding sources.</span></span> <span data-ttu-id="0c655-140">Тези сценарии се основават на следните предположения:</span><span class="sxs-lookup"><span data-stu-id="0c655-140">These scenarios are based on the following assumptions:</span></span>

-   <span data-ttu-id="0c655-141">Приоритетните настройки се вземат предвид при разпределението на средствата, преди да се приложат други критерии на правилата за финансиране.</span><span class="sxs-lookup"><span data-stu-id="0c655-141">Priority settings are factored into the allocation of funds before other funding rule criteria are applied.</span></span>
-   <span data-ttu-id="0c655-142">Не е посочен период от време, за да се определи периодът d, когато правилото за финансиране е валидно.</span><span class="sxs-lookup"><span data-stu-id="0c655-142">No date range has been specified to define the period d when the funding rule is valid.</span></span>

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="0c655-143"><strong>Сценарий</strong></span><span class="sxs-lookup"><span data-stu-id="0c655-143"><strong>Scenario</strong></span></span></td>
<td><span data-ttu-id="0c655-144"><strong>Източник на финансиране</strong></span><span class="sxs-lookup"><span data-stu-id="0c655-144"><strong>Funding source</strong></span></span></td>
<td><span data-ttu-id="0c655-145"><strong>Процент на разпределение</strong></span><span class="sxs-lookup"><span data-stu-id="0c655-145"><strong>Allocation percentage</strong></span></span></td>
<td><span data-ttu-id="0c655-146"><strong>Приоритет на разпределението</strong></span><span class="sxs-lookup"><span data-stu-id="0c655-146"><strong>Allocation priority</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0c655-147">Искате да разпределите разходите към един източник на финансиране, докато неговите средства бъдат изчерпани, да разпределите разходите към втори източник на финансиране до изчерпване на средствата му и накрая да разпределите останалите разходи към трети източник на финансиране.</span><span class="sxs-lookup"><span data-stu-id="0c655-147">You want to allocate costs to one funding source until its funds are exhausted, allocate costs to a second funding source until its funds are exhausted, and finally allocate the remaining costs to a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="0c655-148">Източник на финансиране 1</span><span class="sxs-lookup"><span data-stu-id="0c655-148">Funding　source　1</span></span></li>
<li><span data-ttu-id="0c655-149">Източник на финансиране 2</span><span class="sxs-lookup"><span data-stu-id="0c655-149">Funding　source　2</span></span></li>
<li><span data-ttu-id="0c655-150">Източник на финансиране 3</span><span class="sxs-lookup"><span data-stu-id="0c655-150">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0c655-151">100%</span><span class="sxs-lookup"><span data-stu-id="0c655-151">100%</span></span></li>
<li><span data-ttu-id="0c655-152">100%</span><span class="sxs-lookup"><span data-stu-id="0c655-152">100%</span></span></li>
<li><span data-ttu-id="0c655-153">100%</span><span class="sxs-lookup"><span data-stu-id="0c655-153">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0c655-154">1</span><span class="sxs-lookup"><span data-stu-id="0c655-154">1</span></span></li>
<li><span data-ttu-id="0c655-155">2</span><span class="sxs-lookup"><span data-stu-id="0c655-155">2</span></span></li>
<li><span data-ttu-id="0c655-156">3</span><span class="sxs-lookup"><span data-stu-id="0c655-156">3</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0c655-157">Искате да разпределите 75 процента от разходите за един източник на финансиране и 25 процента за втори източник на финансиране.</span><span class="sxs-lookup"><span data-stu-id="0c655-157">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="0c655-158">Когато някой от тези източници на финансиране е изчерпан, искате да платите останалите разходи от трети източник на финансиране.</span><span class="sxs-lookup"><span data-stu-id="0c655-158">When either of those funding sources is exhausted, you want to pay the remaining costs from a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="0c655-159">Източник на финансиране 1</span><span class="sxs-lookup"><span data-stu-id="0c655-159">Funding　source　1</span></span></li>
<li><span data-ttu-id="0c655-160">Източник на финансиране 2</span><span class="sxs-lookup"><span data-stu-id="0c655-160">Funding　source　2</span></span></li>
<li><span data-ttu-id="0c655-161">Източник на финансиране 3</span><span class="sxs-lookup"><span data-stu-id="0c655-161">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0c655-162">75%</span><span class="sxs-lookup"><span data-stu-id="0c655-162">75%</span></span></li>
<li><span data-ttu-id="0c655-163">25%</span><span class="sxs-lookup"><span data-stu-id="0c655-163">25%</span></span></li>
<li><span data-ttu-id="0c655-164">100%</span><span class="sxs-lookup"><span data-stu-id="0c655-164">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0c655-165">1</span><span class="sxs-lookup"><span data-stu-id="0c655-165">1</span></span></li>
<li><span data-ttu-id="0c655-166">1</span><span class="sxs-lookup"><span data-stu-id="0c655-166">1</span></span></li>
<li><span data-ttu-id="0c655-167">2</span><span class="sxs-lookup"><span data-stu-id="0c655-167">2</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0c655-168">Искате да разпределите 75 процента от разходите за един източник на финансиране и 25 процента за втори източник на финансиране.</span><span class="sxs-lookup"><span data-stu-id="0c655-168">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="0c655-169">Когато някой от тези източници на финансиране е изчерпан, е добре да разделите оставащия разход между трети и четвърти източник на финансиране.</span><span class="sxs-lookup"><span data-stu-id="0c655-169">When either of those funding sources is exhausted, you want to split the remaining costs between a third funding source and a fourth funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="0c655-170">Източник на финансиране 1</span><span class="sxs-lookup"><span data-stu-id="0c655-170">Funding　source　1</span></span></li>
<li><span data-ttu-id="0c655-171">Източник на финансиране 2</span><span class="sxs-lookup"><span data-stu-id="0c655-171">Funding　source　2</span></span></li>
<li><span data-ttu-id="0c655-172">Източник на финансиране 3</span><span class="sxs-lookup"><span data-stu-id="0c655-172">Funding　source　3</span></span></li>
<li><span data-ttu-id="0c655-173">Източник на финансиране 4</span><span class="sxs-lookup"><span data-stu-id="0c655-173">Funding　source　4</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0c655-174">75%</span><span class="sxs-lookup"><span data-stu-id="0c655-174">75%</span></span></li>
<li><span data-ttu-id="0c655-175">25%</span><span class="sxs-lookup"><span data-stu-id="0c655-175">25%</span></span></li>
<li><span data-ttu-id="0c655-176">50%</span><span class="sxs-lookup"><span data-stu-id="0c655-176">50%</span></span></li>
<li><span data-ttu-id="0c655-177">50%</span><span class="sxs-lookup"><span data-stu-id="0c655-177">50%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0c655-178">1</span><span class="sxs-lookup"><span data-stu-id="0c655-178">1</span></span></li>
<li><span data-ttu-id="0c655-179">1</span><span class="sxs-lookup"><span data-stu-id="0c655-179">1</span></span></li>
<li><span data-ttu-id="0c655-180">2</span><span class="sxs-lookup"><span data-stu-id="0c655-180">2</span></span></li>
<li><span data-ttu-id="0c655-181">2</span><span class="sxs-lookup"><span data-stu-id="0c655-181">2</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0c655-182">Искате да разпределите първите 25 процента от разходите за един източник на финансиране и остатъка за втори източник на финансиране.</span><span class="sxs-lookup"><span data-stu-id="0c655-182">You want to allocate the first 25 percent of costs to one funding source and the rest to a second funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="0c655-183">Източник на финансиране 1</span><span class="sxs-lookup"><span data-stu-id="0c655-183">Funding　source　1</span></span></li>
<li><span data-ttu-id="0c655-184">Източник на финансиране 2</span><span class="sxs-lookup"><span data-stu-id="0c655-184">Funding　source　2</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0c655-185">25%</span><span class="sxs-lookup"><span data-stu-id="0c655-185">25%</span></span></li>
<li><span data-ttu-id="0c655-186">100%</span><span class="sxs-lookup"><span data-stu-id="0c655-186">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0c655-187">1</span><span class="sxs-lookup"><span data-stu-id="0c655-187">1</span></span></li>
<li><span data-ttu-id="0c655-188">2</span><span class="sxs-lookup"><span data-stu-id="0c655-188">2</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

### <a name="example-multiple-funding-sources-complex"></a><span data-ttu-id="0c655-189">Пример: Множество източници на финансиране (сложни)</span><span class="sxs-lookup"><span data-stu-id="0c655-189">Example: Multiple funding sources (complex)</span></span>

<span data-ttu-id="0c655-190">Имате три източника на финансиране, които искате да използвате в следния ред:</span><span class="sxs-lookup"><span data-stu-id="0c655-190">You have three funding sources that you want to use in the following order:</span></span>

1.  <span data-ttu-id="0c655-191">Използвайте източник на финансиране 2 и източник на финансиране еднакво, докато източникът на финансиране 2 бъде изчерпан.</span><span class="sxs-lookup"><span data-stu-id="0c655-191">Use funding source 2 and funding source 3 equally until funding source 2 is exhausted.</span></span>
2.  <span data-ttu-id="0c655-192">Продължавайте да използвате източник на финансиране 3, докато той бъде изчерпан.</span><span class="sxs-lookup"><span data-stu-id="0c655-192">Continue to use funding source 3 until it is exhausted.</span></span>
3.  <span data-ttu-id="0c655-193">Използвайте източник на финансиране 1, след като източникът на финансиране 3 бъде изчерпан.</span><span class="sxs-lookup"><span data-stu-id="0c655-193">Use funding source 1 after funding source 3 is exhausted.</span></span>

<span data-ttu-id="0c655-194">За да постигнете целта си, първо трябва да направите следното:</span><span class="sxs-lookup"><span data-stu-id="0c655-194">To accomplish this goal, you must do the following:</span></span>

-   <span data-ttu-id="0c655-195">Създайте лимити за финансиране за източник на финансиране 2 и източник на финансиране 3 за съответните им суми.</span><span class="sxs-lookup"><span data-stu-id="0c655-195">Set up funding limits for funding source 2 and funding source 3, for their respective amounts.</span></span>
-   <span data-ttu-id="0c655-196">Създайте следните правила за финансиране:</span><span class="sxs-lookup"><span data-stu-id="0c655-196">Create the following funding rules:</span></span>
    -   <span data-ttu-id="0c655-197">Правило 1 (Приоритет 1): Разпределете 50 процента от транзакциите към източник на финансиране 2 и 50 процента към източник на финансиране 3.</span><span class="sxs-lookup"><span data-stu-id="0c655-197">Rule 1 (Priority 1): Allocate 50 percent of transactions to funding source 2 and 50 percent to funding source 3.</span></span>
    -   <span data-ttu-id="0c655-198">Правило 2 (Приоритет 2): Разпределете 100 процента от транзакциите към източника на финансиране 3.</span><span class="sxs-lookup"><span data-stu-id="0c655-198">Rule 2 (Priority 2): Allocate 100 percent of transactions to funding source 3.</span></span>
    -   <span data-ttu-id="0c655-199">Правило 3 (Приоритет 3): Разпределете 100 процента от транзакциите към източника на финансиране 1.</span><span class="sxs-lookup"><span data-stu-id="0c655-199">Rule 3 (Priority 3): Allocate 100 percent of transactions to funding source 1.</span></span>

<span data-ttu-id="0c655-200">Тази настройка работи, тъй като транзакциите се проверяват по правила и ограничения, за да се определи дали някоя от тях се отнася за транзакцията.</span><span class="sxs-lookup"><span data-stu-id="0c655-200">This setup works because transactions are checked against rules and limits to determine whether any of them apply to the transaction.</span></span> <span data-ttu-id="0c655-201">Ако към транзакцията не се прилагат конкретни правила или ограничения, се прилага правилото Всички транзакции.</span><span class="sxs-lookup"><span data-stu-id="0c655-201">If no specific rules or limits apply to the transaction, the All transactions rule applies.</span></span> <span data-ttu-id="0c655-202">Правилото Всички транзакции съвпада с всички транзакции.</span><span class="sxs-lookup"><span data-stu-id="0c655-202">The All transactions rule matches all transactions.</span></span> 

<span data-ttu-id="0c655-203">Ако бъде намерено правило, което съответства на транзакция, процентът, който е бил разпределен в това правило, се прилага първо, но само след като съвпаденията са проверени спрямо ограниченията, които са били настроени.</span><span class="sxs-lookup"><span data-stu-id="0c655-203">If a rule is found that matches a transaction, the percentage that has been allocated in that rule is applied first, but only after the matches are checked against any limits that have been set up.</span></span> <span data-ttu-id="0c655-204">Ако е спазен лимит и средствата на източника на финансиране са изчерпани, правилото за финансиране, свързано с лимита на финансиране, се пренебрегва и програмата проверява следващото правило, което се прилага.</span><span class="sxs-lookup"><span data-stu-id="0c655-204">If a limit has been met, and a funding source’s funds are exhausted, the funding rule that is associated with the funding limit is disregarded, and the program checks for the next rule that applies.</span></span> 

<span data-ttu-id="0c655-205">В някои случаи само част от транзакцията може да бъде разпределена по правило.</span><span class="sxs-lookup"><span data-stu-id="0c655-205">In some cases, only part of a transaction can be allocated under a rule.</span></span> <span data-ttu-id="0c655-206">Това може да се случи, тъй като при достигане на транзакцията е достигнат лимит.</span><span class="sxs-lookup"><span data-stu-id="0c655-206">This might happen because a limit is reached when the transaction is allocated.</span></span> <span data-ttu-id="0c655-207">В този случай според това правило се разпределя само определена сума, като 50 процента за всеки източник на финансиране.</span><span class="sxs-lookup"><span data-stu-id="0c655-207">In this case, only a certain amount is allocated according to that rule, such as 50 percent to each funding source.</span></span> <span data-ttu-id="0c655-208">Такъв е случаят в правило 1, което е описано по-рано в този раздел.</span><span class="sxs-lookup"><span data-stu-id="0c655-208">This is the case in rule 1, which is described earlier in this section.</span></span> <span data-ttu-id="0c655-209">Остатъкът се разпределя съгласно следващото правило в последователността.</span><span class="sxs-lookup"><span data-stu-id="0c655-209">The remainder is allocated according to the next rule in the sequence.</span></span> 

<span data-ttu-id="0c655-210">Следващата таблица разглежда по-подробно този сценарий.</span><span class="sxs-lookup"><span data-stu-id="0c655-210">The following table examines this scenario in more detail.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="0c655-211"><strong>Фокус</strong></span><span class="sxs-lookup"><span data-stu-id="0c655-211"><strong>Focus</strong></span></span></td>
<td><span data-ttu-id="0c655-212"><strong>Подробности</strong></span><span class="sxs-lookup"><span data-stu-id="0c655-212"><strong>Details</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0c655-213">Правила за финансиране</span><span class="sxs-lookup"><span data-stu-id="0c655-213">Funding rules</span></span></td>
<td><ul>
<li><span data-ttu-id="0c655-214">Правило 1 (Приоритет 1): Всички транзакции.</span><span class="sxs-lookup"><span data-stu-id="0c655-214">Rule 1 (Priority 1): All transactions.</span></span> <span data-ttu-id="0c655-215">Разпределете източник на финансиране 2 на 50% и източник на финансиране 3 на 50%.</span><span class="sxs-lookup"><span data-stu-id="0c655-215">Allocate funding source 2 at 50% and funding source 3 at 50%.</span></span></li>
<li><span data-ttu-id="0c655-216">Правило 2 (Приоритет 2): Всички транзакции.</span><span class="sxs-lookup"><span data-stu-id="0c655-216">Rule 2 (Priority 2): All transactions.</span></span> <span data-ttu-id="0c655-217">Разпределете източника на финансиране 3 на 100%.</span><span class="sxs-lookup"><span data-stu-id="0c655-217">Allocate funding source 3 at 100%.</span></span></li>
<li><span data-ttu-id="0c655-218">Правило 3 (Приоритет 2): Всички транзакции.</span><span class="sxs-lookup"><span data-stu-id="0c655-218">Rule 3 (Priority 2): All transactions.</span></span> <span data-ttu-id="0c655-219">Разпределете източника на финансиране 1 на 100%.</span><span class="sxs-lookup"><span data-stu-id="0c655-219">Allocate funding source 1 at 100%.</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0c655-220">Лимити за финансиране</span><span class="sxs-lookup"><span data-stu-id="0c655-220">Funding limits</span></span></td>
<td><ul>
<li><span data-ttu-id="0c655-221">Лимит на източник на финансиране 1 = 10 000,00</span><span class="sxs-lookup"><span data-stu-id="0c655-221">Funding source 1 limit = 10,000.00</span></span></li>
<li><span data-ttu-id="0c655-222">Лимит на източник на финансиране 2 = 500,00</span><span class="sxs-lookup"><span data-stu-id="0c655-222">Funding source 2 limit = 500.00</span></span></li>
<li><span data-ttu-id="0c655-223">Лимит на източник на финансиране 3 = 750,00</span><span class="sxs-lookup"><span data-stu-id="0c655-223">Funding source 3 limit = 750.00</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0c655-224">Транзакция 1</span><span class="sxs-lookup"><span data-stu-id="0c655-224">Transaction 1</span></span></td>
<td><span data-ttu-id="0c655-225"><strong>Сума на транзакцията:</strong> 100,00<strong>Финансиране:</strong> Транзакцията се заплаща само съгласно правило 1, тъй като транзакцията се заплаща изцяло след прилагане на правило 1.</span><span class="sxs-lookup"><span data-stu-id="0c655-225"><strong>Transaction amount:</strong> 100.00<strong>Funding:</strong> The transaction is paid according to rule 1 only, because the transaction is fully paid after rule 1 is applied.</span></span> <span data-ttu-id="0c655-226">Транзакцията се финансира по равно между източника на финансиране 2 и източника на финансиране 3.</span><span class="sxs-lookup"><span data-stu-id="0c655-226">The transaction is funded equally between funding source 2 and funding source 3.</span></span>
<ul>
<li><span data-ttu-id="0c655-227">Източник на финансиране 2: 50,00</span><span class="sxs-lookup"><span data-stu-id="0c655-227">Funding source 2: 50.00</span></span></li>
<li><span data-ttu-id="0c655-228">Източник на финансиране 3: 50,00</span><span class="sxs-lookup"><span data-stu-id="0c655-228">Funding source 3: 50.00</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0c655-229">Транзакция 2</span><span class="sxs-lookup"><span data-stu-id="0c655-229">Transaction 2</span></span></td>
<td><span data-ttu-id="0c655-230"><strong>Сума на транзакцията:</strong> 5 000,00<strong>Финансиране:</strong> Транзакцията се заплаща в съответствие с трите правила.</span><span class="sxs-lookup"><span data-stu-id="0c655-230"><strong>Transaction amount:</strong> 5,000.00<strong>Funding:</strong> The transaction is paid according to all three rules.</span></span> <span data-ttu-id="0c655-231"><strong>Правило 1</strong>
</span><span class="sxs-lookup"><span data-stu-id="0c655-231"><strong>Rule 1</strong>
</span></span><ul>
<li><span data-ttu-id="0c655-232">Източник на финансиране 2: 450,00</span><span class="sxs-lookup"><span data-stu-id="0c655-232">Funding source 2: 450.00</span></span></li>
<li><span data-ttu-id="0c655-233">Източник на финансиране 3: 450,00</span><span class="sxs-lookup"><span data-stu-id="0c655-233">Funding source 3: 450.00</span></span></li>
</ul><span data-ttu-id="0c655-234">
<strong>Правило 2</strong>
</span><span class="sxs-lookup"><span data-stu-id="0c655-234">
<strong>Rule 2</strong>
</span></span><ul>
<li><span data-ttu-id="0c655-235">Източник на финансиране 3: 250,00 (= 750,00 – 50,00 – 450,00)</span><span class="sxs-lookup"><span data-stu-id="0c655-235">Funding source 3: 250.00 (= 750.00 – 50.00 – 450.00)</span></span></li>
</ul><span data-ttu-id="0c655-236">
<strong>Правило 3</strong>
</span><span class="sxs-lookup"><span data-stu-id="0c655-236">
<strong>Rule 3</strong>
</span></span><ul>
<li><span data-ttu-id="0c655-237">Източник на финансиране 1: 3 850,00 (= 5 000,00 – 450,00 – 450,00 – 250,00)</span><span class="sxs-lookup"><span data-stu-id="0c655-237">Funding source 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0c655-238">Общо средства, които се разпределят за всеки източник на финансиране</span><span class="sxs-lookup"><span data-stu-id="0c655-238">Total funds that are distributed for each funding source</span></span></td>
<td><ul>
<li><span data-ttu-id="0c655-239">Източник на финансиране 1: 3.850,00</span><span class="sxs-lookup"><span data-stu-id="0c655-239">Funding source 1: 3,850.00</span></span></li>
<li><span data-ttu-id="0c655-240">Източник на финансиране 2: 500,00</span><span class="sxs-lookup"><span data-stu-id="0c655-240">Funding source 2: 500.00</span></span></li>
<li><span data-ttu-id="0c655-241">Източник на финансиране 3: 750,00</span><span class="sxs-lookup"><span data-stu-id="0c655-241">Funding source 3: 750.00</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="billing-rules"></a><span data-ttu-id="0c655-242">Правила за фактуриране</span><span class="sxs-lookup"><span data-stu-id="0c655-242">Billing rules</span></span>
<span data-ttu-id="0c655-243">Когато договаряте договор за проект с клиент, вие определяте как и кога можете да фактурирате клиента за работа по проект.</span><span class="sxs-lookup"><span data-stu-id="0c655-243">When you negotiate a project contract with a customer, you define how and when you can invoice the customer for work on a project.</span></span> <span data-ttu-id="0c655-244">След като настроите договор за проект и проекта, можете да зададете правила за фактуриране на проекта.</span><span class="sxs-lookup"><span data-stu-id="0c655-244">After you set up the project contract and the project, you can set up billing rules for the project.</span></span> <span data-ttu-id="0c655-245">Правилата за фактуриране се основават на условията на проекта, посочени в договора за проект.</span><span class="sxs-lookup"><span data-stu-id="0c655-245">Billing rules are based on the project terms that are specified in the project contract.</span></span> <span data-ttu-id="0c655-246">Правилата за фактуриране, които можете да създадете, зависят от условията на договор за проект и вида на проекта, като Време и материал или Фиксирана цена, които свързвате с правилото за фактуриране.</span><span class="sxs-lookup"><span data-stu-id="0c655-246">The billing rules that you can create depend on the terms of the project contract and the project type, such as Time and material or Fixed-price, that you associate with the billing rule.</span></span> <span data-ttu-id="0c655-247">Можете да създадете повече от едно правило за фактуриране за договор за проект.</span><span class="sxs-lookup"><span data-stu-id="0c655-247">You can create more than one billing rule for a project contract.</span></span> <span data-ttu-id="0c655-248">Можете също да присвоите правило за фактуриране на множество проекти, които са свързани с един и същ договор за проект и имат сходни условия за фактуриране.</span><span class="sxs-lookup"><span data-stu-id="0c655-248">You can also assign a billing rule to multiple projects that are associated with the same project contract and have similar billing terms.</span></span> 

<span data-ttu-id="0c655-249">Можете да настроите следните видове правила за таксуване:</span><span class="sxs-lookup"><span data-stu-id="0c655-249">You can set up the following types of billing rules:</span></span>

-   <span data-ttu-id="0c655-250">**Единица за доставка** - Фактурирайте клиент, когато попълните единица доставка.</span><span class="sxs-lookup"><span data-stu-id="0c655-250">**Unit of delivery** – Invoice a customer when you complete a unit of delivery.</span></span> <span data-ttu-id="0c655-251">Вие определяте мерните единици за доставка в договора.</span><span class="sxs-lookup"><span data-stu-id="0c655-251">You define the units of delivery in the contract.</span></span>
-   <span data-ttu-id="0c655-252">**Напредък** - Фактурирайте клиент, когато завършите определен процент от проекта.</span><span class="sxs-lookup"><span data-stu-id="0c655-252">**Progress** – Invoice a customer when you complete a specified percentage of the project.</span></span> <span data-ttu-id="0c655-253">Можете да настроите правило за таксуване, за да изчислявате автоматично процента на завършена работа, или можете ръчно да изчислявате процента на завършена работа и сумата, за да фактурирате клиента.</span><span class="sxs-lookup"><span data-stu-id="0c655-253">You can set up a billing rule to automatically calculate the percentage of work completed, or you can manually calculate the percentage of work completed and the amount to invoice the customer.</span></span>
-   <span data-ttu-id="0c655-254">**Контролна точка** - Фактурирайте клиент за пълния размер на етапа на проекта, когато той бъде достигнат.</span><span class="sxs-lookup"><span data-stu-id="0c655-254">**Milestone** – Invoice a customer for the full amount of a project milestone when the milestone is reached.</span></span>
-   <span data-ttu-id="0c655-255">**Такса** - Фактурирайте клиент за вашите услуги плюс такса за управление, която обикновено е процент от цената на услугите.</span><span class="sxs-lookup"><span data-stu-id="0c655-255">**Fee** – Invoice a customer for your services plus a management fee, which is typically a percentage of the cost of services.</span></span>
-   <span data-ttu-id="0c655-256">**Време и материал** - Фактурирайте клиент за стойността на времето и материалите, използвани по даден проект.</span><span class="sxs-lookup"><span data-stu-id="0c655-256">**Time and material** – Invoice a customer for the value of time and materials that are used on a project.</span></span>

<span data-ttu-id="0c655-257">За всички видове правила за таксуване можете да посочите процент на задържане, който се приспада от фактурите на клиентите, докато проектът достигне договорения етап.</span><span class="sxs-lookup"><span data-stu-id="0c655-257">For all types of billing rules, you can specify a retention percentage that is deducted from customer invoices until a project reaches an agreed-upon stage.</span></span> <span data-ttu-id="0c655-258">Процентът на задържане на плащането е посочен в договора за проект.</span><span class="sxs-lookup"><span data-stu-id="0c655-258">The payment retention percentage is specified in the project contract.</span></span> <span data-ttu-id="0c655-259">Сумата се изчислява въз основа и се изважда от общата стойност на редовете във фактура на клиента.</span><span class="sxs-lookup"><span data-stu-id="0c655-259">The amount is calculated based on, and subtracted from, the total value of the lines in a customer invoice.</span></span> 

<span data-ttu-id="0c655-260">За правила за таксуване **Време и материал** и **Напредък**, можете да присвоите таксувани категории.</span><span class="sxs-lookup"><span data-stu-id="0c655-260">For **Time and material** and **Progress** billing rules, you can assign chargeable categories.</span></span> <span data-ttu-id="0c655-261">Категориите за таксуване показват транзакциите, които трябва да бъдат включени във фактурите на клиентите.</span><span class="sxs-lookup"><span data-stu-id="0c655-261">Chargeable categories indicate the transactions that should be included in customer invoices.</span></span> 

<span data-ttu-id="0c655-262">Когато сте готови да фактурирате клиента, сумата за фактура за проекта се изчислява въз основа на правилата за фактуриране и се генерира предложение за фактура за проект.</span><span class="sxs-lookup"><span data-stu-id="0c655-262">When you are ready to invoice the customer, the amount to invoice for the project is calculated based on the billing rules, and a project invoice proposal is generated.</span></span> 

<span data-ttu-id="0c655-263">Следващите раздели предоставят примери, които показват как да настроите и управлявате правилата за фактуриране на проект.</span><span class="sxs-lookup"><span data-stu-id="0c655-263">The following sections provide examples that show how to set up and manage billing rules for a project.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-the-number-of-units-delivered"></a><span data-ttu-id="0c655-264">Пример: Създайте правило за фактуриране, което се основава на броя на доставените единици</span><span class="sxs-lookup"><span data-stu-id="0c655-264">Example: Create a billing rule that is based on the number of units delivered</span></span>

<span data-ttu-id="0c655-265">Вашата организация сключва споразумение за предоставяне на общо пет сесии за обучение на служителите на клиента на цена от 10 000 на сесия на обучение.</span><span class="sxs-lookup"><span data-stu-id="0c655-265">Your organization enters into an agreement to provide a total of five training sessions to a customer’s employees at a cost of 10,000 per training session.</span></span> <span data-ttu-id="0c655-266">Фактурирате клиента след всяка сесия на обучение.</span><span class="sxs-lookup"><span data-stu-id="0c655-266">You invoice the customer after each training session.</span></span> 

<span data-ttu-id="0c655-267">Когато настройвате правилата за фактуриране на договора, използвате следните стойности:</span><span class="sxs-lookup"><span data-stu-id="0c655-267">When you set up the billing rules for the contract, you use the following values:</span></span>

-   <span data-ttu-id="0c655-268">Единицата на доставка е една тренировка.</span><span class="sxs-lookup"><span data-stu-id="0c655-268">The unit of delivery is one training session.</span></span>
-   <span data-ttu-id="0c655-269">Единичната цена е 10 000 на тренировка.</span><span class="sxs-lookup"><span data-stu-id="0c655-269">The unit price is 10,000 per training session.</span></span>
-   <span data-ttu-id="0c655-270">Общият брой на единиците е пет тренировъчни сесии.</span><span class="sxs-lookup"><span data-stu-id="0c655-270">The total number of units is five training sessions.</span></span>

<span data-ttu-id="0c655-271">Когато завършите една тренировъчна сесия, можете да създадете фактура за 10 000 за първата единица, която е доставена, и да изпратите фактурата на клиента.</span><span class="sxs-lookup"><span data-stu-id="0c655-271">When you have completed one training session, you can create an invoice for 10,000, for the first unit that was delivered, and send the invoice to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-manual-calculation"></a><span data-ttu-id="0c655-272">Пример: Създайте правило за таксуване, което се основава на определен процент от завършеността на проекта (ръчно изчисление)</span><span class="sxs-lookup"><span data-stu-id="0c655-272">Example: Create a billing rule that is based on a specified percentage of project completion (manual calculation)</span></span>

<span data-ttu-id="0c655-273">Вашата организация, консултантска фирма за софтуер, сключва споразумение с клиент за разработване на част от продукт, който клиентът разработва.</span><span class="sxs-lookup"><span data-stu-id="0c655-273">Your organization, a software consulting firm, enters into an agreement with a customer to develop part of a product that the customer is developing.</span></span> <span data-ttu-id="0c655-274">Вашата организация се съгласява да доставя софтуерния код за период от шест месеца.</span><span class="sxs-lookup"><span data-stu-id="0c655-274">Your organization agrees to deliver the software code over a period of six months.</span></span> <span data-ttu-id="0c655-275">Клиентът се съгласява да плати на вашата организация общо 100 000 за работата.</span><span class="sxs-lookup"><span data-stu-id="0c655-275">The customer agrees to pay your organization a total of 100,000 for the work.</span></span> <span data-ttu-id="0c655-276">Създавате правило за фактуриране, за да фактурирате клиента въз основа на процента работа, завършена по проекта, както е посочено в договора.</span><span class="sxs-lookup"><span data-stu-id="0c655-276">You create a billing rule to invoice the customer based on the percentage of work that is completed on the project, as specified in the contract.</span></span>

-   <span data-ttu-id="0c655-277">В края на първия месец се срещате с клиента, за да определите процента на завършената работа.</span><span class="sxs-lookup"><span data-stu-id="0c655-277">At the end of the first month, you meet with the customer to determine the percentage of work completed.</span></span> <span data-ttu-id="0c655-278">След като вие и клиентът прегледате проекта, решавате, че проектът е завършен на 15 процента.</span><span class="sxs-lookup"><span data-stu-id="0c655-278">After you and the customer review the project, you decide that the project is 15 percent completed.</span></span>
-   <span data-ttu-id="0c655-279">Създавате фактура за 15 000 (15 процента от 100 000) и я изпращате на клиента.</span><span class="sxs-lookup"><span data-stu-id="0c655-279">You create an invoice for 15,000 (15 percent of 100,000) and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-automatic-calculation"></a><span data-ttu-id="0c655-280">Пример: Създайте правило за таксуване, което се основава на определен процент от завършеността на проекта (автоматично изчисление)</span><span class="sxs-lookup"><span data-stu-id="0c655-280">Example: Create a billing rule that is based on a specified percentage of project completion (automatic calculation)</span></span>

<span data-ttu-id="0c655-281">Вашата организация, фирма за разработка на софтуер, се съгласява да разработи пакет за отчитане на заплати за клиент за 30 000.</span><span class="sxs-lookup"><span data-stu-id="0c655-281">Your organization, a software development firm, agrees to develop a payroll accounting package for a customer for 30,000.</span></span> <span data-ttu-id="0c655-282">Клиентът се съгласява да плати на вашата организация въз основа на процента на изработената работа.</span><span class="sxs-lookup"><span data-stu-id="0c655-282">The customer agrees to pay your organization based on the percentage of work completed.</span></span> <span data-ttu-id="0c655-283">Смятате, че разходите по проекта са 20 000.</span><span class="sxs-lookup"><span data-stu-id="0c655-283">You estimate that the project costs are 20,000.</span></span> <span data-ttu-id="0c655-284">Проектният договор определя категориите работа, които използвате в процеса на фактуриране.</span><span class="sxs-lookup"><span data-stu-id="0c655-284">The project contract specifies the categories of work that you use in the billing process.</span></span> <span data-ttu-id="0c655-285">Настройвате правила за таксуване, които автоматично изчисляват сумите на фактурите за процента на завършена работа за всяка категория.</span><span class="sxs-lookup"><span data-stu-id="0c655-285">You set up billing rules that automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="0c655-286">Вие определяте бюджет за всяка категория:</span><span class="sxs-lookup"><span data-stu-id="0c655-286">You set up a budget for each category:</span></span>

-   <span data-ttu-id="0c655-287">**Развитие** - Разходи от 15 000 и приходи от 20 000</span><span class="sxs-lookup"><span data-stu-id="0c655-287">**Development** – Cost of 15,000 and revenue of 20,000</span></span>
-   <span data-ttu-id="0c655-288">**Инсталация** - Разходи от 5 000 и приходи от 10 000</span><span class="sxs-lookup"><span data-stu-id="0c655-288">**Installation** – Cost of 5,000 and revenue of 10,000</span></span>

<span data-ttu-id="0c655-289">Когато създавате фактура за клиент за първи път, сумата на фактурата се изчислява автоматично въз основа на следната информация:</span><span class="sxs-lookup"><span data-stu-id="0c655-289">When you create a customer invoice for the first time, the invoice amount is automatically calculated based on the following information:</span></span>

-   <span data-ttu-id="0c655-290">След месец работникът по проекта представя работен лист за проекта.</span><span class="sxs-lookup"><span data-stu-id="0c655-290">After a month, the worker on the project submits a timesheet for the project.</span></span> <span data-ttu-id="0c655-291">Цената на часовете на работника е 5000 за разработка и 1000 за монтаж.</span><span class="sxs-lookup"><span data-stu-id="0c655-291">The cost of the worker’s hours is 5,000 for development and 1,000 for installation.</span></span> <span data-ttu-id="0c655-292">Работата по разработката е завършена с 33 процента (5000 действителни разходи/15 000 бюджетни разходи), а монтажната работа е завършена с 20 процента (1000 действителни разходи / 5000 бюджетни разходи).</span><span class="sxs-lookup"><span data-stu-id="0c655-292">The development work is 33 percent completed (5,000 actual cost/15,000 budget cost), and the installation work is 20 percent completed (1,000 actual cost/5,000 budget cost).</span></span>
-   <span data-ttu-id="0c655-293">Сумата на фактурата от 8 667 се изчислява автоматично (33 процента от 20 000 + 20 процента от 10 000).</span><span class="sxs-lookup"><span data-stu-id="0c655-293">The invoice amount of 8,667 is automatically calculated (33 percent of 20,000 + 20 percent of 10,000).</span></span>
-   <span data-ttu-id="0c655-294">Създавате фактура за 8667 и я изпращате на клиента.</span><span class="sxs-lookup"><span data-stu-id="0c655-294">You create an invoice for 8,667 and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-agreed-upon-milestones"></a><span data-ttu-id="0c655-295">Пример: Създайте правило за таксуване, което се основава на договорени етапи</span><span class="sxs-lookup"><span data-stu-id="0c655-295">Example: Create a billing rule that is based on agreed-upon milestones</span></span>

<span data-ttu-id="0c655-296">Вашата организация, консултантска фирма за управление, се съгласява да проведе проучване на пазара за потребителски продукт, който клиентът планира да продаде.</span><span class="sxs-lookup"><span data-stu-id="0c655-296">Your organization, a management consulting firm, agrees to conduct market research for a consumer product that the customer plans to sell.</span></span> <span data-ttu-id="0c655-297">Клиентът се съгласява да използва вашите услуги за период от три месеца, започващ през март, и се съгласява да плати на вашата организация 50 000.</span><span class="sxs-lookup"><span data-stu-id="0c655-297">The customer agrees to use your services for a period of three months, starting in March, and agrees to pay your organization 50,000.</span></span> <span data-ttu-id="0c655-298">Проектът има три основни етапа:</span><span class="sxs-lookup"><span data-stu-id="0c655-298">The project has three milestones:</span></span>

-   <span data-ttu-id="0c655-299">Етап 1: Събиране на потребителски данни - 31 март</span><span class="sxs-lookup"><span data-stu-id="0c655-299">Milestone 1: Collect consumer data – March 31</span></span>
-   <span data-ttu-id="0c655-300">Етап 2: Анализирайте потребителските данни - 30 април</span><span class="sxs-lookup"><span data-stu-id="0c655-300">Milestone 2: Analyze consumer data – April 30</span></span>
-   <span data-ttu-id="0c655-301">Етап 3: Представяне на предложение за жизнеспособност на продукта - 31 май</span><span class="sxs-lookup"><span data-stu-id="0c655-301">Milestone 3: Present a product viability proposal – May 31</span></span>

<span data-ttu-id="0c655-302">Клиентът се съгласява да плати на вашата организация 10 000 за първия етап, 20 000 за втория етап и 20 000 за третия етап.</span><span class="sxs-lookup"><span data-stu-id="0c655-302">The customer agrees to pay your organization 10,000 for the first milestone, 20,000 for the second milestone, and 20,000 for the third milestone.</span></span> 

<span data-ttu-id="0c655-303">Когато създавате договор за проект, вие се съгласявате да таксувате на клиента въз основа на крайния етап, който е завършен.</span><span class="sxs-lookup"><span data-stu-id="0c655-303">When you set up the project contract, you agree to bill the customer based on the milestone that has been completed.</span></span> <span data-ttu-id="0c655-304">Настройката на правилото за таксуване включва следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="0c655-304">The billing rule setup includes the following steps:</span></span>

-   <span data-ttu-id="0c655-305">Определете етапите на проекта.</span><span class="sxs-lookup"><span data-stu-id="0c655-305">Define the project milestones.</span></span>
-   <span data-ttu-id="0c655-306">Определете сумата за фактуриране на клиента, когато всеки етап е изпълнен.</span><span class="sxs-lookup"><span data-stu-id="0c655-306">Define the amount to invoice the customer when each milestone is completed.</span></span>

<span data-ttu-id="0c655-307">Когато първият етап завърши на 31 март, вие отбелязвате етапа като завършен и след това създавате фактура за 10 000 и го изпращате на клиента.</span><span class="sxs-lookup"><span data-stu-id="0c655-307">When the first milestone is completed on March 31, you mark the milestone as completed, and then create an invoice for 10,000 and send it to the customer.</span></span> <span data-ttu-id="0c655-308">Не можете да създадете фактура за крайъгълен камък, докато не го маркирате като завършен.</span><span class="sxs-lookup"><span data-stu-id="0c655-308">You can’t create an invoice for a milestone until you have marked the milestone as completed.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-services-plus-a-management-fee"></a><span data-ttu-id="0c655-309">Пример: Създайте правило за таксуване, което се основава на услуги плюс такса за управление</span><span class="sxs-lookup"><span data-stu-id="0c655-309">Example: Create a billing rule that is based on services plus a management fee</span></span>

<span data-ttu-id="0c655-310">Вашата организация, консултантска фирма за управление, се съгласява да проведе пазарни проучвания, за да оцени жизнеспособността на продукт, който клиентът, компания на дребно, разработва.</span><span class="sxs-lookup"><span data-stu-id="0c655-310">Your organization, a management consulting firm, agrees to conduct market research to evaluate the viability of a product that the customer, a retail company, is developing.</span></span> <span data-ttu-id="0c655-311">Условията на споразумението уточняват, че ще предоставяте услугите на вашите три водещи консултанти по мениджмънт, които ще провеждат изследванията на базата на време и материали.</span><span class="sxs-lookup"><span data-stu-id="0c655-311">The terms of the agreement specify that you will provide the services of your top three management consultants, who will conduct the research on a time-and-materials basis.</span></span> <span data-ttu-id="0c655-312">Клиентът се съгласява да плаща 100 на час, плюс 10 такса за управление за консултантските часове, които се начисляват по проекта.</span><span class="sxs-lookup"><span data-stu-id="0c655-312">The customer agrees to pay 100 per hour, plus a 10 percent management fee for the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="0c655-313">Когато настройвате договор за проект, създайте правило за фактуриране, за да добавите 10 процента такса за управление към часовете за консултации, които се начисляват на проекта.</span><span class="sxs-lookup"><span data-stu-id="0c655-313">When you set up the project contract, create a billing rule to add a 10 percent management fee to the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="0c655-314">Когато създавате фактура за клиента, клиентът получава такса за управление от 10 процента плюс разходите за консултантските часове.</span><span class="sxs-lookup"><span data-stu-id="0c655-314">When you create an invoice for the customer, the customer is billed a 10 percent management fee plus the cost of the consulting hours.</span></span> <span data-ttu-id="0c655-315">Например, ако тримата консултанти са работили общо 200 часа по проекта, се създава фактура за 22 000 въз основа на следното изчисление:</span><span class="sxs-lookup"><span data-stu-id="0c655-315">For example, if the three consultants worked a total of 200 hours on the project, an invoice for 22,000 is created based on the following calculation:</span></span>

-   <span data-ttu-id="0c655-316">200 часа при 100 на час = 20 000</span><span class="sxs-lookup"><span data-stu-id="0c655-316">200 hours at 100 per hour = 20,000</span></span>
-   <span data-ttu-id="0c655-317">10 процента такса за управление = 2000</span><span class="sxs-lookup"><span data-stu-id="0c655-317">10 percent management fee = 2,000</span></span>
-   <span data-ttu-id="0c655-318">Обща сума за фактуриране = 22 000</span><span class="sxs-lookup"><span data-stu-id="0c655-318">Total invoice amount = 22,000</span></span>

<span data-ttu-id="0c655-319">Ако таксите се облагат с клиент и вие изберете група за данък върху продажбите в договора за проект, групата за данък върху продажбите автоматично се въвежда в правило за таксуване.</span><span class="sxs-lookup"><span data-stu-id="0c655-319">If fees are taxable to a customer, and you select a sales tax group in the project contract, the sales tax group is automatically entered in a billing rule for fees.</span></span>

### <a name="example-create-a-billing-rule-for-the-value-of-time-and-materials"></a><span data-ttu-id="0c655-320">Пример: Създайте правило за таксуване за стойността на времето и материалите</span><span class="sxs-lookup"><span data-stu-id="0c655-320">Example: Create a billing rule for the value of time and materials</span></span>

<span data-ttu-id="0c655-321">Вашата организация, консултантска фирма за софтуер, се съгласява да предостави пет технически консултанти, които да работят по проект за разработване на софтуер за клиент през следващите шест месеца.</span><span class="sxs-lookup"><span data-stu-id="0c655-321">Your organization, a software consulting firm, agrees to provide five technical consultants to work on a software development project for a customer for the next six months.</span></span> <span data-ttu-id="0c655-322">Клиентът се съгласява да плати 150 за всеки консултативен час, плюс разходите за офис консумативи.</span><span class="sxs-lookup"><span data-stu-id="0c655-322">The customer agrees to pay 150 for each consulting hour, plus the cost of office supplies.</span></span> <span data-ttu-id="0c655-323">Вашата организация изпраща фактура до клиента в края на всеки месец.</span><span class="sxs-lookup"><span data-stu-id="0c655-323">Your organization sends an invoice to the customer at the end of each month.</span></span> 

<span data-ttu-id="0c655-324">Когато сключвате договор за проект, вие се съгласявате да таксувате на клиента всеки месец за времето и материалите по проекта.</span><span class="sxs-lookup"><span data-stu-id="0c655-324">When you set up the project contract, you agree to bill the customer each month for time and materials on the project.</span></span> <span data-ttu-id="0c655-325">Създавате правило за таксуване, което включва следната информация:</span><span class="sxs-lookup"><span data-stu-id="0c655-325">You create a billing rule that includes the following information:</span></span>

-   <span data-ttu-id="0c655-326">Срокът на договора е шест месеца.</span><span class="sxs-lookup"><span data-stu-id="0c655-326">The contract period is six months.</span></span>
-   <span data-ttu-id="0c655-327">Времето за консултации се изчислява със скорост 150 на час.</span><span class="sxs-lookup"><span data-stu-id="0c655-327">Consulting time is calculated at a rate of 150 per hour.</span></span>
-   <span data-ttu-id="0c655-328">Офис консумативите се фактурират по себестойност, а общите разходи за проекта не трябва да надвишават 10 000.</span><span class="sxs-lookup"><span data-stu-id="0c655-328">Office supplies are invoiced at cost, and the total cost for the project must not exceed 10,000.</span></span>
-   <span data-ttu-id="0c655-329">Вие създавате клиентска фактура в края на всеки календарен месец по време на проекта.</span><span class="sxs-lookup"><span data-stu-id="0c655-329">You create a customer invoice at the end of each calendar month during the project.</span></span>

<span data-ttu-id="0c655-330">През първия месец консултантите по проекта записват общо 800 часа.</span><span class="sxs-lookup"><span data-stu-id="0c655-330">During the first month, a total of 800 hours are recorded by the consultants on the project.</span></span> <span data-ttu-id="0c655-331">Цената на офис консумативи, които се начисляват по проекта, е 2000.</span><span class="sxs-lookup"><span data-stu-id="0c655-331">The cost of office supplies that are charged to the project is 2,000.</span></span> <span data-ttu-id="0c655-332">Следователно в края на месеца създавате фактура за 122 000, което се изчислява като 800 часа при 150 на час, плюс 2000 за офис консумативи.</span><span class="sxs-lookup"><span data-stu-id="0c655-332">Therefore, at the end of the month, you create an invoice for 122,000, which is calculated as 800 hours at 150 per hour, plus 2,000 for office supplies.</span></span>





[!INCLUDE[footer-include](../includes/footer-banner.md)]