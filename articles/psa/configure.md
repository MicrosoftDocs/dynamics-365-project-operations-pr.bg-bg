---
title: Конфигуриране на Project Service Automation
description: Стъпки за конфигуриране на Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 06a29f67040cd7da583bdeae85d6a0f6a3684c52
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290571"
---
# <a name="configure-project-service"></a><span data-ttu-id="5b30c-103">Конфигуриране на Project Service</span><span class="sxs-lookup"><span data-stu-id="5b30c-103">Configure Project Service</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="5b30c-104">Преди да използвате възможностите на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] в [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] за управляване на вашите акаунти, проекти и ресурси, трябва да изпълните няколко конфигурационни стъпки, за да гарантирате, че решението [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] отговаря на нуждите на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="5b30c-104">Before you can use the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automation capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] to manage your accounts, projects, and resources, you need to complete a few configuration steps to ensure the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] solution matches your organization’s needs.</span></span> <span data-ttu-id="5b30c-105">Тези стъпки включват:</span><span class="sxs-lookup"><span data-stu-id="5b30c-105">These steps include:</span></span>  
  
-   <span data-ttu-id="5b30c-106">[Задаване на единици за време](../psa/set-up-time-units.md).</span><span class="sxs-lookup"><span data-stu-id="5b30c-106">[Set up time units](../psa/set-up-time-units.md).</span></span> <span data-ttu-id="5b30c-107">Конфигуриране на единици за време в продуктовия каталог, който ще използвате като основа за планиране и фактуриране на вашите проекти.</span><span class="sxs-lookup"><span data-stu-id="5b30c-107">Configure the time units in the product catalog that you’ll use as a base for scheduling and billing your projects.</span></span>  
  
-   <span data-ttu-id="5b30c-108">[Настройване на валути и валутни курсове](../psa/set-up-currencies-exchange-rates.md).</span><span class="sxs-lookup"><span data-stu-id="5b30c-108">[Set up currencies and exchange rates](../psa/set-up-currencies-exchange-rates.md).</span></span> <span data-ttu-id="5b30c-109">Настройване на валутите, които да използвате за вашите проекти.</span><span class="sxs-lookup"><span data-stu-id="5b30c-109">Set up the currencies to use for your projects.</span></span>  
  
-   <span data-ttu-id="5b30c-110">[Създаване на организационни единици](../psa/create-organizational-units.md).</span><span class="sxs-lookup"><span data-stu-id="5b30c-110">[Create organizational units](../psa/create-organizational-units.md).</span></span> <span data-ttu-id="5b30c-111">Настройване на групи, които вашата фирма използва за разделяне на бизнеса си, независимо дали по географски признак, бизнес функция, или друго логическо разделение.</span><span class="sxs-lookup"><span data-stu-id="5b30c-111">Set up the groups that your company uses to divide its business, whether by geography, business function, or other logical division.</span></span>  
  
-   <span data-ttu-id="5b30c-112">[Задаване на честоти на фактури](../psa/set-up-invoice-frequencies.md).</span><span class="sxs-lookup"><span data-stu-id="5b30c-112">[Set up invoice frequencies](../psa/set-up-invoice-frequencies.md).</span></span> <span data-ttu-id="5b30c-113">Настройване на периоди от време, които искате да използвате за фактуриране на вашите клиенти.</span><span class="sxs-lookup"><span data-stu-id="5b30c-113">Set up time periods that you want to use for billing your clients.</span></span>  
  
-   <span data-ttu-id="5b30c-114">[Конфигуриране на категории транзакции](../psa/configure-transaction-categories.md).</span><span class="sxs-lookup"><span data-stu-id="5b30c-114">[Configure transaction categories](../psa/configure-transaction-categories.md).</span></span> <span data-ttu-id="5b30c-115">Настройване на категориите транзакции, в които вашите консултанти могат да налагат своите платими и неплатими разходи.</span><span class="sxs-lookup"><span data-stu-id="5b30c-115">Set up transaction categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="5b30c-116">[Конфигуриране на категории разходи](../psa/configure-expense-categories.md).</span><span class="sxs-lookup"><span data-stu-id="5b30c-116">[Configure expense categories](../psa/configure-expense-categories.md).</span></span> <span data-ttu-id="5b30c-117">Настройване на категориите, в които вашите консултанти могат да налагат своите платими и неплатими разходи.</span><span class="sxs-lookup"><span data-stu-id="5b30c-117">Set up the categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="5b30c-118">[Създаване на елементи в продуктов каталог](../psa/create-product-catalog-items.md).</span><span class="sxs-lookup"><span data-stu-id="5b30c-118">[Create product catalog items](../psa/create-product-catalog-items.md).</span></span> <span data-ttu-id="5b30c-119">Добавяне на продуктите, които продавате, като например софтуерни лицензи, към продуктовия каталог.</span><span class="sxs-lookup"><span data-stu-id="5b30c-119">Add the products you sell, such as software licenses, to the product catalog.</span></span>  
  
-   <span data-ttu-id="5b30c-120">[Създаване на ценова листа](../psa/create-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="5b30c-120">[Create a price list](../psa/create-price-list.md).</span></span> <span data-ttu-id="5b30c-121">Конфигуриране на различни ценови листи в зависимост от това колко искате да таксувате своите клиенти за всяка роля, която изисква техният проект.</span><span class="sxs-lookup"><span data-stu-id="5b30c-121">Configure different price lists, depending on how much you want to charge your clients for each role their project requires.</span></span>  
  
-   <span data-ttu-id="5b30c-122">[Задаване на ресурси](../psa/set-up-resources.md).</span><span class="sxs-lookup"><span data-stu-id="5b30c-122">[Set up resources](../psa/set-up-resources.md).</span></span> <span data-ttu-id="5b30c-123">Добавяне на умения, нива на професионална подготовка, роли на ресурси и друга информация за ресурсите, която ще ви трябва за вашите проекти.</span><span class="sxs-lookup"><span data-stu-id="5b30c-123">Add the skills, proficiencies, resource roles, and other resource information that you’ll need for your projects.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="5b30c-124">Вижте също</span><span class="sxs-lookup"><span data-stu-id="5b30c-124">See Also</span></span>  
 <span data-ttu-id="5b30c-125">[Преглед на Project Service Automation](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="5b30c-125">[Overview of Project Service Automation](../psa/overview.md) </span></span>  
 <span data-ttu-id="5b30c-126">[Конфигуриране на Project Service Automation](../psa/configure.md) </span><span class="sxs-lookup"><span data-stu-id="5b30c-126">[Configure Project Service Automation](../psa/configure.md) </span></span>  
 <span data-ttu-id="5b30c-127">[Ръководство за мениджъри на акаунти](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="5b30c-127">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="5b30c-128">[Ръководство за мениджъри на проекти](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="5b30c-128">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="5b30c-129">[Ръководство за мениджъри на ресурси](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="5b30c-129">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="5b30c-130">Ръководство за време, разходи и сътрудничество</span><span class="sxs-lookup"><span data-stu-id="5b30c-130">Time, Expense, and Collaboration Guid</span></span>](../psa/time-expense-collaboration-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]