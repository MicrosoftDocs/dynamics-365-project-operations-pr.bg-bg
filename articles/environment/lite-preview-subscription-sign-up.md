---
title: Регистриране за абонамент за преглед
description: Тази тема предоставя информация за това как да се абонирате и разгърнете внедряване на Project Operations lite - сделка за проформа фактуриране.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5342466f308ab62a9f73a85fbd838d7c33bb1f47
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071683"
---
# <a name="sign-up-for-a-preview-subscription-for-lite-deployment--deal-to-proforma-invoicing"></a><span data-ttu-id="4650c-103">Регистрирайте се за предварителен абонамент за опростено внедряване - сключете проформа за фактуриране</span><span class="sxs-lookup"><span data-stu-id="4650c-103">Sign up for a preview subscription for lite deployment – deal to proforma invoicing</span></span>

<span data-ttu-id="4650c-104">Тази тема обяснява как да се абонирате за предложението на партньора за преглед и да внедрите Dynamics 365 Project Operations lite - сделка за проформа фактуриране.</span><span class="sxs-lookup"><span data-stu-id="4650c-104">This topic explains how to subscribe to the preview partner offer and deploy Dynamics 365 Project Operations lite deployment - deal to proforma invoicing.</span></span>

> [!NOTE]
> <span data-ttu-id="4650c-105">Този процес ще се промени в предстоящите версии на Project Operations.</span><span class="sxs-lookup"><span data-stu-id="4650c-105">This process will change in upcoming releases of Project Operations.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4650c-106">Предварителни изисквания</span><span class="sxs-lookup"><span data-stu-id="4650c-106">Prerequisites</span></span>

- <span data-ttu-id="4650c-107">Ще получите имейл с покана да участвате в визуализацията.</span><span class="sxs-lookup"><span data-stu-id="4650c-107">You'll receive an email inviting you to participate in the preview.</span></span> <span data-ttu-id="4650c-108">Можете да поискате визуализация на [Уебсайт на Project Operations](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span><span class="sxs-lookup"><span data-stu-id="4650c-108">You can request a preview on the [Project Operations website](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span></span>
- <span data-ttu-id="4650c-109">Потребителят, който използва визуализацията, трябва да има права на глобален администратор на Клиент на Azure.</span><span class="sxs-lookup"><span data-stu-id="4650c-109">The user who deploys the preview must have Azure tenant global administrator rights.</span></span>
- <span data-ttu-id="4650c-110">Прегледайте всички условия.</span><span class="sxs-lookup"><span data-stu-id="4650c-110">Review all terms and conditions.</span></span>

## <a name="subscribe"></a><span data-ttu-id="4650c-111">Абониране</span><span class="sxs-lookup"><span data-stu-id="4650c-111">Subscribe</span></span>

<span data-ttu-id="4650c-112">Когато получите одобрение за [заявка за предварителен преглед](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u), ще получите две оферти от Microsoft по имейл.</span><span class="sxs-lookup"><span data-stu-id="4650c-112">When you receive a [preview request](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) approval, you'll receive two offers from Microsoft by email.</span></span> <span data-ttu-id="4650c-113">Тези предложения ви позволяват да разгърнете визуализацията на Project Operations:</span><span class="sxs-lookup"><span data-stu-id="4650c-113">These offers allow you to deploy the Project Operations Preview:</span></span>

- <span data-ttu-id="4650c-114">Dynamics 365 Project Operations (CRM) – пробна версия за преглед</span><span class="sxs-lookup"><span data-stu-id="4650c-114">Dynamics 365 Project Operations (CRM) - Preview Trial</span></span>
- <span data-ttu-id="4650c-115">Office 365 Project Operations - Пробна версия за преглед</span><span class="sxs-lookup"><span data-stu-id="4650c-115">Office 365 Project Operations - Preview Trial</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4650c-116">Само един човек, администраторът на наемател, в дадена организация трябва да изпълни тази задача.</span><span class="sxs-lookup"><span data-stu-id="4650c-116">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="4650c-117">Ако не сте абонат на тази версия, изчакайте, докато организацията ви бъде регистрирана и не получите потребителските си идентификационни данни.</span><span class="sxs-lookup"><span data-stu-id="4650c-117">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>

### <a name="dynamics-365-project-operations-crm---preview-trial"></a><span data-ttu-id="4650c-118">Dynamics 365 Project Operations (CRM) – пробна версия за преглед</span><span class="sxs-lookup"><span data-stu-id="4650c-118">Dynamics 365 Project Operations (CRM) - Preview Trial</span></span> 

<span data-ttu-id="4650c-119">Преди да започнете, уверете се, че сте влезли в браузър с потребителския работен акаунт в наемателя, където искате визуализация на Project Operations.</span><span class="sxs-lookup"><span data-stu-id="4650c-119">Before you begin, make sure you are logged in to a browser with the user work account in the tenant where you want the Project Operations preview.</span></span>

1. <span data-ttu-id="4650c-120">Осребрете първия код на офертата, **Dynamics 365 Project Operations (CRM) - Преглед на пробен период** като го поставите в URL адреса на браузъра.</span><span class="sxs-lookup"><span data-stu-id="4650c-120">Redeem the first offer code, **Dynamics 365 Project Operations (CRM) - Preview Trial** by pasting it into the browser URL.</span></span>

![Осребряване на оферта](./media/16RedeemFirstOfferNew.png)

2. <span data-ttu-id="4650c-122">Потвърдете поръчката си.</span><span class="sxs-lookup"><span data-stu-id="4650c-122">Confirm your order.</span></span>
<span data-ttu-id="4650c-123">![Потвърждаване на поръчката](./media/17ConfirmOrderNew.png)</span><span class="sxs-lookup"><span data-stu-id="4650c-123">![Confirm the order](./media/17ConfirmOrderNew.png)</span></span>

<span data-ttu-id="4650c-124">Ще видите, че офертата за потвърждение е осребрена успешно.</span><span class="sxs-lookup"><span data-stu-id="4650c-124">You'll see confirmation offer was successfully redeemed.</span></span>

![Потвърждение](./media/18OrderConfirmationNew.png)

### <a name="office-365-project-operations---preview-trial"></a><span data-ttu-id="4650c-126">Office 365 Project Operations - Пробна версия за преглед</span><span class="sxs-lookup"><span data-stu-id="4650c-126">Office 365 Project Operations - Preview Trial</span></span>

<span data-ttu-id="4650c-127">Повторете същите стъпки като при първия код на офертата.</span><span class="sxs-lookup"><span data-stu-id="4650c-127">Repeat the same steps as with the first offer code.</span></span> <span data-ttu-id="4650c-128">Не забравяйте да добавите втория код на офертата, като използвате същия потребителски акаунт, който е използван с първия код на офертата.</span><span class="sxs-lookup"><span data-stu-id="4650c-128">Make sure to add the second offer code using the same user account that was used with the first offer code.</span></span>

## <a name="assign-licenses"></a><span data-ttu-id="4650c-129">Присвояване на лиценз</span><span class="sxs-lookup"><span data-stu-id="4650c-129">Assign licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4650c-130">Ще ви е необходим административен достъп до организацията на Портал на Microsoft 365 на вашата организация, за да изпълните следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="4650c-130">You will need administrative access to your organization's Microsoft 365 Portal to complete the following steps.</span></span>


1. <span data-ttu-id="4650c-131">Отидете на [Административен център на Microsoft 365](https://portal.office.com/), за да присвоите лицензите на вашите потребители.</span><span class="sxs-lookup"><span data-stu-id="4650c-131">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign the licenses to your users.</span></span>

![Начална страница на център за администрация](./media/14AdminPortal.png)

2. <span data-ttu-id="4650c-133">На страницата **Активни потребители** изберете потребителите, на които искате да присвоите лиценз.</span><span class="sxs-lookup"><span data-stu-id="4650c-133">On the **Active users** page, select the users that you want to assign a license to.</span></span>

![Присвояване на лицензи](./media/15AssignLicenses.png)

3. <span data-ttu-id="4650c-135">Проверете дали **Преглед на Dynamics 365 Project Operations (CRM)** и **Office 365 Project Operations - Преглед** лицензите са избрани.</span><span class="sxs-lookup"><span data-stu-id="4650c-135">Verify that the **Dynamics 365 Project Operations (CRM) Preview** and **Office 365 Project Operations - Preview** licenses are selected.</span></span> 
4. <span data-ttu-id="4650c-136">Изберете **Записване на промените**.</span><span class="sxs-lookup"><span data-stu-id="4650c-136">Select **Save changes**.</span></span>

## <a name="create-a-new-cds-environment"></a><span data-ttu-id="4650c-137">Създаване на нова среда на CDS</span><span class="sxs-lookup"><span data-stu-id="4650c-137">Create a new CDS environment</span></span>

1. <span data-ttu-id="4650c-138">Осигурете нова среда за внедряване на CDS за Project Operations, като следвате инструкциите в темата, [Модел за внедряване на CDS](lite-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="4650c-138">Provision a new Project Operations CDS deployment environment by following instructions in the topic, [CDS deployment model](lite-deployment.md).</span></span> <span data-ttu-id="4650c-139">Когато изберете типа среда, не забравяйте да използвате **Пробен период (базиран на абонамент)**.</span><span class="sxs-lookup"><span data-stu-id="4650c-139">When you select the environment type, make sure to use **Trial (Subscription based)**.</span></span>
<span data-ttu-id="4650c-140">![Нова среда](./media/19CreateEnvironment.png)</span><span class="sxs-lookup"><span data-stu-id="4650c-140">![New environment](./media/19CreateEnvironment.png)</span></span>

2. <span data-ttu-id="4650c-141">Изберете **Активирайте приложенията на Dynamics 365** настройка и оставете **Автоматично внедряване на тези приложения** празно.</span><span class="sxs-lookup"><span data-stu-id="4650c-141">Select the **Enable Dynamics 365 apps** setting, and leave **Automatically deploy these apps** blank.</span></span>  
3. <span data-ttu-id="4650c-142">Изберете **Запиши** , за да създадете средата.</span><span class="sxs-lookup"><span data-stu-id="4650c-142">Select **Save** to create the environment.</span></span>

![Добавяне на база данни](./media/20CreateEnvironment1.png)

4. <span data-ttu-id="4650c-144">След като средата е създадена, инсталирайте **Microsoft Dynamics 365 Project Operations** решение.</span><span class="sxs-lookup"><span data-stu-id="4650c-144">After the environment is created, install **Microsoft Dynamics 365 Project Operations** solution.</span></span> 

![Инсталиране на решение](./media/21InstallSolution.png)

## <a name="install-a-cds-configuration-and-setup-demo-data"></a><span data-ttu-id="4650c-146">Инсталирайте конфигурация на CDS и настройте демонстрационни данни</span><span class="sxs-lookup"><span data-stu-id="4650c-146">Install a CDS configuration and setup demo data</span></span>

<span data-ttu-id="4650c-147">Инсталирайте конфигурацията на CDS и настройте демонстрационни данни, като следвате инструкциите в темата, [Приложете демо настройка и данни за конфигурация](lite-apply-demo-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="4650c-147">Install the CDS configuration and set up demo data by following instructions in the topic, [Apply demo setup and configuration data](lite-apply-demo-setup-config-data.md).</span></span>
