---
title: Базирани на проект редове на оферта (Pro)
description: Тази тема предоставя информация за използването на проектни базирани реплики за проектна работа. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a409d1e378afe97de7fb6c77cf3ad6703661bdff
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071750"
---
# <a name="project-based-quote-lines-pro"></a><span data-ttu-id="80c64-104">Базирани на проект редове на оферта (Pro)</span><span class="sxs-lookup"><span data-stu-id="80c64-104">Project-based quote lines (Pro)</span></span>

<span data-ttu-id="80c64-105">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="80c64-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="80c64-106">Котировъчните редове, базирани на проекти, са предназначени да помогнат да се оцени работата по проекта по ангажимент.</span><span class="sxs-lookup"><span data-stu-id="80c64-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="80c64-107">Структурата на проектна линия на оферти се разширява за проектни оценки със следните концепции:</span><span class="sxs-lookup"><span data-stu-id="80c64-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="80c64-108">Метод на фактуриране</span><span class="sxs-lookup"><span data-stu-id="80c64-108">Billing Method</span></span>
- <span data-ttu-id="80c64-109">Съпоставяне на проект и задача</span><span class="sxs-lookup"><span data-stu-id="80c64-109">Project and Task Mapping</span></span>
- <span data-ttu-id="80c64-110">Включени класове за транзакции</span><span class="sxs-lookup"><span data-stu-id="80c64-110">Included Transaction classes</span></span>
- <span data-ttu-id="80c64-111">Ограничение, което да не се надвишава</span><span class="sxs-lookup"><span data-stu-id="80c64-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="80c64-112">Настройка на платимост</span><span class="sxs-lookup"><span data-stu-id="80c64-112">Chargeability setup</span></span>
- <span data-ttu-id="80c64-113">Оценка с помощта на подробности за цитираната линия</span><span class="sxs-lookup"><span data-stu-id="80c64-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="80c64-114">Клиенти от ред на оферта</span><span class="sxs-lookup"><span data-stu-id="80c64-114">Quote line Customers</span></span>

<span data-ttu-id="80c64-115">Следващата таблица предоставя информация за полетата на раздела **Общи** на котирана линия, базирана на проекти.</span><span class="sxs-lookup"><span data-stu-id="80c64-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="80c64-116">Тези полета помагат да се създаде основата за подробна, обоснована оценка на работата по проекта.</span><span class="sxs-lookup"><span data-stu-id="80c64-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="80c64-117">**Поле**</span><span class="sxs-lookup"><span data-stu-id="80c64-117">**Field**</span></span> | <span data-ttu-id="80c64-118">**Уместност, цел и насоки**</span><span class="sxs-lookup"><span data-stu-id="80c64-118">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="80c64-119">**Въздействие надолу по течението**</span><span class="sxs-lookup"><span data-stu-id="80c64-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="80c64-120">Име</span><span class="sxs-lookup"><span data-stu-id="80c64-120">Name</span></span> | <span data-ttu-id="80c64-121">Името на котировката, която трябва да ви помогне да идентифицирате отделния компонент на котировката, която се оценява.</span><span class="sxs-lookup"><span data-stu-id="80c64-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="80c64-122">Копира се в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="80c64-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="80c64-123">Метод на фактуриране</span><span class="sxs-lookup"><span data-stu-id="80c64-123">Billing Method</span></span> | <span data-ttu-id="80c64-124">При оферта, създадена от възможност, тази стойност се копира от съответното поле на реда за възможности.</span><span class="sxs-lookup"><span data-stu-id="80c64-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="80c64-125">Това поле включва двата основни модела за договаряне, поддържани от Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="80c64-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="80c64-126">- Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="80c64-126">- Fixed price</span></span></br><span data-ttu-id="80c64-127">- Време и материали.</span><span class="sxs-lookup"><span data-stu-id="80c64-127">- Time and material.</span></span>| <span data-ttu-id="80c64-128">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="80c64-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="80c64-129">Project</span><span class="sxs-lookup"><span data-stu-id="80c64-129">Project</span></span> | <span data-ttu-id="80c64-130">Използвайте това незадължително поле, за да идентифицирате проекта, който ще бъде използван за изпълнение на работата по този ангажимент.</span><span class="sxs-lookup"><span data-stu-id="80c64-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="80c64-131">Когато даден проект се картографира в котировъчен ред, това помага при настройването на таксувани задачи, а също и при въвеждането на прогнозна оценка, базирана на проекта, в линията на котировката като подробности за цитатната линия.</span><span class="sxs-lookup"><span data-stu-id="80c64-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="80c64-132">Когато даден проект не е съпоставен с проектна линия на котировка, оценката трябва да бъде създадена ръчно чрез създаване на всеки детайл на котировката.</span><span class="sxs-lookup"><span data-stu-id="80c64-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="80c64-133">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="80c64-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="80c64-134">Включени задачи</span><span class="sxs-lookup"><span data-stu-id="80c64-134">Included Tasks</span></span> | <span data-ttu-id="80c64-135">Показва дали този ред с редове на оферта се използва за всички или някои от проектните задачи за избрания проект.</span><span class="sxs-lookup"><span data-stu-id="80c64-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="80c64-136">Това поле има следните възможни стойности:</span><span class="sxs-lookup"><span data-stu-id="80c64-136">This field has the following possible values:</span></span></br><span data-ttu-id="80c64-137">- Всички задачи по проекта</span><span class="sxs-lookup"><span data-stu-id="80c64-137">- All project tasks</span></span></br><span data-ttu-id="80c64-138">- Само избрани задачи по проекта</span><span class="sxs-lookup"><span data-stu-id="80c64-138">- Selected project tasks only</span></span></br><span data-ttu-id="80c64-139">Празна стойност в това поле е еквивалентна на опцията **Всички проектни задачи**.</span><span class="sxs-lookup"><span data-stu-id="80c64-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="80c64-140">Когато е избрано **Само избрани проектни задачи** на страницата на проекта, разделът **Настройка на фактурирането на задачата** ви позволява да изберете конкретни задачи, за да ги свържете с този ред на офертите.</span><span class="sxs-lookup"><span data-stu-id="80c64-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="80c64-141">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="80c64-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="80c64-142">Включване на време</span><span class="sxs-lookup"><span data-stu-id="80c64-142">Include Time</span></span> | <span data-ttu-id="80c64-143">Флагът **Да**/**Не** показва дали транзакциите във времето или разходите за труд по избрания проект ще бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="80c64-144">Стойността **Не** показва, че транзакциите за времето или разходите за труд няма да бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="80c64-145">Стойността **Да** показва, че транзакциите за времето или разходите за труд ще да бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="80c64-146">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="80c64-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="80c64-147">Включване на разход</span><span class="sxs-lookup"><span data-stu-id="80c64-147">Include Expense</span></span> | <span data-ttu-id="80c64-148">Флагът **Да**/**Не** показва дали разходите по избрания проект ще бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="80c64-149">Стойността **Не** показва, че разходите няма да бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="80c64-150">Стойността **Да** показва, че разходите ще бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="80c64-151">Стойността на това поле се копира върху реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="80c64-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="80c64-152">Включване на такса</span><span class="sxs-lookup"><span data-stu-id="80c64-152">Include Fee</span></span> | <span data-ttu-id="80c64-153">Флагът **Да**/**Не** показва дали таксите за избрания проект ще бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="80c64-154">Стойността **Не** показва, че таксите няма да бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="80c64-155">Стойността **Да** показва, че таксите ще бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="80c64-156">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="80c64-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="80c64-157">Оферирана сума</span><span class="sxs-lookup"><span data-stu-id="80c64-157">Quoted Amount</span></span> | <span data-ttu-id="80c64-158">Това е сумата, която ще бъде предоставена на клиента за цялата работа, предвидена по този проект, базиран на котировъчен ред.</span><span class="sxs-lookup"><span data-stu-id="80c64-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="80c64-159">При оферта, създадена от възможност, тази стойност се копира от полето **Бюджет на клиента** на реда за възможности.</span><span class="sxs-lookup"><span data-stu-id="80c64-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="80c64-160">Когато проектната линия за оферти съдържа подробности за реда, това поле се заключва за редактиране и се обобщава от сумата в подробностите за реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="80c64-161">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="80c64-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="80c64-162">Изчислен данък</span><span class="sxs-lookup"><span data-stu-id="80c64-162">Estimated Tax</span></span> | <span data-ttu-id="80c64-163">Това е поле за редактиране, за да може потребителят да добави прогнозната сума на данъка в линията на офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="80c64-164">Когато проектната линия за оферти съдържа подробности за реда, това поле се заключва за редактиране и се обобщава от данъчната сума в подробностите за реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="80c64-165">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="80c64-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="80c64-166">Оферирана сума след данък</span><span class="sxs-lookup"><span data-stu-id="80c64-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="80c64-167">Това поле е сумата на котировъчния ред след данъци и е само за четене.</span><span class="sxs-lookup"><span data-stu-id="80c64-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="80c64-168">Сумата в това поле се изчислява като *Сума по оферта + данък*.</span><span class="sxs-lookup"><span data-stu-id="80c64-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="80c64-169">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="80c64-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="80c64-170">Ограничение, което да не се надвишава</span><span class="sxs-lookup"><span data-stu-id="80c64-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="80c64-171">Това поле може да се редактира и е достъпно само за проектни базирани реплики, които имат метод на фактуриране **Време и материал**.</span><span class="sxs-lookup"><span data-stu-id="80c64-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="80c64-172">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="80c64-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="80c64-173">Бюджет на клиента</span><span class="sxs-lookup"><span data-stu-id="80c64-173">Customer Budget</span></span> | <span data-ttu-id="80c64-174">Това поле може да се редактира и се копира от съответното поле на реда на възможност, ако офертата е била създадена от възможност.</span><span class="sxs-lookup"><span data-stu-id="80c64-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="80c64-175">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="80c64-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="80c64-176">Правила за валидиране на полета в раздела Общи на базирани на проекти редове за котировки</span><span class="sxs-lookup"><span data-stu-id="80c64-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="80c64-177">**Правило 1** : Ако полето **Включени задачи** е празно или ако е зададено на **Всички проектни задачи** , проект е включен в ред на оферта.</span><span class="sxs-lookup"><span data-stu-id="80c64-177">**Rule 1** : If the **Included Tasks** field is blank, or if it is set to **All project tasks** , a project is included in the quote line.</span></span>

<span data-ttu-id="80c64-178">**Правило 2** : Ако полето **Включени задачи** е празно или ако е зададено на **Всички проектни задачи** , проект и определен клас транзакции могат да бъдат включени само в един проект, базиран на ред на оферта за офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-178">**Rule 2** : If the **Included Tasks** field is blank, or if it is set to **All project tasks** , a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="80c64-179">**Правило 3** : Ако полето **Включени задачи** е зададено на **само за избраните задачи по проект** , проект и определен клас транзакции могат да бъдат включени в множество проекти, базиран на редове на оферта за офертата.</span><span class="sxs-lookup"><span data-stu-id="80c64-179">**Rule 3** : If the **Included Tasks** field is set to **Selected project tasks only** , a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="80c64-180">**Правило 4** : Ако дадена възможност има множество редове на оферта, може да има редове на оферта от различни оферти, които всички препращат към един и същ проект и включват един и същ клас транзакции.</span><span class="sxs-lookup"><span data-stu-id="80c64-180">**Rule 4** : If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="80c64-181">**Правило 5** : Ако кавичките не принадлежат към една и съща възможност, те не могат да включват един и същ проект и клас на транзакция.</span><span class="sxs-lookup"><span data-stu-id="80c64-181">**Rule 5** : If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="80c64-182">
                    <strong>Възможност</strong>
                </span><span class="sxs-lookup"><span data-stu-id="80c64-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="80c64-183">
                    <strong>Оферта</strong>
                </span><span class="sxs-lookup"><span data-stu-id="80c64-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="80c64-184">
                    <strong>Ред на оферта</strong>
                </span><span class="sxs-lookup"><span data-stu-id="80c64-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="80c64-185">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="80c64-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="80c64-186">
                    <strong>Включени задачи</strong>
                </span><span class="sxs-lookup"><span data-stu-id="80c64-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="80c64-187">
                    <strong>Включване на време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="80c64-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="80c64-188">
                    <strong>Включване на разход</strong>
                </span><span class="sxs-lookup"><span data-stu-id="80c64-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="80c64-189">
                    <strong>Включване</strong>
                </span><span class="sxs-lookup"><span data-stu-id="80c64-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="80c64-190">
                    <strong>Такса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="80c64-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="80c64-191">
                    <strong>Валидно/невалидно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="80c64-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="80c64-192">
                    <strong>Причина</strong>
                </span><span class="sxs-lookup"><span data-stu-id="80c64-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-193">O1</span><span class="sxs-lookup"><span data-stu-id="80c64-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-194">Трмс1</span><span class="sxs-lookup"><span data-stu-id="80c64-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-195">QL1</span><span class="sxs-lookup"><span data-stu-id="80c64-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-196">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-197">Празно</span><span class="sxs-lookup"><span data-stu-id="80c64-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-198">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-199">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-200">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="80c64-201">Невалидно</span><span class="sxs-lookup"><span data-stu-id="80c64-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="80c64-202">Нарушение на правило №2.</span><span class="sxs-lookup"><span data-stu-id="80c64-202">Violation of Rule #2.</span></span> <span data-ttu-id="80c64-203">Времето, разходите и таксите по проект P1 са включени в реда на оферта, QL1 и QL2.</span><span class="sxs-lookup"><span data-stu-id="80c64-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-204">O1</span><span class="sxs-lookup"><span data-stu-id="80c64-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-205">Трмс1</span><span class="sxs-lookup"><span data-stu-id="80c64-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-206">QL2</span><span class="sxs-lookup"><span data-stu-id="80c64-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-207">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-208">Празно</span><span class="sxs-lookup"><span data-stu-id="80c64-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-209">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-210">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-211">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-211">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-212">O1</span><span class="sxs-lookup"><span data-stu-id="80c64-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-213">Трмс1</span><span class="sxs-lookup"><span data-stu-id="80c64-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-214">QL1</span><span class="sxs-lookup"><span data-stu-id="80c64-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-215">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-216">Празно</span><span class="sxs-lookup"><span data-stu-id="80c64-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-217">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-218">No</span><span class="sxs-lookup"><span data-stu-id="80c64-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-219">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="80c64-220">Невалидно</span><span class="sxs-lookup"><span data-stu-id="80c64-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="80c64-221">Нарушение на правило №2.</span><span class="sxs-lookup"><span data-stu-id="80c64-221">Violation of Rule #2.</span></span> <span data-ttu-id="80c64-222">Времето и таксите по проект P1 са включени в редовете на оферта, QL1 и QL2.</span><span class="sxs-lookup"><span data-stu-id="80c64-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-223">O1</span><span class="sxs-lookup"><span data-stu-id="80c64-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-224">Трмс1</span><span class="sxs-lookup"><span data-stu-id="80c64-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-225">QL2</span><span class="sxs-lookup"><span data-stu-id="80c64-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-226">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-227">Празно</span><span class="sxs-lookup"><span data-stu-id="80c64-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-228">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-229">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-230">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-230">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-231">O1</span><span class="sxs-lookup"><span data-stu-id="80c64-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-232">Трмс1</span><span class="sxs-lookup"><span data-stu-id="80c64-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-233">QL1</span><span class="sxs-lookup"><span data-stu-id="80c64-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-234">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-235">Празно</span><span class="sxs-lookup"><span data-stu-id="80c64-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-236">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-237">No</span><span class="sxs-lookup"><span data-stu-id="80c64-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-238">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="80c64-239">Валидно</span><span class="sxs-lookup"><span data-stu-id="80c64-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="80c64-240">Времето и таксите за проект P1 са включени в QL1.</span><span class="sxs-lookup"><span data-stu-id="80c64-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="80c64-241">Разходите за проект P1 са включени в QL2.</span><span class="sxs-lookup"><span data-stu-id="80c64-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="80c64-242">Няма припокриване на това, което е включено на всеки ред на офертата и е валидно.</span><span class="sxs-lookup"><span data-stu-id="80c64-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-243">O1</span><span class="sxs-lookup"><span data-stu-id="80c64-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-244">Трмс1</span><span class="sxs-lookup"><span data-stu-id="80c64-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-245">QL2</span><span class="sxs-lookup"><span data-stu-id="80c64-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-246">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-247">Празно</span><span class="sxs-lookup"><span data-stu-id="80c64-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-248">No</span><span class="sxs-lookup"><span data-stu-id="80c64-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-249">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-250">No</span><span class="sxs-lookup"><span data-stu-id="80c64-250">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-251">O1</span><span class="sxs-lookup"><span data-stu-id="80c64-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-252">Трмс1</span><span class="sxs-lookup"><span data-stu-id="80c64-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-253">QL1</span><span class="sxs-lookup"><span data-stu-id="80c64-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-254">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-255">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="80c64-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-256">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-257">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-258">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="80c64-259">Невалидно</span><span class="sxs-lookup"><span data-stu-id="80c64-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="80c64-260">Нарушение на правило №2 по-горе</span><span class="sxs-lookup"><span data-stu-id="80c64-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="80c64-261">Q1 включва време, разходи и такси за подмножество от задачи по проект P1.</span><span class="sxs-lookup"><span data-stu-id="80c64-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="80c64-262">QL2 включва време, разходи и такси за целия проект P1 и се припокрива с това, което е включено в Q1.</span><span class="sxs-lookup"><span data-stu-id="80c64-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-263">O1</span><span class="sxs-lookup"><span data-stu-id="80c64-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-264">Трмс1</span><span class="sxs-lookup"><span data-stu-id="80c64-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-265">QL2</span><span class="sxs-lookup"><span data-stu-id="80c64-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-266">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-267">Празно</span><span class="sxs-lookup"><span data-stu-id="80c64-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-268">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-269">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-270">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-270">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-271">O1</span><span class="sxs-lookup"><span data-stu-id="80c64-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-272">Трмс1</span><span class="sxs-lookup"><span data-stu-id="80c64-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-273">QL1</span><span class="sxs-lookup"><span data-stu-id="80c64-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-274">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-275">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="80c64-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-276">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-277">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-278">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="80c64-279">Валидно</span><span class="sxs-lookup"><span data-stu-id="80c64-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="80c64-280">Съгласно правило №3 по-горе,</span><span class="sxs-lookup"><span data-stu-id="80c64-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="80c64-281">Q1 включва време, разходи и такси за подмножество от задачи по проект P1.</span><span class="sxs-lookup"><span data-stu-id="80c64-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="80c64-282">QL2 включва време, разходи и такси за подмножество от задачи по проект P1.</span><span class="sxs-lookup"><span data-stu-id="80c64-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="80c64-283">Единствената допълнителна проверка е около подмножеството от задачи на QL1, които са различни от подмножеството от задачи на QL2.</span><span class="sxs-lookup"><span data-stu-id="80c64-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="80c64-284">Това гарантира, че няма припокривания.</span><span class="sxs-lookup"><span data-stu-id="80c64-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="80c64-285">Това се прави от системата, когато са свързани задачи.</span><span class="sxs-lookup"><span data-stu-id="80c64-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-286">O1</span><span class="sxs-lookup"><span data-stu-id="80c64-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-287">Трмс1</span><span class="sxs-lookup"><span data-stu-id="80c64-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-288">QL2</span><span class="sxs-lookup"><span data-stu-id="80c64-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-289">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-290">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="80c64-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-291">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-292">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-293">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-293">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-294">O1</span><span class="sxs-lookup"><span data-stu-id="80c64-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-295">Трмс1</span><span class="sxs-lookup"><span data-stu-id="80c64-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-296">QL1</span><span class="sxs-lookup"><span data-stu-id="80c64-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-297">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-298">Всички задачи по проекта или празно</span><span class="sxs-lookup"><span data-stu-id="80c64-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-299">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-300">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-301">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="80c64-302">Валидно</span><span class="sxs-lookup"><span data-stu-id="80c64-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="80c64-303">Въз основа на правило # 5, Q1 и Q2 са две оферти за една и съща възможност, така че и двете могат да оценят за едни и същи компоненти на даден проект.</span><span class="sxs-lookup"><span data-stu-id="80c64-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-304">O1</span><span class="sxs-lookup"><span data-stu-id="80c64-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-305">Трмс2</span><span class="sxs-lookup"><span data-stu-id="80c64-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-306">QL1</span><span class="sxs-lookup"><span data-stu-id="80c64-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-307">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-308">Всички задачи по проекта или празно</span><span class="sxs-lookup"><span data-stu-id="80c64-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-309">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-310">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-311">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-311">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-312">O1</span><span class="sxs-lookup"><span data-stu-id="80c64-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-313">Трмс1</span><span class="sxs-lookup"><span data-stu-id="80c64-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-314">QL1</span><span class="sxs-lookup"><span data-stu-id="80c64-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-315">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-316">Всички задачи по проекта или празно</span><span class="sxs-lookup"><span data-stu-id="80c64-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-317">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-318">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-319">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="80c64-320">Валидно</span><span class="sxs-lookup"><span data-stu-id="80c64-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="80c64-321">Въз основа на правило # 4, Q1 и Q2 са две оферти на различни възможности, така че могат да оценят за едни и същи компоненти на един и същ проект.</span><span class="sxs-lookup"><span data-stu-id="80c64-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="80c64-322">O2</span><span class="sxs-lookup"><span data-stu-id="80c64-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="80c64-323">Трмс1</span><span class="sxs-lookup"><span data-stu-id="80c64-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-324">QL1</span><span class="sxs-lookup"><span data-stu-id="80c64-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-325">П1</span><span class="sxs-lookup"><span data-stu-id="80c64-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="80c64-326">Всички задачи по проекта или празно</span><span class="sxs-lookup"><span data-stu-id="80c64-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-327">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="80c64-328">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="80c64-329">Да</span><span class="sxs-lookup"><span data-stu-id="80c64-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="80c64-330">Невалидно</span><span class="sxs-lookup"><span data-stu-id="80c64-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

