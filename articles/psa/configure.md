---
title: Конфигуриране на Project Service Automation
description: Стъпки за конфигуриране на Project Service
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: fd02611b5b3133e097b2818a725b6c5d667e5ac0
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071929"
---
# <a name="configure-project-service"></a><span data-ttu-id="64cf6-103">Конфигуриране на Project Service</span><span class="sxs-lookup"><span data-stu-id="64cf6-103">Configure Project Service</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="64cf6-104">Преди да използвате възможностите на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] в [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] за управляване на вашите акаунти, проекти и ресурси, трябва да изпълните няколко конфигурационни стъпки, за да гарантирате, че решението [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] отговаря на нуждите на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="64cf6-104">Before you can use the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automation capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] to manage your accounts, projects, and resources, you need to complete a few configuration steps to ensure the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] solution matches your organization’s needs.</span></span> <span data-ttu-id="64cf6-105">Тези стъпки включват:</span><span class="sxs-lookup"><span data-stu-id="64cf6-105">These steps include:</span></span>  
  
-   <span data-ttu-id="64cf6-106">[Задаване на единици за време](../psa/set-up-time-units.md).</span><span class="sxs-lookup"><span data-stu-id="64cf6-106">[Set up time units](../psa/set-up-time-units.md).</span></span> <span data-ttu-id="64cf6-107">Конфигуриране на единици за време в продуктовия каталог, който ще използвате като основа за планиране и фактуриране на вашите проекти.</span><span class="sxs-lookup"><span data-stu-id="64cf6-107">Configure the time units in the product catalog that you’ll use as a base for scheduling and billing your projects.</span></span>  
  
-   <span data-ttu-id="64cf6-108">[Настройване на валути и валутни курсове](../psa/set-up-currencies-exchange-rates.md).</span><span class="sxs-lookup"><span data-stu-id="64cf6-108">[Set up currencies and exchange rates](../psa/set-up-currencies-exchange-rates.md).</span></span> <span data-ttu-id="64cf6-109">Настройване на валутите, които да използвате за вашите проекти.</span><span class="sxs-lookup"><span data-stu-id="64cf6-109">Set up the currencies to use for your projects.</span></span>  
  
-   <span data-ttu-id="64cf6-110">[Създаване на организационни единици](../psa/create-organizational-units.md).</span><span class="sxs-lookup"><span data-stu-id="64cf6-110">[Create organizational units](../psa/create-organizational-units.md).</span></span> <span data-ttu-id="64cf6-111">Настройване на групи, които вашата фирма използва за разделяне на бизнеса си, независимо дали по географски признак, бизнес функция, или друго логическо разделение.</span><span class="sxs-lookup"><span data-stu-id="64cf6-111">Set up the groups that your company uses to divide its business, whether by geography, business function, or other logical division.</span></span>  
  
-   <span data-ttu-id="64cf6-112">[Задаване на честоти на фактури](../psa/set-up-invoice-frequencies.md).</span><span class="sxs-lookup"><span data-stu-id="64cf6-112">[Set up invoice frequencies](../psa/set-up-invoice-frequencies.md).</span></span> <span data-ttu-id="64cf6-113">Настройване на периоди от време, които искате да използвате за фактуриране на вашите клиенти.</span><span class="sxs-lookup"><span data-stu-id="64cf6-113">Set up time periods that you want to use for billing your clients.</span></span>  
  
-   <span data-ttu-id="64cf6-114">[Конфигуриране на категории транзакции](../psa/configure-transaction-categories.md).</span><span class="sxs-lookup"><span data-stu-id="64cf6-114">[Configure transaction categories](../psa/configure-transaction-categories.md).</span></span> <span data-ttu-id="64cf6-115">Настройване на категориите транзакции, в които вашите консултанти могат да налагат своите платими и неплатими разходи.</span><span class="sxs-lookup"><span data-stu-id="64cf6-115">Set up transaction categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="64cf6-116">[Конфигуриране на категории разходи](../psa/configure-expense-categories.md).</span><span class="sxs-lookup"><span data-stu-id="64cf6-116">[Configure expense categories](../psa/configure-expense-categories.md).</span></span> <span data-ttu-id="64cf6-117">Настройване на категориите, в които вашите консултанти могат да налагат своите платими и неплатими разходи.</span><span class="sxs-lookup"><span data-stu-id="64cf6-117">Set up the categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="64cf6-118">[Създаване на елементи в продуктов каталог](../psa/create-product-catalog-items.md).</span><span class="sxs-lookup"><span data-stu-id="64cf6-118">[Create product catalog items](../psa/create-product-catalog-items.md).</span></span> <span data-ttu-id="64cf6-119">Добавяне на продуктите, които продавате, като например софтуерни лицензи, към продуктовия каталог.</span><span class="sxs-lookup"><span data-stu-id="64cf6-119">Add the products you sell, such as software licenses, to the product catalog.</span></span>  
  
-   <span data-ttu-id="64cf6-120">[Създаване на ценова листа](../psa/create-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="64cf6-120">[Create a price list](../psa/create-price-list.md).</span></span> <span data-ttu-id="64cf6-121">Конфигуриране на различни ценови листи в зависимост от това колко искате да таксувате своите клиенти за всяка роля, която изисква техният проект.</span><span class="sxs-lookup"><span data-stu-id="64cf6-121">Configure different price lists, depending on how much you want to charge your clients for each role their project requires.</span></span>  
  
-   <span data-ttu-id="64cf6-122">[Задаване на ресурси](../psa/set-up-resources.md).</span><span class="sxs-lookup"><span data-stu-id="64cf6-122">[Set up resources](../psa/set-up-resources.md).</span></span> <span data-ttu-id="64cf6-123">Добавяне на умения, нива на професионална подготовка, роли на ресурси и друга информация за ресурсите, която ще ви трябва за вашите проекти.</span><span class="sxs-lookup"><span data-stu-id="64cf6-123">Add the skills, proficiencies, resource roles, and other resource information that you’ll need for your projects.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="64cf6-124">Вижте също</span><span class="sxs-lookup"><span data-stu-id="64cf6-124">See Also</span></span>  
 <span data-ttu-id="64cf6-125">[Преглед на Project Service Automation](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="64cf6-125">[Overview of Project Service Automation](../psa/overview.md) </span></span>  
 <span data-ttu-id="64cf6-126">[Конфигуриране на Project Service Automation](../psa/configure.md) </span><span class="sxs-lookup"><span data-stu-id="64cf6-126">[Configure Project Service Automation](../psa/configure.md) </span></span>  
 <span data-ttu-id="64cf6-127">[Ръководство за мениджъри на акаунти](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="64cf6-127">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="64cf6-128">[Ръководство за мениджъри на проекти](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="64cf6-128">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="64cf6-129">[Ръководство за мениджъри на ресурси](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="64cf6-129">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="64cf6-130">Ръководство за време, разходи и сътрудничество</span><span class="sxs-lookup"><span data-stu-id="64cf6-130">Time, Expense, and Collaboration Guid</span></span>](../psa/time-expense-collaboration-guide.md)
