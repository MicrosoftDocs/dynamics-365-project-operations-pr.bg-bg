---
title: Актуализиране на атрибути на добавка за включване на нови ценови измерения
description: Тази тема предоставя информация за актуализирането на атрибутите на добавката за ценови измерения.
author: Rumant
manager: kfend
ms.custom: ''
ms.date: 11/19/2018
ms.topic: article
ms.service: project-operations
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 958646c9e06a15e265bc0caa8b0f3eb9f79fc347
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281780"
---
# <a name="update-plug-in-attributes-to-include-new-pricing-dimensions"></a><span data-ttu-id="a6b47-103">Актуализиране на атрибути на добавка за включване на нови ценови измерения</span><span class="sxs-lookup"><span data-stu-id="a6b47-103">Update plug-in attributes to include new pricing dimensions</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

> [!NOTE]
> <span data-ttu-id="a6b47-104">Ако не използвате функциите за офериране и договаряне на Project Service Automation (PSA), можете да пропуснете тази тема.</span><span class="sxs-lookup"><span data-stu-id="a6b47-104">If you are not using the Project Service Automation (PSA) Quoting and Contracting features, you can skip this topic.</span></span>

<span data-ttu-id="a6b47-105">Тази тема предполага, че сте изпълнили процедурите в темите [Създавате на персонализирани полета и обекти](create-custom-fields-entities.md), [Добавяне на персонализирани полета към настройка на цени и обекти за транзакции](field-references.md) и [Настройване на персонализирани полета като ценови измерения](set-up-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="a6b47-105">This topic assumes that you have completed the procedures in the topics, [Create custom fields and entities](create-custom-fields-entities.md), [Add custom fields to price setup and transactional entities](field-references.md), and [Set up custom fields as pricing dimensions](set-up-pricing-dimensions.md).</span></span> <span data-ttu-id="a6b47-106">Ако не сте изпълнили тези процедури, върнете се и ги изпълнете, след което се върнете към тази тема.</span><span class="sxs-lookup"><span data-stu-id="a6b47-106">If you haven't completed those procedures, go back and complete them and then return to this topic.</span></span>

<span data-ttu-id="a6b47-107">Когато се създават подробности за ред на оферта в страницата **Ред на оферта** за ред за оферта по проект, системата създава два реда за прогнозна оценка във фонов режим – един ред за страната на разходите на прогнозата и един за страната на продажбите.</span><span class="sxs-lookup"><span data-stu-id="a6b47-107">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines in the background -- one line for the cost side of the estimate and one for sales side.</span></span> <span data-ttu-id="a6b47-108">Същото важи и за редовете на договор по проект.</span><span class="sxs-lookup"><span data-stu-id="a6b47-108">This is the same  for project contract lines.</span></span>

<span data-ttu-id="a6b47-109">Когато правите промяна в количеството или поле от страната на разходите, тази промяна се попълва от страната на продажбите.</span><span class="sxs-lookup"><span data-stu-id="a6b47-109">When you make a change to the quantity or a field on the cost side, that change is propagated to the sales side.</span></span> <span data-ttu-id="a6b47-110">Това е възможно поради следните добавки, които трябва да бъдат регистрирани отново след промяна на ценови измерения.</span><span class="sxs-lookup"><span data-stu-id="a6b47-110">This is possible because of the following plug-ins that must be re-registered after a change to pricing dimensions.</span></span>

- <span data-ttu-id="a6b47-111">PreOperationContractLineDetailUpdate – актуализира **msdyn_orderlinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="a6b47-111">PreOperationContractLineDetailUpdate - Updates **msdyn_orderlinetransaction**.</span></span>
- <span data-ttu-id="a6b47-112">PreOperationQuoteLineDetailUpdate – актуализира **msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="a6b47-112">PreOperationQuoteLineDetailUpdate - Updates **msdyn_quotelinetransaction**.</span></span>

<span data-ttu-id="a6b47-113">Следващите стъпки ви превеждат през процеса на регистриране на добавките.</span><span class="sxs-lookup"><span data-stu-id="a6b47-113">The following steps walk you through the process of registering the plug-ins.</span></span>

1. <span data-ttu-id="a6b47-114">Отворете **PluginRegistrationTool** и се свържете към вашия онлайн екземпляр.</span><span class="sxs-lookup"><span data-stu-id="a6b47-114">Open the **PluginRegistrationTool** and connect to your online instance.</span></span>
2. <span data-ttu-id="a6b47-115">Щракнете върху **Търсене** и потърсете добавката за актуализация.</span><span class="sxs-lookup"><span data-stu-id="a6b47-115">Click **Search** and search for the plug-in to be updated.</span></span>

 ![Екранна снимка на дървото за търсене](media/PRT-1.png)

3. <span data-ttu-id="a6b47-117">След като намерите добавката, изберете я и след това щракнете върху **Избор в главния формуляр**.</span><span class="sxs-lookup"><span data-stu-id="a6b47-117">After the plug-in is found, select it and then click **Select on Main Form**.</span></span>

4. <span data-ttu-id="a6b47-118">Изберете стъпката на добавката за актуализиране, щракнете с десния бутон, след което изберете **Актуализиране**.</span><span class="sxs-lookup"><span data-stu-id="a6b47-118">Select the step of the plug-in to be updated, right-click, and then select **Update**.</span></span>

 ![Екранна снимка на добавката за актуализиране](media/PRT-2.png)
 
5. <span data-ttu-id="a6b47-120">В прозореца за актуализация щракнете върху многоточието (**...**) в атрибутите за филтриране.</span><span class="sxs-lookup"><span data-stu-id="a6b47-120">In the update window, click the ellipsis (**...**) in the filtering attributes.</span></span>

 ![Екранна снимка на актуализацията на информацията за конфигуриране на съществуваща стъпка](media/PRT-3.png)
 
6. <span data-ttu-id="a6b47-122">Поставете отметки в квадратчетата на атрибутите за ценообразуване.</span><span class="sxs-lookup"><span data-stu-id="a6b47-122">Select the pricing attribute check boxes.</span></span>

 ![Екранна снимка, показваща поставянето на отметки за ценовите атрибути](media/PRT-4.png)

7. <span data-ttu-id="a6b47-124">Щракнете върху **OK**, за да затворите страницата, след което изберете **Актуализиране на стъпката**.</span><span class="sxs-lookup"><span data-stu-id="a6b47-124">Click **OK** to close the page and then select **Update Step**.</span></span>

 ![Екранна снимка, показваща бутона „Актуализиране на стъпката“](media/PRT-5.png)
 
8. <span data-ttu-id="a6b47-126">Повторете този процес за втората добавка **PreOperationQuoteLineDetail - актуализира msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="a6b47-126">Repeat this process for the second plug-in, **PreOperationQuoteLineDetail - Update of msdyn_quotelinetransaction**.</span></span>

9. <span data-ttu-id="a6b47-127">Затворете инструмента за регистрация на добавки.</span><span class="sxs-lookup"><span data-stu-id="a6b47-127">Close the plug-in registration tool.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]