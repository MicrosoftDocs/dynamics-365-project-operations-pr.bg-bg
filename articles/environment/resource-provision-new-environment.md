---
title: Осигуряване на нова среда
description: Тази тема предоставя информация за това как да се осигури нова среда за Project Operations.
author: sigitac
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d0712d9d5dfc6c35ccd07142ff5948f50e6a254c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995473"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="d84df-103">Осигуряване на нова среда</span><span class="sxs-lookup"><span data-stu-id="d84df-103">Provision a new environment</span></span>

<span data-ttu-id="d84df-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="d84df-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="d84df-105">Тази тема предоставя информация за начина на осигуряване на нова среда на Dynamics 365 Project Operations за сценарии, базирани на ресурси/неналичност.</span><span class="sxs-lookup"><span data-stu-id="d84df-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="d84df-106">Активирайте автоматизираното осигуряване на Project Operations в LCS проект</span><span class="sxs-lookup"><span data-stu-id="d84df-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="d84df-107">Използвайте следните стъпки, за да активирате потока за автоматизирано предоставяне на Project Operations за вашия LCS проект.</span><span class="sxs-lookup"><span data-stu-id="d84df-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="d84df-108">Отидете на [LCS](https://lcs.dynamics.com/v2) и изберете плочката **Преглед на Управление на функции**.</span><span class="sxs-lookup"><span data-stu-id="d84df-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="d84df-109">В списъка **Функция за предварителен преглед** изберете **Функция Project Operations** и след това изберете **Функцията за преглед е активирана** за активиране на Project Operations.</span><span class="sxs-lookup"><span data-stu-id="d84df-109">In the **Preview feature** list, select **Project Operations Feature**, and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="d84df-110">Тази стъпка се извършва само веднъж за LCS проект.</span><span class="sxs-lookup"><span data-stu-id="d84df-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="d84df-111">Осигуряване на среда за Project Operations</span><span class="sxs-lookup"><span data-stu-id="d84df-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="d84df-112">Отворете ново внедряване в [демонстрационна среда](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) на Dynamics 365 Finance или [среда в ограничителен режим/производство](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="d84df-112">Open a new Dynamics 365 Finance [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="d84df-113">Преминете през съветника **Осигуряване на среда**.</span><span class="sxs-lookup"><span data-stu-id="d84df-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="d84df-114">Уверете се, че избраната версия на приложението е 10.0.13 или по-нова.</span><span class="sxs-lookup"><span data-stu-id="d84df-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="d84df-115">За предоставяне на Project Operations, под **Предварителни настройки**, изберете **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="d84df-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="d84df-116">Активирайте **Настройка на Common Data Service**, като изберете **Да**, и след това въведете информация в задължителните полета:</span><span class="sxs-lookup"><span data-stu-id="d84df-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="d84df-117">Име</span><span class="sxs-lookup"><span data-stu-id="d84df-117">Name</span></span>
  - <span data-ttu-id="d84df-118">Регион</span><span class="sxs-lookup"><span data-stu-id="d84df-118">Region</span></span>
  - <span data-ttu-id="d84df-119">Език</span><span class="sxs-lookup"><span data-stu-id="d84df-119">Language</span></span>
  - <span data-ttu-id="d84df-120">Валута</span><span class="sxs-lookup"><span data-stu-id="d84df-120">Currency</span></span>
 
5. <span data-ttu-id="d84df-121">В полето **Шаблон на Common Data Service** изберете **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="d84df-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="d84df-122">Изберете типа на среда за внедряването си.</span><span class="sxs-lookup"><span data-stu-id="d84df-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="d84df-123">Пробен период, базиран на абонамент, ще ви позволи да внедрите CDS среда за 30 дни.</span><span class="sxs-lookup"><span data-stu-id="d84df-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![Настройки за внедряване](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="d84df-125">Изберете **Съгласявам се**, за да потвърдите условията на услугата и след това да изберете **Готово**, за да се върнете към настройките за разполагане.</span><span class="sxs-lookup"><span data-stu-id="d84df-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![Съгласие за внедряване](./media/2DeploymentConsent.png)

7. <span data-ttu-id="d84df-127">По избор - Приложете демонстрационни данни към околната среда.</span><span class="sxs-lookup"><span data-stu-id="d84df-127">Optional - Apply demo data to the environment.</span></span> <span data-ttu-id="d84df-128">Отидете на **Разширени настройки**, изберете **Персонализирайте конфигурацията на базата данни на SQL** и задайте **Посочете набор от данни за база данни на приложения** на **Dемонстрация**.</span><span class="sxs-lookup"><span data-stu-id="d84df-128">Go to **Advanced settings**, select **Customize SQL Database Configuration**, and set **Specify a dataset for Application database** to **Demo**.</span></span>

8. <span data-ttu-id="d84df-129">Попълнете останалите задължителни полета в съветника и потвърдете разполагането.</span><span class="sxs-lookup"><span data-stu-id="d84df-129">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="d84df-130">Времето за осигуряване на среда варира в зависимост от типа на околната среда.</span><span class="sxs-lookup"><span data-stu-id="d84df-130">The time to provision the environment varies based on the environment type.</span></span> <span data-ttu-id="d84df-131">Предоставянето може да отнеме до шест часа.</span><span class="sxs-lookup"><span data-stu-id="d84df-131">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="d84df-132">След като разполагането завърши успешно, средата ще се покаже като **Внедрена**.</span><span class="sxs-lookup"><span data-stu-id="d84df-132">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

9. <span data-ttu-id="d84df-133">За да потвърдите, че средата се е разположила успешно, изберете **Вход** и влезте в средата, за да потвърдите.</span><span class="sxs-lookup"><span data-stu-id="d84df-133">To confirm that the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![Подробности за среди на ](./media/3EnvironmentDetails.png)

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="d84df-135">Прилагане на актуализации към среда на Finance</span><span class="sxs-lookup"><span data-stu-id="d84df-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="d84df-136">Project Operations изисква среда на Finance с версия на приложението **10.0.13 (10.0.569.20009)** или по-висока.</span><span class="sxs-lookup"><span data-stu-id="d84df-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="d84df-137">Може да се наложи да приложите качествени актуализации към вашата финансова среда, за да получите тази версия.</span><span class="sxs-lookup"><span data-stu-id="d84df-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="d84df-138">В LCS, на страницата **Подробности за среда** в секцията **Налични актуализации** изберете **Преглед на актуализацията**.</span><span class="sxs-lookup"><span data-stu-id="d84df-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![Преглед на актуализации](./media/5ViewUpdates.png)

2. <span data-ttu-id="d84df-140">На страницата **Двоични актуализации** изберете **Запазване на пакета.**</span><span class="sxs-lookup"><span data-stu-id="d84df-140">On the **Binary updates** page, select **Save package.**</span></span>

![Запазване на пакета](./media/6SavePackage.png)

3. <span data-ttu-id="d84df-142">Щракнете върху **Избор на всички** и след това изберете **Записване на пакета**.</span><span class="sxs-lookup"><span data-stu-id="d84df-142">Click **Select all** and then select **Save package**.</span></span>

![Преглед и запис на актуализации](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="d84df-144">Въведете име и описание на пакета и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="d84df-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="d84df-145">В зависимост от интернет връзката този процес може да отнеме известно време.</span><span class="sxs-lookup"><span data-stu-id="d84df-145">Depending on the internet connection, this process might take some time.</span></span>

![Качете пакета в библиотеката на активите](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="d84df-147">След като пакетът бъде запазен, изберете **готово** и запазете този пакет в библиотеката на активите във вашия LCS проект.</span><span class="sxs-lookup"><span data-stu-id="d84df-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="d84df-148">Запазването и валидирането на пакета може да отнеме ~15 минути.</span><span class="sxs-lookup"><span data-stu-id="d84df-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="d84df-149">За да приложите актуализацията, отидете на страницата **Подробности за среда** в LCS и изберете **Поддържане** > **Прилагане на актуализации**.</span><span class="sxs-lookup"><span data-stu-id="d84df-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![Поддръжка на среди](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="d84df-151">В списъка с актуализации изберете пакета, който сте създали, и изберете **Приложи**.</span><span class="sxs-lookup"><span data-stu-id="d84df-151">In the updates list select the package you created, and select **Apply**.</span></span>

![Прилагане на актуализации](./media/10ApplyUpdates.png)

<span data-ttu-id="d84df-153">Обслужването на околната среда ще отнеме известно време.</span><span class="sxs-lookup"><span data-stu-id="d84df-153">Environment servicing will take some time.</span></span> <span data-ttu-id="d84df-154">След като завърши, средата ще се върне в разположено състояние.</span><span class="sxs-lookup"><span data-stu-id="d84df-154">After it is complete, the environment will return to a deployed state.</span></span>

![Средата е внедрена](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="d84df-156">Установете връзка с двоен запис</span><span class="sxs-lookup"><span data-stu-id="d84df-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="d84df-157">Във вашия LCS проект отидете на страницата **Подробности за среда**.</span><span class="sxs-lookup"><span data-stu-id="d84df-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="d84df-158">Под **Информация за среда на Common Data Service** изберете **Връзка към CDS за приложения**.</span><span class="sxs-lookup"><span data-stu-id="d84df-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="d84df-159">След като връзката завърши, изберете отново **Връзка към CDS за приложения**.</span><span class="sxs-lookup"><span data-stu-id="d84df-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="d84df-160">Ще бъдете пренасочени към Двойно записване във Finance.</span><span class="sxs-lookup"><span data-stu-id="d84df-160">You will be redirected to Dual Write in Finance.</span></span>

![Връзка към CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="d84df-162">Изберете **Нанесете разтвор** за достъп до обектите, които ще бъдат картографирани в интеграцията.</span><span class="sxs-lookup"><span data-stu-id="d84df-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![Прилагане на решения](./media/13ApplySolutions.png)

5. <span data-ttu-id="d84df-164">Изберете двете решения, **Съпоставяне на обект с двукратно записване в Dynamics 365 Finance and Operations** и **Съпоставяния на обект с двукратно записване в Dynamics 365 Project Operations**, след което изберете **Прилагане**.</span><span class="sxs-lookup"><span data-stu-id="d84df-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![Потвърдете решенията](./media/14ConfirmSolutions.png)

<span data-ttu-id="d84df-166">След прилагането на решенията, обектите за двоен запис се прилагат към околната среда.</span><span class="sxs-lookup"><span data-stu-id="d84df-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![Прилагане на решения](./media/15ApplyingSolutions.png)

<span data-ttu-id="d84df-168">След като обектите са приложени, всички налични съпоставяния са изброени в средата.</span><span class="sxs-lookup"><span data-stu-id="d84df-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![Карти с двоен запис](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="d84df-170">Опреснете субектите на данни след актуализацията</span><span class="sxs-lookup"><span data-stu-id="d84df-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="d84df-171">Във Finance отидете на работното пространство **Управление на данни**.</span><span class="sxs-lookup"><span data-stu-id="d84df-171">In Finance, go to the **Data management** workspace.</span></span>

![Работно пространство за управление на данни](./media/16DataManagement.png)

2. <span data-ttu-id="d84df-173">Изберете плочката **Параметри на рамката**.</span><span class="sxs-lookup"><span data-stu-id="d84df-173">Select the **Framework parameters** tile.</span></span>

![Параметри на рамката](./media/17FrameworkParameters.png)

3. <span data-ttu-id="d84df-175">На страницата **Настройки на обекта** изберете **Опресняване на списъка с обекти**.</span><span class="sxs-lookup"><span data-stu-id="d84df-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![Обновяване на списък с обекти](./media/18RefreshEntityList.png)

<span data-ttu-id="d84df-177">Опресняването ще отнеме около 20 минути.</span><span class="sxs-lookup"><span data-stu-id="d84df-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="d84df-178">Ще получите предупреждение, когато приключи.</span><span class="sxs-lookup"><span data-stu-id="d84df-178">You will receive an alert when it is complete.</span></span>

![Потвърждение на обновяване](./media/19RefreshConfirmation.png)

## <a name="update-security-settings-on-project-operations-on-dataverse"></a><span data-ttu-id="d84df-180">Актуализирайте настройките за защита на Project Operations на Dataverse</span><span class="sxs-lookup"><span data-stu-id="d84df-180">Update security settings on Project Operations on Dataverse</span></span>

1. <span data-ttu-id="d84df-181">Отидете на Project Operations на средата на Dataverse.</span><span class="sxs-lookup"><span data-stu-id="d84df-181">Go to Project Operations on your Dataverse environment.</span></span> 
2. <span data-ttu-id="d84df-182">Отидете в **Настройки** > **Защита** > **Роли на защита**.</span><span class="sxs-lookup"><span data-stu-id="d84df-182">Go to **Settings** > **Security** > **Security roles**.</span></span> 
3. <span data-ttu-id="d84df-183">На страницата **Роли на защита** в списъка с роли изберете **потребител на приложение с двойно писане** и изберете раздела **Персонализирани обекти**.</span><span class="sxs-lookup"><span data-stu-id="d84df-183">On the **Security roles** page, in the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span>  
4. <span data-ttu-id="d84df-184">Проверете дали ролята имат разрешения **Четене** и **Добавяне към** за:</span><span class="sxs-lookup"><span data-stu-id="d84df-184">Verify that the role has **Read** and **Append To** permissions for the:</span></span>
      
      - <span data-ttu-id="d84df-185">**Тип на обменната валута**</span><span class="sxs-lookup"><span data-stu-id="d84df-185">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="d84df-186">**Диаграма с акаунти**</span><span class="sxs-lookup"><span data-stu-id="d84df-186">**Chart Of Accounts**</span></span>
      - <span data-ttu-id="d84df-187">**Финансов календар**</span><span class="sxs-lookup"><span data-stu-id="d84df-187">**Fiscal Calendar**</span></span>
      - <span data-ttu-id="d84df-188">**Счетоводна книга**</span><span class="sxs-lookup"><span data-stu-id="d84df-188">**Ledger**</span></span>

5. <span data-ttu-id="d84df-189">След като ролята на защита бъде актуализирана, отидете на **Настройки** > **Сигурност** > **Екипи** и изберете екипа по подразбиране в **Собственик на местен бизнес** екипен изглед.</span><span class="sxs-lookup"><span data-stu-id="d84df-189">After the security role is updated, go to **Settings** > **Security** > **Teams**, and select the default team in the **Local Business Owner** team view.</span></span>
6. <span data-ttu-id="d84df-190">Изберете **Управление на ролите** и проверете дали **потребител на приложение с двойно писане** привилегията за сигурност се прилага към този екип.</span><span class="sxs-lookup"><span data-stu-id="d84df-190">Select **Manage Roles** and verify that the **dual-write app user** security privilege is applied to this team.</span></span>

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="d84df-191">Изпълнение на карти Двойно записване на Project Operations</span><span class="sxs-lookup"><span data-stu-id="d84df-191">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="d84df-192">Във вашия LCS проект отидете на страницата **Подробности за среда**.</span><span class="sxs-lookup"><span data-stu-id="d84df-192">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="d84df-193">Под **Информация за среда на Common Data Service** изберете **Връзка към CDS за приложения**.</span><span class="sxs-lookup"><span data-stu-id="d84df-193">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="d84df-194">След като изберете връзката, ще бъдете пренасочени към списъка с обекти в съпоставянията.</span><span class="sxs-lookup"><span data-stu-id="d84df-194">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="d84df-195">Стартирайте картите, както е описано в следващата таблица.</span><span class="sxs-lookup"><span data-stu-id="d84df-195">Start the maps as described in the following table.</span></span> <span data-ttu-id="d84df-196">Не забравяйте да следвате последователността, както е изброено.</span><span class="sxs-lookup"><span data-stu-id="d84df-196">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="d84df-197">**Схема на свързване на обект**</span><span class="sxs-lookup"><span data-stu-id="d84df-197">**Entity Map**</span></span> | <span data-ttu-id="d84df-198">**Обновяване на обект**</span><span class="sxs-lookup"><span data-stu-id="d84df-198">**Refresh entity**</span></span> | <span data-ttu-id="d84df-199">**Първоначална синхронизация**</span><span class="sxs-lookup"><span data-stu-id="d84df-199">**Initial sync**</span></span> | <span data-ttu-id="d84df-200">**Главен елемент за първоначална синхронизация**</span><span class="sxs-lookup"><span data-stu-id="d84df-200">**Master for initial sync**</span></span> | <span data-ttu-id="d84df-201">**Изпълнение на предварителни изисквания**</span><span class="sxs-lookup"><span data-stu-id="d84df-201">**Run prerequisites**</span></span> | <span data-ttu-id="d84df-202">**Първоначална синхронизация на предварителни изисквания**</span><span class="sxs-lookup"><span data-stu-id="d84df-202">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="d84df-203">**Роли на проектните ресурси за всички фирми (резервационни ресурси)**</span><span class="sxs-lookup"><span data-stu-id="d84df-203">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="d84df-204">No</span><span class="sxs-lookup"><span data-stu-id="d84df-204">No</span></span> | <span data-ttu-id="d84df-205">Да</span><span class="sxs-lookup"><span data-stu-id="d84df-205">Yes</span></span> | <span data-ttu-id="d84df-206">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="d84df-206">Common Data Service</span></span> | <span data-ttu-id="d84df-207">No</span><span class="sxs-lookup"><span data-stu-id="d84df-207">No</span></span> | <span data-ttu-id="d84df-208">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-208">N\A</span></span> |
| <span data-ttu-id="d84df-209">**Юридически лица (cdm\_фирми)**</span><span class="sxs-lookup"><span data-stu-id="d84df-209">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="d84df-210">No</span><span class="sxs-lookup"><span data-stu-id="d84df-210">No</span></span> | <span data-ttu-id="d84df-211">Да</span><span class="sxs-lookup"><span data-stu-id="d84df-211">Yes</span></span> | <span data-ttu-id="d84df-212">Приложения на Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="d84df-212">Finance and Operations apps</span></span> | <span data-ttu-id="d84df-213">No</span><span class="sxs-lookup"><span data-stu-id="d84df-213">No</span></span> | <span data-ttu-id="d84df-214">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-214">N\A</span></span> |
| <span data-ttu-id="d84df-215">**Книга (msdyn_ledgers)**</span><span class="sxs-lookup"><span data-stu-id="d84df-215">**Ledger (msdyn_ledgers)**</span></span> | <span data-ttu-id="d84df-216">No</span><span class="sxs-lookup"><span data-stu-id="d84df-216">No</span></span> | <span data-ttu-id="d84df-217">Да</span><span class="sxs-lookup"><span data-stu-id="d84df-217">Yes</span></span> | <span data-ttu-id="d84df-218">Приложения на Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="d84df-218">Finance and Operations apps</span></span> | <span data-ttu-id="d84df-219">Да</span><span class="sxs-lookup"><span data-stu-id="d84df-219">Yes</span></span> | <span data-ttu-id="d84df-220">Да, приложения Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="d84df-220">Yes, Finance and Operations apps</span></span> |
| <span data-ttu-id="d84df-221">**Действителни данни за интеграция на Project Operations (msdyn\_действителни)**</span><span class="sxs-lookup"><span data-stu-id="d84df-221">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="d84df-222">No</span><span class="sxs-lookup"><span data-stu-id="d84df-222">No</span></span> | <span data-ttu-id="d84df-223">No</span><span class="sxs-lookup"><span data-stu-id="d84df-223">No</span></span> | <span data-ttu-id="d84df-224">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-224">N\A</span></span> | <span data-ttu-id="d84df-225">Да</span><span class="sxs-lookup"><span data-stu-id="d84df-225">Yes</span></span> | <span data-ttu-id="d84df-226">No</span><span class="sxs-lookup"><span data-stu-id="d84df-226">No</span></span> |
| <span data-ttu-id="d84df-227">**Аспекти на договор по проект (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="d84df-227">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="d84df-228">No</span><span class="sxs-lookup"><span data-stu-id="d84df-228">No</span></span> | <span data-ttu-id="d84df-229">No</span><span class="sxs-lookup"><span data-stu-id="d84df-229">No</span></span> | <span data-ttu-id="d84df-230">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-230">N\A</span></span> | <span data-ttu-id="d84df-231">No</span><span class="sxs-lookup"><span data-stu-id="d84df-231">No</span></span> | <span data-ttu-id="d84df-232">No</span><span class="sxs-lookup"><span data-stu-id="d84df-232">No</span></span> |
| <span data-ttu-id="d84df-233">**Интеграционен обект за взаимоотношения на проектни транзакции (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="d84df-233">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="d84df-234">No</span><span class="sxs-lookup"><span data-stu-id="d84df-234">No</span></span> | <span data-ttu-id="d84df-235">No</span><span class="sxs-lookup"><span data-stu-id="d84df-235">No</span></span> | <span data-ttu-id="d84df-236">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-236">N\A</span></span> | <span data-ttu-id="d84df-237">No</span><span class="sxs-lookup"><span data-stu-id="d84df-237">No</span></span> | <span data-ttu-id="d84df-238">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-238">N\A</span></span> |
| <span data-ttu-id="d84df-239">**Основни етапи на договора за интеграция на Project Operations (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="d84df-239">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="d84df-240">No</span><span class="sxs-lookup"><span data-stu-id="d84df-240">No</span></span> | <span data-ttu-id="d84df-241">No</span><span class="sxs-lookup"><span data-stu-id="d84df-241">No</span></span> | <span data-ttu-id="d84df-242">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-242">N\A</span></span> | <span data-ttu-id="d84df-243">No</span><span class="sxs-lookup"><span data-stu-id="d84df-243">No</span></span> | <span data-ttu-id="d84df-244">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-244">N\A</span></span> |
| <span data-ttu-id="d84df-245">**Обект за интеграция на Project Operations за оценки на разходите (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="d84df-245">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="d84df-246">No</span><span class="sxs-lookup"><span data-stu-id="d84df-246">No</span></span> | <span data-ttu-id="d84df-247">No</span><span class="sxs-lookup"><span data-stu-id="d84df-247">No</span></span> | <span data-ttu-id="d84df-248">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-248">N\A</span></span> | <span data-ttu-id="d84df-249">No</span><span class="sxs-lookup"><span data-stu-id="d84df-249">No</span></span> | <span data-ttu-id="d84df-250">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-250">N\A</span></span> |
| <span data-ttu-id="d84df-251">**Обект за експортиране на категории на разход по проект за интеграция на Project Operations (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="d84df-251">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="d84df-252">No</span><span class="sxs-lookup"><span data-stu-id="d84df-252">No</span></span> | <span data-ttu-id="d84df-253">No</span><span class="sxs-lookup"><span data-stu-id="d84df-253">No</span></span> | <span data-ttu-id="d84df-254">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-254">N\A</span></span> | <span data-ttu-id="d84df-255">No</span><span class="sxs-lookup"><span data-stu-id="d84df-255">No</span></span> | <span data-ttu-id="d84df-256">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-256">N\A</span></span> |
| <span data-ttu-id="d84df-257">**Обект за експортиране на Project Operations за интегриране на проектни разходи (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="d84df-257">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="d84df-258">Да</span><span class="sxs-lookup"><span data-stu-id="d84df-258">Yes</span></span> | <span data-ttu-id="d84df-259">No</span><span class="sxs-lookup"><span data-stu-id="d84df-259">No</span></span> | <span data-ttu-id="d84df-260">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-260">N\A</span></span> | <span data-ttu-id="d84df-261">No</span><span class="sxs-lookup"><span data-stu-id="d84df-261">No</span></span> | <span data-ttu-id="d84df-262">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-262">N\A</span></span> |
| <span data-ttu-id="d84df-263">**Обект за интеграция на Project Operations за оценки на часове (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="d84df-263">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="d84df-264">Да</span><span class="sxs-lookup"><span data-stu-id="d84df-264">Yes</span></span> | <span data-ttu-id="d84df-265">No</span><span class="sxs-lookup"><span data-stu-id="d84df-265">No</span></span> | <span data-ttu-id="d84df-266">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-266">N\A</span></span> | <span data-ttu-id="d84df-267">No</span><span class="sxs-lookup"><span data-stu-id="d84df-267">No</span></span> | <span data-ttu-id="d84df-268">Няма</span><span class="sxs-lookup"><span data-stu-id="d84df-268">N\A</span></span> |


4. <span data-ttu-id="d84df-269">За да опресните обекта, изберете името на картата и след това изберете **Опресняване на обекти**.</span><span class="sxs-lookup"><span data-stu-id="d84df-269">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![Обновяване на карта](./media/20RefreshMapping.png)

5. <span data-ttu-id="d84df-271">Изпълнете картата след завършване на опресняването.</span><span class="sxs-lookup"><span data-stu-id="d84df-271">After the refresh is complete, run the map.</span></span> <span data-ttu-id="d84df-272">Преди да активирате следващата карта, проверете дали картата в таблицата е в състояние на **Изпълнение**.</span><span class="sxs-lookup"><span data-stu-id="d84df-272">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="d84df-273">Изпълнението на карти с по-голям брой предпоставки може да отнеме известно време.</span><span class="sxs-lookup"><span data-stu-id="d84df-273">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="d84df-274">За да стартирате карта с предпоставки, активирайте превключвателя **Показване на свързани карти на обекти**.</span><span class="sxs-lookup"><span data-stu-id="d84df-274">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="d84df-275">Ако таблицата показва **Предварително първоначално синхронизиране** като **Не**, проверете дали флагът **Първоначално синхронизиране** е **Изключен** във всички необходими карти, преди да го стартирате.</span><span class="sxs-lookup"><span data-stu-id="d84df-275">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![Стартирайте карта](./media/21RunMap.png)

6. <span data-ttu-id="d84df-277">Проверете дали всички свързани с проекта карти са в работно състояние.</span><span class="sxs-lookup"><span data-stu-id="d84df-277">Validate all project related maps are in the running state.</span></span>

![Всички карти работят](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a><span data-ttu-id="d84df-279">Прилагане на конфигурационни данни в CDS за Project Operations (по избор)</span><span class="sxs-lookup"><span data-stu-id="d84df-279">Apply configuration data in CDS for Project Operations (optional)</span></span>

<span data-ttu-id="d84df-280">Ако сте приложили демонстрационни данни към средата на Finance, вижте [Настройка и прилагане на конфигурационни данни в Common Data Service за Project Operations](resource-apply-pro-setup-config-data.md), за да приложите демонстрационни данни към среда на CDS.</span><span class="sxs-lookup"><span data-stu-id="d84df-280">If you have applied demo data to the Finance environment, see [Set up and apply configuration data in the Common Data Service for Project Operations](resource-apply-pro-setup-config-data.md) to apply demo data to CDS environment.</span></span>


<span data-ttu-id="d84df-281">Средата на Project Operations вече е подготвена и конфигурирана.</span><span class="sxs-lookup"><span data-stu-id="d84df-281">Your Project Operations environment is now provisioned and configured.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]