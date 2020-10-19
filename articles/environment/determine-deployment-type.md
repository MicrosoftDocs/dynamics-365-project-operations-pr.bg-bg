---
title: Типове внедряване
description: Тази тема предоставя информация, която да ви помогне да определите правилния тип на внедряване за Project Operations за фирмата си.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: c3cf378caae4510482a8ee6771bf2e6decfe3b48
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948748"
---
# <a name="deployment-types"></a><span data-ttu-id="73de7-103">Типове внедряване</span><span class="sxs-lookup"><span data-stu-id="73de7-103">Deployment types</span></span>

<span data-ttu-id="73de7-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="73de7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="73de7-105">След като закупите лиценза, започнете оттук, за да определите най-добрия модел за внедряване на Dynamics 365 Project Operations с помощта на [Направляван поток на инсталация](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="73de7-105">After you purchase the license, start here to determine the best deployment model of Dynamics 365 Project Operations using the [Guided installation flow](https://aka.ms/provisionprojectoperations).</span></span>
> <span data-ttu-id="73de7-106">След като завършите ръководството за инсталиране, ще бъдете насочени към правилния портал за управление, за да завършите инсталацията си.</span><span class="sxs-lookup"><span data-stu-id="73de7-106">After you have finshed the Guided installation flow, you will be directed to the correct management portal to complete your installation.</span></span> <span data-ttu-id="73de7-107">Вижте подробностите за разполагане по-долу, за да завършите инсталацията.</span><span class="sxs-lookup"><span data-stu-id="73de7-107">See the deployment details below to complete the installation.</span></span>


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a><span data-ttu-id="73de7-108">Съществуващите клиенти на Dynamics използват Dynamics 365 Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="73de7-108">Existing customers of Dynamics using Dynamics 365 Project Service Automation</span></span>
<span data-ttu-id="73de7-109">Project Operations включва възможностите, предоставени с Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="73de7-109">Project Operations includes the capabilities that shipped with Project Service Automation.</span></span> <span data-ttu-id="73de7-110">Пътека за надграждане ще бъде пусната за тези клиенти в бъдеще.</span><span class="sxs-lookup"><span data-stu-id="73de7-110">An upgrade path will be released for these customers in the future.</span></span>

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a><span data-ttu-id="73de7-111">Съществуващи клиенти на Dynamics 365 Finance използват управление на проекти и счетоводство</span><span class="sxs-lookup"><span data-stu-id="73de7-111">Existing customers of Dynamics 365 Finance using Project management and accounting</span></span> 

<span data-ttu-id="73de7-112">Съществуващите клиенти на Finance, които използват функционалността за управление на проекта и счетоводството, могат да продължат да използват това, както е.</span><span class="sxs-lookup"><span data-stu-id="73de7-112">Existing customers of Finance who use the Project management and accounting functionality can continue use this as is.</span></span> <span data-ttu-id="73de7-113">Вижте [Project Operations за сценарии, базирани на наличност/поръчка за производство](#pma).</span><span class="sxs-lookup"><span data-stu-id="73de7-113">See [Project Operations for stocked/production order scenarios](#pma).</span></span>

<span data-ttu-id="73de7-114">Project Operations поддържа множество опции за разполагане, за да отговарят на вашите изисквания.</span><span class="sxs-lookup"><span data-stu-id="73de7-114">Project Operations supports multiple deployment options to match your requirements.</span></span> <span data-ttu-id="73de7-115">Независимо дали сте нов или съществуващ клиент на Dynamics 365, Project Operations може да поддържа вашите нужди.</span><span class="sxs-lookup"><span data-stu-id="73de7-115">Whether you are a new or existing Dynamics 365 customer, Project Operations can support your needs.</span></span>

<span data-ttu-id="73de7-116">Нашият [Въпросник за разполагане](https://aka.ms/provisionprojectoperations) ще ви помогне да определите правилното внедряване.</span><span class="sxs-lookup"><span data-stu-id="73de7-116">Our [Deployment questionnaire](https://aka.ms/provisionprojectoperations) will help you determine the right deployment.</span></span> <span data-ttu-id="73de7-117">Резултатите ще ви насочат към един от следните типове внедряване:</span><span class="sxs-lookup"><span data-stu-id="73de7-117">The results will guide you toward one of the following deployment types:</span></span>

- [<span data-ttu-id="73de7-118">Леко внедряване – фактуриране на сделката към проформа</span><span class="sxs-lookup"><span data-stu-id="73de7-118">Lite deployment – deal to proforma invoicing</span></span>](#lite)
- [<span data-ttu-id="73de7-119">Project Operations за сценарии, базирани на ресурси/неналичност</span><span class="sxs-lookup"><span data-stu-id="73de7-119">Project Operations for resource/non-stocked scenarios</span></span>](#integrated)
- [<span data-ttu-id="73de7-120">Project Operations за сценарии, базирани на наличност/поръчка за производство</span><span class="sxs-lookup"><span data-stu-id="73de7-120">Project Operations for stocked/production order scenarios</span></span>](#pma)

<span data-ttu-id="73de7-121">Project Operations поддържа сценарии за складирани / производствени поръчки и нескладирани / базирани на ресурси сценарии в същата среда чрез конфигурации на ниво юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="73de7-121">Project Operations support stocked/production order scenarios and non-stocked/resource-based scenarios on the same environment through legal entity-level configurations.</span></span> <span data-ttu-id="73de7-122">Например Contoso може да се възползва от възможностите за складиране / производствени поръчки в тяхното производствено съоръжение в САЩ (Юридическо лице = Contoso Manufacturing Съединени щати) и нескладови / базирани на ресурси възможности в сервиза си за обслужване Contoso Robotics Arms в Обединеното кралство (Юридическо лице = Contoso Robotics Обединено кралство).</span><span class="sxs-lookup"><span data-stu-id="73de7-122">For example, Contoso can leverage stocked/production order capabilities in their US manufacturing facility (Legal entity = Contoso Manufacturing United States) and non-stocked/resource-based capabilities in their Contoso Robotics Arms servicing facility in UK (Legal entity = Contoso Robotics United Kingdom).</span></span>

## <a name="a-namelitelite-deployment---deal-to-proforma-invoicing"></a><span data-ttu-id="73de7-123"><a name="lite"><a/>Леко внедряване – фактуриране на сделката към проформа</span><span class="sxs-lookup"><span data-stu-id="73de7-123"><a name="lite"><a/>Lite deployment - deal to proforma invoicing</span></span>
<span data-ttu-id="73de7-124">Вграденото внедряване включва следните възможности:</span><span class="sxs-lookup"><span data-stu-id="73de7-124">The lite deployment includes the following capabilities:</span></span>

- <span data-ttu-id="73de7-125">Планиране на проекти с помощта на Microsoft Project за мрежата</span><span class="sxs-lookup"><span data-stu-id="73de7-125">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="73de7-126">Многоизмерно ценообразуване</span><span class="sxs-lookup"><span data-stu-id="73de7-126">Multi-dimensional pricing</span></span>
- <span data-ttu-id="73de7-127">Унифицирано управление на ресурси</span><span class="sxs-lookup"><span data-stu-id="73de7-127">Unified Resource Management</span></span>
- <span data-ttu-id="73de7-128">Проследяване на време</span><span class="sxs-lookup"><span data-stu-id="73de7-128">Time Tracking</span></span>
- <span data-ttu-id="73de7-129">Основни разходи</span><span class="sxs-lookup"><span data-stu-id="73de7-129">Basic Expense</span></span>
- <span data-ttu-id="73de7-130">Предложение за фактура</span><span class="sxs-lookup"><span data-stu-id="73de7-130">Invoice Proposal</span></span>

### <a name="deployment-steps"></a><span data-ttu-id="73de7-131">Стъпки на внедряването:</span><span class="sxs-lookup"><span data-stu-id="73de7-131">Deployment steps:</span></span>
<span data-ttu-id="73de7-132">Определете най-добрия модел за внедряване на Project Operations с помощта на [Въпросник за разполагане](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="73de7-132">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="73de7-133">За това разполагане вижте [Регистрация за абонаменти за предварителен преглед](lite-preview-subscription-sign-up.md) и [Осигуряване на нова среда](lite-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="73de7-133">For this deployment, see [Sign-up for preview subscriptions](lite-preview-subscription-sign-up.md) and [Provision new environment](lite-deployment.md).</span></span> 


## <a name="a-nameintegratedproject-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="73de7-134"><a name="integrated"><a/>Project Operations за сценарии, базирани на ресурси/неналичност</span><span class="sxs-lookup"><span data-stu-id="73de7-134"><a name="integrated"><a/>Project Operations for resource/non-stocked scenarios</span></span>
<span data-ttu-id="73de7-135">Project Operations за сценарии с ресурси / не складирани включват следните възможности:</span><span class="sxs-lookup"><span data-stu-id="73de7-135">The Project Operations for resource/non-stocked scenarios includes the following capabilities:</span></span>
  
- <span data-ttu-id="73de7-136">Планиране на проекти с помощта на Microsoft Project за мрежата</span><span class="sxs-lookup"><span data-stu-id="73de7-136">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="73de7-137">Многоизмерно ценообразуване</span><span class="sxs-lookup"><span data-stu-id="73de7-137">Multi-dimensional pricing</span></span>
- <span data-ttu-id="73de7-138">Унифицирано управление на ресурси</span><span class="sxs-lookup"><span data-stu-id="73de7-138">Unified Resource Management</span></span>
- <span data-ttu-id="73de7-139">Проследяване на време</span><span class="sxs-lookup"><span data-stu-id="73de7-139">Time Tracking</span></span>
- <span data-ttu-id="73de7-140">Основни разходи</span><span class="sxs-lookup"><span data-stu-id="73de7-140">Basic Expense</span></span>
- <span data-ttu-id="73de7-141">Пълен разход</span><span class="sxs-lookup"><span data-stu-id="73de7-141">Full Expense</span></span>
- <span data-ttu-id="73de7-142">OCR на разписка</span><span class="sxs-lookup"><span data-stu-id="73de7-142">Receipt OCR</span></span>
- <span data-ttu-id="73de7-143">Пълно фактуриране</span><span class="sxs-lookup"><span data-stu-id="73de7-143">Full Invoicing</span></span>
- <span data-ttu-id="73de7-144">Признаване на приходите</span><span class="sxs-lookup"><span data-stu-id="73de7-144">Revenue Recognition</span></span>

### <a name="deployment-steps"></a><span data-ttu-id="73de7-145">Стъпки на внедряването:</span><span class="sxs-lookup"><span data-stu-id="73de7-145">Deployment steps:</span></span>
<span data-ttu-id="73de7-146">Определете най-добрия модел за внедряване на Project Operations с помощта на [Въпросник за разполагане](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="73de7-146">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="73de7-147">За това разполагане вижте [Регистрация за абонаменти за предварителен преглед](resource-sign-up-preview-subscription.md) и [Осигуряване на нова среда](resource-provision-new-environment.md).</span><span class="sxs-lookup"><span data-stu-id="73de7-147">For this deployment, see [Sign-up for preview subscriptions](resource-sign-up-preview-subscription.md) and [Provision new environment](resource-provision-new-environment.md).</span></span> 


## <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a><span data-ttu-id="73de7-148">Project Operations за сценарии, базирани на наличност/поръчка за производство</span><span class="sxs-lookup"><span data-stu-id="73de7-148">Project Operations for stocked/production order scenarios</span></span>

- <span data-ttu-id="73de7-149">Планиране на проект с помощта на ССР</span><span class="sxs-lookup"><span data-stu-id="73de7-149">Project planning using WBS</span></span>
- <span data-ttu-id="73de7-150">Управление на ресурс</span><span class="sxs-lookup"><span data-stu-id="73de7-150">Resource Management</span></span>
- <span data-ttu-id="73de7-151">Проследяване на време</span><span class="sxs-lookup"><span data-stu-id="73de7-151">Time Tracking</span></span>
- <span data-ttu-id="73de7-152">Пълен разход</span><span class="sxs-lookup"><span data-stu-id="73de7-152">Full Expense</span></span>
- <span data-ttu-id="73de7-153">OCR на разписка</span><span class="sxs-lookup"><span data-stu-id="73de7-153">Receipt OCR</span></span>
- <span data-ttu-id="73de7-154">Пълно фактуриране</span><span class="sxs-lookup"><span data-stu-id="73de7-154">Full Invoicing</span></span>
- <span data-ttu-id="73de7-155">Признаване на приходите</span><span class="sxs-lookup"><span data-stu-id="73de7-155">Revenue Recognition</span></span>
- <span data-ttu-id="73de7-156">Производствени поръчки</span><span class="sxs-lookup"><span data-stu-id="73de7-156">Production Orders</span></span>
- <span data-ttu-id="73de7-157">Поддръжка на материали</span><span class="sxs-lookup"><span data-stu-id="73de7-157">Materials support</span></span>

### <a name="deployment-steps"></a><span data-ttu-id="73de7-158">Стъпки на внедряването:</span><span class="sxs-lookup"><span data-stu-id="73de7-158">Deployment steps:</span></span>
<span data-ttu-id="73de7-159">Определете най-добрия модел за внедряване на Project Operations с помощта на [Въпросник за разполагане](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="73de7-159">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="73de7-160">За това разполагане вижте [Регистрация за абонаменти за предварителен преглед](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) и [Осигуряване на нова среда](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json).</span><span class="sxs-lookup"><span data-stu-id="73de7-160">For this deployment, see [Sign-up for preview subscriptions](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) and [Provision new environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json).</span></span> 



