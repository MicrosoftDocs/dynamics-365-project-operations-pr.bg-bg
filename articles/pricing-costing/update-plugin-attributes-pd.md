---
title: Актуализиране на атрибути на добавка с нови измерения на ценообразуване
description: Тази тема предоставя информация за начина на актуализиране на атрибутите на добавката за измерения на ценообразуване.
author: rumant
ms.date: 11/18/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 54b87a993929edbf89ef48741ba0a06c6c42ec4e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004608"
---
# <a name="update-plug-in-attributes-with-new-pricing-dimensions"></a><span data-ttu-id="ffb3b-103">Актуализиране на атрибути на добавка с нови измерения на ценообразуване</span><span class="sxs-lookup"><span data-stu-id="ffb3b-103">Update plug-in attributes with new pricing dimensions</span></span>

<span data-ttu-id="ffb3b-104">Тази тема предоставя информация за начина на актуализиране на атрибутите на добавката за измерения на ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-104">This topic provides information about how to update plug-in attributes for pricing dimensions.</span></span>

> [!NOTE]
> <span data-ttu-id="ffb3b-105">Тази тема е приложима само за функциите за оферта и договор в Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-105">This topic is only applicable to the quote and contract features in Dynamics 365 Project Operations.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffb3b-106">Предварителни изисквания</span><span class="sxs-lookup"><span data-stu-id="ffb3b-106">Prerequisites</span></span>
<span data-ttu-id="ffb3b-107">Преди да изпълните стъпките в тази тема, трябва да сте изпълнили процедурите в следните теми:</span><span class="sxs-lookup"><span data-stu-id="ffb3b-107">Before you complete the steps in this topic, you must have completed the procedures in the following topics:</span></span>

  - [<span data-ttu-id="ffb3b-108">Създаване на персонализирани полета и обекти</span><span class="sxs-lookup"><span data-stu-id="ffb3b-108">Create custom fields and entities</span></span>](create-custom-fields-entities-pricing-dimensions.md) 
  - [<span data-ttu-id="ffb3b-109">Добавяне на персонализирани полета към настройка на цени и обекти на трансакции </span><span class="sxs-lookup"><span data-stu-id="ffb3b-109">Add custom fields to price setup and transactional entities</span></span>](add-custom-fields-price-setup-transactional-entities.md)
  - <span data-ttu-id="ffb3b-110">[Настройване на персонализирани полета като измерения на ценообразуване](set-up-custom-fields-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="ffb3b-110">[Set up custom fields as pricing dimensions](set-up-custom-fields-pricing-dimensions.md).</span></span> 
  
<span data-ttu-id="ffb3b-111">Ако не сте изпълнили тези процедури, изпълнете ги, след което се върнете към тази тема.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-111">If you haven't completed those procedures, complete them and then return to this topic.</span></span>

## <a name="register-a-plug-in"></a><span data-ttu-id="ffb3b-112">Регистриране на добавка</span><span class="sxs-lookup"><span data-stu-id="ffb3b-112">Register a plug-in</span></span>
<span data-ttu-id="ffb3b-113">Когато се създаде подробност за ред на оферта, на страницата **Ред на оферта** за ред на оферта по проект системата създава два реда за оценка.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-113">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines.</span></span> <span data-ttu-id="ffb3b-114">Единият ред е за разходната страна на прогнозата, а другият ред е за продажбите.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-114">One line is for the cost side of the estimate and the other line is for sales the side.</span></span> <span data-ttu-id="ffb3b-115">Същото важи и за редовете на договор по проект.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-115">This is the same  for project contract lines.</span></span>

<span data-ttu-id="ffb3b-116">Когато правите промяна в количеството или поле от страната на разходите, тази промяна се и за продажбите.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-116">When you make a change to the quantity or a field on the cost side, that change is also made on the sales side.</span></span> <span data-ttu-id="ffb3b-117">Това е възможно, защото добавките PreOperation на обектите за подробности Quotelinedetail и contractline свързват специфични атрибути от страната на разходите към страната на продажбите на трансакцията.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-117">This is possible because the PreOperation plug-ins on Quotelinedetail and contractline detail entities connect specific attributes on the cost side to the sales side of the transaction.</span></span> <span data-ttu-id="ffb3b-118">Ако е необходимо направените промени на стойностите на измерение на ценообразуване от страната на продажбите да се направят и в страната на разходите, следващите добавки трябва да се регистрират повторно след извършването на промени в измерение на ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-118">If you need changes made to the pricing dimension values on the sales side to also be made on the cost side, the following plug-ins must be re-registered after making changes to a pricing dimension.</span></span>

<span data-ttu-id="ffb3b-119">Това са добавките за актуализиране и повторно регистриране:</span><span class="sxs-lookup"><span data-stu-id="ffb3b-119">These are the plug-ins to update and re-register:</span></span>

- <span data-ttu-id="ffb3b-120">PreOperationContractLineDetailUpdate – **Актуализира msdyn_orderlinetransaction**</span><span class="sxs-lookup"><span data-stu-id="ffb3b-120">PreOperationContractLineDetailUpdate - **Update msdyn_orderlinetransaction**</span></span>
- <span data-ttu-id="ffb3b-121">PreOperationQuoteLineDetailUpdate - **Актуализира msdyn_quotelinetransaction**</span><span class="sxs-lookup"><span data-stu-id="ffb3b-121">PreOperationQuoteLineDetailUpdate - **Updates msdyn_quotelinetransaction**</span></span>

<span data-ttu-id="ffb3b-122">Изпълнете следните стъпки, за да актуализирате и регистрирате повторно добавките.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-122">Complete the following steps to update and re-register the plug-ins.</span></span>

1. <span data-ttu-id="ffb3b-123">Отворете **PluginRegistrationTool** и се свържете със средата на Project Operations Dataverse.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-123">Open **PluginRegistrationTool** and connect to your Project Operations Dataverse environment.</span></span>
2. <span data-ttu-id="ffb3b-124">Изберете **Търсене** и въведете първите няколко букви от добавката, която ще се актуализира.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-124">Select **Search**, and type in the first few letters of the plug-in to be updated.</span></span>
3. <span data-ttu-id="ffb3b-125">След като намерите добавката, изберете я и след това изберете **Избор в главния формуляр**.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-125">After the plug-in is found, select it, and then select **Select on Main Form**.</span></span>
4. <span data-ttu-id="ffb3b-126">Изберете стъпката **Актуализиране на msdyn_orderlinetransaction**, щракнете с десния бутон, след което изберете **Актуализиране**.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-126">Select the **Update msdyn_orderlinetransaction** step, right-click, and then select **Update**.</span></span>
5. <span data-ttu-id="ffb3b-127">На страницата с диалога **Актуализиране** изберете многоточието (**...**) в атрибутите за филтриране.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-127">In the **Update** dialog page, select the ellipsis (**...**) in the filtering attributes.</span></span>
6. <span data-ttu-id="ffb3b-128">Отваря се прозорецът за филтриране на атрибути и предоставя списък с всички атрибути в обекта и измеренията на ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-128">The filtering attributes window opens and provides a list of all attributes in the entity and the pricing dimensions.</span></span> <span data-ttu-id="ffb3b-129">Поставете отметки в квадратчетата за атрибутите на измерението на ценообразуването.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-129">Select the check boxes for the pricing dimension attributes.</span></span>
7. <span data-ttu-id="ffb3b-130">Изберете **OK**, за да затворите страницата, след което изберете **Актуализиране на стъпката**.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-130">Select **OK** to close the page, and then select **Update Step**.</span></span>
8. <span data-ttu-id="ffb3b-131">Повторете стъпки 2-7 за втората добавка, **PreOperationQuoteLineDetail**.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-131">Repeat steps 2-7 for the second plug-in, **PreOperationQuoteLineDetail**.</span></span> <span data-ttu-id="ffb3b-132">За тази добавка трябва да актуализирате стъпката **Актуализиране на msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-132">For this plug-in, you need to update the **Update of msdyn_quotelinetransaction** step.</span></span>
9. <span data-ttu-id="ffb3b-133">Затворете **PluginRegistrationTool**.</span><span class="sxs-lookup"><span data-stu-id="ffb3b-133">Close **PluginRegistrationTool**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]