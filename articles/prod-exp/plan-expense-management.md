---
title: Конфигуриране на управление на разходите
description: Тази статия описва съображенията и решенията, които трябва да вземете по време на процеса на планиране, преди да конфигурирате управлението на разходите в Microsoft Dynamics 365 Finance.
author: KimANelson
ms.date: 08/29/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: GlobalCategory, ProjCategory, TrvLocations, TrvParameters, TrvPaymethod, TrvPerDiems
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 23001
ms.assetid: aa3fd14d-7e94-4603-985f-ca26d6f860ea
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 52538946c7260fad4076a64e8dc34fecf08b90cf
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005373"
---
# <a name="configure-expense-management"></a><span data-ttu-id="190dd-103">Конфигуриране на управление на разходите</span><span class="sxs-lookup"><span data-stu-id="190dd-103">Configure expense management</span></span>

<span data-ttu-id="190dd-104">Тази тема описва съображенията и решенията, които трябва да вземете по време на процеса на планиране, преди да конфигурирате управлението на разходите.</span><span class="sxs-lookup"><span data-stu-id="190dd-104">This topic describes the considerations and the decisions that you must make during the planning process before you configure Expense management.</span></span> <span data-ttu-id="190dd-105">В управлението на разходите можете да съхранявате информация за начините на плащане, заявките за пътуване, отчетите за разходите, политиките и т.н.</span><span class="sxs-lookup"><span data-stu-id="190dd-105">In Expense management, you can store information about payment methods, travel requisitions, expense reports, policies, and so on.</span></span>

<span data-ttu-id="190dd-106">Тъй като много от решенията, които вземате, когато планирате конфигурацията си за управление на разходите, се основават на йерархията и финансовата структура на вашата организация, трябва да се обърнете към документите за планиране за тези области.</span><span class="sxs-lookup"><span data-stu-id="190dd-106">Because many of the decisions that you make when you plan your configuration for Expense management are based on your organization’s hierarchy and financial structure, you must refer to the planning documents for those areas.</span></span>

## <a name="intercompany-expenses"></a><span data-ttu-id="190dd-107">Междуфирмени разходи</span><span class="sxs-lookup"><span data-stu-id="190dd-107">Intercompany expenses</span></span>

<span data-ttu-id="190dd-108">Когато разрешите вътрешнофирмени разходи, разрешавате на юридически лица и служители да извършват разходи от името на друго юридическо лице и да събират плащания от юридическото лице по заетостта във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="190dd-108">When you enable intercompany expenses, you allow legal entities and employees to incur expenses on behalf of another legal entity, and collect payment from the legal entity of employment within your organization.</span></span> <span data-ttu-id="190dd-109">Например служител в юридическо лице А завършва проект за юридическо лице Б и проектът поема разходи, свързани с пътуването.</span><span class="sxs-lookup"><span data-stu-id="190dd-109">For example, an employee in legal entity A completes a project for legal entity B, and the project incurs travel related expenses.</span></span> <span data-ttu-id="190dd-110">Ако са разрешени вътрешнофирмени разходи, служителят може да подаде отчет за разходите, който ще осчетоводи разходите на юридическо лице Б, а разходите трябва да бъдат платени от юридическо лице А. Ако вашата организация няма няколко юридически лица, вие не не трябва да позволяват вътрешнофирмени разходи.</span><span class="sxs-lookup"><span data-stu-id="190dd-110">If intercompany expenses are enabled, the employee can then file an expense report that will post the expense to legal entity B, and the expense must then be paid by legal entity A. If your organization doesn’t have multiple legal entities, you don’t have to enable intercompany expenses.</span></span>

<span data-ttu-id="190dd-111">**Решение:** Искате ли да активирате вътрешнофирмени разходи?</span><span class="sxs-lookup"><span data-stu-id="190dd-111">**Decision:** Do you want to enable intercompany expenses?</span></span>

## <a name="financial-management"></a><span data-ttu-id="190dd-112">Финансово управление</span><span class="sxs-lookup"><span data-stu-id="190dd-112">Financial management</span></span>

<span data-ttu-id="190dd-113">Управлението на разходите е тясно интегрирано с финансовото управление на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="190dd-113">Expense management is tightly integrated with the financial management of your organization.</span></span> <span data-ttu-id="190dd-114">Голяма част от вашата конфигурация за управление на разходите ще се основава на решенията, които сте взели относно финансите на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="190dd-114">Lots of your configuration for Expense management will be based on the decisions that you’ve made about your organization’s finances.</span></span> <span data-ttu-id="190dd-115">Следващите раздели описват различните области, които изискват планиране и решения, въз основа на финансовите решения на вашата организация и насоки от вашия ръководен екип.</span><span class="sxs-lookup"><span data-stu-id="190dd-115">The following sections describe the various areas that require planning and decisions, based on your organization’s financial decisions and guidance from your leadership team.</span></span>

### <a name="per-diems"></a><span data-ttu-id="190dd-116">Дневни разходи</span><span class="sxs-lookup"><span data-stu-id="190dd-116">Per diems</span></span>

<span data-ttu-id="190dd-117">Трябва да определите дневните за служителите, които вашата организация предоставя.</span><span class="sxs-lookup"><span data-stu-id="190dd-117">You must define the employee per diems that your organization provides.</span></span> <span data-ttu-id="190dd-118">Тъй като дневните обикновено се използват за покриване на разходи като храна, квартира и други съпътстващи разходи, можете да създадете правила за дневни надбавки, които вашата организация предлага.</span><span class="sxs-lookup"><span data-stu-id="190dd-118">Because per diems are typically used to cover expenses such as meals, lodging, and other incidental expenses, you can create rules for the per diem allowances that your organization offers.</span></span> <span data-ttu-id="190dd-119">тарифите за дневни могат да се основават на времето на годината, местоположението на пътуването или и двете.</span><span class="sxs-lookup"><span data-stu-id="190dd-119">per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="190dd-120">Когато определяте правило за дневни, можете да посочите, че процент от дневния размер ще бъде удържан, ако работникът получи безплатни ястия или услуги.</span><span class="sxs-lookup"><span data-stu-id="190dd-120">When you define a per diem rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="190dd-121">Можете също така да определите нива на тарифа за дневни разходи, за да зададете минимален и максимален брой часове, които дневната ставка може да се прилага за пътуването на работник.</span><span class="sxs-lookup"><span data-stu-id="190dd-121">You can also define per diem rate tiers to set the minimum and maximum number of hours that the per diem rate can be applied to a worker’s travel.</span></span>

<span data-ttu-id="190dd-122">**Решения:**</span><span class="sxs-lookup"><span data-stu-id="190dd-122">**Decisions:**</span></span>

- <span data-ttu-id="190dd-123">Правила за дневни дни по подразбиране за първия и последния ден:</span><span class="sxs-lookup"><span data-stu-id="190dd-123">Default per diem rules for the first and last days:</span></span>

    - <span data-ttu-id="190dd-124">Какъв е минималният брой часове, които служителят може да иска за един ден и въпреки това да получава дневни?</span><span class="sxs-lookup"><span data-stu-id="190dd-124">What is the minimum number of hours that an employee can claim for a day and still receive a per diem?</span></span>
    - <span data-ttu-id="190dd-125">Има ли намаление в количеството, което се предлага за хранене за първия ден и последния ден?</span><span class="sxs-lookup"><span data-stu-id="190dd-125">Is there a reduction in the amount that is offered for meals for the first day and last day?</span></span> <span data-ttu-id="190dd-126">Ако има намаление, какъв е процентът на намалението?</span><span class="sxs-lookup"><span data-stu-id="190dd-126">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="190dd-127">Има ли намаление в количеството, което се предлага за хотел за първия ден и последния ден?</span><span class="sxs-lookup"><span data-stu-id="190dd-127">Is there a reduction in the amount that is offered for a hotel for the first day and last day?</span></span> <span data-ttu-id="190dd-128">Ако има намаление, какъв е процентът на намалението?</span><span class="sxs-lookup"><span data-stu-id="190dd-128">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="190dd-129">Има ли намаление в количеството, което се предлага за други разходи, които са направени на първия ден и последния ден?</span><span class="sxs-lookup"><span data-stu-id="190dd-129">Is there a reduction in the amount that is offered for other expenses that are incurred on the first day and last day?</span></span> <span data-ttu-id="190dd-130">Ако има намаление, какъв е процентът на намалението?</span><span class="sxs-lookup"><span data-stu-id="190dd-130">If there is a reduction, what is the percentage of the reduction?</span></span>

- <span data-ttu-id="190dd-131">Правила за дневни разходи по подразбиране:</span><span class="sxs-lookup"><span data-stu-id="190dd-131">Default per diem rules:</span></span>

    - <span data-ttu-id="190dd-132">Има ли процентно намаление на дневната надбавка за всяко хранене, ако например храната е безплатна?</span><span class="sxs-lookup"><span data-stu-id="190dd-132">Is there a percentage reduction in the per diem allowance for each meal if, for example, the meal is complimentary?</span></span> <span data-ttu-id="190dd-133">Ако има намаление, какъв е процентът на намалението за всяко хранене?</span><span class="sxs-lookup"><span data-stu-id="190dd-133">If there is a reduction, what is the reduction percentage for each meal?</span></span>
    - <span data-ttu-id="190dd-134">Намаляването на храненето изчислява ли се на ден, на пътуване или по броя на храненията на ден?</span><span class="sxs-lookup"><span data-stu-id="190dd-134">Is the meal reduction calculated per day, per trip, or by the number of meals per day?</span></span>
    - <span data-ttu-id="190dd-135">Трябва ли сумите за дневни да се закръглят редовно или да се закръглят нагоре?</span><span class="sxs-lookup"><span data-stu-id="190dd-135">Should per diem amounts be rounded in the regular manner or rounded up?</span></span>
    - <span data-ttu-id="190dd-136">Изчисляват ли се дневните за 24-часов период или за календарен ден?</span><span class="sxs-lookup"><span data-stu-id="190dd-136">Are per diems calculated on a 24-hour period or on a calendar day?</span></span>

- <span data-ttu-id="190dd-137">Правила за дневни, които се основават на местоположението:</span><span class="sxs-lookup"><span data-stu-id="190dd-137">Per diem rules that are based on location:</span></span>

    - <span data-ttu-id="190dd-138">Размерите на дневните варират ли в зависимост от местоположението?</span><span class="sxs-lookup"><span data-stu-id="190dd-138">Do per diem rates vary according to location?</span></span> <span data-ttu-id="190dd-139">Какви места са включени?</span><span class="sxs-lookup"><span data-stu-id="190dd-139">What locations are included?</span></span>
    - <span data-ttu-id="190dd-140">Ако дневните ставки се различават в зависимост от местоположението, какъв процент се предоставя за следните видове разходи:</span><span class="sxs-lookup"><span data-stu-id="190dd-140">If per diem rates vary according to location, for each location, what percentage amount is provided for the following types of expenses:</span></span>

        - <span data-ttu-id="190dd-141">Хранене</span><span class="sxs-lookup"><span data-stu-id="190dd-141">Meals</span></span>
        - <span data-ttu-id="190dd-142">Хотел</span><span class="sxs-lookup"><span data-stu-id="190dd-142">Hotel</span></span>
        - <span data-ttu-id="190dd-143">Други разходи</span><span class="sxs-lookup"><span data-stu-id="190dd-143">Other expenses</span></span>

### <a name="expense-management-journals-and-accounts"></a><span data-ttu-id="190dd-144">Списания и сметки за управление на разходите</span><span class="sxs-lookup"><span data-stu-id="190dd-144">Expense management journals and accounts</span></span>

<span data-ttu-id="190dd-145">Управлението на разходите изисква да използвате множество списания и акаунти.</span><span class="sxs-lookup"><span data-stu-id="190dd-145">Expense management requires that you use multiple journals and accounts.</span></span> <span data-ttu-id="190dd-146">Трябва да решите например дали същата сметка се използва за авансови плащания и спорове по кредитни карти.</span><span class="sxs-lookup"><span data-stu-id="190dd-146">You must decide, for example, whether the same account is used for cash advances and credit card disputes.</span></span>

<span data-ttu-id="190dd-147">**Решения:**</span><span class="sxs-lookup"><span data-stu-id="190dd-147">**Decisions:**</span></span>

- <span data-ttu-id="190dd-148">В кой дневник на счетоводната книга се публикуват одобрените отчети за разходите?</span><span class="sxs-lookup"><span data-stu-id="190dd-148">Which ledger journal are approved expense reports posted to?</span></span>
- <span data-ttu-id="190dd-149">Коя сметка се използва за авансови плащания в брой?</span><span class="sxs-lookup"><span data-stu-id="190dd-149">Which account is used for cash advances?</span></span>
- <span data-ttu-id="190dd-150">Трябва ли авансовите плащания да бъдат осчетоводени незабавно?</span><span class="sxs-lookup"><span data-stu-id="190dd-150">Should cash advances be posted immediately?</span></span>

### <a name="payment-methods"></a><span data-ttu-id="190dd-151">Методи на плащане</span><span class="sxs-lookup"><span data-stu-id="190dd-151">Payment methods</span></span>

<span data-ttu-id="190dd-152">Когато позволявате на служителите да правят разходи от името на вашия бизнес, трябва да определите начините на плащане, които служителите имат право да използват.</span><span class="sxs-lookup"><span data-stu-id="190dd-152">When you allow employees to incur expenses on behalf of your business, you must define the payment methods that employees are allowed to use.</span></span> <span data-ttu-id="190dd-153">Например можете да разрешите на служителите да използват пари в брой или корпоративна кредитна карта.</span><span class="sxs-lookup"><span data-stu-id="190dd-153">For example, you might allow employees to use cash or a corporate credit card.</span></span> <span data-ttu-id="190dd-154">Можете също така да позволите на служителите да използват лични кредитни карти и след това да възстановите разходите на служителите.</span><span class="sxs-lookup"><span data-stu-id="190dd-154">You might also allow employees to use personal credit cards, and then reimburse the employees.</span></span> <span data-ttu-id="190dd-155">Трябва да вземете следните решения за всеки разрешен от вас начин на плащане.</span><span class="sxs-lookup"><span data-stu-id="190dd-155">You must make the following decisions for each payment method that you allow.</span></span>

<span data-ttu-id="190dd-156">**Решения:**</span><span class="sxs-lookup"><span data-stu-id="190dd-156">**Decisions:**</span></span>

- <span data-ttu-id="190dd-157">Какви методи на плащане са разрешени?</span><span class="sxs-lookup"><span data-stu-id="190dd-157">What payment methods are allowed?</span></span>
- <span data-ttu-id="190dd-158">Кой е собственик на разходите по метода на плащане?</span><span class="sxs-lookup"><span data-stu-id="190dd-158">Who owns the payment method expenses?</span></span>
- <span data-ttu-id="190dd-159">Има ли компенсиран тип акаунт?</span><span class="sxs-lookup"><span data-stu-id="190dd-159">Is there an offset account type?</span></span> <span data-ttu-id="190dd-160">Ако има компенсиран тип акаунт, какъв е той?</span><span class="sxs-lookup"><span data-stu-id="190dd-160">If there is an offset account type, what is it?</span></span>
- <span data-ttu-id="190dd-161">Ако има компенсиран акаунт, какъв е той?</span><span class="sxs-lookup"><span data-stu-id="190dd-161">If there is an offset account, what is the account?</span></span>
- <span data-ttu-id="190dd-162">Ако методът на плащане е кредитна карта, трябва ли методът на плащане да се използва само при внесени транзакции?</span><span class="sxs-lookup"><span data-stu-id="190dd-162">If the payment method is a credit card, should the payment method be used only with imported transactions?</span></span>

### <a name="expense-categories-and-shared-categories"></a><span data-ttu-id="190dd-163">Категории разходи и споделени категории</span><span class="sxs-lookup"><span data-stu-id="190dd-163">Expense categories and shared categories</span></span>

<span data-ttu-id="190dd-164">Когато служителите създават отчет за разходите, всеки разход, който записват, трябва да бъде свързан с категория разходи.</span><span class="sxs-lookup"><span data-stu-id="190dd-164">When employees create an expense report, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="190dd-165">Категориите на разходите се извличат от споделени категории, които могат да се споделят между юридическите лица във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="190dd-165">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="190dd-166">Тези категории могат да се споделят и в управлението на проекти и счетоводството, в зависимост от начина, по който е дефинирана вашата организация.</span><span class="sxs-lookup"><span data-stu-id="190dd-166">These categories can also be shared in Project management and accounting, depending on the way that your organization is defined.</span></span> <span data-ttu-id="190dd-167">Въз основа на дефиницията на вашата организация и насоки от екипа за внедряване, определете дали категориите, които се използват в управлението на разходите, ще се използват само в управлението на разходите или дали трябва да бъдат споделяни между управлението на проекти и управлението на счетоводство и разходи.</span><span class="sxs-lookup"><span data-stu-id="190dd-167">Based on the definition of your organization and guidance from the implementation team, determine whether the categories that are used in Expense management will be used only in Expense management, or whether they should be shared between Project management and accounting and Expense management.</span></span> <span data-ttu-id="190dd-168">Обърнете внимание, че тези категории могат да се споделят между проекти и разходи или Проект и производство, но не между Разходи и Производство.</span><span class="sxs-lookup"><span data-stu-id="190dd-168">Note that these categories can be shared between Project and Expense or Project and Production, but not between Expense and Production.</span></span> <span data-ttu-id="190dd-169">Трябва да вземете следните решения за всяка категория разходи.</span><span class="sxs-lookup"><span data-stu-id="190dd-169">You must make the following decisions for each expense category.</span></span>

<span data-ttu-id="190dd-170">**Решения:**</span><span class="sxs-lookup"><span data-stu-id="190dd-170">**Decisions:**</span></span>

- <span data-ttu-id="190dd-171">Каква е категорията на разхода?</span><span class="sxs-lookup"><span data-stu-id="190dd-171">What is the expense category?</span></span> <span data-ttu-id="190dd-172">Примерите включват категории за полети, хотел или пробег.</span><span class="sxs-lookup"><span data-stu-id="190dd-172">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="190dd-173">Може ли категорията на разходите да се използва и в управлението на проекти и счетоводството?</span><span class="sxs-lookup"><span data-stu-id="190dd-173">Can the expense category also be used in Project management and accounting?</span></span>
- <span data-ttu-id="190dd-174">Какъв е типът на разхода?</span><span class="sxs-lookup"><span data-stu-id="190dd-174">What is the expense type?</span></span>
- <span data-ttu-id="190dd-175">Какъв е методът на плащане по подразбиране за категорията разходи?</span><span class="sxs-lookup"><span data-stu-id="190dd-175">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="190dd-176">Трябва ли разходите в категорията на разходите да бъдат детайлизирани?</span><span class="sxs-lookup"><span data-stu-id="190dd-176">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="190dd-177">Какъв е основният акаунт по подразбиране за категорията разходи?</span><span class="sxs-lookup"><span data-stu-id="190dd-177">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="190dd-178">Каква е групата по данък върху продажбите по подразбиране за категорията на разходите?</span><span class="sxs-lookup"><span data-stu-id="190dd-178">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="190dd-179">Разрешени ли са допълнителни методи на плащане за разходната категория?</span><span class="sxs-lookup"><span data-stu-id="190dd-179">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="190dd-180">Ако са разрешени допълнителни методи на плащане, кои са те?</span><span class="sxs-lookup"><span data-stu-id="190dd-180">If additional payment methods are allowed, what are they?</span></span>
- <span data-ttu-id="190dd-181">Има ли подкатегории в тази категория разходи?</span><span class="sxs-lookup"><span data-stu-id="190dd-181">Are there subcategories in this expense category?</span></span> <span data-ttu-id="190dd-182">Ако има подкатегории, вие също трябва да вземете следните решения:</span><span class="sxs-lookup"><span data-stu-id="190dd-182">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="190dd-183">Изключена ли е някоя от подкатегориите от събирането на данъци?</span><span class="sxs-lookup"><span data-stu-id="190dd-183">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="190dd-184">Каква е групата за данък върху продажбите на артикули в подкатегориите?</span><span class="sxs-lookup"><span data-stu-id="190dd-184">What is the item sales tax group of the subcategories?</span></span>

<span data-ttu-id="190dd-185">Ако категорията разходи се използва и в управлението на проекти и счетоводството, отговорете на останалите въпроси.</span><span class="sxs-lookup"><span data-stu-id="190dd-185">If the expense category is also used in Project management and accounting, answer the remaining questions.</span></span> <span data-ttu-id="190dd-186">В противен случай преминете към следващия раздел.</span><span class="sxs-lookup"><span data-stu-id="190dd-186">Otherwise, move on to the next section.</span></span>

- <span data-ttu-id="190dd-187">Кои сметки за разходи ще бъдат използвани за следните разходи?</span><span class="sxs-lookup"><span data-stu-id="190dd-187">Which cost accounts will be used for the following expenses?</span></span>

    - <span data-ttu-id="190dd-188">Разход</span><span class="sxs-lookup"><span data-stu-id="190dd-188">Cost</span></span>
    - <span data-ttu-id="190dd-189">Разпределение на изплащания</span><span class="sxs-lookup"><span data-stu-id="190dd-189">Payroll allocation</span></span>
    - <span data-ttu-id="190dd-190">Стойност на разход за WIP</span><span class="sxs-lookup"><span data-stu-id="190dd-190">WIP-cost value</span></span>
    - <span data-ttu-id="190dd-191">Елемент на разходите</span><span class="sxs-lookup"><span data-stu-id="190dd-191">Cost-item</span></span>
    - <span data-ttu-id="190dd-192">Елемент на стойност на елемент на WIP</span><span class="sxs-lookup"><span data-stu-id="190dd-192">WIP-cost value-item</span></span>
    - <span data-ttu-id="190dd-193">Натрупана загуба</span><span class="sxs-lookup"><span data-stu-id="190dd-193">Accrued loss</span></span>
    - <span data-ttu-id="190dd-194">WIP - натрупана загуба</span><span class="sxs-lookup"><span data-stu-id="190dd-194">WIP-accrued loss</span></span>

- <span data-ttu-id="190dd-195">Кои сметки за приходи ще бъдат използвани за следните?</span><span class="sxs-lookup"><span data-stu-id="190dd-195">Which revenue accounts will be used for the following?</span></span>

    - <span data-ttu-id="190dd-196">Фактурирани приходи</span><span class="sxs-lookup"><span data-stu-id="190dd-196">Invoiced revenue</span></span>
    - <span data-ttu-id="190dd-197">Начислени приходи - Стойност на продажби</span><span class="sxs-lookup"><span data-stu-id="190dd-197">Accrued revenue-sales value</span></span>
    - <span data-ttu-id="190dd-198">WIP-продажбена стойност</span><span class="sxs-lookup"><span data-stu-id="190dd-198">WIP-sales value</span></span>
    - <span data-ttu-id="190dd-199">Натрупани приходи-производство</span><span class="sxs-lookup"><span data-stu-id="190dd-199">Accrued revenue-production</span></span>
    - <span data-ttu-id="190dd-200">WIP-Продукция</span><span class="sxs-lookup"><span data-stu-id="190dd-200">WIP-production</span></span>
    - <span data-ttu-id="190dd-201">Натрупани приходи-приход</span><span class="sxs-lookup"><span data-stu-id="190dd-201">Accrued revenue-profit</span></span>
    - <span data-ttu-id="190dd-202">WIP-приход</span><span class="sxs-lookup"><span data-stu-id="190dd-202">WIP-profit</span></span>
    - <span data-ttu-id="190dd-203">Натрупани приходи-абонамент</span><span class="sxs-lookup"><span data-stu-id="190dd-203">Accrued revenue-subscription</span></span>
    - <span data-ttu-id="190dd-204">WIP-Абонамент</span><span class="sxs-lookup"><span data-stu-id="190dd-204">WIP-subscription</span></span>

### <a name="taxes"></a><span data-ttu-id="190dd-205">Данъци</span><span class="sxs-lookup"><span data-stu-id="190dd-205">Taxes</span></span>

<span data-ttu-id="190dd-206">За данъци, свързани с разходите, трябва да определите какво е включено или разрешено в отчетите за разходите.</span><span class="sxs-lookup"><span data-stu-id="190dd-206">For expense-related taxes, you must determine what is included or enabled on expense reports.</span></span>

<span data-ttu-id="190dd-207">**Решения:**</span><span class="sxs-lookup"><span data-stu-id="190dd-207">**Decisions:**</span></span>

- <span data-ttu-id="190dd-208">Данъкът върху продажбите включен ли е в сумите на разходите?</span><span class="sxs-lookup"><span data-stu-id="190dd-208">Is sales tax included in the expense amounts?</span></span>
- <span data-ttu-id="190dd-209">Трябва ли да се даде възможност за събиране на данъци върху разходите?</span><span class="sxs-lookup"><span data-stu-id="190dd-209">Should tax recovery be enabled on expenses?</span></span>

    > [!NOTE]
    > <span data-ttu-id="190dd-210">Когато сте планирали главната книга, ако сте решили да приложите данък върху продажбите в САЩ и да използвате данъчни правила, не можете да разрешите възстановяване на данъци върху разходите.</span><span class="sxs-lookup"><span data-stu-id="190dd-210">When you were planning the general ledger, if you decided to apply U.S. sales tax and use tax rules, you can’t enable tax recovery on expenses.</span></span> <span data-ttu-id="190dd-211">(За да приложите данък върху продажбите в САЩ и да използвате данъчни правила, задайте опцията **Прилагайте правилата за данъчно облагане на продажбите** на **Да**.)</span><span class="sxs-lookup"><span data-stu-id="190dd-211">(To apply U.S. sales tax and use tax rules, set the **Apply sales tax taxations rules** option to **Yes**.)</span></span>

## <a name="policies"></a><span data-ttu-id="190dd-212">Правила</span><span class="sxs-lookup"><span data-stu-id="190dd-212">Policies</span></span>

<span data-ttu-id="190dd-213">Създавайки политики за отчети за разходите, можете да помогнете на вашата организация да спести време и пари, когато служителите правят разходи от нейно име.</span><span class="sxs-lookup"><span data-stu-id="190dd-213">By creating expense report policies, you can help your organization save time and money when employees incur expenses on its behalf.</span></span> <span data-ttu-id="190dd-214">Политиките помагат да се гарантира, че служителите остават в бюджета, предоставят цялата необходима информация и харчат пари само както им е необходимо.</span><span class="sxs-lookup"><span data-stu-id="190dd-214">Policies help guarantee that employees stay in budget, provide all required information, and spend money only as they require it.</span></span> <span data-ttu-id="190dd-215">Трябва да вземете следните решения за всяка политика на отчета за разходите и всяка политика за одобрение на отчета за разходите, която създавате.</span><span class="sxs-lookup"><span data-stu-id="190dd-215">You must make the following decisions for each expense report policy and each expense report approval policy that you create.</span></span>

<span data-ttu-id="190dd-216">**Решения:**</span><span class="sxs-lookup"><span data-stu-id="190dd-216">**Decisions:**</span></span>

- <span data-ttu-id="190dd-217">Какво е името на политиката?</span><span class="sxs-lookup"><span data-stu-id="190dd-217">What is the name of the policy?</span></span>
- <span data-ttu-id="190dd-218">За какво служи разходната политика?</span><span class="sxs-lookup"><span data-stu-id="190dd-218">What is the expense policy for?</span></span>
- <span data-ttu-id="190dd-219">Ако преди това сте решили да разрешите вътрешнофирмени разходи, за кои компании във вашата организация ще се прилага тази политика?</span><span class="sxs-lookup"><span data-stu-id="190dd-219">If you previously decided to enable intercompany expenses, which companies in your organization will this policy apply to?</span></span>
- <span data-ttu-id="190dd-220">Кога политиката влиза в сила?</span><span class="sxs-lookup"><span data-stu-id="190dd-220">When does the policy become effective?</span></span>
- <span data-ttu-id="190dd-221">Кога изтича политиката?</span><span class="sxs-lookup"><span data-stu-id="190dd-221">When does the policy expire?</span></span>
- <span data-ttu-id="190dd-222">Какво е правилото на политиката?</span><span class="sxs-lookup"><span data-stu-id="190dd-222">What is the policy rule?</span></span>
- <span data-ttu-id="190dd-223">Какъв е резултатът от правилото на политиката?</span><span class="sxs-lookup"><span data-stu-id="190dd-223">What is the outcome of the policy rule?</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]