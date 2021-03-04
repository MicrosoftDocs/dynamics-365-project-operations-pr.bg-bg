---
title: Настройване на политики за разходи
description: Можете да настройвате политики за разходите, които вашите работници трябва да спазват, когато въвеждат и подават отчети за разходите и заявки за пътуване в Microsoft Dynamics 365 Finance.
author: suvaidya
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysPolicyListPage, TrvPolicyRule
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: ab99c0ec769eb2e0914fc7d993f83d20e2c327f6
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960684"
---
# <a name="set-up-expense-policies"></a><span data-ttu-id="70798-103">Настройване на политики за разходи</span><span class="sxs-lookup"><span data-stu-id="70798-103">Set up expense policies</span></span>

<span data-ttu-id="70798-104">Можете да определите политики, които вашите работници трябва да спазват, когато въвеждат и подават отчети за разходите и заявки за пътуване.</span><span class="sxs-lookup"><span data-stu-id="70798-104">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="70798-105">Прилагането на политики за разходите може да ви помогне да управлявате ефективно разходите.</span><span class="sxs-lookup"><span data-stu-id="70798-105">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="70798-106">Например можете да зададете политика за хотелски разходи в Ню Йорк, която гласи, че разходите за нощувка не могат да надвишават USD 250.</span><span class="sxs-lookup"><span data-stu-id="70798-106">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="70798-107">Ако работникът представи отчет за разходите или заявка за пътуване, в които цената на стаята надвишава тази сума, системата ще уведоми</span><span class="sxs-lookup"><span data-stu-id="70798-107">If a worker submits an expense report or a travel requisition in which the room rate exceeds this amount, the system will notify the</span></span>        
<span data-ttu-id="70798-108">работник, че размерът на полицата за разхода е надвишен.</span><span class="sxs-lookup"><span data-stu-id="70798-108">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="70798-109">Можете да конфигурирате съобщението, което работникът ще получи, когато вие</span><span class="sxs-lookup"><span data-stu-id="70798-109">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="70798-110">определяте политиката.</span><span class="sxs-lookup"><span data-stu-id="70798-110">define the policy.</span></span>      
        
<span data-ttu-id="70798-111">Можете да определите три типа политики:</span><span class="sxs-lookup"><span data-stu-id="70798-111">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="70798-112">Предупреждение – Позволява на работника да представи отчет за разходите или заявка за пътуване, но разходът ще бъде отбелязан за всички одобряващи и</span><span class="sxs-lookup"><span data-stu-id="70798-112">Warning – Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>        
  <span data-ttu-id="70798-113">за по-късно докладване.</span><span class="sxs-lookup"><span data-stu-id="70798-113">for later reporting.</span></span>        

- <span data-ttu-id="70798-114">Грешка – Изисква работникът да преразгледа разходите, за да се съобрази с политиката, преди да представи отчет за разходите или заявка за пътуване.</span><span class="sxs-lookup"><span data-stu-id="70798-114">Error – Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>       
 
 - <span data-ttu-id="70798-115">Обосновка – Изисква работникът или мениджърът да въведе обосновка за надвишаване на сумата на полицата, преди да представи отчет за разходите или заявка за пътуване.</span><span class="sxs-lookup"><span data-stu-id="70798-115">Justification – Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="70798-116">Съвети за политиката</span><span class="sxs-lookup"><span data-stu-id="70798-116">Policy tips</span></span>
<span data-ttu-id="70798-117">Ето няколко предложения, които могат да ви помогнат при създаването на нови правила за управление на разходите.</span><span class="sxs-lookup"><span data-stu-id="70798-117">Here are a few suggestions that can assist you when creating new policies for expense management.</span></span> 
* <span data-ttu-id="70798-118">Политиките са в сила от дата и няма да влязат в сила, ако политиката е създадена с дата след датата на възникване на разходите.</span><span class="sxs-lookup"><span data-stu-id="70798-118">Policies are date effective and won't take effect if the policy is created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="70798-119">Например, ако създавате нова политика днес, за да приложите максимален разход за хранене от $50, тогава всички съществуващи разходи, въведени от вчера, няма да бъдат проверени спрямо тази политика.</span><span class="sxs-lookup"><span data-stu-id="70798-119">For example, if you are creating a new policy today to enforce a maximum meal expense of $50, then any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
* <span data-ttu-id="70798-120">Когато създавате политика за категория разходи, която може да бъде детайлизирана, помислете дали да не добавите условие за типа линия на разходите.</span><span class="sxs-lookup"><span data-stu-id="70798-120">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="70798-121">Някои политики, като например изискване на разписка, може да нямат смисъл за подредени редове и трябва да се прилагат само за заглавния ред или неразделен ред.</span><span class="sxs-lookup"><span data-stu-id="70798-121">Some policies such as requiring a receipt may not make sense for itemized lines and should only be applied to the header line or a non-itemized line.</span></span> 
* <span data-ttu-id="70798-122">Политиките за управление на разходите по подразбиране се оценяват спрямо субекта източник.</span><span class="sxs-lookup"><span data-stu-id="70798-122">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="70798-123">За вътрешнофирмени сценарии можете вместо това да настроите политиката да се оценява спрямо обекта на местоназначението (обект за заем).</span><span class="sxs-lookup"><span data-stu-id="70798-123">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="70798-124">За да стартирате политиките срещу обекта дестинация, включете функцията „Оценяване на политиката на разходите срещу вземане на юридическо лице“ в работна област **Управление на функции**.</span><span class="sxs-lookup"><span data-stu-id="70798-124">To run the policies against the destination entity, turn on the "Evaluate Expense policy against borrowing legal entity" feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="70798-125">Кога да се оценяват политиките</span><span class="sxs-lookup"><span data-stu-id="70798-125">When to evaluate policies</span></span>

<span data-ttu-id="70798-126">В параметрите за управление на разходите има опция да оцените политиките за управление на разходите, когато дадена линия е запазена или когато е изпратен отчет за разходите.</span><span class="sxs-lookup"><span data-stu-id="70798-126">In expense management parameters, there is an option to either evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="70798-127">Ако изберете да оцените кога дадена линия е запазена, това гарантира, че потребителите ще имат по-ранна видимост какво трябва да направят, за да попълнят отчета си за разходи наведнъж.</span><span class="sxs-lookup"><span data-stu-id="70798-127">If you choose to evaluate when a line is saved this ensures that users have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="70798-128">В противен случай можете да забавите оценката на политиката и да спестите време, ако валидирането става в края, по време на подаването в работния поток.</span><span class="sxs-lookup"><span data-stu-id="70798-128">Otherwise, you can delay policy evaluation and save time if you have validation occur at the end, during submission to workflow.</span></span>
