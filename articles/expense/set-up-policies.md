---
title: Определете политики за разходите
description: Можете да определите политики за разходите, които вашите работници трябва да спазват, когато въвеждат и подават отчети за разходите и заявки за пътуване.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 863d1e44dad9fa0d2174cf77582a1d820988e92d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276065"
---
# <a name="define-expense-policies"></a><span data-ttu-id="d0667-103">Определете политики за разходите</span><span class="sxs-lookup"><span data-stu-id="d0667-103">Define expense policies</span></span>

<span data-ttu-id="d0667-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="d0667-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d0667-105">Можете да определите политики, които вашите работници трябва да спазват, когато въвеждат и подават отчети за разходите и заявки за пътуване.</span><span class="sxs-lookup"><span data-stu-id="d0667-105">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="d0667-106">Прилагането на политики за разходите може да ви помогне да управлявате ефективно разходите.</span><span class="sxs-lookup"><span data-stu-id="d0667-106">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="d0667-107">Например можете да зададете политика за хотелски разходи в Ню Йорк, която гласи, че разходите за нощувка не могат да надвишават USD 250.</span><span class="sxs-lookup"><span data-stu-id="d0667-107">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="d0667-108">Ако работникът представи отчет за разходите или заявка за пътуване, когато цената на стаята надвишава тази сума, системата ще уведоми</span><span class="sxs-lookup"><span data-stu-id="d0667-108">If a worker submits an expense report or travel requisition where the room rate exceeds this amount, the system will notify the</span></span>         
<span data-ttu-id="d0667-109">работник, че размерът на полицата за разхода е надвишен.</span><span class="sxs-lookup"><span data-stu-id="d0667-109">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="d0667-110">Можете да конфигурирате съобщението, което работникът ще получи, когато вие</span><span class="sxs-lookup"><span data-stu-id="d0667-110">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="d0667-111">определяте политиката.</span><span class="sxs-lookup"><span data-stu-id="d0667-111">define the policy.</span></span>      
        
<span data-ttu-id="d0667-112">Можете да определите три типа политики:</span><span class="sxs-lookup"><span data-stu-id="d0667-112">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="d0667-113">**Внимание**: Позволява на работника да представи отчет за разходите или заявка за пътуване, но разходът ще бъде отбелязан за всички одобряващи и</span><span class="sxs-lookup"><span data-stu-id="d0667-113">**Warning**: Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>         
  <span data-ttu-id="d0667-114">за по-късно докладване.</span><span class="sxs-lookup"><span data-stu-id="d0667-114">for later reporting.</span></span>        

- <span data-ttu-id="d0667-115">**Грешка**: Изисква работникът да преразгледа разходите, за да се съобрази с политиката, преди да представи отчет за разходите или заявка за пътуване.</span><span class="sxs-lookup"><span data-stu-id="d0667-115">**Error**: Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>        
 
 - <span data-ttu-id="d0667-116">**Обосновка**: Изисква работникът или мениджърът да въведе обосновка за надвишаване на сумата на полицата, преди да представи отчет за разходите или заявка за пътуване.</span><span class="sxs-lookup"><span data-stu-id="d0667-116">**Justification**: Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="d0667-117">Съвети за политиката</span><span class="sxs-lookup"><span data-stu-id="d0667-117">Policy tips</span></span>
<span data-ttu-id="d0667-118">Ето няколко предложения, които могат да ви помогнат при създаването на нови правила за управление на разходите:</span><span class="sxs-lookup"><span data-stu-id="d0667-118">Here are a few suggestions that can assist you when creating new policies for expense management:</span></span> 

- <span data-ttu-id="d0667-119">Политиките са в сила от датата, което означава, че политиката няма да влезе в сила, ако е създадена с дата след датата на възникване на разходите.</span><span class="sxs-lookup"><span data-stu-id="d0667-119">Policies are date effective which means a policy won't take effect if it's created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="d0667-120">Например, създавате нова политика днес, за да приложите максимален разход за хранене от $50.</span><span class="sxs-lookup"><span data-stu-id="d0667-120">For example, you create a new policy today to enforce a maximum meal expense of $50.</span></span> <span data-ttu-id="d0667-121">Всички съществуващи разходи, въведени от вчера, няма да бъдат проверени по тази политика.</span><span class="sxs-lookup"><span data-stu-id="d0667-121">Any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
- <span data-ttu-id="d0667-122">Когато създавате политика за категория разходи, която може да бъде детайлизирана, помислете дали да не добавите условие за типа линия на разходите.</span><span class="sxs-lookup"><span data-stu-id="d0667-122">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="d0667-123">Някои правила, като например изискване на разписка, може да нямат смисъл за подробни редове.</span><span class="sxs-lookup"><span data-stu-id="d0667-123">Some policies, such as requiring a receipt, may not make sense for itemized lines.</span></span> <span data-ttu-id="d0667-124">В тази ситуация политиката се прилага само към заглавния ред или неразделен ред.</span><span class="sxs-lookup"><span data-stu-id="d0667-124">In this situation, the policy only is applied to the header line or a non-itemized line.</span></span> 
- <span data-ttu-id="d0667-125">Политиките за управление на разходите по подразбиране се оценяват спрямо субекта източник.</span><span class="sxs-lookup"><span data-stu-id="d0667-125">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="d0667-126">За вътрешнофирмени сценарии можете вместо това да настроите политиката да се оценява спрямо обекта на местоназначението (обект за заем).</span><span class="sxs-lookup"><span data-stu-id="d0667-126">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="d0667-127">За да стартирате политиките срещу обекта дестинация, включете функцията **Оценяване на политиката на разходите срещу вземане на юридическо лице** в работна област **Управление на функции**.</span><span class="sxs-lookup"><span data-stu-id="d0667-127">To run the policies against the destination entity, turn on the **Evaluate Expense policy against borrowing legal entity** feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="d0667-128">Кога да се оценяват политиките</span><span class="sxs-lookup"><span data-stu-id="d0667-128">When to evaluate policies</span></span>

<span data-ttu-id="d0667-129">В параметрите за управление на разходите можете да изберете да оцените политиките за управление на разходите, когато дадена линия е запазена или когато е изпратен отчет за разходите.</span><span class="sxs-lookup"><span data-stu-id="d0667-129">In expense management parameters, you can select to evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="d0667-130">Ако изберете да оцените кога дадена линия е запазена, потребителите ще имат по-ранна видимост какво трябва да направят, за да попълнят отчета си за разходи наведнъж.</span><span class="sxs-lookup"><span data-stu-id="d0667-130">If you choose to evaluate when a line is saved, users will have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="d0667-131">В противен случай можете да забавите оценката на политиката и да спестите време, като проверите в края, по време на подаването в работния процес.</span><span class="sxs-lookup"><span data-stu-id="d0667-131">Otherwise, you can delay policy evaluation and save time by validating at the end, during the submission to workflow.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]