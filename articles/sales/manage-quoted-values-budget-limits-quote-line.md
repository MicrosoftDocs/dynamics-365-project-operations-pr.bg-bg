---
title: Общ преглед на редове на оферта по проект
description: Тази тема предоставя информация за това как да използвате редове на оферта по проект за работа по проект.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: fa48a90c275eae1b0c0dbce685ae718dd9674c88
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858010"
---
# <a name="project-quote-lines-overview"></a><span data-ttu-id="bd4e8-103">Общ преглед на редове на оферта по проект</span><span class="sxs-lookup"><span data-stu-id="bd4e8-103">Project quote lines overview</span></span>

<span data-ttu-id="bd4e8-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="bd4e8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="bd4e8-105">Котировъчните редове, базирани на проекти, са предназначени да помогнат да се оцени работата по проекта по ангажимент.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="bd4e8-106">Структурата на проектна линия на оферти се разширява за проектни оценки със следните концепции:</span><span class="sxs-lookup"><span data-stu-id="bd4e8-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="bd4e8-107">Метод на фактуриране</span><span class="sxs-lookup"><span data-stu-id="bd4e8-107">Billing Method</span></span>
- <span data-ttu-id="bd4e8-108">Проектиране на проекти</span><span class="sxs-lookup"><span data-stu-id="bd4e8-108">Project Mapping</span></span>
- <span data-ttu-id="bd4e8-109">Включени класове за транзакции</span><span class="sxs-lookup"><span data-stu-id="bd4e8-109">Included Transaction classes</span></span>
- <span data-ttu-id="bd4e8-110">Ограничение, което да не се надвишава</span><span class="sxs-lookup"><span data-stu-id="bd4e8-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="bd4e8-111">Настройка на платимост</span><span class="sxs-lookup"><span data-stu-id="bd4e8-111">Chargeability setup</span></span>
- <span data-ttu-id="bd4e8-112">Оценка с помощта на подробности за цитираната линия</span><span class="sxs-lookup"><span data-stu-id="bd4e8-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="bd4e8-113">Клиенти от ред на оферта</span><span class="sxs-lookup"><span data-stu-id="bd4e8-113">Quote line Customers</span></span>

<span data-ttu-id="bd4e8-114">Следващата таблица предоставя информация за полетата на раздела **Общи** на котирана линия, базирана на проекти.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="bd4e8-115">Тези полета помагат да се създаде основата за подробна, обоснована оценка на работата по проекта.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="bd4e8-116">**Поле**</span><span class="sxs-lookup"><span data-stu-id="bd4e8-116">**Field**</span></span> | <span data-ttu-id="bd4e8-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd4e8-117">**Description**</span></span> | <span data-ttu-id="bd4e8-118">**Въздействие надолу по течението**</span><span class="sxs-lookup"><span data-stu-id="bd4e8-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="bd4e8-119">Име</span><span class="sxs-lookup"><span data-stu-id="bd4e8-119">Name</span></span> | <span data-ttu-id="bd4e8-120">Името на котировката, която трябва да ви помогне да идентифицирате отделния компонент на котировката, която се оценява.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-120">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="bd4e8-121">Копира се в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bd4e8-122">Метод на фактуриране</span><span class="sxs-lookup"><span data-stu-id="bd4e8-122">Billing Method</span></span> | <span data-ttu-id="bd4e8-123">При оферта, създадена от възможност, тази стойност се копира от съответното поле на реда за възможности.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="bd4e8-124">Това поле включва двата основни модела за договаряне, поддържани от Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="bd4e8-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="bd4e8-125">- Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="bd4e8-125">- Fixed price</span></span></br><span data-ttu-id="bd4e8-126">- Време и материали.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-126">- Time and material.</span></span>| <span data-ttu-id="bd4e8-127">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-127">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bd4e8-128">Project</span><span class="sxs-lookup"><span data-stu-id="bd4e8-128">Project</span></span> | <span data-ttu-id="bd4e8-129">Използвайте това незадължително поле, за да идентифицирате проекта, който ще бъде използван за изпълнение на работата по този ангажимент.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="bd4e8-130">Когато даден проект се картографира в котировъчен ред, това помага при настройването на таксувани задачи, а също и при въвеждането на прогнозна оценка, базирана на проекта, в линията на котировката като подробности за цитатната линия.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="bd4e8-131">Когато даден проект не е съпоставен с проектна линия на котировка, оценката трябва да бъде създадена ръчно чрез създаване на всеки детайл на котировката.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="bd4e8-132">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-132">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bd4e8-133">Включване на време</span><span class="sxs-lookup"><span data-stu-id="bd4e8-133">Include Time</span></span> | <span data-ttu-id="bd4e8-134">Флагът **Да**/**Не** показва дали транзакциите във времето или разходите за труд по избрания проект ще бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-134">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="bd4e8-135">Стойността **Не** показва, че транзакциите за времето или разходите за труд няма да бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-135">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="bd4e8-136">Стойността **Да** показва, че транзакциите за времето или разходите за труд ще да бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-136">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="bd4e8-137">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-137">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bd4e8-138">Включване на разход</span><span class="sxs-lookup"><span data-stu-id="bd4e8-138">Include Expense</span></span> | <span data-ttu-id="bd4e8-139">Флагът **Да**/**Не** показва дали разходите по избрания проект ще бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-139">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="bd4e8-140">Стойността **Не** показва, че разходите няма да бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-140">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="bd4e8-141">Стойността **Да** показва, че разходите ще бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-141">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="bd4e8-142">Стойността на това поле се копира върху реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-142">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bd4e8-143">Включване на такса</span><span class="sxs-lookup"><span data-stu-id="bd4e8-143">Include Fee</span></span> | <span data-ttu-id="bd4e8-144">Флагът **Да**/**Не** показва дали таксите за избрания проект ще бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-144">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="bd4e8-145">Стойността **Не** показва, че таксите няма да бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-145">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="bd4e8-146">Стойността **Да** показва, че таксите ще бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-146">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="bd4e8-147">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-147">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bd4e8-148">Оферирана сума</span><span class="sxs-lookup"><span data-stu-id="bd4e8-148">Quoted Amount</span></span> | <span data-ttu-id="bd4e8-149">Това е сумата, която ще бъде предоставена на клиента за цялата работа, предвидена по този проект, базиран на котировъчен ред.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-149">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="bd4e8-150">При оферта, създадена от възможност, тази стойност се копира от полето **Бюджет на клиента** на реда за възможности.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-150">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="bd4e8-151">Когато проектната линия за оферти съдържа подробности за реда, това поле се заключва за редактиране и се обобщава от сумата в подробностите за реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-151">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="bd4e8-152">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-152">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bd4e8-153">Изчислен данък</span><span class="sxs-lookup"><span data-stu-id="bd4e8-153">Estimated Tax</span></span> | <span data-ttu-id="bd4e8-154">Това е поле за редактиране, за да може потребителят да добави прогнозната сума на данъка в линията на офертата.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-154">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="bd4e8-155">Когато проектната линия за оферти съдържа подробности за реда, това поле се заключва за редактиране и се обобщава от данъчната сума в подробностите за реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-155">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="bd4e8-156">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-156">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bd4e8-157">Оферирана сума след данък</span><span class="sxs-lookup"><span data-stu-id="bd4e8-157">Quoted Amount after Tax</span></span> | <span data-ttu-id="bd4e8-158">Това поле е сумата на котировъчния ред след данъци и е само за четене.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-158">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="bd4e8-159">Сумата в това поле се изчислява като *Сума по оферта + данък*.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-159">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="bd4e8-160">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-160">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bd4e8-161">Ограничение, което да не се надвишава</span><span class="sxs-lookup"><span data-stu-id="bd4e8-161">Not-to-exceed Limit</span></span> | <span data-ttu-id="bd4e8-162">Това поле може да се редактира и е достъпно само за проектни базирани реплики, които имат метод на фактуриране **Време и материал**.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-162">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="bd4e8-163">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-163">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="bd4e8-164">Бюджет на клиента</span><span class="sxs-lookup"><span data-stu-id="bd4e8-164">Customer Budget</span></span> | <span data-ttu-id="bd4e8-165">Това поле може да се редактира и се копира от съответното поле на реда на възможност, ако офертата е била създадена от възможност.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-165">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="bd4e8-166">Стойността на това поле се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-166">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="bd4e8-167">Правила за валидиране на полета в раздела Общи на базирани на проекти редове за котировки</span><span class="sxs-lookup"><span data-stu-id="bd4e8-167">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="bd4e8-168">**Правило 1**: Определен клас транзакции за избрания проект може да бъде включен само в един проект, базиран на котировъчен ред на оферта.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-168">**Rule 1**: A certain transaction class on the selected project can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="bd4e8-169">**Правило 2**: Ако дадена възможност има множество редове на оферта, може да има редове на оферта от различни оферти, които всички препращат към един и същ проект и включват един и същ клас транзакции.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-169">**Rule 2**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="bd4e8-170">**Правило 3**: Ако кавичките не принадлежат към една и съща възможност, те не могат да включват един и същ проект и клас на транзакция.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-170">**Rule 3**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="1" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="bd4e8-171">
                    <strong>Възможност</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bd4e8-171">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="bd4e8-172">
                    <strong>Оферта</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bd4e8-172">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="bd4e8-173">
                    <strong>Ред на оферта</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bd4e8-173">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="bd4e8-174">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bd4e8-174">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="bd4e8-175">
                    <strong>Включване на време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bd4e8-175">
                    <strong>Include time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="bd4e8-176">
                    <strong>Включване на разход</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bd4e8-176">
                    <strong>Include expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="bd4e8-177">
                    <strong>Включване</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bd4e8-177">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="bd4e8-178">
                    <strong>такса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bd4e8-178">
                    <strong>fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="bd4e8-179">
                    <strong>Валидно/невалидно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bd4e8-179">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="bd4e8-180">
                    <strong>Причина</strong>
                </span><span class="sxs-lookup"><span data-stu-id="bd4e8-180">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bd4e8-181">O1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-181">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bd4e8-182">Трмс1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-182">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-183">QL1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-183">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-184">П1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-184">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-185">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-185">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-186">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-186">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-187">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-187">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bd4e8-188">Невалидно</span><span class="sxs-lookup"><span data-stu-id="bd4e8-188">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bd4e8-189">Нарушение на правило №1.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-189">Violation of Rule #1.</span></span> <span data-ttu-id="bd4e8-190">Времето, разходите и таксите по проект P1 са включени в двата котировъчни реда, QL1 и QL2.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-190">Time, Expense, and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bd4e8-191">O1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-191">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bd4e8-192">Трмс1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-192">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-193">QL2</span><span class="sxs-lookup"><span data-stu-id="bd4e8-193">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-194">П1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-194">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-195">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-195">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-196">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-196">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-197">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-197">Yes</span></span> </p>
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
<span data-ttu-id="bd4e8-198">O1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-198">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bd4e8-199">Трмс1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-199">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-200">QL1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-200">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-201">П1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-201">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-202">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-202">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-203">No</span><span class="sxs-lookup"><span data-stu-id="bd4e8-203">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-204">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-204">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bd4e8-205">Невалидно</span><span class="sxs-lookup"><span data-stu-id="bd4e8-205">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bd4e8-206">Нарушение на правило №1.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-206">Violation of Rule #1.</span></span> <span data-ttu-id="bd4e8-207">Времето и таксите по проект P1 са включени в двата котировъчни реда, QL1 и QL2.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-207">Time and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bd4e8-208">O1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-208">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bd4e8-209">Трмс1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-209">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-210">QL2</span><span class="sxs-lookup"><span data-stu-id="bd4e8-210">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-211">П1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-211">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-212">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-212">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-213">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-213">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-214">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-214">Yes</span></span> </p>
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
<span data-ttu-id="bd4e8-215">O1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-215">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bd4e8-216">Трмс1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-216">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-217">QL1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-217">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-218">П1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-218">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-219">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-219">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-220">No</span><span class="sxs-lookup"><span data-stu-id="bd4e8-220">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-221">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-221">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bd4e8-222">Валидно</span><span class="sxs-lookup"><span data-stu-id="bd4e8-222">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                 <p>
<span data-ttu-id="bd4e8-223">Времето и таксите за проект P1 са включени в QL1.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-223">Time and fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="bd4e8-224">Разходите за проект P1 са включени в QL2.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-224">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="bd4e8-225">Няма припокриване на това, което е включено на всеки ред на офертата, така че е валидно.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-225">There is no overlap in what is being included on each quote line so it is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bd4e8-226">O1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-226">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bd4e8-227">Трмс1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-227">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-228">QL2</span><span class="sxs-lookup"><span data-stu-id="bd4e8-228">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-229">П1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-229">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-230">No</span><span class="sxs-lookup"><span data-stu-id="bd4e8-230">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-231">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-231">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-232">No</span><span class="sxs-lookup"><span data-stu-id="bd4e8-232">No</span></span> </p>
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
<span data-ttu-id="bd4e8-233">O1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-233">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bd4e8-234">Трмс1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-234">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-235">QL1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-235">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-236">П1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-236">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-237">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-237">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-238">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-238">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-239">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-239">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bd4e8-240">Невалидно</span><span class="sxs-lookup"><span data-stu-id="bd4e8-240">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bd4e8-241">Нарушение на правило №1 по-горе</span><span class="sxs-lookup"><span data-stu-id="bd4e8-241">Violation of Rule #1 above</span></span> </p>
                <p>
<span data-ttu-id="bd4e8-242">Q1 включва време, разходи и такси за целия проект P1.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-242">Q1 includes Time, Expenses, and Fees for the whole project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="bd4e8-243">QL2 включва време, разходи и такси за целия проект P1 и се припокрива с това, което е включено в Q1.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-243">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bd4e8-244">O1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-244">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bd4e8-245">Трмс1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-245">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-246">QL2</span><span class="sxs-lookup"><span data-stu-id="bd4e8-246">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-247">П1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-247">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-248">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-248">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-249">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-250">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-250">Yes</span></span> </p>
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
<span data-ttu-id="bd4e8-251">O1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bd4e8-252">Трмс1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-253">QL1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-254">П1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-254">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-255">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-255">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-256">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-257">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-257">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="bd4e8-258">Валидно</span><span class="sxs-lookup"><span data-stu-id="bd4e8-258">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bd4e8-259">Въз основа на правило # 2, Q1 и Q2 са две оферти за една и съща възможност, така че и двете могат да оценят за едни и същи компоненти на даден проект.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-259">Based on Rule #2, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bd4e8-260">O1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-260">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bd4e8-261">Трмс2</span><span class="sxs-lookup"><span data-stu-id="bd4e8-261">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-262">QL1 на Q2</span><span class="sxs-lookup"><span data-stu-id="bd4e8-262">QL1 on Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-263">П1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-263">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-264">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-264">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-265">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-266">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-266">Yes</span></span> </p>
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
<span data-ttu-id="bd4e8-267">O1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-267">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bd4e8-268">Трмс1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-268">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-269">QL1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-269">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-270">П1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-270">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-271">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-271">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-272">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-272">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-273">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-273">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="bd4e8-274">Валидно</span><span class="sxs-lookup"><span data-stu-id="bd4e8-274">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="bd4e8-275">Въз основа на правило # 3, Q1 и Q2 са две оферти на различни възможности, така че могат да оценят за едни и същи компоненти на един и същ проект.</span><span class="sxs-lookup"><span data-stu-id="bd4e8-275">Based on Rule #3, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="bd4e8-276">O2</span><span class="sxs-lookup"><span data-stu-id="bd4e8-276">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="bd4e8-277">Трмс1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-277">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-278">QL1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-278">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-279">П1</span><span class="sxs-lookup"><span data-stu-id="bd4e8-279">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-280">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-280">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="bd4e8-281">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-281">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="bd4e8-282">Да</span><span class="sxs-lookup"><span data-stu-id="bd4e8-282">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="bd4e8-283">Невалидно</span><span class="sxs-lookup"><span data-stu-id="bd4e8-283">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../includes/footer-banner.md)]
