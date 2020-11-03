---
title: Създаване и потвърждаване на журнали за корекции
description: Тази тема предоставя информация за това как да създадете и потвърдите журнал за корекции.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 855593df1ea14827f06961dda5b4becd2fa75c18
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071817"
---
# <a name="create-and-confirm-correction-journals"></a><span data-ttu-id="79abc-103">Създаване и потвърждаване на журнали за корекции</span><span class="sxs-lookup"><span data-stu-id="79abc-103">Create and confirm Correction journals</span></span>

<span data-ttu-id="79abc-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="79abc-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="79abc-105">Понякога записът за време или разход може да бъде въведен неправилно.</span><span class="sxs-lookup"><span data-stu-id="79abc-105">Occasionally a time or expense entry may be entered incorrectly.</span></span> <span data-ttu-id="79abc-106">Например, консултант може да избере грешна дата при създаване на времеви запис или може да транспонира номерата при въвеждане на разход.</span><span class="sxs-lookup"><span data-stu-id="79abc-106">For example, a consultant might select the wrong date when creating a time entry or they might transpose the numbers when entering an expense.</span></span> <span data-ttu-id="79abc-107">Ако консултант не може да извърши актуализациите на подадените записи, администратор може директно да коригира записа за проект.</span><span class="sxs-lookup"><span data-stu-id="79abc-107">If a consultant can’t make the updates to the submitted entries, an administrator can directly correct the entry for a project.</span></span>

<span data-ttu-id="79abc-108">За да завършите процедурите в тази тема, ще ви трябват разрешения за администратор.</span><span class="sxs-lookup"><span data-stu-id="79abc-108">To complete the procedures in this topic, you will need Administrator permissions.</span></span>

## <a name="correct-approved-time-entries"></a><span data-ttu-id="79abc-109">Правилни одобрени записи за време</span><span class="sxs-lookup"><span data-stu-id="79abc-109">Correct approved time entries</span></span>     

<span data-ttu-id="79abc-110">Изпълнете следните стъпки, за да коригирате един или няколко записа за време.</span><span class="sxs-lookup"><span data-stu-id="79abc-110">Complete the following steps to correct single or multiple time entries for a project.</span></span>

1. <span data-ttu-id="79abc-111">В областта **Продажби** изберете **Трансакции** и след това изберете **Час на одобряване**.</span><span class="sxs-lookup"><span data-stu-id="79abc-111">In the **Sales** area, select **Transactions** , and then select **Approved Time**.</span></span> 

2. <span data-ttu-id="79abc-112">В списъка **Час на одобряване** намерете и изберете един или повече одобрени записи за време, които да коригирате.</span><span class="sxs-lookup"><span data-stu-id="79abc-112">In the **Approved Time** list, locate and select one or more approved time entries to correct.</span></span> <span data-ttu-id="79abc-113">Можете да използвате филтъра, за да намерите свързани записи.</span><span class="sxs-lookup"><span data-stu-id="79abc-113">You can use the filter to locate related entries.</span></span> <span data-ttu-id="79abc-114">Например, можете да филтрирате по ИД на проекта и да изберете всички одобрени записи за време с този ИД на проект.</span><span class="sxs-lookup"><span data-stu-id="79abc-114">For example, you might filter on a Project ID, and select all approved time entries with that Project ID.</span></span>

3. <span data-ttu-id="79abc-115">Изберете **Правилни записи**.</span><span class="sxs-lookup"><span data-stu-id="79abc-115">Select **Correct entries**.</span></span> <span data-ttu-id="79abc-116">Автоматично се създава нов журнал за корекция с присвоен тип **Корекция на времето**.</span><span class="sxs-lookup"><span data-stu-id="79abc-116">A new correction journal is automatically created, with the assigned type **Time correction**.</span></span> <span data-ttu-id="79abc-117">Избраните от вас записи се добавят към дневника.</span><span class="sxs-lookup"><span data-stu-id="79abc-117">The entries you selected are added to the journal.</span></span> 

4. <span data-ttu-id="79abc-118">На страницата **Нов дневник** въведете **Описание** за вашия корекционен дневник и след това изберете раздела **Корекции за времеви записи**.</span><span class="sxs-lookup"><span data-stu-id="79abc-118">On the **New Journal** page, enter a **Description** for your correction journal, and then select the **Time Entry Corrections** tab.</span></span>  

5. <span data-ttu-id="79abc-119">В секцията **Нови стойности за времеви записи** актуализирайте полетата с необходимата информация.</span><span class="sxs-lookup"><span data-stu-id="79abc-119">In the **New Values for Time Entries** section, update the fields with the correct information as necessary.</span></span> <span data-ttu-id="79abc-120">Например, можете да промените зададения проект или наличния ресурс.</span><span class="sxs-lookup"><span data-stu-id="79abc-120">For example, you can change the assigned project or the bookable resource.</span></span>

6. <span data-ttu-id="79abc-121">Изберете **Преглед**.</span><span class="sxs-lookup"><span data-stu-id="79abc-121">Select **Preview**.</span></span> <span data-ttu-id="79abc-122">В диалоговия прозорец изберете **ОК**.</span><span class="sxs-lookup"><span data-stu-id="79abc-122">In the dialog box, select **OK**.</span></span> <span data-ttu-id="79abc-123">В раздела **Счетоводни записи** можете да видите списък на оригиналните актуални данни, които са свързани с избраните времеви записи, които са обърнати, и коригираните съответни редове, които са създадени.</span><span class="sxs-lookup"><span data-stu-id="79abc-123">On the **Journal lines** tab, you can view a list of the original actuals that are related to the selected time entries that have been reversed and the corrected corresponding lines that have been created.</span></span> <span data-ttu-id="79abc-124">Ако е необходимо да се направят допълнителни корекции, повторете стъпки 5 и 6.</span><span class="sxs-lookup"><span data-stu-id="79abc-124">If additional corrections need to be made, repeat steps 5 and 6.</span></span> 

> [!NOTE]
> <span data-ttu-id="79abc-125">Всички коригирани актуални данни ще имат същите стойности, които сте избрали в секцията **Нови стойности за времевите записи**.</span><span class="sxs-lookup"><span data-stu-id="79abc-125">All the corrected actuals will have the same values that you selected in the **New values for Time Entries** section.</span></span>

7. <span data-ttu-id="79abc-126">Ако корекциите се появят според очакванията, изберете **Потвърждение**.</span><span class="sxs-lookup"><span data-stu-id="79abc-126">If the corrections appear as expected, select **Confirm**.</span></span> <span data-ttu-id="79abc-127">В диалоговия прозорец изберете **ОК**.</span><span class="sxs-lookup"><span data-stu-id="79abc-127">In the dialog box, select **OK**.</span></span>

8. <span data-ttu-id="79abc-128">Върнете се към областта **Продажби** , изберете **Проекти** и след това отворете проекта, за който току-що сте актуализирали записите във времето.</span><span class="sxs-lookup"><span data-stu-id="79abc-128">Return to the **Sales** area, select **Projects** , and then open the project for which you just updated the time entries.</span></span> 

9. <span data-ttu-id="79abc-129">На страницата **Проекти** в раздела **Действителни данни** разгледайте промените, които сте направили.</span><span class="sxs-lookup"><span data-stu-id="79abc-129">On the **Projects** page, on the **Actuals** tab, view the changes that you made.</span></span> 

> [!NOTE]
> <span data-ttu-id="79abc-130">Ако разделът **Действителни данни** не се вижда, изберете **Свързани** > **Действителни данни**.</span><span class="sxs-lookup"><span data-stu-id="79abc-130">If the **Actuals** tab is not visible, select **Related** > **Actuals**.</span></span>  

10. <span data-ttu-id="79abc-131">В списъка **Свързан изглед на действителни данни** можете да видите, че първоначалните времеви записи, които са били обърнати, все още са изброени, както и съответните коригирани записи на времето.</span><span class="sxs-lookup"><span data-stu-id="79abc-131">In the **Actual Associated View** list, you can see that the original time entries that have been reversed are still listed, as are the corresponding corrected time entries.</span></span> 

<span data-ttu-id="79abc-132">За пример в следващата графика има две договорени позиции с количество 8,00, които имат дебити, изброени в колоната „Сума”.</span><span class="sxs-lookup"><span data-stu-id="79abc-132">For example, in the following graphic, there are two line items with a quantity of 8.00 that have debits listed in the Amount column.</span></span> <span data-ttu-id="79abc-133">Освен това има две договорени покупки с количество от -8.00, които показват кредитирани суми в колоната „Сума”.</span><span class="sxs-lookup"><span data-stu-id="79abc-133">Additionally, there are two line items with a quantity of -8.00 that show credited amounts in the Amount column.</span></span> <span data-ttu-id="79abc-134">Тези корекции довеждат количеството до нула.</span><span class="sxs-lookup"><span data-stu-id="79abc-134">These corrections bring the quantity to zero.</span></span>

 
## <a name="correct-approved-expense-entries"></a><span data-ttu-id="79abc-135">Правилни одобрени записи за разходи</span><span class="sxs-lookup"><span data-stu-id="79abc-135">Correct approved expense entries</span></span>

<span data-ttu-id="79abc-136">Изпълнете следните стъпки, за да коригирате един или повече записи на разходите.</span><span class="sxs-lookup"><span data-stu-id="79abc-136">Complete the following steps to correct one or more expense entries.</span></span> 

1. <span data-ttu-id="79abc-137">В областта **Продажби** в левия панел за навигация, под **Трансакции** изберете **Одобрени разходи**.</span><span class="sxs-lookup"><span data-stu-id="79abc-137">In the **Sales** area, in the left navigation pane, under **Transactions** , select **Approved Expenses**.</span></span>

2. <span data-ttu-id="79abc-138">В списъка **Одобрени разходи** изберете проекта, който искате да коригирате, и след това изберете **Правилни записи**.</span><span class="sxs-lookup"><span data-stu-id="79abc-138">In the **Approved Expenses** list, select the project that you want to correct, and then select **Correct entries**.</span></span> <span data-ttu-id="79abc-139">Автоматично се създава нов журнал за корекция с присвоен тип **Корекция на разход**.</span><span class="sxs-lookup"><span data-stu-id="79abc-139">A new correction journal will be created automatically with the assigned type of **Expense correction**.</span></span> 

3. <span data-ttu-id="79abc-140">На страницата **Нов дневник** въведете **Описание** за корекцията и в раздела **Корекция на разходите** в секцията **Нови стойности за разходи** изберете полетата за данни, които искате да коригирате за избраните редове разходи.</span><span class="sxs-lookup"><span data-stu-id="79abc-140">On the **New Journal** page, enter a **Description** for the correction, and on the **Expense Correction** tab, in the **New Values for Expenses** section, select the data fields that you want to correct for the selected expense lines.</span></span> <span data-ttu-id="79abc-141">Можете например да прехвърлите разходите на друг **Проект** или да коригирате **Категория разходи** , **Дата на разход** или **Наличен ресурс**.</span><span class="sxs-lookup"><span data-stu-id="79abc-141">For example, you can assign the expense to another **Project** , or correct the **Expense Category** , **Expense Date** , or **Bookable Resource**.</span></span>

4. <span data-ttu-id="79abc-142">Изберете **Преглед**.</span><span class="sxs-lookup"><span data-stu-id="79abc-142">Select **Preview**.</span></span> <span data-ttu-id="79abc-143">В диалоговия прозорец изберете **ОК**.</span><span class="sxs-lookup"><span data-stu-id="79abc-143">In the dialog box, select **OK**.</span></span> 

5. <span data-ttu-id="79abc-144">Проверете корекциите в раздела **Счетоводни записи**. Можете да видите списък на оригиналните актуални данни, които са свързани с избраните записи за разходи, които са обърнати, и коригираните съответни редове, които са създадени.</span><span class="sxs-lookup"><span data-stu-id="79abc-144">Verify the corrections on the **Journal lines** tab. You can view a list of the original actuals that are related to the selected expense entries that have been reversed and the corrected corresponding lines that have been created.</span></span>

6. <span data-ttu-id="79abc-145">Ако коригираните стойности се появят според очакванията, изберете **Потвърждение**.</span><span class="sxs-lookup"><span data-stu-id="79abc-145">If the corrected values are as expected, select **Confirm**.</span></span> <span data-ttu-id="79abc-146">В диалоговия прозорец изберете **ОК**.</span><span class="sxs-lookup"><span data-stu-id="79abc-146">In the dialog box, select **OK.**</span></span> <span data-ttu-id="79abc-147">Ако стойностите не се показват според очакванията, изберете **Отмяна** , за да се върнете към списъка **Одобрени разходи**.</span><span class="sxs-lookup"><span data-stu-id="79abc-147">If the values are not showing as expected, select **Cancel** to return to the **Approved Expenses** list.</span></span> <span data-ttu-id="79abc-148">Повторете стъпки 2 до 5.</span><span class="sxs-lookup"><span data-stu-id="79abc-148">Repeat steps 2 through 5.</span></span> 

> [!NOTE]
> <span data-ttu-id="79abc-149">Коригираните действителни данни ще имат същите стойности, които сте избрали в секцията **Нови стойности за разходи**.</span><span class="sxs-lookup"><span data-stu-id="79abc-149">The corrected actuals will have the same values that you selected in the **New values for Expenses** section.</span></span>

7. <span data-ttu-id="79abc-150">След като потвърдите дневника за корекция, върнете се към проекта или проектите, които сте актуализирали, за да видите промените си.</span><span class="sxs-lookup"><span data-stu-id="79abc-150">After you confirm the correction journal, navigate back to the project or projects that you updated, to view your changes.</span></span>  

8. <span data-ttu-id="79abc-151">В страницата на проекта, в раздела **Действителни данни** прегледайте **Свързан изглед на действителни данни**.</span><span class="sxs-lookup"><span data-stu-id="79abc-151">In the project page, on the **Actuals** tab, review the **Actual Associated View**.</span></span> <span data-ttu-id="79abc-152">Оригиналните записи и коригираните записи са изброени.</span><span class="sxs-lookup"><span data-stu-id="79abc-152">The original entries and the corrected entries are listed.</span></span> <span data-ttu-id="79abc-153">Следващата графика показва оригиналните суми за въвеждане на разходи и съответните коригирани суми за входящи разходи.</span><span class="sxs-lookup"><span data-stu-id="79abc-153">The following graphic shows original expense entry amounts and the corresponding corrected expense entry amounts.</span></span> 


