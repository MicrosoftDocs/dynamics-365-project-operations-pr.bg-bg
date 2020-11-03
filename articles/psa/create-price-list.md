---
title: Създаване на ценова листа
description: Как се създава ценова листа в Project Service
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: bf75286fd1837e27a9b6053ccb21b60771ee197d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071856"
---
# <a name="create-a-price-list-project-service"></a><span data-ttu-id="017f4-103">Създаване на ценова листа (Project Service)</span><span class="sxs-lookup"><span data-stu-id="017f4-103">Create a price list (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="017f4-104">Ценовите листи предоставят шаблон, който мениджърите на клиенти могат да използват за създаване на проекти и оферти и за установяване на разходите на даден проект.</span><span class="sxs-lookup"><span data-stu-id="017f4-104">Price lists provide a template your account managers can use for creating quotes and projects, and for establishing the costs of a project.</span></span> <span data-ttu-id="017f4-105">Те осигуряват списък с елементи на ролите и разходите, както и цената, която таксувате за всяка от тях.</span><span class="sxs-lookup"><span data-stu-id="017f4-105">They provide a line item list of roles and expenses, and the price you will charge for each.</span></span> <span data-ttu-id="017f4-106">Може да създадете няколко ценови листи, за да можете да поддържате отделни ценови структури за различни региони, в които се продават продуктите ви, или за различни канали за продажби.</span><span class="sxs-lookup"><span data-stu-id="017f4-106">You can create multiple price lists so that you can maintain separate price structures for different regions you sell your products in or for different sales channels.</span></span> <span data-ttu-id="017f4-107">Добра идея е да създадете поне една ценова листа за всяка валута, в която планирате да таксувате клиентите си.</span><span class="sxs-lookup"><span data-stu-id="017f4-107">It’s a good idea to create at least one price list for every currency you plan to bill your customers in.</span></span>  
  
<span data-ttu-id="017f4-108">За да създадете финансови прогнози за работа, която трябва да бъде извършена, уверете се, че всеки проект цена и ценова листа за продажби.</span><span class="sxs-lookup"><span data-stu-id="017f4-108">To create financial estimates for the work to be delivered, make sure every project has a backing cost and sales price list.</span></span> <span data-ttu-id="017f4-109">Задайте цена и ценова листа за продажби по подразбиране, която важи за всички проекти, създадени в организацията ви.</span><span class="sxs-lookup"><span data-stu-id="017f4-109">Set up a default cost and sales pricelist that applies to all projects created in your organization.</span></span>  
  
<span data-ttu-id="017f4-110">Ценовите листи разчитат на категории на роли и разходи, така че преди да създадете ценова листа, се уверете, че вече сте конфигурирали категориите на ролите и разходите, които искате да използвате при създаване на ценовата листа.</span><span class="sxs-lookup"><span data-stu-id="017f4-110">Price lists rely on roles and expense categories, so before you create a price list, make sure you’ve already configured the roles and expense categories you want to use while creating the price list.</span></span>  
  
1.  <span data-ttu-id="017f4-111">Отидете на **Project Service > Ценови листи**.</span><span class="sxs-lookup"><span data-stu-id="017f4-111">Go to **Project Service > Price Lists**.</span></span>  
  
2.  <span data-ttu-id="017f4-112">Щракнете върху **Нов**.</span><span class="sxs-lookup"><span data-stu-id="017f4-112">Click **New**.</span></span>  
  
3.  <span data-ttu-id="017f4-113">В **Контекст** изберете дали тази ценова листа е за **Разходи** , **Покупка** или **Продажби**.</span><span class="sxs-lookup"><span data-stu-id="017f4-113">In **Context** , select whether this price list is for **Cost** , **Purchase** , or **Sales**.</span></span>  
  
4.  <span data-ttu-id="017f4-114">В **Име** въведете име за ценовата листа.</span><span class="sxs-lookup"><span data-stu-id="017f4-114">In **Name** , enter a name for the price list.</span></span>  
  
5.  <span data-ttu-id="017f4-115">Във **Валута** изберете валутата, която ще използвате за фактуриране или ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="017f4-115">In **Currency** , select the currency you’re going to use for billing or costing.</span></span>  
  
6.  <span data-ttu-id="017f4-116">В **Единица време** задайте периода от време, за който важи цената, например ден или час.</span><span class="sxs-lookup"><span data-stu-id="017f4-116">In **Time Unit** , specify the period of time the price applies to, such as day or hour.</span></span>  
  
7.  <span data-ttu-id="017f4-117">Попълнете **Начална дата** , **Крайна дата** и **Описание** , ако е необходимо.</span><span class="sxs-lookup"><span data-stu-id="017f4-117">Fill in the **Start Date** , **End Date** , and **Description** as needed.</span></span>  
  
8.  <span data-ttu-id="017f4-118">Щракнете върху **Запиши** , за да създадете записа, така че да можете да продължите да го редактирате.</span><span class="sxs-lookup"><span data-stu-id="017f4-118">Click **Save** to create the record so you can continue editing it.</span></span>  
  
9. <span data-ttu-id="017f4-119">За да добавите цена на роля към ценовата листа, щракнете върху **+** под **Цени на роли**.</span><span class="sxs-lookup"><span data-stu-id="017f4-119">To add a role price to the price list, click **+** under **Role prices**.</span></span>  
  
10. <span data-ttu-id="017f4-120">В екрана **Цена на роля** попълнете детайлите и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="017f4-120">In the **Role Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="017f4-121">Продължете да добавяте цени на роли, докато е необходимо.</span><span class="sxs-lookup"><span data-stu-id="017f4-121">Continue adding role prices as necessary.</span></span> <span data-ttu-id="017f4-122">Когато сте готови, щракнете върху **Запиши** в долния десен ъгъл на екрана.</span><span class="sxs-lookup"><span data-stu-id="017f4-122">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
11. <span data-ttu-id="017f4-123">За да добавите цена за категория разходи към ценовата листа, щракнете върху **+** под **Цени на категории**.</span><span class="sxs-lookup"><span data-stu-id="017f4-123">To add an expense category price to the price list, click **+** under **Category prices**.</span></span>  
  
12. <span data-ttu-id="017f4-124">В екрана **Цена на категория транзакция** попълнете детайлите и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="017f4-124">In the **Transaction Category Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="017f4-125">Продължете да добавяте цени на категории, докато е необходимо.</span><span class="sxs-lookup"><span data-stu-id="017f4-125">Continue adding category prices as necessary.</span></span> <span data-ttu-id="017f4-126">Когато сте готови, щракнете върху **Запиши** в долния десен ъгъл на екрана.</span><span class="sxs-lookup"><span data-stu-id="017f4-126">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
13. <span data-ttu-id="017f4-127">За да добавите елементи в ценова листа към ценовата листа, щракнете върху **+** под **Елементи в ценова листа**.</span><span class="sxs-lookup"><span data-stu-id="017f4-127">To add price list items to the price list, click **+** under **Price List Items**.</span></span>  
  
14. <span data-ttu-id="017f4-128">В екрана **Елемент в ценовата листа** попълнете детайлите и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="017f4-128">In the **Price List Item** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="017f4-129">Продължете да добавяте елементи в ценовата листа, докато е необходимо.</span><span class="sxs-lookup"><span data-stu-id="017f4-129">Continue adding price list items as necessary.</span></span> <span data-ttu-id="017f4-130">Когато сте готови, щракнете върху **Запиши** в долния десен ъгъл на екрана.</span><span class="sxs-lookup"><span data-stu-id="017f4-130">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
15. <span data-ttu-id="017f4-131">За да добавите релации на региони към ценовата листа, щракнете върху **+** под **Релации на региони**.</span><span class="sxs-lookup"><span data-stu-id="017f4-131">To add territory relationships to the price list, click **+** under **Territory Relationships**.</span></span>  
  
16. <span data-ttu-id="017f4-132">В прозореца **Нова връзка** попълнете детайлите и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="017f4-132">In the **New Connection** window, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="017f4-133">Продължете да добавяте релации на региони, докато е необходимо.</span><span class="sxs-lookup"><span data-stu-id="017f4-133">Continue adding territory relationships as necessary.</span></span> <span data-ttu-id="017f4-134">Когато сте готови, щракнете върху **Запиши** в долния десен ъгъл на екрана.</span><span class="sxs-lookup"><span data-stu-id="017f4-134">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="017f4-135">Вижте също</span><span class="sxs-lookup"><span data-stu-id="017f4-135">See Also</span></span>  
 [<span data-ttu-id="017f4-136">Конфигуриране на Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="017f4-136">Configure Project Service Automation</span></span>](../psa/configure.md)
