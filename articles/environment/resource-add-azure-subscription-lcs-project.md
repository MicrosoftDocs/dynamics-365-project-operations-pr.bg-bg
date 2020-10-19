---
title: Добавяне на абонамент за Azure към проект на LCS
description: Тази тема предоставя информация за това как да свържете абонамента си за Azure с LCS проект.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 0b5703542ac58adcc710890d9676dd0090a82f25
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948751"
---
# <a name="add-an-azure-subscription-to-lcs-project"></a><span data-ttu-id="b0408-103">Добавяне на абонамент за Azure към проект на LCS</span><span class="sxs-lookup"><span data-stu-id="b0408-103">Add an Azure subscription to LCS project</span></span>

<span data-ttu-id="b0408-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="b0408-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="b0408-105">Облачно хостваните среди трябва да бъдат разположени с помощта на съществуващ абонамент за Azure.</span><span class="sxs-lookup"><span data-stu-id="b0408-105">Cloud-hosted environments must be deployed using an existing Azure subscription.</span></span> <span data-ttu-id="b0408-106">Тази тема обяснява как свържете съществуващ абонамент в Azure с проект на LCS.</span><span class="sxs-lookup"><span data-stu-id="b0408-106">This topic explains how to connect your existing Azure subscription to an LCS project.</span></span> 

## <a name="grant-admin-consent"></a><span data-ttu-id="b0408-107">Предоставяне на съгласие на администратора</span><span class="sxs-lookup"><span data-stu-id="b0408-107">Grant admin consent</span></span>

1. <span data-ttu-id="b0408-108">Във вашия LCS проект, в раздела **Среда** изберете **Настройки на Microsoft Azure**.</span><span class="sxs-lookup"><span data-stu-id="b0408-108">In your LCS project, in the **Environments** section, select **Microsoft Azure settings**.</span></span>

![Настройки на Microsoft Azure](./media/1MicrosoftAzureSettings.png)

2. <span data-ttu-id="b0408-110">На страницата **Настройки на проекта** на раздела **Конектори на Azure** изберете **Удостоверяване**.</span><span class="sxs-lookup"><span data-stu-id="b0408-110">On the **Project settings** page, on the **Azure connectors** tab, select **Authorize**.</span></span> <span data-ttu-id="b0408-111">Това позволява средите да бъдат разположени в този проект.</span><span class="sxs-lookup"><span data-stu-id="b0408-111">This allows environments to be deployed to this project.</span></span>

![Конектори на Azure](./media/2AzureConnectors.png)

3. <span data-ttu-id="b0408-113">Изберете отново **Удостоверяване**, за да предоставите съгласие на администратора.</span><span class="sxs-lookup"><span data-stu-id="b0408-113">Select **Authorize** again to provide admin consent.</span></span>

![Предоставяне на съгласие на администратора](./media/3GrantAdminConsent.png)

4. <span data-ttu-id="b0408-115">Приемете искането за разрешения.</span><span class="sxs-lookup"><span data-stu-id="b0408-115">Accept the permissions request.</span></span>

![Приемане на заявка за разрешение](./media/4AcceptPermissionRequest.png)

<span data-ttu-id="b0408-117">Упълномощаването вече е завършено.</span><span class="sxs-lookup"><span data-stu-id="b0408-117">The authorization is now complete.</span></span> 

![Упълномощаването е успешно](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a><span data-ttu-id="b0408-119">Осигурете достъп до услуги за внедряване на Dynamics до вашия абонамент за Azure</span><span class="sxs-lookup"><span data-stu-id="b0408-119">Provide Dynamics Deployment Services access to your Azure subscription</span></span>

1. <span data-ttu-id="b0408-120">Отидете на [фактуриране на Microsoft Azure](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) и изберете абонамента си.</span><span class="sxs-lookup"><span data-stu-id="b0408-120">Go to [Microsoft Azure billing](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) and select your subscription.</span></span> <span data-ttu-id="b0408-121">Dynamics Deployment Services трябва да има достъп до този абонамент, за да може да внедрява среди.</span><span class="sxs-lookup"><span data-stu-id="b0408-121">Dynamics Deployment Services needs to access this subscription to be able to deploy environments.</span></span>

![Подробни данни за абонамент на Azure](./media/6AzureSubscription.png)

2. <span data-ttu-id="b0408-123">Изберете **Контрол на достъпа (IAM)** в навигационния екран и след това изберете **Добавете назначение на роля**.</span><span class="sxs-lookup"><span data-stu-id="b0408-123">Select **Access control (IAM)** in the navigation pane, and then select **Add role assignment**.</span></span>
3. <span data-ttu-id="b0408-124">В плъзгача от дясната страна изберете **Роля на сътрудник** и в предоставения списък намерете и изберете **Услуги за внедряване на Dynamics**.</span><span class="sxs-lookup"><span data-stu-id="b0408-124">In the slider on the right side, select **Contributor role**, and in the list provided, find and select **Dynamics Deployment Services**.</span></span> 
4. <span data-ttu-id="b0408-125">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="b0408-125">Select **Save**.</span></span>

![Достъп до абонамент](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a><span data-ttu-id="b0408-127">Добавяне на конектор за абонамент към проект на LCS</span><span class="sxs-lookup"><span data-stu-id="b0408-127">Add a subscription connector to an LCS project</span></span>

1. <span data-ttu-id="b0408-128">Във вашия LCS проект, на страницата **настройки на Microsoft Azure** изберете **Добавяне**, за да добавите нов съединител.</span><span class="sxs-lookup"><span data-stu-id="b0408-128">In your LCS project, on the **Microsoft Azure settings** page, select **Add** to add a new connector.</span></span>
2. <span data-ttu-id="b0408-129">Въведете вашия ИД на абонамент за Azure.</span><span class="sxs-lookup"><span data-stu-id="b0408-129">Enter your Azure subscription ID.</span></span> <span data-ttu-id="b0408-130">Можете да намерите вашия ИД на абонамент за Azure в [Портал на Azure](https://ms.portal.azure.com/) под **Настройки** в долния ляв ъгъл на екрана.</span><span class="sxs-lookup"><span data-stu-id="b0408-130">You can find your Azure subscription ID in the [Azure portal](https://ms.portal.azure.com/), under  **Settings**  in the lower left of the screen.</span></span>
3. <span data-ttu-id="b0408-131">В полето **Конфигурирайте да използвате Azure Resource Manager** изберете **Да**.</span><span class="sxs-lookup"><span data-stu-id="b0408-131">In the **Configure to use Azure Resource Manager** field, select **Yes**.</span></span>
4. <span data-ttu-id="b0408-132">Уверете се, че абонаментният домейн на AAD за абонамент на Azure съответства на притежаващия домейн абонамент за Azure, който използвате, и изберете **Напред**.</span><span class="sxs-lookup"><span data-stu-id="b0408-132">Make sure Azure's Subscription AAD Tenant Domain matches the domain-owning Azure subscription that you are using, and select **Next**.</span></span>
5. <span data-ttu-id="b0408-133">На екрана **Настройка на Microsoft Azure** изберете **Напред**, за да потвърдите.</span><span class="sxs-lookup"><span data-stu-id="b0408-133">On the **Microsoft Azure Setup** screen, select **Next** to confirm.</span></span> <span data-ttu-id="b0408-134">Ако получите грешка на този екран, върнете се в раздела [Осигурете достъп до услуги за внедряване на Dynamics до абонамент за Azure](#provide) в тази тема и се уверете, че сте изпълнили всички стъпки.</span><span class="sxs-lookup"><span data-stu-id="b0408-134">If you receive an error on this screen, return to the section [Provide Dynamics Deployment Services access to Azure subscription](#provide) in this topic and make sure you have completed all of the steps.</span></span>
6. <span data-ttu-id="b0408-135">Изтеглете сертификата за управление на Azure в локална папка на вашия компютър и след това го качете на портала за управление на Azure, като отидете на **Настройки** > **Сертификати за управление**.</span><span class="sxs-lookup"><span data-stu-id="b0408-135">Download the Azure Management Certificate to a local folder on your computer, and then upload it to Azure Management Portal by going to **Settings** > **Management Certificates**.</span></span> <span data-ttu-id="b0408-136">Този сертификат ще позволи на LCS да комуникира с Azure от ваше име.</span><span class="sxs-lookup"><span data-stu-id="b0408-136">This certificate will enable LCS to communicate with Azure on your behalf.</span></span> <span data-ttu-id="b0408-137">Можете да пропуснете тази стъпка, ако вашият потребител има достъп до абонамента.</span><span class="sxs-lookup"><span data-stu-id="b0408-137">You can skip this step if your user has access to the subscription.</span></span>
7. <span data-ttu-id="b0408-138">Изберете **Напред**.</span><span class="sxs-lookup"><span data-stu-id="b0408-138">Select  **Next**.</span></span>
8. <span data-ttu-id="b0408-139">Изберете региона на Azure за разполагане и изберете център за данни, който е близо до мястото, където планирате да използвате тази система.</span><span class="sxs-lookup"><span data-stu-id="b0408-139">Select the Azure region to deploy in and select a data center that is close to where you plan to use this system.</span></span>
9.  <span data-ttu-id="b0408-140">Изберете **Свързване**.</span><span class="sxs-lookup"><span data-stu-id="b0408-140">Select  **Connect**.</span></span>

<span data-ttu-id="b0408-141">Успешно сте свързали абонамента си за Azure.</span><span class="sxs-lookup"><span data-stu-id="b0408-141">You have successfully connected your Azure subscription.</span></span> <span data-ttu-id="b0408-142">Вече можете да внедрявате облачно хоствани в Dynamics 365 Finance среди.</span><span class="sxs-lookup"><span data-stu-id="b0408-142">You can now deploy Dynamics 365 Finance cloud-hosted environments.</span></span>


