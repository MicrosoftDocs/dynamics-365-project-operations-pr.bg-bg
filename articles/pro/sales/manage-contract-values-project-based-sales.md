---
title: Общ преглед на базирани на проект аспекти на договор
description: Тази тема предоставя информация за работа с базирани на продукт аспекти на договор.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 824fdd54d7b513b49afd1a6d76d3387df81418e2
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858145"
---
# <a name="project-based-contract-lines-overview"></a><span data-ttu-id="df520-103">Общ преглед на базирани на проект аспекти на договор</span><span class="sxs-lookup"><span data-stu-id="df520-103">Project-based contract lines overview</span></span>

<span data-ttu-id="df520-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="df520-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="df520-105">Базираните на проект аспекти на договор в Dynamics 365 Project Operations са проектирани да съхраняват прогнозите и споразуменията за фактуриране за конкретни компоненти на работата по проект за ангажимент.</span><span class="sxs-lookup"><span data-stu-id="df520-105">Project-based contract lines in Dynamics 365 Project Operations are designed to hold the estimate and billing agreements for specific components of project work on an engagement.</span></span> <span data-ttu-id="df520-106">Структурата на базираните на проект аспекти на договор е разширена за прогнозни оценки на проект и сценарии за фактуриране със следните концепции:</span><span class="sxs-lookup"><span data-stu-id="df520-106">The structure of a project–based contract line is extended for project estimates and billing scenarios with the following concepts:</span></span>

- <span data-ttu-id="df520-107">Метод на фактуриране</span><span class="sxs-lookup"><span data-stu-id="df520-107">Billing method</span></span>
- <span data-ttu-id="df520-108">Съпоставяне на проект и задача</span><span class="sxs-lookup"><span data-stu-id="df520-108">Project and task mapping</span></span>
- <span data-ttu-id="df520-109">Класове на включени трансакции</span><span class="sxs-lookup"><span data-stu-id="df520-109">Included transaction classes</span></span>
- <span data-ttu-id="df520-110">Ограничение, което да не се надвишава</span><span class="sxs-lookup"><span data-stu-id="df520-110">Not-to-exceed limit</span></span>
- <span data-ttu-id="df520-111">Настройка на платимост</span><span class="sxs-lookup"><span data-stu-id="df520-111">Chargeability setup</span></span>
- <span data-ttu-id="df520-112">Прогнозни оценки с помощта на подробности за аспекти на договор</span><span class="sxs-lookup"><span data-stu-id="df520-112">Estimates using contract line details</span></span>
- <span data-ttu-id="df520-113">Клиенти на аспекти на договор</span><span class="sxs-lookup"><span data-stu-id="df520-113">Contract line customers</span></span>

<span data-ttu-id="df520-114">Следващата таблица включва полетата в раздела **Общи** на базирани на проект аспекти на договор, които помагат да се създаде основата за подробна, основателна оценка и правилата за фактуриране за работа, базирана на проект.</span><span class="sxs-lookup"><span data-stu-id="df520-114">The following table includes the fields on the **General** tab of project–based contract lines that help set up the basis for a detailed, ground–up estimate and billing arrangements for project–based work.</span></span>

| <span data-ttu-id="df520-115">Поле</span><span class="sxs-lookup"><span data-stu-id="df520-115">Field</span></span> | <span data-ttu-id="df520-116">Описание</span><span class="sxs-lookup"><span data-stu-id="df520-116">Description</span></span> | <span data-ttu-id="df520-117">Въздействие надолу по течението</span><span class="sxs-lookup"><span data-stu-id="df520-117">Downstream impact</span></span> |
| --- | --- | --- |
| <span data-ttu-id="df520-118">**Име**</span><span class="sxs-lookup"><span data-stu-id="df520-118">**Name**</span></span> | <span data-ttu-id="df520-119">Име на аспектите на договор.</span><span class="sxs-lookup"><span data-stu-id="df520-119">Name of the contract line.</span></span> <span data-ttu-id="df520-120">То идентифицира отделния компонент на договора, който се оценява.</span><span class="sxs-lookup"><span data-stu-id="df520-120">This identifies the discrete component of the contract that is being estimated.</span></span> <span data-ttu-id="df520-121">За договор по проект, създаден от оферта, тази стойност се копира от съответната стойност на базирания на проект ред на оферта.</span><span class="sxs-lookup"><span data-stu-id="df520-121">For a project contract created from a quote, this value is copied from a corresponding value of the project-based quote line.</span></span> | <span data-ttu-id="df520-122">Името се копира в реда на фактурата по проекта, който се създава от тези аспекти на договор при създаването на фактурата.</span><span class="sxs-lookup"><span data-stu-id="df520-122">The name copied over to the project invoice line that is created from this contract line when the invoice is created.</span></span> |
| <span data-ttu-id="df520-123">**Метод на фактуриране**</span><span class="sxs-lookup"><span data-stu-id="df520-123">**Billing Method**</span></span> | <span data-ttu-id="df520-124">В договор по проект, създаден от оферта, тази стойност се копира от съответното поле в реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="df520-124">On a project contract created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="df520-125">Това е набор от опции, който представлява двата основни модела за договаряне, поддържани от Project Operations:</span><span class="sxs-lookup"><span data-stu-id="df520-125">This is an option set that represents the two main contracting models supported by Project Operations:</span></span></br><span data-ttu-id="df520-126">- **Фиксирана цена**</span><span class="sxs-lookup"><span data-stu-id="df520-126">- **Fixed Price**</span></span></br><span data-ttu-id="df520-127">- **Време и материал**</span><span class="sxs-lookup"><span data-stu-id="df520-127">- **Time and Material**</span></span> | <span data-ttu-id="df520-128">Въз основа на метода за фактуриране на посочените аспекти на договор, действителната трансакция ще бъде обработена.</span><span class="sxs-lookup"><span data-stu-id="df520-128">Based on the billing method of the referenced contract line, the actual transaction will be processed.</span></span> <span data-ttu-id="df520-129">Ако аспектите на договора, посочени от действителните данни, имат метод за фактуриране на време и материал, се създават записи на действителни данни за разходи и нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="df520-129">If the contract line referenced by the actual has a time and material billing method, cost and unbilled sales actual records are created.</span></span> <span data-ttu-id="df520-130">Ако аспектите на договора, посочени от действителните данни, имат метод за фактуриране по фиксирана цена, се създават само действителни данни за разход.</span><span class="sxs-lookup"><span data-stu-id="df520-130">If the contract line referenced by the actual has a fixed price billing method, only a cost actual is created.</span></span> |
| <span data-ttu-id="df520-131">**Project**</span><span class="sxs-lookup"><span data-stu-id="df520-131">**Project**</span></span> | <span data-ttu-id="df520-132">Използвайте това поле, за да идентифицирате проекта, който ще се използва за изпълнение на работата по този ангажимент.</span><span class="sxs-lookup"><span data-stu-id="df520-132">Use this field to identify the project that will be used to deliver the work on this engagement.</span></span> | <span data-ttu-id="df520-133">Тази стойност ще се използва заедно с **Включени задачи** и **Включени класове на транзакции** за разрешаване на референтната линия на договора върху действителен или прогнозен редовен запис.</span><span class="sxs-lookup"><span data-stu-id="df520-133">This value will be used in conjunction with **Included Tasks** and **Included Transaction Classes** to resolve the contract line reference on an actual or estimate line record.</span></span> |
| <span data-ttu-id="df520-134">**Включени задачи**</span><span class="sxs-lookup"><span data-stu-id="df520-134">**Included Tasks**</span></span> | <span data-ttu-id="df520-135">Показва дали тези аспекти на договор включват всички задачи по проекта за избрания проект, или само поднабор от задачите.</span><span class="sxs-lookup"><span data-stu-id="df520-135">Indicates if this contract line includes all project tasks for the selected project or only a subset of the tasks.</span></span> <span data-ttu-id="df520-136">Това е набор от опции, който има следните възможни стойности:</span><span class="sxs-lookup"><span data-stu-id="df520-136">This is an option set that has the following possible values:</span></span></br><span data-ttu-id="df520-137">- **Всички задачи от проекти**</span><span class="sxs-lookup"><span data-stu-id="df520-137">- **All Project Tasks**</span></span></br><span data-ttu-id="df520-138">- **Само избрани задачи по проекта**.</span><span class="sxs-lookup"><span data-stu-id="df520-138">- **Selected Project Tasks Only**.</span></span> <span data-ttu-id="df520-139">Празна стойност в това поле е равна на избор на **Всички задачи по проект**.</span><span class="sxs-lookup"><span data-stu-id="df520-139">A blank value in this field is equal to selecting **All Project Tasks**.</span></span> | <span data-ttu-id="df520-140">Ако е избрано **Само избрани задачи** може да изберете конкретни задачи и да ги свържете с тези аспекти на договор в раздела **Настройка на фактуриране на задача** на страницата **Проект**.</span><span class="sxs-lookup"><span data-stu-id="df520-140">If **Selected Tasks Only** is selected, you can select specific tasks and associate them to this contract line on the **Task Billing Setup** tab on the **Project** page.</span></span> <span data-ttu-id="df520-141">Стойността ще се използва заедно с **Проект** и класовете на **включените трансакции** за разрешаване на препратката на аспектите на договора в действителни данни или запис на ред на оценка.</span><span class="sxs-lookup"><span data-stu-id="df520-141">The value will be used in conjunction with **Project** and **Included Transaction** classes to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="df520-142">**Включване на време**</span><span class="sxs-lookup"><span data-stu-id="df520-142">**Include Time**</span></span> | <span data-ttu-id="df520-143">Стойност **Да**/**Не** показва дали транзакциите във времето или разходите за труд по избрания проект ще бъдат включени в тези аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="df520-143">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="df520-144">Стойност **Не** показва, че трансакциите „Време” или разходът за труд няма да се включат в тези аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="df520-144">A **No** value indicates that the time transactions or labor cost will not be included on this contract line.</span></span> <span data-ttu-id="df520-145">Стойност **Да** показва, че ще се включат.</span><span class="sxs-lookup"><span data-stu-id="df520-145">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="df520-146">Тази стойност се използва заедно с проекта за разрешаване на референтната линия на договора на действителен или запис на прогнозна линия.</span><span class="sxs-lookup"><span data-stu-id="df520-146">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="df520-147">**Включване на разход**</span><span class="sxs-lookup"><span data-stu-id="df520-147">**Include Expense**</span></span> | <span data-ttu-id="df520-148">Стойност **Да**/**Не** показва дали разходите за избрания проект ще бъдат включени в тези аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="df520-148">A **Yes**/**No** value indicates if expense costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="df520-149">Стойност **Не** показва, че размерът на разхода няма да се включи в тези аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="df520-149">A **No** value indicates that the expense cost will not be included on this contract line.</span></span> <span data-ttu-id="df520-150">Стойност **Да** показва, че ще се включи.</span><span class="sxs-lookup"><span data-stu-id="df520-150">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="df520-151">Тази стойност се използва заедно с проекта за разрешаване на референтната линия на договора на действителен или запис на прогнозна линия.</span><span class="sxs-lookup"><span data-stu-id="df520-151">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="df520-152">**Включване на материали**</span><span class="sxs-lookup"><span data-stu-id="df520-152">**Include Materials**</span></span> | <span data-ttu-id="df520-153">Стойност **Да**/**Не** показва дали разходите за материали за избрания проект ще бъдат включени в тези аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="df520-153">A **Yes**/**No** value indicates if material costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="df520-154">Стойност **Не** показва дали разходите за материали няма да бъдат включени в тези аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="df520-154">A **No** value indicates that the material costs will not be included on this contract line.</span></span> <span data-ttu-id="df520-155">Стойност **Да** показва, че ще се включи.</span><span class="sxs-lookup"><span data-stu-id="df520-155">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="df520-156">Тази стойност се използва заедно с проекта за разрешаване на референтната линия на договора на действителен или запис на прогнозна линия.</span><span class="sxs-lookup"><span data-stu-id="df520-156">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="df520-157">**Включване на такса**</span><span class="sxs-lookup"><span data-stu-id="df520-157">**Include Fee**</span></span> | <span data-ttu-id="df520-158">Стойност **Да**/**Не** показва дали таксите за избрания проект ще бъдат включени в тези аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="df520-158">A **Yes**/**No** value indicates if fees on the selected project will be included on this contract line.</span></span> <span data-ttu-id="df520-159">Стойност **Не** показва, че таксите няма да се включат в тези аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="df520-159">A **No** value indicates that the fees will not be included on this contract line.</span></span> <span data-ttu-id="df520-160">Стойност **Да** показва, че ще се включат.</span><span class="sxs-lookup"><span data-stu-id="df520-160">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="df520-161">Тази стойност се използва заедно с проекта за разрешаване на референтната линия на договора на действителен или запис на прогнозна линия.</span><span class="sxs-lookup"><span data-stu-id="df520-161">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="df520-162">**Договорена сума**</span><span class="sxs-lookup"><span data-stu-id="df520-162">**Contracted Amount**</span></span> | <span data-ttu-id="df520-163">В аспекти на договор с фиксирана цена тази стойност е договорената стойност, която ще се фактурира на клиента за всички компоненти на работата, свързани с тези аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="df520-163">On a fixed price contract line, this amount is the agreed-on value that will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="df520-164">В аспекти на договор за време и материал тази сума е прогнозната стойност на това, което ще се фактурира на клиента за всички компоненти на работата, свързани с тези аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="df520-164">On a time and material contract line, this amount is an estimated value of what will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="df520-165">В договор по проект, който е създаден от оферта, тази стойност се копира от съответното поле в реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="df520-165">On a project contract that is created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="df520-166">Когато базирани на проект аспекти на договор съдържат подробности за ред, това поле се заключва за редактиране и се обобщава от сумата в подробностите за аспектите на договора.</span><span class="sxs-lookup"><span data-stu-id="df520-166">When a project–based contract line has line details, this field is locked for editing and is summarized from the amount on the contract line details.</span></span> | <span data-ttu-id="df520-167">Когато аспектите на договора съдържат подробности за ред, тази стойност може да се променя чрез промяна на сумите в подробностите за реда.</span><span class="sxs-lookup"><span data-stu-id="df520-167">When the contract line has line details, this value can be modified by changing the amounts on the line details.</span></span> <span data-ttu-id="df520-168">В аспекти на договор с фиксирана цена тази стойност се използва за генериране на сумата преди данъците в контролните точки за периодично фактуриране.</span><span class="sxs-lookup"><span data-stu-id="df520-168">On a fixed price contract line, this value is used to generate the amount before tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="df520-169">**Изчислен данък**</span><span class="sxs-lookup"><span data-stu-id="df520-169">**Estimated Tax**</span></span> | <span data-ttu-id="df520-170">Потребителят може да редактира това поле, за да въведе прогнозната сума на данъка в аспектите на договора.</span><span class="sxs-lookup"><span data-stu-id="df520-170">The user can edit this field to input the estimated tax amount on the contract line.</span></span> <span data-ttu-id="df520-171">Когато базирани на проект аспекти на договор съдържат подробности за ред, това поле се заключва за редактиране и се обобщава от сумата на данъка в подробностите за аспектите на договора.</span><span class="sxs-lookup"><span data-stu-id="df520-171">When a project–based contract line has line details, this field is locked for editing and is summarized from the tax amount on the contract line details.</span></span> | <span data-ttu-id="df520-172">Когато аспектите на договора съдържат подробности за ред, тази стойност може да се променя чрез промяна на сумите на данъка в подробностите за реда.</span><span class="sxs-lookup"><span data-stu-id="df520-172">When the contract line has line details, this value can be modified by changing the tax amounts on the line details.</span></span> <span data-ttu-id="df520-173">В аспекти на договор с фиксирана цена тази стойност се използва за генериране на данъка в контролните точки за периодично фактуриране.</span><span class="sxs-lookup"><span data-stu-id="df520-173">On a fixed price contract line, this value is used to generate the tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="df520-174">**Договорена сума след данък**</span><span class="sxs-lookup"><span data-stu-id="df520-174">**Contracted Amount after Tax**</span></span> | <span data-ttu-id="df520-175">Сумата на аспектите на договора след данъка.</span><span class="sxs-lookup"><span data-stu-id="df520-175">The contract line amount after tax.</span></span> <span data-ttu-id="df520-176">Това поле е само за четене и се изчислява като **Договорена сума + данък**.</span><span class="sxs-lookup"><span data-stu-id="df520-176">This field is read only and is calculated as **Contracted Amount + Tax**.</span></span> | <span data-ttu-id="df520-177">В аспекти на договор с фиксирана цена тази стойност се използва за генериране на контролните точки за периодично фактуриране.</span><span class="sxs-lookup"><span data-stu-id="df520-177">On a fixed price contract line, this value is used to generate periodic billing milestones.</span></span> |
| <span data-ttu-id="df520-178">**Ограничение, което да не се надвишава**</span><span class="sxs-lookup"><span data-stu-id="df520-178">**Not-to-Exceed Limit**</span></span> | <span data-ttu-id="df520-179">Потребителят може да редактира това поле и то е достъпно само за базирани на проект аспекти на договор, които имат зададен метод за фактуриране като „Време” и „Материали”.</span><span class="sxs-lookup"><span data-stu-id="df520-179">The user can edit this field and it is only available on project-based contract lines that have the billing method set as time and material.</span></span> | <span data-ttu-id="df520-180">Потребителят може да редактира това поле.</span><span class="sxs-lookup"><span data-stu-id="df520-180">The user can edit this field.</span></span> <span data-ttu-id="df520-181">Когато действителни данни за време или материали посочват тези аспекти на договор за време и материал, сумата в действителните данни се оценява спрямо ограничението, което не трябва да се надвишава в аспектите на договора.</span><span class="sxs-lookup"><span data-stu-id="df520-181">When an actual for time and material references this contract line for time and material, the amount on the actual is evaluated against the not-to-exceed limit on the contract line.</span></span> <span data-ttu-id="df520-182">Тази оценка приключва след отчитане на вече изразходваните и разпределените суми.</span><span class="sxs-lookup"><span data-stu-id="df520-182">This evaluation is completed after  the already spent and committed amounts are accounted for.</span></span> |
| <span data-ttu-id="df520-183">**Бюджет на клиента**</span><span class="sxs-lookup"><span data-stu-id="df520-183">**Customer Budget**</span></span> | <span data-ttu-id="df520-184">Това поле може да се редактира и се копира от съответното поле в реда на офертата, ако договорът е създаден от оферта.</span><span class="sxs-lookup"><span data-stu-id="df520-184">This field is editable and is copied from the corresponding field on the quote line if the contract was created from a quote.</span></span> | <span data-ttu-id="df520-185">Това поле се използва само за информация и няма никакво значение надолу по веригата.</span><span class="sxs-lookup"><span data-stu-id="df520-185">This field is only used for information and does not have any downstream significance.</span></span> |

## <a name="validation-rules-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a><span data-ttu-id="df520-186">Правила за проверка на опциите в раздела „Общи” на базирани на проект аспекти на договор</span><span class="sxs-lookup"><span data-stu-id="df520-186">Validation rules for the options on the General tab of project-based contract lines</span></span>

<span data-ttu-id="df520-187">Правило 1: Ако полето **Включени задачи** е празно или е зададено на **Всички задачи по проект**, всички задачи по проекта ще се включат в аспектите на договора.</span><span class="sxs-lookup"><span data-stu-id="df520-187">Rule 1: If the **Included Tasks** field is blank or set to **All Project Tasks**, all tasks of the project are included on the contract line.</span></span>

<span data-ttu-id="df520-188">Правило 2: Когато полето **Включени задачи** е празно или е изрично зададено на **Всички задачи по проект**, могат да се включат проект и определен клас трансакции само в един аспект на договор, базиран на проект, на даден договор.</span><span class="sxs-lookup"><span data-stu-id="df520-188">Rule 2: When the **Included Tasks** field is blank or explicitly set to **All Project Tasks**, a project and a certain transaction class can only be included on one project-based contract line of a contract.</span></span>

<span data-ttu-id="df520-189">Правило 3: Когато полето **Включени задачи** е празно или е зададено на **Само избрани задачи по проект**, могат да се включат проект и определен клас трансакции в няколко аспекта на договор, базиран на проект, на даден договор.</span><span class="sxs-lookup"><span data-stu-id="df520-189">Rule 3: When the **Included Tasks** field is set to **Selected Project Tasks Only**, a project and a certain transaction class can be included on multiple project-based contract lines of a contract.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="43" valign="top">
                <p><span data-ttu-id="df520-190">
                    <strong>Договор</strong>
                </span><span class="sxs-lookup"><span data-stu-id="df520-190">
                    <strong>Contract</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="df520-191">
                    <strong>Aспекти на договор</strong>
                </span><span class="sxs-lookup"><span data-stu-id="df520-191">
                    <strong>Contract line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="df520-192">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="df520-192">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="67" valign="top">
                <p><span data-ttu-id="df520-193">
                    <strong>Включени задачи</strong>
                </span><span class="sxs-lookup"><span data-stu-id="df520-193">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="df520-194">
                    <strong>Включване на време</strong>
                </span><span class="sxs-lookup"><span data-stu-id="df520-194">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="df520-195">
                    <strong>Включване на разход</strong>
                </span><span class="sxs-lookup"><span data-stu-id="df520-195">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="df520-196">
                    <strong>Включване на материали</strong>
                </span><span class="sxs-lookup"><span data-stu-id="df520-196">
                    <strong>Include Materials</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="df520-197">
                    <strong>Включване</strong>
                </span><span class="sxs-lookup"><span data-stu-id="df520-197">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="df520-198">
                    <strong>Такса</strong>
                </span><span class="sxs-lookup"><span data-stu-id="df520-198">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="53" valign="top">
                <p><span data-ttu-id="df520-199">
                    <strong>Валидно/невалидно</strong>
                </span><span class="sxs-lookup"><span data-stu-id="df520-199">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="250" valign="top">
                <p><span data-ttu-id="df520-200">
                    <strong>Причина</strong>
                </span><span class="sxs-lookup"><span data-stu-id="df520-200">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="df520-201">С1</span><span class="sxs-lookup"><span data-stu-id="df520-201">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="df520-202">CL1</span><span class="sxs-lookup"><span data-stu-id="df520-202">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-203">П1</span><span class="sxs-lookup"><span data-stu-id="df520-203">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="df520-204">Празно</span><span class="sxs-lookup"><span data-stu-id="df520-204">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-205">Да</span><span class="sxs-lookup"><span data-stu-id="df520-205">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-206">Да</span><span class="sxs-lookup"><span data-stu-id="df520-206">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-207">Да</span><span class="sxs-lookup"><span data-stu-id="df520-207">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-208">Да</span><span class="sxs-lookup"><span data-stu-id="df520-208">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="df520-209">Невалидно</span><span class="sxs-lookup"><span data-stu-id="df520-209">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="df520-210">Нарушение на правило №2.</span><span class="sxs-lookup"><span data-stu-id="df520-210">Violation of Rule #2.</span></span> <span data-ttu-id="df520-211">Времето, разходите, материалите и таксите по проект P1 са включени и двата реда на оферта – CL1 и CL2.</span><span class="sxs-lookup"><span data-stu-id="df520-211">Time, Expense, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="df520-212">С1</span><span class="sxs-lookup"><span data-stu-id="df520-212">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="df520-213">CL2</span><span class="sxs-lookup"><span data-stu-id="df520-213">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-214">П1</span><span class="sxs-lookup"><span data-stu-id="df520-214">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="df520-215">Празно</span><span class="sxs-lookup"><span data-stu-id="df520-215">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-216">Да</span><span class="sxs-lookup"><span data-stu-id="df520-216">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-217">Да</span><span class="sxs-lookup"><span data-stu-id="df520-217">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-218">Да</span><span class="sxs-lookup"><span data-stu-id="df520-218">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-219">Да</span><span class="sxs-lookup"><span data-stu-id="df520-219">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="df520-220">С1</span><span class="sxs-lookup"><span data-stu-id="df520-220">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="df520-221">CL1</span><span class="sxs-lookup"><span data-stu-id="df520-221">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-222">П1</span><span class="sxs-lookup"><span data-stu-id="df520-222">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="df520-223">Празно</span><span class="sxs-lookup"><span data-stu-id="df520-223">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-224">Да</span><span class="sxs-lookup"><span data-stu-id="df520-224">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-225">No</span><span class="sxs-lookup"><span data-stu-id="df520-225">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-226">Да</span><span class="sxs-lookup"><span data-stu-id="df520-226">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-227">Да</span><span class="sxs-lookup"><span data-stu-id="df520-227">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="df520-228">Невалидно</span><span class="sxs-lookup"><span data-stu-id="df520-228">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="df520-229">Нарушение на правило №2.</span><span class="sxs-lookup"><span data-stu-id="df520-229">Violation of Rule #2.</span></span> <span data-ttu-id="df520-230">Времето, материалите и таксите по проект P1 са включени и двата реда на оферта – CL1 и CL2.</span><span class="sxs-lookup"><span data-stu-id="df520-230">Time, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="df520-231">С1</span><span class="sxs-lookup"><span data-stu-id="df520-231">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="df520-232">CL2</span><span class="sxs-lookup"><span data-stu-id="df520-232">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-233">П1</span><span class="sxs-lookup"><span data-stu-id="df520-233">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="df520-234">Празно</span><span class="sxs-lookup"><span data-stu-id="df520-234">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-235">Да</span><span class="sxs-lookup"><span data-stu-id="df520-235">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-236">Да</span><span class="sxs-lookup"><span data-stu-id="df520-236">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-237">Да</span><span class="sxs-lookup"><span data-stu-id="df520-237">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-238">Да</span><span class="sxs-lookup"><span data-stu-id="df520-238">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="df520-239">С1</span><span class="sxs-lookup"><span data-stu-id="df520-239">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="df520-240">CL1</span><span class="sxs-lookup"><span data-stu-id="df520-240">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-241">П1</span><span class="sxs-lookup"><span data-stu-id="df520-241">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="df520-242">Празно</span><span class="sxs-lookup"><span data-stu-id="df520-242">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-243">Да</span><span class="sxs-lookup"><span data-stu-id="df520-243">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-244">No</span><span class="sxs-lookup"><span data-stu-id="df520-244">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-245">Да</span><span class="sxs-lookup"><span data-stu-id="df520-245">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-246">Да</span><span class="sxs-lookup"><span data-stu-id="df520-246">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="df520-247">Валидно</span><span class="sxs-lookup"><span data-stu-id="df520-247">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="df520-248">Времето, материалите и таксите по проект P1 са включени в CL1.</span><span class="sxs-lookup"><span data-stu-id="df520-248">Time, Materials, and Fees on P1 project are included on CL1.</span></span>
                </p>
                <ul>
                    <li>
<span data-ttu-id="df520-249">Разходите за проект P1 са включени в CL2.</span><span class="sxs-lookup"><span data-stu-id="df520-249">Expense on P1 project is included on CL2.</span></span>
                    </li>
                </ul>
                <p>
<span data-ttu-id="df520-250">Няма припокриване на това, което е включено във всички аспекти на договор и следователно е валидно.</span><span class="sxs-lookup"><span data-stu-id="df520-250">No overlap in what is being included on each Contract line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="df520-251">С1</span><span class="sxs-lookup"><span data-stu-id="df520-251">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="df520-252">CL2</span><span class="sxs-lookup"><span data-stu-id="df520-252">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-253">П1</span><span class="sxs-lookup"><span data-stu-id="df520-253">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="df520-254">Празно</span><span class="sxs-lookup"><span data-stu-id="df520-254">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-255">No</span><span class="sxs-lookup"><span data-stu-id="df520-255">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-256">Да</span><span class="sxs-lookup"><span data-stu-id="df520-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-257">No</span><span class="sxs-lookup"><span data-stu-id="df520-257">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-258">No</span><span class="sxs-lookup"><span data-stu-id="df520-258">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="df520-259">С1</span><span class="sxs-lookup"><span data-stu-id="df520-259">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="df520-260">CL1</span><span class="sxs-lookup"><span data-stu-id="df520-260">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-261">П1</span><span class="sxs-lookup"><span data-stu-id="df520-261">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="df520-262">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="df520-262">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-263">Да</span><span class="sxs-lookup"><span data-stu-id="df520-263">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-264">Да</span><span class="sxs-lookup"><span data-stu-id="df520-264">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-265">Да</span><span class="sxs-lookup"><span data-stu-id="df520-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-266">Да</span><span class="sxs-lookup"><span data-stu-id="df520-266">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="df520-267">Невалидно</span><span class="sxs-lookup"><span data-stu-id="df520-267">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="df520-268">Нарушение на правило №2</span><span class="sxs-lookup"><span data-stu-id="df520-268">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="df520-269">C1 включва време, материали, разходи и такси за подмножество от задачи по проект P1.</span><span class="sxs-lookup"><span data-stu-id="df520-269">C1 includes Time, Materials, Expenses and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="df520-270">CL2 включва време, материали, разходи и такси за целия проект P1 и следователно се припокрива с това, което е включено в C1.</span><span class="sxs-lookup"><span data-stu-id="df520-270">CL2 includes Time, Materials, Expenses and Fees for the whole project P1 and therefore overlaps with what is included on C1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="df520-271">С1</span><span class="sxs-lookup"><span data-stu-id="df520-271">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="df520-272">CL2</span><span class="sxs-lookup"><span data-stu-id="df520-272">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-273">П1</span><span class="sxs-lookup"><span data-stu-id="df520-273">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="df520-274">Празно</span><span class="sxs-lookup"><span data-stu-id="df520-274">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-275">Да</span><span class="sxs-lookup"><span data-stu-id="df520-275">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-276">Да</span><span class="sxs-lookup"><span data-stu-id="df520-276">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-277">Да</span><span class="sxs-lookup"><span data-stu-id="df520-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-278">Да</span><span class="sxs-lookup"><span data-stu-id="df520-278">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="df520-279">С1</span><span class="sxs-lookup"><span data-stu-id="df520-279">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="df520-280">CL1</span><span class="sxs-lookup"><span data-stu-id="df520-280">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-281">П1</span><span class="sxs-lookup"><span data-stu-id="df520-281">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="df520-282">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="df520-282">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-283">Да</span><span class="sxs-lookup"><span data-stu-id="df520-283">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-284">Да</span><span class="sxs-lookup"><span data-stu-id="df520-284">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-285">Да</span><span class="sxs-lookup"><span data-stu-id="df520-285">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-286">Да</span><span class="sxs-lookup"><span data-stu-id="df520-286">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="df520-287">Валидно</span><span class="sxs-lookup"><span data-stu-id="df520-287">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="df520-288">Съгласно правило #3</span><span class="sxs-lookup"><span data-stu-id="df520-288">Per Rule #3</span></span> </p>
                <p>
<span data-ttu-id="df520-289">C1 включва време, материали, разходи и такси за подмножество от задачи по проект P1.</span><span class="sxs-lookup"><span data-stu-id="df520-289">C1 includes Time, Expenses, Materials, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="df520-290">CL2 включва време, материал, разходи и такси за подмножество от задачи по проект P1.</span><span class="sxs-lookup"><span data-stu-id="df520-290">CL2 includes Time, Expenses, Materials, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="df520-291">Единствената допълнителна проверка е около подмножеството от задачи на CL1, което е различно от подмножеството от задачи на CL2, за да се гарантира, че няма припокриване.</span><span class="sxs-lookup"><span data-stu-id="df520-291">The only additional validation is around the subset of tasks on CL1 is different from the subset of tasks on CL2 to ensure that there are no overlaps there.</span></span> <span data-ttu-id="df520-292">Това се прави от системата, когато са свързани задачи.</span><span class="sxs-lookup"><span data-stu-id="df520-292">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="df520-293">С1</span><span class="sxs-lookup"><span data-stu-id="df520-293">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="df520-294">CL2</span><span class="sxs-lookup"><span data-stu-id="df520-294">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-295">П1</span><span class="sxs-lookup"><span data-stu-id="df520-295">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="df520-296">Само избрани задачи</span><span class="sxs-lookup"><span data-stu-id="df520-296">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-297">Да</span><span class="sxs-lookup"><span data-stu-id="df520-297">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="df520-298">Да</span><span class="sxs-lookup"><span data-stu-id="df520-298">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-299">Да</span><span class="sxs-lookup"><span data-stu-id="df520-299">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="df520-300">Да</span><span class="sxs-lookup"><span data-stu-id="df520-300">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
