---
title: Осигуряване на нова среда
description: Тази тема предоставя информация за това как да се осигури нова среда за Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a43b947207b6d4276ef27ec996713bf3883e7906
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071707"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="8a937-103">Осигуряване на нова среда</span><span class="sxs-lookup"><span data-stu-id="8a937-103">Provision a new environment</span></span>

<span data-ttu-id="8a937-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="8a937-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="8a937-105">Тази тема предоставя информация за това как да осигурите нова среда на операциите на Dynamics 365 Project Operations за сценарии, базирани на ресурс/без наличност.</span><span class="sxs-lookup"><span data-stu-id="8a937-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="8a937-106">Активирайте автоматизираното осигуряване на Project Operations в LCS проект</span><span class="sxs-lookup"><span data-stu-id="8a937-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="8a937-107">Използвайте следните стъпки, за да активирате потока за автоматизирано предоставяне на Project Operations за вашия LCS проект.</span><span class="sxs-lookup"><span data-stu-id="8a937-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="8a937-108">Отидете на [LCS](https://lcs.dynamics.com/v2) и изберете плочката **Преглед на Управление на функции**.</span><span class="sxs-lookup"><span data-stu-id="8a937-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="8a937-109">В списъка **Функция за предварителен преглед** изберете **Функция Project Operations** и след това изберете **Функцията за преглед е активирана** за активиране на Project Operations.</span><span class="sxs-lookup"><span data-stu-id="8a937-109">In the **Preview feature** list, select **Project Operations Feature** , and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="8a937-110">Тази стъпка се извършва само веднъж за LCS проект.</span><span class="sxs-lookup"><span data-stu-id="8a937-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="8a937-111">Осигуряване на среда за Project Operations</span><span class="sxs-lookup"><span data-stu-id="8a937-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="8a937-112">Отворете ново внедряване в [демонстрационна среда](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) на Dynamics 365 Finance или [среда в ограничителен режим/производство](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="8a937-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="8a937-113">Преминете през съветника **Осигуряване на среда**.</span><span class="sxs-lookup"><span data-stu-id="8a937-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="8a937-114">Уверете се, че избраната версия на приложението е 10.0.13 или по-нова.</span><span class="sxs-lookup"><span data-stu-id="8a937-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="8a937-115">За предоставяне на Project Operations, под **Предварителни настройки** , изберете **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="8a937-115">To provision Project Operations, under **Advance settings** , select **Common Data Service**.</span></span> 
4. <span data-ttu-id="8a937-116">Активирайте **Настройка на Common Data Service** , като изберете **Да** , и след това въведете информация в задължителните полета:</span><span class="sxs-lookup"><span data-stu-id="8a937-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="8a937-117">Име</span><span class="sxs-lookup"><span data-stu-id="8a937-117">Name</span></span>
  - <span data-ttu-id="8a937-118">Регион</span><span class="sxs-lookup"><span data-stu-id="8a937-118">Region</span></span>
  - <span data-ttu-id="8a937-119">Език</span><span class="sxs-lookup"><span data-stu-id="8a937-119">Language</span></span>
  - <span data-ttu-id="8a937-120">Валута</span><span class="sxs-lookup"><span data-stu-id="8a937-120">Currency</span></span>
 
5. <span data-ttu-id="8a937-121">В полето **Шаблон на Common Data Service** изберете **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="8a937-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="8a937-122">Изберете типа на среда за внедряването си.</span><span class="sxs-lookup"><span data-stu-id="8a937-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="8a937-123">Пробен период, базиран на абонамент, ще ви позволи да внедрите CDS среда за 30 дни.</span><span class="sxs-lookup"><span data-stu-id="8a937-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![Настройки за внедряване](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="8a937-125">Изберете **Съгласявам се** , за да потвърдите условията на услугата и след това да изберете **Готово** , за да се върнете към настройките за разполагане.</span><span class="sxs-lookup"><span data-stu-id="8a937-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![Съгласие за внедряване](./media/2DeploymentConsent.png)

7. <span data-ttu-id="8a937-127">Попълнете останалите задължителни полета в съветника и потвърдете разполагането.</span><span class="sxs-lookup"><span data-stu-id="8a937-127">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="8a937-128">Времето за осигуряване на околната среда варира в зависимост от типа среда.</span><span class="sxs-lookup"><span data-stu-id="8a937-128">Environment provisioning time varies based on the environment type.</span></span> <span data-ttu-id="8a937-129">Предоставянето може да отнеме до шест часа.</span><span class="sxs-lookup"><span data-stu-id="8a937-129">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="8a937-130">След като разполагането завърши успешно, средата ще се покаже като **Внедрена**.</span><span class="sxs-lookup"><span data-stu-id="8a937-130">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

8. <span data-ttu-id="8a937-131">За да потвърдите, че средата е внедрена успешно, изберете **Вход** и влезте в средата, за да потвърдите.</span><span class="sxs-lookup"><span data-stu-id="8a937-131">To confirm the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![Подробности за среди на ](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a><span data-ttu-id="8a937-133">Прилагане на демонстрационни данни за Project Operations Finance (незадължителна стъпка)</span><span class="sxs-lookup"><span data-stu-id="8a937-133">Apply Project Operations Finance demo data (optional step)</span></span>

<span data-ttu-id="8a937-134">Приложете демонстрационни данни за Project Operations Finance към 10.0.13 освобождаване на услугата, хоствана в облак, както е описано в [тази статия](resource-apply-finance-demo-data.md).</span><span class="sxs-lookup"><span data-stu-id="8a937-134">Apply Project Operations Finance demo data to 10.0.13 service release Cloud Hosted Environment as described in [this article](resource-apply-finance-demo-data.md).</span></span>

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="8a937-135">Прилагане на актуализации към среда на Finance</span><span class="sxs-lookup"><span data-stu-id="8a937-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="8a937-136">Project Operations изисква среда на Finance с версия на приложението **10.0.13 (10.0.569.20009)** или по-висока.</span><span class="sxs-lookup"><span data-stu-id="8a937-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="8a937-137">Може да се наложи да приложите качествени актуализации към вашата финансова среда, за да получите тази версия.</span><span class="sxs-lookup"><span data-stu-id="8a937-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="8a937-138">В LCS, на страницата **Подробности за среда** в секцията **Налични актуализации** изберете **Преглед на актуализацията**.</span><span class="sxs-lookup"><span data-stu-id="8a937-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![Преглед на актуализации](./media/5ViewUpdates.png)

2. <span data-ttu-id="8a937-140">На страницата **Двоични актуализации** изберете **Запазване на пакета.**</span><span class="sxs-lookup"><span data-stu-id="8a937-140">On the **Binary updates** page, select **Save package.**</span></span>

![Запазване на пакета](./media/6SavePackage.png)

3. <span data-ttu-id="8a937-142">Щракнете върху **Избор на всички** и след това изберете **Записване на пакета**.</span><span class="sxs-lookup"><span data-stu-id="8a937-142">Click **Select all** and then select **Save package**.</span></span>

![Преглед и запис на актуализации](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="8a937-144">Въведете име и описание на пакета и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="8a937-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="8a937-145">В зависимост от интернет връзката този процес може да отнеме известно време.</span><span class="sxs-lookup"><span data-stu-id="8a937-145">Depending on the internet connection, this process might take some time.</span></span>

![Качете пакета в библиотеката на активите](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="8a937-147">След като пакетът бъде запазен, изберете **готово** и запазете този пакет в библиотеката на активите във вашия LCS проект.</span><span class="sxs-lookup"><span data-stu-id="8a937-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="8a937-148">Запазването и валидирането на пакета може да отнеме ~15 минути.</span><span class="sxs-lookup"><span data-stu-id="8a937-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="8a937-149">За да приложите актуализацията, отидете на страницата **Подробности за среда** в LCS и изберете **Поддържане** > **Прилагане на актуализации**.</span><span class="sxs-lookup"><span data-stu-id="8a937-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![Поддръжка на среди](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="8a937-151">В списъка с актуализации изберете пакета, който сте създали, и изберете **Приложи**.</span><span class="sxs-lookup"><span data-stu-id="8a937-151">In the updates list select the package you created, and select **Apply**.</span></span>

![Прилагане на актуализации](./media/10ApplyUpdates.png)

<span data-ttu-id="8a937-153">Обслужването на околната среда ще отнеме известно време.</span><span class="sxs-lookup"><span data-stu-id="8a937-153">Environment servicing will take some time.</span></span> <span data-ttu-id="8a937-154">След като завърши, средата ще се върне в разположено състояние.</span><span class="sxs-lookup"><span data-stu-id="8a937-154">After it is complete, the environment will return to a deployed state.</span></span>

![Средата е внедрена](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="8a937-156">Установете връзка с двоен запис</span><span class="sxs-lookup"><span data-stu-id="8a937-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="8a937-157">Във вашия LCS проект отидете на страницата **Подробности за среда**.</span><span class="sxs-lookup"><span data-stu-id="8a937-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="8a937-158">Под **Информация за среда на Common Data Service** изберете **Връзка към CDS за приложения**.</span><span class="sxs-lookup"><span data-stu-id="8a937-158">Under **Common Data Service Environment Information** , select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="8a937-159">След като връзката завърши, изберете отново **Връзка към CDS за приложения**.</span><span class="sxs-lookup"><span data-stu-id="8a937-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="8a937-160">Ще бъдете пренасочени към Двойно записване във Finance.</span><span class="sxs-lookup"><span data-stu-id="8a937-160">You will be redirected to Dual Write in Finance.</span></span>

![Връзка към CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="8a937-162">Изберете **Нанесете разтвор** за достъп до обектите, които ще бъдат картографирани в интеграцията.</span><span class="sxs-lookup"><span data-stu-id="8a937-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![Прилагане на решения](./media/13ApplySolutions.png)

5. <span data-ttu-id="8a937-164">Изберете и двете решения, **Карта на обекти за двоен запис на Dynamics 365 Finance and Operations** и **Карти на обекти за двойно записване на Dynamics 365 Project Operations** и след това изберете **Приложи**.</span><span class="sxs-lookup"><span data-stu-id="8a937-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps** , and then select **Apply**.</span></span>

![Потвърдете решенията](./media/14ConfirmSolutions.png)

<span data-ttu-id="8a937-166">След прилагането на решенията, обектите за двоен запис се прилагат към околната среда.</span><span class="sxs-lookup"><span data-stu-id="8a937-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![Прилагане на решения](./media/15ApplyingSolutions.png)

<span data-ttu-id="8a937-168">След като обектите са приложени, всички налични съпоставяния са изброени в средата.</span><span class="sxs-lookup"><span data-stu-id="8a937-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![Карти с двоен запис](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="8a937-170">Опреснете субектите на данни след актуализацията</span><span class="sxs-lookup"><span data-stu-id="8a937-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="8a937-171">Във Finance отидете на работното пространство **Управление на данни**.</span><span class="sxs-lookup"><span data-stu-id="8a937-171">In Finance, go to the **Data management** workspace.</span></span>

![Работно пространство за управление на данни](./media/16DataManagement.png)

2. <span data-ttu-id="8a937-173">Изберете плочката **Параметри на рамката**.</span><span class="sxs-lookup"><span data-stu-id="8a937-173">Select the **Framework parameters** tile.</span></span>

![Параметри на рамката](./media/17FrameworkParameters.png)

3. <span data-ttu-id="8a937-175">На страницата **Настройки на обекта** изберете **Опресняване на списъка с обекти**.</span><span class="sxs-lookup"><span data-stu-id="8a937-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![Обновяване на списък с обекти](./media/18RefreshEntityList.png)

<span data-ttu-id="8a937-177">Опресняването ще отнеме около 20 минути.</span><span class="sxs-lookup"><span data-stu-id="8a937-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="8a937-178">Ще получите предупреждение, когато приключи.</span><span class="sxs-lookup"><span data-stu-id="8a937-178">You will receive an alert when it is complete.</span></span>

![Потвърждение на обновяване](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="8a937-180">Изпълнение на карти Двойно записване на Project Operations</span><span class="sxs-lookup"><span data-stu-id="8a937-180">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="8a937-181">Във вашия LCS проект отидете на страницата **Подробности за среда**.</span><span class="sxs-lookup"><span data-stu-id="8a937-181">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="8a937-182">Под **Информация за среда на Common Data Service** изберете **Връзка към CDS за приложения**.</span><span class="sxs-lookup"><span data-stu-id="8a937-182">Under **Common Data Service Environment Information** , select **Link to CDS for Apps.**</span></span> <span data-ttu-id="8a937-183">След като изберете връзката, ще бъдете пренасочени към списъка с обекти в съпоставянията.</span><span class="sxs-lookup"><span data-stu-id="8a937-183">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="8a937-184">Стартирайте картите, както е описано в следващата таблица.</span><span class="sxs-lookup"><span data-stu-id="8a937-184">Start the maps as described in the following table.</span></span> <span data-ttu-id="8a937-185">Не забравяйте да следвате последователността, както е изброено.</span><span class="sxs-lookup"><span data-stu-id="8a937-185">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="8a937-186">**Схема на свързване на обект**</span><span class="sxs-lookup"><span data-stu-id="8a937-186">**Entity Map**</span></span> | <span data-ttu-id="8a937-187">**Обновяване на обект**</span><span class="sxs-lookup"><span data-stu-id="8a937-187">**Refresh entity**</span></span> | <span data-ttu-id="8a937-188">**Първоначална синхронизация**</span><span class="sxs-lookup"><span data-stu-id="8a937-188">**Initial sync**</span></span> | <span data-ttu-id="8a937-189">**Главен елемент за първоначална синхронизация**</span><span class="sxs-lookup"><span data-stu-id="8a937-189">**Master for initial sync**</span></span> | <span data-ttu-id="8a937-190">**Изпълнение на предварителни изисквания**</span><span class="sxs-lookup"><span data-stu-id="8a937-190">**Run prerequisites**</span></span> | <span data-ttu-id="8a937-191">**Първоначална синхронизация на предварителни изисквания**</span><span class="sxs-lookup"><span data-stu-id="8a937-191">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="8a937-192">**Роли на проектните ресурси за всички фирми (резервационни ресурси)**</span><span class="sxs-lookup"><span data-stu-id="8a937-192">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="8a937-193">No</span><span class="sxs-lookup"><span data-stu-id="8a937-193">No</span></span> | <span data-ttu-id="8a937-194">Да</span><span class="sxs-lookup"><span data-stu-id="8a937-194">Yes</span></span> | <span data-ttu-id="8a937-195">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="8a937-195">Common Data Service</span></span> | <span data-ttu-id="8a937-196">No</span><span class="sxs-lookup"><span data-stu-id="8a937-196">No</span></span> | <span data-ttu-id="8a937-197">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-197">N\A</span></span> |
| <span data-ttu-id="8a937-198">**Юридически лица (cdm\_фирми)**</span><span class="sxs-lookup"><span data-stu-id="8a937-198">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="8a937-199">No</span><span class="sxs-lookup"><span data-stu-id="8a937-199">No</span></span> | <span data-ttu-id="8a937-200">Да</span><span class="sxs-lookup"><span data-stu-id="8a937-200">Yes</span></span> | <span data-ttu-id="8a937-201">Приложения на Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="8a937-201">Finance and Operations apps</span></span> | <span data-ttu-id="8a937-202">No</span><span class="sxs-lookup"><span data-stu-id="8a937-202">No</span></span> | <span data-ttu-id="8a937-203">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-203">N\A</span></span> |
| <span data-ttu-id="8a937-204">**Действителни данни за интеграция на Project Operations (msdyn\_действителни)**</span><span class="sxs-lookup"><span data-stu-id="8a937-204">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="8a937-205">No</span><span class="sxs-lookup"><span data-stu-id="8a937-205">No</span></span> | <span data-ttu-id="8a937-206">No</span><span class="sxs-lookup"><span data-stu-id="8a937-206">No</span></span> | <span data-ttu-id="8a937-207">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-207">N\A</span></span> | <span data-ttu-id="8a937-208">Да</span><span class="sxs-lookup"><span data-stu-id="8a937-208">Yes</span></span> | <span data-ttu-id="8a937-209">No</span><span class="sxs-lookup"><span data-stu-id="8a937-209">No</span></span> |
| <span data-ttu-id="8a937-210">**Аспекти на договор по проект (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="8a937-210">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="8a937-211">No</span><span class="sxs-lookup"><span data-stu-id="8a937-211">No</span></span> | <span data-ttu-id="8a937-212">No</span><span class="sxs-lookup"><span data-stu-id="8a937-212">No</span></span> | <span data-ttu-id="8a937-213">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-213">N\A</span></span> | <span data-ttu-id="8a937-214">No</span><span class="sxs-lookup"><span data-stu-id="8a937-214">No</span></span> | <span data-ttu-id="8a937-215">No</span><span class="sxs-lookup"><span data-stu-id="8a937-215">No</span></span> |
| <span data-ttu-id="8a937-216">**Интеграционен обект за взаимоотношения на проектни транзакции (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="8a937-216">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="8a937-217">No</span><span class="sxs-lookup"><span data-stu-id="8a937-217">No</span></span> | <span data-ttu-id="8a937-218">No</span><span class="sxs-lookup"><span data-stu-id="8a937-218">No</span></span> | <span data-ttu-id="8a937-219">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-219">N\A</span></span> | <span data-ttu-id="8a937-220">No</span><span class="sxs-lookup"><span data-stu-id="8a937-220">No</span></span> | <span data-ttu-id="8a937-221">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-221">N\A</span></span> |
| <span data-ttu-id="8a937-222">**Основни етапи на договора за интеграция на Project Operations (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="8a937-222">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="8a937-223">No</span><span class="sxs-lookup"><span data-stu-id="8a937-223">No</span></span> | <span data-ttu-id="8a937-224">No</span><span class="sxs-lookup"><span data-stu-id="8a937-224">No</span></span> | <span data-ttu-id="8a937-225">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-225">N\A</span></span> | <span data-ttu-id="8a937-226">No</span><span class="sxs-lookup"><span data-stu-id="8a937-226">No</span></span> | <span data-ttu-id="8a937-227">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-227">N\A</span></span> |
| <span data-ttu-id="8a937-228">**Обект за интеграция на Project Operations за оценки на разходите (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="8a937-228">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="8a937-229">No</span><span class="sxs-lookup"><span data-stu-id="8a937-229">No</span></span> | <span data-ttu-id="8a937-230">No</span><span class="sxs-lookup"><span data-stu-id="8a937-230">No</span></span> | <span data-ttu-id="8a937-231">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-231">N\A</span></span> | <span data-ttu-id="8a937-232">No</span><span class="sxs-lookup"><span data-stu-id="8a937-232">No</span></span> | <span data-ttu-id="8a937-233">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-233">N\A</span></span> |
| <span data-ttu-id="8a937-234">**Обект за експортиране на категории на разход по проект за интеграция на Project Operations (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="8a937-234">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="8a937-235">No</span><span class="sxs-lookup"><span data-stu-id="8a937-235">No</span></span> | <span data-ttu-id="8a937-236">No</span><span class="sxs-lookup"><span data-stu-id="8a937-236">No</span></span> | <span data-ttu-id="8a937-237">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-237">N\A</span></span> | <span data-ttu-id="8a937-238">No</span><span class="sxs-lookup"><span data-stu-id="8a937-238">No</span></span> | <span data-ttu-id="8a937-239">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-239">N\A</span></span> |
| <span data-ttu-id="8a937-240">**Обект за експортиране на Project Operations за интегриране на проектни разходи (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="8a937-240">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="8a937-241">Да</span><span class="sxs-lookup"><span data-stu-id="8a937-241">Yes</span></span> | <span data-ttu-id="8a937-242">No</span><span class="sxs-lookup"><span data-stu-id="8a937-242">No</span></span> | <span data-ttu-id="8a937-243">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-243">N\A</span></span> | <span data-ttu-id="8a937-244">No</span><span class="sxs-lookup"><span data-stu-id="8a937-244">No</span></span> | <span data-ttu-id="8a937-245">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-245">N\A</span></span> |
| <span data-ttu-id="8a937-246">**Обект за интеграция на Project Operations за оценки на часове (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="8a937-246">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="8a937-247">Да</span><span class="sxs-lookup"><span data-stu-id="8a937-247">Yes</span></span> | <span data-ttu-id="8a937-248">No</span><span class="sxs-lookup"><span data-stu-id="8a937-248">No</span></span> | <span data-ttu-id="8a937-249">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-249">N\A</span></span> | <span data-ttu-id="8a937-250">No</span><span class="sxs-lookup"><span data-stu-id="8a937-250">No</span></span> | <span data-ttu-id="8a937-251">Няма</span><span class="sxs-lookup"><span data-stu-id="8a937-251">N\A</span></span> |


4. <span data-ttu-id="8a937-252">За да опресните обекта, изберете името на картата и след това изберете **Опресняване на обекти**.</span><span class="sxs-lookup"><span data-stu-id="8a937-252">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![Обновяване на карта](./media/20RefreshMapping.png)

5. <span data-ttu-id="8a937-254">Изпълнете картата след завършване на опресняването.</span><span class="sxs-lookup"><span data-stu-id="8a937-254">After the refresh is complete, run the map.</span></span> <span data-ttu-id="8a937-255">Преди да активирате следващата карта, проверете дали картата в таблицата е в състояние на **Изпълнение**.</span><span class="sxs-lookup"><span data-stu-id="8a937-255">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="8a937-256">Изпълнението на карти с по-голям брой предпоставки може да отнеме известно време.</span><span class="sxs-lookup"><span data-stu-id="8a937-256">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="8a937-257">За да стартирате карта с предпоставки, активирайте превключвателя **Показване на свързани карти на обекти**.</span><span class="sxs-lookup"><span data-stu-id="8a937-257">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="8a937-258">Ако таблицата показва **Предварително първоначално синхронизиране** като **Не** , проверете дали флагът **Първоначално синхронизиране** е **Изключен** във всички необходими карти, преди да го стартирате.</span><span class="sxs-lookup"><span data-stu-id="8a937-258">If the table indicates **Prerequisite initial sync** is **No** , verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![Стартирайте карта](./media/21RunMap.png)

6. <span data-ttu-id="8a937-260">Проверете дали всички свързани с проекта карти са в работно състояние.</span><span class="sxs-lookup"><span data-stu-id="8a937-260">Validate all project related maps are in the running state.</span></span>

![Всички карти работят](./media/22AllMapsRunning.png)

<span data-ttu-id="8a937-262">Средата на Project Operations вече е подготвена и конфигурирана.</span><span class="sxs-lookup"><span data-stu-id="8a937-262">Your Project Operations environment is now provisioned and configured.</span></span>
