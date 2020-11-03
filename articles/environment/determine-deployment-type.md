---
title: Определяне на типа на внедряването ви
description: Тази тема предоставя информация, която да ви помогне да определите правилния тип на внедряване за Project Operations за фирмата си.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 564f2878553fe3904a7c47c7e80a3b57c763a3b2
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071824"
---
# <a name="determine-your-deployment-type"></a><span data-ttu-id="17196-103">Определяне на типа на внедряването ви</span><span class="sxs-lookup"><span data-stu-id="17196-103">Determine your deployment type</span></span>

<span data-ttu-id="17196-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="17196-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="17196-105">След като закупите лиценза, започнете оттук, за да определите най-добрия модел за внедряване на Dynamics 365 Project Operations с помощта на [Направляван поток на инсталация](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="17196-105">After you purchase the license, start here to determine the best deployment model of Dynamics 365 Project Operations using the [Guided installation flow](https://aka.ms/provisionprojectoperations).</span></span>
> <span data-ttu-id="17196-106">След като завършите ръководството за инсталиране, ще бъдете насочени към правилния портал за управление, за да завършите инсталацията си.</span><span class="sxs-lookup"><span data-stu-id="17196-106">After you have finshed the Guided installation flow, you will be directed to the correct management portal to complete your installation.</span></span> <span data-ttu-id="17196-107">Вижте подробностите за разполагане, за да завършите инсталацията.</span><span class="sxs-lookup"><span data-stu-id="17196-107">See the deployment details to complete the installation.</span></span>


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a><span data-ttu-id="17196-108">Съществуващите клиенти на Dynamics използват Dynamics 365 Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="17196-108">Existing customers of Dynamics using Dynamics 365 Project Service Automation</span></span>
<span data-ttu-id="17196-109">Project Operations включва възможностите, предоставени с Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="17196-109">Project Operations includes the capabilities that shipped with Project Service Automation.</span></span> <span data-ttu-id="17196-110">Пътека за надграждане ще бъде пусната за тези клиенти в бъдеще.</span><span class="sxs-lookup"><span data-stu-id="17196-110">An upgrade path will be released for these customers in the future.</span></span>

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a><span data-ttu-id="17196-111">Съществуващи клиенти на Dynamics 365 Finance използват управление на проекти и счетоводство</span><span class="sxs-lookup"><span data-stu-id="17196-111">Existing customers of Dynamics 365 Finance using Project management and accounting</span></span> 

<span data-ttu-id="17196-112">Съществуващите клиенти на Finance, които използват функционалността за управление на проекта и счетоводството, могат да продължат да използват това, както е.</span><span class="sxs-lookup"><span data-stu-id="17196-112">Existing customers of Finance who use the Project management and accounting functionality can continue to use this as is.</span></span> <span data-ttu-id="17196-113">Вижте [Project Operations за сценарии, базирани на наличност/поръчка за производство](#pma).</span><span class="sxs-lookup"><span data-stu-id="17196-113">See [Project Operations for stocked/production order scenarios](#pma).</span></span>


## <a name="deployment-types"></a><span data-ttu-id="17196-114">Типове внедряване</span><span class="sxs-lookup"><span data-stu-id="17196-114">Deployment types</span></span>
<span data-ttu-id="17196-115">Project Operations поддържа множество опции за разполагане, за да отговарят на вашите изисквания.</span><span class="sxs-lookup"><span data-stu-id="17196-115">Project Operations supports multiple deployment options to match your requirements.</span></span> <span data-ttu-id="17196-116">Независимо дали сте нов или съществуващ клиент на Dynamics 365, Project Operations може да поддържа вашите нужди.</span><span class="sxs-lookup"><span data-stu-id="17196-116">Whether you're a new or existing Dynamics 365 customer, Project Operations can support your needs.</span></span>

<span data-ttu-id="17196-117">Нашият [Въпросник за разполагане](https://aka.ms/provisionprojectoperations) ще ви помогне да определите правилното внедряване.</span><span class="sxs-lookup"><span data-stu-id="17196-117">Our [Deployment questionnaire](https://aka.ms/provisionprojectoperations) will help you determine the right deployment.</span></span> <span data-ttu-id="17196-118">Резултатите ще ви насочат към един от следните типове внедряване:</span><span class="sxs-lookup"><span data-stu-id="17196-118">The results will guide you toward one of the following deployment types:</span></span>

- [<span data-ttu-id="17196-119">Леко внедряване – фактуриране на сделката към проформа</span><span class="sxs-lookup"><span data-stu-id="17196-119">Lite deployment – deal to proforma invoicing</span></span>](#lite)
- [<span data-ttu-id="17196-120">Project Operations за сценарии, базирани на ресурси/неналичност</span><span class="sxs-lookup"><span data-stu-id="17196-120">Project Operations for resource/non-stocked scenarios</span></span>](#integrated)
- [<span data-ttu-id="17196-121">Project Operations за сценарии, базирани на наличност/поръчка за производство</span><span class="sxs-lookup"><span data-stu-id="17196-121">Project Operations for stocked/production order scenarios</span></span>](#pma)

<span data-ttu-id="17196-122">Project Operations поддържа сценарии за складирани / производствени поръчки и нескладирани / базирани на ресурси сценарии в същата среда чрез конфигурации на ниво юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="17196-122">Project Operations support stocked/production order scenarios and non-stocked/resource-based scenarios on the same environment through legal entity-level configurations.</span></span> <span data-ttu-id="17196-123">Например Contoso може да използва възможностите за складиране / производствени поръчки в своето производствено съоръжение в САЩ (юридическо лице = Contoso Manufacturing United States).</span><span class="sxs-lookup"><span data-stu-id="17196-123">For example, Contoso can use the stocked/production order capabilities in their US manufacturing facility (Legal entity = Contoso Manufacturing United States).</span></span> <span data-ttu-id="17196-124">Contoso може да използва нескладовите / базирани на ресурси възможности в тяхното съоръжение за обслужване на Contoso Robotics Arms в Обединеното кралство (юридическо лице = Contoso Robotics United Kingdom).</span><span class="sxs-lookup"><span data-stu-id="17196-124">Contoso can use the non-stocked/resource-based capabilities in their Contoso Robotics Arms servicing facility in UK (Legal entity = Contoso Robotics United Kingdom).</span></span>

### <a name="lite-deployment---deal-to-proforma-invoicing"></a><a  name="lite"></a><span data-ttu-id="17196-125">Леко внедряване – фактуриране на сделката към проформа</span><span class="sxs-lookup"><span data-stu-id="17196-125">Lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="17196-126">Вграденото внедряване включва следните възможности:</span><span class="sxs-lookup"><span data-stu-id="17196-126">The lite deployment includes the following capabilities:</span></span>

- <span data-ttu-id="17196-127">Планиране на проекти с помощта на Microsoft Project за мрежата</span><span class="sxs-lookup"><span data-stu-id="17196-127">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="17196-128">Многоизмерно ценообразуване</span><span class="sxs-lookup"><span data-stu-id="17196-128">Multi-dimensional pricing</span></span>
- <span data-ttu-id="17196-129">Унифицирано управление на ресурси</span><span class="sxs-lookup"><span data-stu-id="17196-129">Unified Resource Management</span></span>
- <span data-ttu-id="17196-130">Проследяване на време</span><span class="sxs-lookup"><span data-stu-id="17196-130">Time Tracking</span></span>
- <span data-ttu-id="17196-131">Основни разходи</span><span class="sxs-lookup"><span data-stu-id="17196-131">Basic Expense</span></span>
- <span data-ttu-id="17196-132">Предложение за фактура</span><span class="sxs-lookup"><span data-stu-id="17196-132">Invoice Proposal</span></span>

#### <a name="deployment-steps"></a><span data-ttu-id="17196-133">Стъпки на внедряването</span><span class="sxs-lookup"><span data-stu-id="17196-133">Deployment steps</span></span>
<span data-ttu-id="17196-134">Определете най-добрия модел за внедряване на Project Operations с помощта на [Въпросник за разполагане](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="17196-134">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="17196-135">За това разполагане вижте [Регистрация за абонаменти за предварителен преглед](lite-preview-subscription-sign-up.md) и [Осигуряване на нова среда](lite-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="17196-135">For this deployment, see [Sign-up for preview subscriptions](lite-preview-subscription-sign-up.md) and [Provision new environment](lite-deployment.md).</span></span> 


### <a name="project-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"></a><span data-ttu-id="17196-136">Project Operations за сценарии, базирани на ресурси/неналичност</span><span class="sxs-lookup"><span data-stu-id="17196-136">Project Operations for resource/non-stocked scenarios</span></span>
<span data-ttu-id="17196-137">Project Operations за сценарии с ресурси / не складирани включват следните възможности:</span><span class="sxs-lookup"><span data-stu-id="17196-137">The Project Operations for resource/non-stocked scenarios includes the following capabilities:</span></span>
  
- <span data-ttu-id="17196-138">Планиране на проекти с помощта на Microsoft Project за мрежата</span><span class="sxs-lookup"><span data-stu-id="17196-138">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="17196-139">Многоизмерно ценообразуване</span><span class="sxs-lookup"><span data-stu-id="17196-139">Multi-dimensional pricing</span></span>
- <span data-ttu-id="17196-140">Унифицирано управление на ресурси</span><span class="sxs-lookup"><span data-stu-id="17196-140">Unified Resource Management</span></span>
- <span data-ttu-id="17196-141">Проследяване на време</span><span class="sxs-lookup"><span data-stu-id="17196-141">Time Tracking</span></span>
- <span data-ttu-id="17196-142">Основни разходи</span><span class="sxs-lookup"><span data-stu-id="17196-142">Basic Expense</span></span>
- <span data-ttu-id="17196-143">Пълен разход</span><span class="sxs-lookup"><span data-stu-id="17196-143">Full Expense</span></span>
- <span data-ttu-id="17196-144">OCR на разписка</span><span class="sxs-lookup"><span data-stu-id="17196-144">Receipt OCR</span></span>
- <span data-ttu-id="17196-145">Пълно фактуриране</span><span class="sxs-lookup"><span data-stu-id="17196-145">Full Invoicing</span></span>
- <span data-ttu-id="17196-146">Признаване на приходите</span><span class="sxs-lookup"><span data-stu-id="17196-146">Revenue Recognition</span></span>

#### <a name="deployment-steps"></a><span data-ttu-id="17196-147">Стъпки на внедряването</span><span class="sxs-lookup"><span data-stu-id="17196-147">Deployment steps</span></span>
<span data-ttu-id="17196-148">Определете най-добрия модел за внедряване на Project Operations с помощта на [Въпросник за разполагане](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="17196-148">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="17196-149">За това разполагане вижте [Регистрация за абонаменти за предварителен преглед](resource-sign-up-preview-subscription.md) и [Осигуряване на нова среда](resource-provision-new-environment.md).</span><span class="sxs-lookup"><span data-stu-id="17196-149">For this deployment, see [Sign-up for preview subscriptions](resource-sign-up-preview-subscription.md) and [Provision new environment](resource-provision-new-environment.md).</span></span> 


### <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a><span data-ttu-id="17196-150">Project Operations за сценарии, базирани на наличност/поръчка за производство</span><span class="sxs-lookup"><span data-stu-id="17196-150">Project Operations for stocked/production order scenarios</span></span>

- <span data-ttu-id="17196-151">Планиране на проект с помощта на ССР</span><span class="sxs-lookup"><span data-stu-id="17196-151">Project planning using WBS</span></span>
- <span data-ttu-id="17196-152">Управление на ресурс</span><span class="sxs-lookup"><span data-stu-id="17196-152">Resource Management</span></span>
- <span data-ttu-id="17196-153">Проследяване на време</span><span class="sxs-lookup"><span data-stu-id="17196-153">Time Tracking</span></span>
- <span data-ttu-id="17196-154">Пълен разход</span><span class="sxs-lookup"><span data-stu-id="17196-154">Full Expense</span></span>
- <span data-ttu-id="17196-155">OCR на разписка</span><span class="sxs-lookup"><span data-stu-id="17196-155">Receipt OCR</span></span>
- <span data-ttu-id="17196-156">Пълно фактуриране</span><span class="sxs-lookup"><span data-stu-id="17196-156">Full Invoicing</span></span>
- <span data-ttu-id="17196-157">Признаване на приходите</span><span class="sxs-lookup"><span data-stu-id="17196-157">Revenue Recognition</span></span>
- <span data-ttu-id="17196-158">Производствени поръчки</span><span class="sxs-lookup"><span data-stu-id="17196-158">Production Orders</span></span>
- <span data-ttu-id="17196-159">Поддръжка на материали</span><span class="sxs-lookup"><span data-stu-id="17196-159">Materials support</span></span>

#### <a name="deployment-steps"></a><span data-ttu-id="17196-160">Стъпки на внедряването</span><span class="sxs-lookup"><span data-stu-id="17196-160">Deployment steps</span></span>
<span data-ttu-id="17196-161">Определете най-добрия модел за внедряване на Project Operations с помощта на [Въпросник за разполагане](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="17196-161">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="17196-162">За това разполагане вижте [Регистрация за абонаменти за предварителен преглед](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) и [Осигуряване на нова среда](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json).</span><span class="sxs-lookup"><span data-stu-id="17196-162">For this deployment, see [Sign-up for preview subscriptions](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) and [Provision new environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json).</span></span> 

