---
title: Регистрирайте се за абонаменти за предварителен преглед на Project Operations за сценарии за ресурси/неналичност
description: Тази тема предоставя информация за това как да се абонирате и да внедрите Project Operations за сценарии, базирани на ресурс/неналичност.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4d35a8bf9e8a841b45808b26ae2587c5b7d99d72
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948752"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a><span data-ttu-id="98de4-103">Регистрирайте се за абонаменти за предварителен преглед на Project Operations за сценарии за ресурси/неналичност</span><span class="sxs-lookup"><span data-stu-id="98de4-103">Sign up for Project Operations preview subscriptions for resource/ non-stocked scenarios</span></span>

<span data-ttu-id="98de4-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="98de4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="98de4-105">Тази тема обяснява как да се абонирате за предварителен преглед/оферта за партньор и да внедрите среда на Project Operations за сценарии, базирани на ресурси/неналичност.</span><span class="sxs-lookup"><span data-stu-id="98de4-105">This topic explains how to subscribe to the preview/partner offer and deploy Project Operations environment for resource/ non-stocked based scenarios.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98de4-106">Предварителни изисквания</span><span class="sxs-lookup"><span data-stu-id="98de4-106">Prerequisites</span></span>

- <span data-ttu-id="98de4-107">Ще получите имейл с покана да участвате в визуализацията.</span><span class="sxs-lookup"><span data-stu-id="98de4-107">You will receive an email inviting you to participate in the preview.</span></span> <span data-ttu-id="98de4-108">Можете да поискате визуализация на [Уебсайт на Project Operations](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span><span class="sxs-lookup"><span data-stu-id="98de4-108">You can request a preview on the [Project Operations website](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span></span>
- <span data-ttu-id="98de4-109">Потребителят, който използва визуализацията, трябва да има права на глобален администратор на Клиент на Azure.</span><span class="sxs-lookup"><span data-stu-id="98de4-109">The user who deploys the preview must have Azure tenant global administrator rights.</span></span>
- <span data-ttu-id="98de4-110">Внедряването на среда на Finance изисква валиден абонамент за Azure, който ще бъде таксуван за среда.</span><span class="sxs-lookup"><span data-stu-id="98de4-110">Deploying a Finance environment requires a valid Azure subscription that will be billed per environment.</span></span> <span data-ttu-id="98de4-111">Можете да използвате съществуващия абонамент на вашите организации или да използвате [пробна версия на Azure](https://azure.microsoft.com/en-us/free/), за да започнете.</span><span class="sxs-lookup"><span data-stu-id="98de4-111">You can use your organizations existing subscription or use an [Azure trial](https://azure.microsoft.com/en-us/free/) to get started.</span></span> <span data-ttu-id="98de4-112">CDS средата ще бъде предоставена безплатно за ограничен период от 30 дни.</span><span class="sxs-lookup"><span data-stu-id="98de4-112">The CDS environment will be provided free for a limited 30 day period.</span></span>

## <a name="subscribe"></a><span data-ttu-id="98de4-113">Абониране</span><span class="sxs-lookup"><span data-stu-id="98de4-113">Subscribe</span></span>

<span data-ttu-id="98de4-114">Когато вашата [заявка за предварителен преглед](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) бъде одобрена, ще получите две оферти от Microsoft по имейл.</span><span class="sxs-lookup"><span data-stu-id="98de4-114">When your [preview request](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) is approved, you will receive two offers from Microsoft by email.</span></span> <span data-ttu-id="98de4-115">Тези предложения ви позволяват да разгърнете визуализацията на Project Operations:</span><span class="sxs-lookup"><span data-stu-id="98de4-115">These offers allow you to deploy the Project Operations Preview:</span></span>

- <span data-ttu-id="98de4-116">Dynamics 365 Project Operations – пробна версия за преглед</span><span class="sxs-lookup"><span data-stu-id="98de4-116">Dynamics 365 Project Operations – Preview Trial</span></span>
- <span data-ttu-id="98de4-117">Пробна версия за преглед на Dynamics 365 for Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="98de4-117">Dynamics 365 for Finance and Operations Preview Trial.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="98de4-118">Само един човек, администраторът на наемател, в дадена организация трябва да изпълни тази задача.</span><span class="sxs-lookup"><span data-stu-id="98de4-118">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="98de4-119">Ако не сте абонат на тази версия, изчакайте, докато организацията ви бъде регистрирана и не получите потребителските си идентификационни данни.</span><span class="sxs-lookup"><span data-stu-id="98de4-119">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>

### <a name="dynamics-365-project-operations--preview-trial"></a><span data-ttu-id="98de4-120">Dynamics 365 Project Operations – пробна версия за преглед</span><span class="sxs-lookup"><span data-stu-id="98de4-120">Dynamics 365 Project Operations – Preview trial</span></span>

1. <span data-ttu-id="98de4-121">Осребрете първата оферта, **Пробна версия на Dynamics 365 Project Operations** с URL адреса, предоставен в имейла за добре дошли.</span><span class="sxs-lookup"><span data-stu-id="98de4-121">Redeem the first offer, **Dynamics 365 Project Operations Trial**, with the URL provided in your welcome email.</span></span>

![Първа оферта](./media/1FirstOffer.png)

2. <span data-ttu-id="98de4-123">Уверете се, че сте влезли като потребител, който принадлежи към организацията, която ще се абонира за услугата.</span><span class="sxs-lookup"><span data-stu-id="98de4-123">Verify that you are logged in as the user who belongs to the organization who will be subscribing to the service.</span></span>
3. <span data-ttu-id="98de4-124">Продължете с осребряването на офертата.</span><span class="sxs-lookup"><span data-stu-id="98de4-124">Proceed with redeeming the offer.</span></span> 
4. <span data-ttu-id="98de4-125">Изберете **Да, добавете го към моя акаунт**.</span><span class="sxs-lookup"><span data-stu-id="98de4-125">Select **Yes, add it to my account**.</span></span>

![Осребряване на оферта](./media/2RedeemFirstOffer.png)

![Потвърдете офертата](./media/3ConfirmFirstOffer.png)

![Офертата е осребрена](./media/4OfferSuccessfulyRedeemed.png)

### <a name="dynamics-365-finance-preview-trial"></a><span data-ttu-id="98de4-129">Пробна версия за преглед на Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="98de4-129">Dynamics 365 Finance preview trial</span></span>

<span data-ttu-id="98de4-130">Повторете същите стъпки с втората оферта от имейла за добре дошли.</span><span class="sxs-lookup"><span data-stu-id="98de4-130">Repeat the same steps with the second offer from the Welcome email.</span></span>

## <a name="assign-licenses"></a><span data-ttu-id="98de4-131">Присвояване на лицензи</span><span class="sxs-lookup"><span data-stu-id="98de4-131">Assign Licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="98de4-132">Ще ви е необходим административен достъп до организацията на Портал на Office 365 на вашата организация, за да изпълните следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="98de4-132">You will need administrative access to your organization's Office 365 Portal to complete the following steps.</span></span>

1. <span data-ttu-id="98de4-133">Отидете на [Административен център на Microsoft 365](https://portal.office.com/), за да присвоите лицензите на вашите потребители.</span><span class="sxs-lookup"><span data-stu-id="98de4-133">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign licenses to your users.</span></span>

![Административен портал на Office](./media/5OfficeAdminPortal.png)

2. <span data-ttu-id="98de4-135">На страницата **Активни потребители** изберете потребителите, на които искате да присвоите лиценз.</span><span class="sxs-lookup"><span data-stu-id="98de4-135">On the **Active users** page, select the users that you want to assign a license to.</span></span>

![Присвояване на лицензи](./media/6AssignLicenses.png)

3. <span data-ttu-id="98de4-137">Проверете дали е избран лицензът Project Operations и изберете **Запазите промените**.</span><span class="sxs-lookup"><span data-stu-id="98de4-137">Verify that the Project Operations license has been selected and select **Save changes**.</span></span> 

> [!NOTE]
> <span data-ttu-id="98de4-138">Пробната оферта за Finance не трябва да се възлага на потребител.</span><span class="sxs-lookup"><span data-stu-id="98de4-138">The Finance trial offer does not need to be assigned to a user.</span></span>

## <a name="start-a-new-project-in-lcs"></a><span data-ttu-id="98de4-139">Стартиране на нов проект в LCS</span><span class="sxs-lookup"><span data-stu-id="98de4-139">Start a new project in LCS</span></span>

<span data-ttu-id="98de4-140">Създайте нов LCS проект, както е описано в темата [Стартирайте нов проект в LCS](create-lcs-project.md)</span><span class="sxs-lookup"><span data-stu-id="98de4-140">Create a new LCS project as described in the topic, [Start a new project in LCS](create-lcs-project.md)</span></span>

## <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="98de4-141">Добавяне на абонамент за Azure към проект на LCS</span><span class="sxs-lookup"><span data-stu-id="98de4-141">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="98de4-142">За да изпълните тази задача, следвайте стъпките в темата [Добавете абонамент за Azure към LCS проект](resource-add-azure-subscription-lcs-project.md).</span><span class="sxs-lookup"><span data-stu-id="98de4-142">To complete this task, follow the steps in the topic, [Add an Azure subscription to LCS project](resource-add-azure-subscription-lcs-project.md).</span></span>

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="98de4-143">Разгърнете демонстрационната среда на Finance с Project Operations за сценарии с ресурси/неналичност</span><span class="sxs-lookup"><span data-stu-id="98de4-143">Deploy Finance demo environment with Project Operations for resource/non-stocked scenarios</span></span>

<span data-ttu-id="98de4-144">Следвайте указанията в темата [Осигурете нова среда](resource-provision-new-environment.md) за завършване на разполагането.</span><span class="sxs-lookup"><span data-stu-id="98de4-144">Follow the guidance in the topic, [Provision a new environment](resource-provision-new-environment.md) to complete the deployment.</span></span> <span data-ttu-id="98de4-145">Използвайте [демо среда](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) тип разполагане за предварителен преглед.</span><span class="sxs-lookup"><span data-stu-id="98de4-145">Use the [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) deployment type for preview.</span></span>

## <a name="install-cds-setup-and-configuration-data"></a><span data-ttu-id="98de4-146">Инсталирайте данни за настройка и конфигурация на CDS</span><span class="sxs-lookup"><span data-stu-id="98de4-146">Install CDS setup and configuration data</span></span>

<span data-ttu-id="98de4-147">Инсталирайте CDS данни за настройка и конфигурация, както е описано в темата [Настройте и приложете конфигурационни данни в Common Data Service](resource-apply-pro-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="98de4-147">Install CDS setup and configuration data as described in the topic, [Set up and apply configuration data in the Common Data Service](resource-apply-pro-setup-config-data.md).</span></span>

