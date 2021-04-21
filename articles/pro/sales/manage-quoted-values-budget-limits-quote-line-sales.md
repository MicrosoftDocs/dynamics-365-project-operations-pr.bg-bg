---
title: Общ преглед на базирани на проект редове на оферта
description: Тази тема предоставя информация за използването на проектни базирани реплики за проектна работа.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: cfe98fc89130c93dd0a36af8583881fdcb4550c0
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858685"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="7f3e6-103">Общ преглед на базирани на проект редове на оферта</span><span class="sxs-lookup"><span data-stu-id="7f3e6-103">Project-based quote lines overview</span></span> 

<span data-ttu-id="7f3e6-104">_**Отнася се за:** Олекотено внедряване – сделка към проформа фактуриране, Project Operations за сценарии, базирани на ресурси / без складови наличности_</span><span class="sxs-lookup"><span data-stu-id="7f3e6-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="7f3e6-105">Котировъчните редове, базирани на проекти, са предназначени да помогнат да се оцени работата по проекта по ангажимент.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="7f3e6-106">Структурата на проектна линия на оферти се разширява за проектни оценки със следните концепции:</span><span class="sxs-lookup"><span data-stu-id="7f3e6-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="7f3e6-107">Метод на фактуриране</span><span class="sxs-lookup"><span data-stu-id="7f3e6-107">Billing Method</span></span>
- <span data-ttu-id="7f3e6-108">Съпоставяне на проект и задача</span><span class="sxs-lookup"><span data-stu-id="7f3e6-108">Project and Task Mapping</span></span>
- <span data-ttu-id="7f3e6-109">Включени класове за транзакции</span><span class="sxs-lookup"><span data-stu-id="7f3e6-109">Included Transaction classes</span></span>
- <span data-ttu-id="7f3e6-110">Ограничение, което да не се надвишава</span><span class="sxs-lookup"><span data-stu-id="7f3e6-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="7f3e6-111">Настройка на платимост</span><span class="sxs-lookup"><span data-stu-id="7f3e6-111">Chargeability setup</span></span>
- <span data-ttu-id="7f3e6-112">Оценка с помощта на подробности за цитираната линия</span><span class="sxs-lookup"><span data-stu-id="7f3e6-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="7f3e6-113">Клиенти от ред на оферта</span><span class="sxs-lookup"><span data-stu-id="7f3e6-113">Quote line Customers</span></span>

<span data-ttu-id="7f3e6-114">Следващата таблица предоставя информация за полетата на раздела **Общи** на котирана линия, базирана на проекти.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="7f3e6-115">Тези полета помагат да се създаде основата за подробна, обоснована оценка на работата по проекта.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="7f3e6-116">**Поле**</span><span class="sxs-lookup"><span data-stu-id="7f3e6-116">**Field**</span></span> | <span data-ttu-id="7f3e6-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7f3e6-117">**Description**</span></span> | <span data-ttu-id="7f3e6-118">**Въздействие надолу по течението**</span><span class="sxs-lookup"><span data-stu-id="7f3e6-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="7f3e6-119">Име</span><span class="sxs-lookup"><span data-stu-id="7f3e6-119">Name</span></span> | <span data-ttu-id="7f3e6-120">Името на реда на офертата, който ви помага да идентифицирате отделния компонент на офертата, която се оценява.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-120">The name of quote line that helps you to identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="7f3e6-121">Копира се в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="7f3e6-122">Метод на фактуриране</span><span class="sxs-lookup"><span data-stu-id="7f3e6-122">Billing Method</span></span> | <span data-ttu-id="7f3e6-123">При оферта, създадена от възможност, тази стойност се копира от съответното поле на реда за възможности.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="7f3e6-124">Това поле включва двата основни модела за договаряне, поддържани от Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="7f3e6-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="7f3e6-125">- Фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="7f3e6-125">- Fixed price</span></span></br><span data-ttu-id="7f3e6-126">- Време и материали.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-126">- Time and material.</span></span>| <span data-ttu-id="7f3e6-127">Тази стойност се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-127">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="7f3e6-128">Project</span><span class="sxs-lookup"><span data-stu-id="7f3e6-128">Project</span></span> | <span data-ttu-id="7f3e6-129">Използвайте това незадължително поле, за да идентифицирате проекта, който ще бъде използван за изпълнение на работата по този ангажимент.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="7f3e6-130">Когато даден проект се картографира в котировъчен ред, това помага при настройването на таксувани задачи, а също и при въвеждането на прогнозна оценка, базирана на проекта, в линията на котировката като подробности за цитатната линия.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="7f3e6-131">Когато даден проект не е съпоставен с проектна линия на котировка, оценката трябва да бъде създадена ръчно чрез създаване на всеки детайл на котировката.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="7f3e6-132">Тази стойност се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-132">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="7f3e6-133">Включени задачи</span><span class="sxs-lookup"><span data-stu-id="7f3e6-133">Included Tasks</span></span> | <span data-ttu-id="7f3e6-134">Показва дали този ред с редове на оферта се използва за всички или някои от проектните задачи за избрания проект.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-134">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="7f3e6-135">Това поле има следните възможни стойности:</span><span class="sxs-lookup"><span data-stu-id="7f3e6-135">This field has the following possible values:</span></span></br><span data-ttu-id="7f3e6-136">- Всички задачи по проекта</span><span class="sxs-lookup"><span data-stu-id="7f3e6-136">- All project tasks</span></span></br><span data-ttu-id="7f3e6-137">- Само избрани задачи по проекта</span><span class="sxs-lookup"><span data-stu-id="7f3e6-137">- Selected project tasks only</span></span></br><span data-ttu-id="7f3e6-138">Празна стойност в това поле е еквивалентна на опцията **Всички проектни задачи**.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-138">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="7f3e6-139">Когато **Само избрани проектни задачи** е избрано на страницата на проекта, разделът **Настройка на фактурирането на задачата** ви позволява да изберете конкретни задачи, за да ги свържете с този ред на офертите.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-139">When **Selected project tasks only** is selected on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="7f3e6-140">Тази стойност се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-140">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="7f3e6-141">Включване на време</span><span class="sxs-lookup"><span data-stu-id="7f3e6-141">Include Time</span></span> | <span data-ttu-id="7f3e6-142">Стойност **Да**/**Не** показва дали транзакциите във времето или разходите за труд по избрания проект ще бъдат включени в оценката на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-142">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="7f3e6-143">Стойността **Не** показва, че транзакциите за времето или разходите за труд няма да бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-143">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="7f3e6-144">Стойността **Да** показва, че транзакциите за времето или разходите за труд ще да бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-144">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="7f3e6-145">Тази стойност се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-145">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="7f3e6-146">Включване на разход</span><span class="sxs-lookup"><span data-stu-id="7f3e6-146">Include Expense</span></span> | <span data-ttu-id="7f3e6-147">Стойност **Да**/**Не** показва дали разходите за избрания проект ще бъдат включени в оценката на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-147">A **Yes**/**No** value indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="7f3e6-148">Стойността **Не** показва, че разходите няма да бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-148">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="7f3e6-149">Стойността **Да** показва, че разходите ще бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-149">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="7f3e6-150">Тази стойност се копира върху реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-150">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="7f3e6-151">Включване на материал</span><span class="sxs-lookup"><span data-stu-id="7f3e6-151">Include Material</span></span> | <span data-ttu-id="7f3e6-152">Стойност **Да**/**Не** показва дали разходите за материали за избрания проект ще бъдат включени в оценката на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-152">A **Yes**/**No** value indicates if material costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="7f3e6-153">Стойност **Не** показва дали разходите за материали няма да бъдат включени в оценката на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-153">A **No** value indicates that the material costs will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="7f3e6-154">Стойност **Да** показва дали разходите за материали ще бъдат включени в оценката на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-154">A **Yes** value indicates that the material costs will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="7f3e6-155">Тази стойност се копира върху реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-155">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="7f3e6-156">Включване на такса</span><span class="sxs-lookup"><span data-stu-id="7f3e6-156">Include Fee</span></span> | <span data-ttu-id="7f3e6-157">Стойност **Да**/**Не** показва дали таксите за избрания проект ще бъдат включени в оценката на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-157">A **Yes**/**No** value indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="7f3e6-158">Стойността **Не** показва, че таксите няма да бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-158">A **No** value indicates that the fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="7f3e6-159">Стойността **Да** показва, че таксите ще бъдат включени в прогнозата на този ред на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-159">A **Yes** value indicates that the fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="7f3e6-160">Тази стойност се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-160">This value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="7f3e6-161">Оферирана сума</span><span class="sxs-lookup"><span data-stu-id="7f3e6-161">Quoted Amount</span></span> | <span data-ttu-id="7f3e6-162">Това е сумата, която ще бъде цитирана на клиента за цялата работа, прогнозирана по този проект, базиран на котировъчен ред.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-162">This is the amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="7f3e6-163">При оферта, създадена от възможност, тази стойност се копира от полето **Бюджет на клиента** на реда за възможности.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-163">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="7f3e6-164">Когато проектната линия за оферти съдържа подробности за реда, това поле се заключва за редактиране и се обобщава от сумата в подробностите за реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-164">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="7f3e6-165">Тази стойност се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-165">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="7f3e6-166">Изчислен данък</span><span class="sxs-lookup"><span data-stu-id="7f3e6-166">Estimated Tax</span></span> | <span data-ttu-id="7f3e6-167">Това е поле за редактиране, за да може потребителят да добави прогнозната сума на данъка в линията на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-167">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="7f3e6-168">Когато проектната линия за оферти съдържа подробности за реда, това поле се заключва за редактиране и се обобщава от данъчната сума в подробностите за реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-168">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="7f3e6-169">Тази стойност се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-169">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="7f3e6-170">Оферирана сума след данък</span><span class="sxs-lookup"><span data-stu-id="7f3e6-170">Quoted Amount after Tax</span></span> | <span data-ttu-id="7f3e6-171">Това поле е сумата на котировъчния ред след данъци и е само за четене.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-171">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="7f3e6-172">Сумата в това поле се изчислява като *Сума по оферта + данък*.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-172">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="7f3e6-173">Тази стойност се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-173">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="7f3e6-174">Ограничение, което да не се надвишава</span><span class="sxs-lookup"><span data-stu-id="7f3e6-174">Not-to-exceed Limit</span></span> | <span data-ttu-id="7f3e6-175">Това поле може да се редактира и е достъпно само за проектни базирани реплики, които имат метод на фактуриране **Време и материал**.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-175">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="7f3e6-176">Тази стойност се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-176">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="7f3e6-177">Бюджет на клиента</span><span class="sxs-lookup"><span data-stu-id="7f3e6-177">Customer Budget</span></span> | <span data-ttu-id="7f3e6-178">Това поле може да се редактира и се копира от съответното поле на реда на възможност, ако офертата е била създадена от възможност.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-178">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="7f3e6-179">Тази стойност се копира в реда на договор за проект, който се създава от този ред на офертата, когато офертата е спечелена.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-179">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="7f3e6-180">Правила за валидиране на полета в раздела Общи на базирани на проекти редове за котировки</span><span class="sxs-lookup"><span data-stu-id="7f3e6-180">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="7f3e6-181">**Правило 1**: Ако полето **Включени задачи** е празно или ако е зададено на **Всички проектни задачи**, проект е включен в ред на оферта.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-181">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="7f3e6-182">**Правило 2**: Ако полето **Включени задачи** е празно или ако е зададено на **Всички проектни задачи**, проект и определен клас транзакции могат да бъдат включени само в един проект, базиран на ред на оферта за офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-182">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="7f3e6-183">**Правило 3**: Ако полето **Включени задачи** е зададено на **само за избраните задачи по проект**, проект и определен клас транзакции могат да бъдат включени в множество проекти, базиран на редове на оферта за офертата.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-183">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="7f3e6-184">**Правило 4**: Ако дадена възможност има множество редове на оферта, може да има редове на оферта от различни оферти, които всички препращат към един и същ проект и включват един и същ клас транзакции.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-184">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="7f3e6-185">**Правило 5**: Ако кавичките не принадлежат към една и съща възможност, те не могат да включват един и същ проект и клас на транзакция.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-185">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p><span data-ttu-id="7f3e6-186">
                    <strong>Възможност</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f3e6-186">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="39" valign="top">
                <p><span data-ttu-id="7f3e6-187">
                    <strong>Оферта</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f3e6-187">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="40" valign="top">
                <p><span data-ttu-id="7f3e6-188">
                    <strong>Ред на оферта</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f3e6-188">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="7f3e6-189">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f3e6-189">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="77" valign="top">
                <p><span data-ttu-id="7f3e6-190">
                    <strong>Включени задачи</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f3e6-190">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="45" valign="top">
                <p><span data-ttu-id="7f3e6-191">
                    <strong>Включване на време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f3e6-191">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="46" valign="top">
                <p><span data-ttu-id="7f3e6-192">
                    <strong>Включване на разход</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f3e6-192">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="43" valign="top">
                <p><span data-ttu-id="7f3e6-193">
                    <strong>Включване на материал</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f3e6-193">
                    <strong>Include Material</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="7f3e6-194">
                    <strong>Включване</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f3e6-194">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="7f3e6-195">
                    <strong>Такса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f3e6-195">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="49" valign="top">
                <p><span data-ttu-id="7f3e6-196">
                    <strong>Валидно/невалидно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f3e6-196">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="200" valign="top">
                <p><span data-ttu-id="7f3e6-197">
                    <strong>Причина</strong>
                </span><span class="sxs-lookup"><span data-stu-id="7f3e6-197">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-198">O1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-198">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-199">Трмс1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-199">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-200">QL1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-200">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-201">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-201">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-202">Празно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-202">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-203">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-203">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-204">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-204">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-205">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-205">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-206">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-206">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-207">Невалидно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-207">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-208">Нарушение на правило №2.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-208">Violation of Rule #2.</span></span> <span data-ttu-id="7f3e6-209">Времето, разходите и таксите по проект P1 са включени в реда на оферта, QL1 и QL2</span><span class="sxs-lookup"><span data-stu-id="7f3e6-209">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-210">O1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-210">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-211">Трмс1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-211">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-212">QL2</span><span class="sxs-lookup"><span data-stu-id="7f3e6-212">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-213">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-213">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-214">Празно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-214">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-215">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-215">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-216">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-216">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-217">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-217">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-218">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-218">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-219">O1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-219">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-220">Трмс1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-220">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-221">QL1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-221">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-222">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-222">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-223">Празно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-223">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-224">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-224">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-225">No</span><span class="sxs-lookup"><span data-stu-id="7f3e6-225">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-226">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-226">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-227">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-227">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-228">Невалидно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-228">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-229">Нарушение на правило №2.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-229">Violation of Rule #2.</span></span> <span data-ttu-id="7f3e6-230">Времето, материалите и таксите по проект P1 са включени в реда на оферта, QL1 и QL2</span><span class="sxs-lookup"><span data-stu-id="7f3e6-230">Time, Material, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-231">O1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-231">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-232">Трмс1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-232">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-233">QL2</span><span class="sxs-lookup"><span data-stu-id="7f3e6-233">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-234">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-234">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-235">Празно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-235">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-236">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-236">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-237">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-237">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-238">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-238">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-239">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-239">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-240">O1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-240">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-241">Трмс1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-241">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-242">QL1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-242">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-243">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-243">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-244">Празно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-244">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-245">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-245">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-246">No</span><span class="sxs-lookup"><span data-stu-id="7f3e6-246">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-247">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-247">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-248">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-248">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-249">Валидно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-249">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-250">Времето, материалите и таксите по проект P1 са включени в QL1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-250">Time, Material, and Fees on P1 project are included on QL1</span></span> <br>
<span data-ttu-id="7f3e6-251">Разходите за проект P1 са включени в QL2</span><span class="sxs-lookup"><span data-stu-id="7f3e6-251">Expense on P1 project is included on QL2</span></span> <br>
<span data-ttu-id="7f3e6-252">Няма припокриване на това, което е включено във всеки ред на офертата и следователно е валидно.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-252">No overlap in what is being included on each quote line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-253">O1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-253">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-254">Трмс1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-254">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-255">QL2</span><span class="sxs-lookup"><span data-stu-id="7f3e6-255">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-256">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-256">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-257">Празно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-257">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-258">No</span><span class="sxs-lookup"><span data-stu-id="7f3e6-258">No</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-259">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-259">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-260">No</span><span class="sxs-lookup"><span data-stu-id="7f3e6-260">No</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-261">No</span><span class="sxs-lookup"><span data-stu-id="7f3e6-261">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-262">O1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-262">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-263">Трмс1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-263">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-264">QL1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-264">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-265">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-265">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-266">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="7f3e6-266">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-267">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-267">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-268">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-268">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-269">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-269">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-270">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-270">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-271">Невалидно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-271">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-272">Нарушение на правило №2</span><span class="sxs-lookup"><span data-stu-id="7f3e6-272">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="7f3e6-273">Q1 включва време, материал, разходи и такси за подмножество от задачи по проект P1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-273">Q1 includes Time, Material, Expenses and Fees on a subset of tasks on project P1</span></span> </p>
                <p>
<span data-ttu-id="7f3e6-274">QL2 включва време, разходи и такси за целия проект P1 и следователно се припокрива с това, което е включено в Q1.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-274">QL2 includes Time, Expenses, and Fees for the whole project P1 and therefore overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-275">O1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-275">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-276">Трмс1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-276">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-277">QL2</span><span class="sxs-lookup"><span data-stu-id="7f3e6-277">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-278">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-278">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-279">Празно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-279">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-280">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-280">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-281">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-281">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-282">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-282">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-283">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-283">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-284">O1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-284">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-285">Трмс1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-285">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-286">QL1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-286">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-287">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-287">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-288">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="7f3e6-288">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-289">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-289">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-290">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-290">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-291">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-291">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-292">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-292">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-293">Валидно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-293">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-294">Съгласно правило №3,</span><span class="sxs-lookup"><span data-stu-id="7f3e6-294">Per Rule #3,</span></span> </p>
                <p>
<span data-ttu-id="7f3e6-295">Q1 включва време, материал, разходи и такси за подмножество от задачи по проект P1.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-295">Q1 includes Time, Material, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="7f3e6-296">QL2 включва време, материал, разходи и такси за подмножество от задачи по проект P1.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-296">QL2 includes Time, Material, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="7f3e6-297">Единствената допълнителна проверка е около подмножеството от задачи на QL1, което е различно от подмножеството от задачи на QL2, за да се гарантира, че няма припокриване.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-297">The only additional validation is around the subset of tasks on QL1 which is different from the subset of tasks on QL2 to ensure that there is no overlap.</span></span> <span data-ttu-id="7f3e6-298">Това се прави от системата, когато са свързани задачи.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-298">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-299">O1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-299">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-300">Трмс1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-300">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-301">QL2</span><span class="sxs-lookup"><span data-stu-id="7f3e6-301">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-302">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-302">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-303">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="7f3e6-303">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-304">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-304">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-305">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-305">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-306">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-306">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-307">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-307">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-308">O1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-308">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-309">Трмс1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-309">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-310">QL1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-310">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-311">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-311">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-312">Всички задачи по проекта или празно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-312">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-313">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-313">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-314">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-314">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-315">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-315">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-316">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-316">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-317">Валидно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-317">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-318">Съгласно правило №5, Q1 и Q2 са две кавички за една и съща възможност, така че и двете могат да оценят за едни и същи компоненти на даден проект.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-318">Per Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-319">O1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-319">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-320">Трмс2</span><span class="sxs-lookup"><span data-stu-id="7f3e6-320">Q2</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-321">QL1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-321">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-322">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-322">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-323">Всички задачи по проекта или празно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-323">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-324">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-324">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-325">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-325">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-326">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-326">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-327">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-327">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-328">O1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-328">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-329">Трмс1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-329">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-330">QL1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-330">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-331">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-331">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-332">Всички задачи по проекта или празно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-332">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-333">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-333">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-334">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-334">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-335">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-335">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-336">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-336">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-337">Невалидно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-337">Not Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="7f3e6-338">Съгласно правило №4, Q1 и Q2 са две оферти за различни възможности, така че не могат да оценят за едни и същи компоненти от един и същ проект.</span><span class="sxs-lookup"><span data-stu-id="7f3e6-338">Per Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="7f3e6-339">O2</span><span class="sxs-lookup"><span data-stu-id="7f3e6-339">O2</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="7f3e6-340">Трмс1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-340">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="7f3e6-341">QL1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-341">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-342">П1</span><span class="sxs-lookup"><span data-stu-id="7f3e6-342">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="7f3e6-343">Всички задачи по проекта или празно</span><span class="sxs-lookup"><span data-stu-id="7f3e6-343">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="7f3e6-344">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-344">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="7f3e6-345">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-345">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="7f3e6-346">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-346">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="7f3e6-347">Да</span><span class="sxs-lookup"><span data-stu-id="7f3e6-347">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
