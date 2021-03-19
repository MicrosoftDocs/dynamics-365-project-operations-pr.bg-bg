---
title: Осигуряване на нова среда
description: Тази тема предоставя информация за това как да се осигури нова среда за Project Operations.
author: sigitac
manager: Annbe
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 50e623d3716c9dd03ce34ec293ba57b5d966d39e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276875"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="013b3-103">Осигуряване на нова среда</span><span class="sxs-lookup"><span data-stu-id="013b3-103">Provision a new environment</span></span>

<span data-ttu-id="013b3-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="013b3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="013b3-105">Тази тема предоставя информация за начина на осигуряване на нова среда на Dynamics 365 Project Operations за сценарии, базирани на ресурси/неналичност.</span><span class="sxs-lookup"><span data-stu-id="013b3-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="013b3-106">Активирайте автоматизираното осигуряване на Project Operations в LCS проект</span><span class="sxs-lookup"><span data-stu-id="013b3-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="013b3-107">Използвайте следните стъпки, за да активирате потока за автоматизирано предоставяне на Project Operations за вашия LCS проект.</span><span class="sxs-lookup"><span data-stu-id="013b3-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="013b3-108">Отидете на [LCS](https://lcs.dynamics.com/v2) и изберете плочката **Преглед на Управление на функции**.</span><span class="sxs-lookup"><span data-stu-id="013b3-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="013b3-109">В списъка **Функция за предварителен преглед** изберете **Функция Project Operations** и след това изберете **Функцията за преглед е активирана** за активиране на Project Operations.</span><span class="sxs-lookup"><span data-stu-id="013b3-109">In the **Preview feature** list, select **Project Operations Feature**, and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="013b3-110">Тази стъпка се извършва само веднъж за LCS проект.</span><span class="sxs-lookup"><span data-stu-id="013b3-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="013b3-111">Осигуряване на среда за Project Operations</span><span class="sxs-lookup"><span data-stu-id="013b3-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="013b3-112">Отворете ново внедряване в [демонстрационна среда](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) на Dynamics 365 Finance или [среда в ограничителен режим/производство](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="013b3-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="013b3-113">Преминете през съветника **Осигуряване на среда**.</span><span class="sxs-lookup"><span data-stu-id="013b3-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="013b3-114">Уверете се, че избраната версия на приложението е 10.0.13 или по-нова.</span><span class="sxs-lookup"><span data-stu-id="013b3-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="013b3-115">За предоставяне на Project Operations, под **Предварителни настройки**, изберете **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="013b3-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="013b3-116">Активирайте **Настройка на Common Data Service**, като изберете **Да**, и след това въведете информация в задължителните полета:</span><span class="sxs-lookup"><span data-stu-id="013b3-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="013b3-117">Име</span><span class="sxs-lookup"><span data-stu-id="013b3-117">Name</span></span>
  - <span data-ttu-id="013b3-118">Регион</span><span class="sxs-lookup"><span data-stu-id="013b3-118">Region</span></span>
  - <span data-ttu-id="013b3-119">Език</span><span class="sxs-lookup"><span data-stu-id="013b3-119">Language</span></span>
  - <span data-ttu-id="013b3-120">Валута</span><span class="sxs-lookup"><span data-stu-id="013b3-120">Currency</span></span>
 
5. <span data-ttu-id="013b3-121">В полето **Шаблон на Common Data Service** изберете **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="013b3-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="013b3-122">Изберете типа на среда за внедряването си.</span><span class="sxs-lookup"><span data-stu-id="013b3-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="013b3-123">Пробен период, базиран на абонамент, ще ви позволи да внедрите CDS среда за 30 дни.</span><span class="sxs-lookup"><span data-stu-id="013b3-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![Настройки за внедряване](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="013b3-125">Изберете **Съгласявам се**, за да потвърдите условията на услугата и след това да изберете **Готово**, за да се върнете към настройките за разполагане.</span><span class="sxs-lookup"><span data-stu-id="013b3-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![Съгласие за внедряване](./media/2DeploymentConsent.png)

7. <span data-ttu-id="013b3-127">По избор - Приложете демонстрационни данни към околната среда.</span><span class="sxs-lookup"><span data-stu-id="013b3-127">Optional - Apply demo data to the environment.</span></span> <span data-ttu-id="013b3-128">Отидете на **Разширени настройки**, изберете **Персонализирайте конфигурацията на базата данни на SQL** и задайте **Посочете набор от данни за база данни на приложения** на **Dемонстрация**.</span><span class="sxs-lookup"><span data-stu-id="013b3-128">Go to **Advanced settings**, select **Customize SQL Database Configuration**, and set **Specify a dataset for Application database** to **Demo**.</span></span>

8. <span data-ttu-id="013b3-129">Попълнете останалите задължителни полета в съветника и потвърдете разполагането.</span><span class="sxs-lookup"><span data-stu-id="013b3-129">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="013b3-130">Времето за осигуряване на среда варира в зависимост от типа на околната среда.</span><span class="sxs-lookup"><span data-stu-id="013b3-130">The time to provision the environment varies based on the environment type.</span></span> <span data-ttu-id="013b3-131">Предоставянето може да отнеме до шест часа.</span><span class="sxs-lookup"><span data-stu-id="013b3-131">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="013b3-132">След като разполагането завърши успешно, средата ще се покаже като **Внедрена**.</span><span class="sxs-lookup"><span data-stu-id="013b3-132">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

9. <span data-ttu-id="013b3-133">За да потвърдите, че средата се е разположила успешно, изберете **Вход** и влезте в средата, за да потвърдите.</span><span class="sxs-lookup"><span data-stu-id="013b3-133">To confirm that the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![Подробности за среди на ](./media/3EnvironmentDetails.png)

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="013b3-135">Прилагане на актуализации към среда на Finance</span><span class="sxs-lookup"><span data-stu-id="013b3-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="013b3-136">Project Operations изисква среда на Finance с версия на приложението **10.0.13 (10.0.569.20009)** или по-висока.</span><span class="sxs-lookup"><span data-stu-id="013b3-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="013b3-137">Може да се наложи да приложите качествени актуализации към вашата финансова среда, за да получите тази версия.</span><span class="sxs-lookup"><span data-stu-id="013b3-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="013b3-138">В LCS, на страницата **Подробности за среда** в секцията **Налични актуализации** изберете **Преглед на актуализацията**.</span><span class="sxs-lookup"><span data-stu-id="013b3-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![Преглед на актуализации](./media/5ViewUpdates.png)

2. <span data-ttu-id="013b3-140">На страницата **Двоични актуализации** изберете **Запазване на пакета.**</span><span class="sxs-lookup"><span data-stu-id="013b3-140">On the **Binary updates** page, select **Save package.**</span></span>

![Запазване на пакета](./media/6SavePackage.png)

3. <span data-ttu-id="013b3-142">Щракнете върху **Избор на всички** и след това изберете **Записване на пакета**.</span><span class="sxs-lookup"><span data-stu-id="013b3-142">Click **Select all** and then select **Save package**.</span></span>

![Преглед и запис на актуализации](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="013b3-144">Въведете име и описание на пакета и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="013b3-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="013b3-145">В зависимост от интернет връзката този процес може да отнеме известно време.</span><span class="sxs-lookup"><span data-stu-id="013b3-145">Depending on the internet connection, this process might take some time.</span></span>

![Качете пакета в библиотеката на активите](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="013b3-147">След като пакетът бъде запазен, изберете **готово** и запазете този пакет в библиотеката на активите във вашия LCS проект.</span><span class="sxs-lookup"><span data-stu-id="013b3-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="013b3-148">Запазването и валидирането на пакета може да отнеме ~15 минути.</span><span class="sxs-lookup"><span data-stu-id="013b3-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="013b3-149">За да приложите актуализацията, отидете на страницата **Подробности за среда** в LCS и изберете **Поддържане** > **Прилагане на актуализации**.</span><span class="sxs-lookup"><span data-stu-id="013b3-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![Поддръжка на среди](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="013b3-151">В списъка с актуализации изберете пакета, който сте създали, и изберете **Приложи**.</span><span class="sxs-lookup"><span data-stu-id="013b3-151">In the updates list select the package you created, and select **Apply**.</span></span>

![Прилагане на актуализации](./media/10ApplyUpdates.png)

<span data-ttu-id="013b3-153">Обслужването на околната среда ще отнеме известно време.</span><span class="sxs-lookup"><span data-stu-id="013b3-153">Environment servicing will take some time.</span></span> <span data-ttu-id="013b3-154">След като завърши, средата ще се върне в разположено състояние.</span><span class="sxs-lookup"><span data-stu-id="013b3-154">After it is complete, the environment will return to a deployed state.</span></span>

![Средата е внедрена](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="013b3-156">Установете връзка с двоен запис</span><span class="sxs-lookup"><span data-stu-id="013b3-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="013b3-157">Във вашия LCS проект отидете на страницата **Подробности за среда**.</span><span class="sxs-lookup"><span data-stu-id="013b3-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="013b3-158">Под **Информация за среда на Common Data Service** изберете **Връзка към CDS за приложения**.</span><span class="sxs-lookup"><span data-stu-id="013b3-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="013b3-159">След като връзката завърши, изберете отново **Връзка към CDS за приложения**.</span><span class="sxs-lookup"><span data-stu-id="013b3-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="013b3-160">Ще бъдете пренасочени към Двойно записване във Finance.</span><span class="sxs-lookup"><span data-stu-id="013b3-160">You will be redirected to Dual Write in Finance.</span></span>

![Връзка към CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="013b3-162">Изберете **Нанесете разтвор** за достъп до обектите, които ще бъдат картографирани в интеграцията.</span><span class="sxs-lookup"><span data-stu-id="013b3-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![Прилагане на решения](./media/13ApplySolutions.png)

5. <span data-ttu-id="013b3-164">Изберете двете решения, **Съпоставяне на обект с двукратно записване в Dynamics 365 Finance and Operations** и **Съпоставяния на обект с двукратно записване в Dynamics 365 Project Operations**, след което изберете **Прилагане**.</span><span class="sxs-lookup"><span data-stu-id="013b3-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![Потвърдете решенията](./media/14ConfirmSolutions.png)

<span data-ttu-id="013b3-166">След прилагането на решенията, обектите за двоен запис се прилагат към околната среда.</span><span class="sxs-lookup"><span data-stu-id="013b3-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![Прилагане на решения](./media/15ApplyingSolutions.png)

<span data-ttu-id="013b3-168">След като обектите са приложени, всички налични съпоставяния са изброени в средата.</span><span class="sxs-lookup"><span data-stu-id="013b3-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![Карти с двоен запис](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="013b3-170">Опреснете субектите на данни след актуализацията</span><span class="sxs-lookup"><span data-stu-id="013b3-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="013b3-171">Във Finance отидете на работното пространство **Управление на данни**.</span><span class="sxs-lookup"><span data-stu-id="013b3-171">In Finance, go to the **Data management** workspace.</span></span>

![Работно пространство за управление на данни](./media/16DataManagement.png)

2. <span data-ttu-id="013b3-173">Изберете плочката **Параметри на рамката**.</span><span class="sxs-lookup"><span data-stu-id="013b3-173">Select the **Framework parameters** tile.</span></span>

![Параметри на рамката](./media/17FrameworkParameters.png)

3. <span data-ttu-id="013b3-175">На страницата **Настройки на обекта** изберете **Опресняване на списъка с обекти**.</span><span class="sxs-lookup"><span data-stu-id="013b3-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![Обновяване на списък с обекти](./media/18RefreshEntityList.png)

<span data-ttu-id="013b3-177">Опресняването ще отнеме около 20 минути.</span><span class="sxs-lookup"><span data-stu-id="013b3-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="013b3-178">Ще получите предупреждение, когато приключи.</span><span class="sxs-lookup"><span data-stu-id="013b3-178">You will receive an alert when it is complete.</span></span>

![Потвърждение на обновяване](./media/19RefreshConfirmation.png)

## <a name="update-security-settings-on-project-operations-on-dataverse"></a><span data-ttu-id="013b3-180">Актуализирайте настройките за защита на Project Operations на Dataverse</span><span class="sxs-lookup"><span data-stu-id="013b3-180">Update security settings on Project Operations on Dataverse</span></span>

1. <span data-ttu-id="013b3-181">Отидете на Project Operations на средата на Dataverse.</span><span class="sxs-lookup"><span data-stu-id="013b3-181">Go to Project Operations on your Dataverse environment.</span></span> 
2. <span data-ttu-id="013b3-182">Отидете в **Настройки** > **Защита** > **Роли на защита**.</span><span class="sxs-lookup"><span data-stu-id="013b3-182">Go to **Settings** > **Security** > **Security roles**.</span></span> 
3. <span data-ttu-id="013b3-183">На страницата **Роли на защита** в списъка с роли изберете **потребител на приложение с двойно писане** и изберете раздела **Персонализирани обекти**.</span><span class="sxs-lookup"><span data-stu-id="013b3-183">On the **Security roles** page, in the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span>  
4. <span data-ttu-id="013b3-184">Проверете дали ролята имат разрешения **Четене** и **Добавяне към** за:</span><span class="sxs-lookup"><span data-stu-id="013b3-184">Verify that the role has **Read** and **Append To** permissions for the:</span></span>
      
      - <span data-ttu-id="013b3-185">**Тип на обменната валута**</span><span class="sxs-lookup"><span data-stu-id="013b3-185">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="013b3-186">**Диаграма с акаунти**</span><span class="sxs-lookup"><span data-stu-id="013b3-186">**Chart Of Accounts**</span></span>
      - <span data-ttu-id="013b3-187">**Финансов календар**</span><span class="sxs-lookup"><span data-stu-id="013b3-187">**Fiscal Calendar**</span></span>
      - <span data-ttu-id="013b3-188">**Счетоводна книга**</span><span class="sxs-lookup"><span data-stu-id="013b3-188">**Ledger**</span></span>

5. <span data-ttu-id="013b3-189">След като ролята на защита бъде актуализирана, отидете на **Настройки** > **Сигурност** > **Екипи** и изберете екипа по подразбиране в **Собственик на местен бизнес** екипен изглед.</span><span class="sxs-lookup"><span data-stu-id="013b3-189">After the security role is updated, go to **Settings** > **Security** > **Teams**, and select the default team in the **Local Business Owner** team view.</span></span>
6. <span data-ttu-id="013b3-190">Изберете **Управление на ролите** и проверете дали **потребител на приложение с двойно писане** привилегията за сигурност се прилага към този екип.</span><span class="sxs-lookup"><span data-stu-id="013b3-190">Select **Manage Roles** and verify that the **dual-write app user** security privilege is applied to this team.</span></span>

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="013b3-191">Изпълнение на карти Двойно записване на Project Operations</span><span class="sxs-lookup"><span data-stu-id="013b3-191">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="013b3-192">Във вашия LCS проект отидете на страницата **Подробности за среда**.</span><span class="sxs-lookup"><span data-stu-id="013b3-192">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="013b3-193">Под **Информация за среда на Common Data Service** изберете **Връзка към CDS за приложения**.</span><span class="sxs-lookup"><span data-stu-id="013b3-193">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="013b3-194">След като изберете връзката, ще бъдете пренасочени към списъка с обекти в съпоставянията.</span><span class="sxs-lookup"><span data-stu-id="013b3-194">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="013b3-195">Стартирайте картите, както е описано в следващата таблица.</span><span class="sxs-lookup"><span data-stu-id="013b3-195">Start the maps as described in the following table.</span></span> <span data-ttu-id="013b3-196">Не забравяйте да следвате последователността, както е изброено.</span><span class="sxs-lookup"><span data-stu-id="013b3-196">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="013b3-197">**Схема на свързване на обект**</span><span class="sxs-lookup"><span data-stu-id="013b3-197">**Entity Map**</span></span> | <span data-ttu-id="013b3-198">**Обновяване на обект**</span><span class="sxs-lookup"><span data-stu-id="013b3-198">**Refresh entity**</span></span> | <span data-ttu-id="013b3-199">**Първоначална синхронизация**</span><span class="sxs-lookup"><span data-stu-id="013b3-199">**Initial sync**</span></span> | <span data-ttu-id="013b3-200">**Главен елемент за първоначална синхронизация**</span><span class="sxs-lookup"><span data-stu-id="013b3-200">**Master for initial sync**</span></span> | <span data-ttu-id="013b3-201">**Изпълнение на предварителни изисквания**</span><span class="sxs-lookup"><span data-stu-id="013b3-201">**Run prerequisites**</span></span> | <span data-ttu-id="013b3-202">**Първоначална синхронизация на предварителни изисквания**</span><span class="sxs-lookup"><span data-stu-id="013b3-202">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="013b3-203">**Роли на проектните ресурси за всички фирми (резервационни ресурси)**</span><span class="sxs-lookup"><span data-stu-id="013b3-203">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="013b3-204">No</span><span class="sxs-lookup"><span data-stu-id="013b3-204">No</span></span> | <span data-ttu-id="013b3-205">Да</span><span class="sxs-lookup"><span data-stu-id="013b3-205">Yes</span></span> | <span data-ttu-id="013b3-206">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="013b3-206">Common Data Service</span></span> | <span data-ttu-id="013b3-207">No</span><span class="sxs-lookup"><span data-stu-id="013b3-207">No</span></span> | <span data-ttu-id="013b3-208">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-208">N\A</span></span> |
| <span data-ttu-id="013b3-209">**Юридически лица (cdm\_фирми)**</span><span class="sxs-lookup"><span data-stu-id="013b3-209">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="013b3-210">No</span><span class="sxs-lookup"><span data-stu-id="013b3-210">No</span></span> | <span data-ttu-id="013b3-211">Да</span><span class="sxs-lookup"><span data-stu-id="013b3-211">Yes</span></span> | <span data-ttu-id="013b3-212">Приложения на Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="013b3-212">Finance and Operations apps</span></span> | <span data-ttu-id="013b3-213">No</span><span class="sxs-lookup"><span data-stu-id="013b3-213">No</span></span> | <span data-ttu-id="013b3-214">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-214">N\A</span></span> |
| <span data-ttu-id="013b3-215">**Книга (msdyn_ledgers)**</span><span class="sxs-lookup"><span data-stu-id="013b3-215">**Ledger (msdyn_ledgers)**</span></span> | <span data-ttu-id="013b3-216">No</span><span class="sxs-lookup"><span data-stu-id="013b3-216">No</span></span> | <span data-ttu-id="013b3-217">Да</span><span class="sxs-lookup"><span data-stu-id="013b3-217">Yes</span></span> | <span data-ttu-id="013b3-218">Приложения на Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="013b3-218">Finance and Operations apps</span></span> | <span data-ttu-id="013b3-219">Да</span><span class="sxs-lookup"><span data-stu-id="013b3-219">Yes</span></span> | <span data-ttu-id="013b3-220">Да, приложения Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="013b3-220">Yes, Finance and Operations apps</span></span> |
| <span data-ttu-id="013b3-221">**Действителни данни за интеграция на Project Operations (msdyn\_действителни)**</span><span class="sxs-lookup"><span data-stu-id="013b3-221">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="013b3-222">No</span><span class="sxs-lookup"><span data-stu-id="013b3-222">No</span></span> | <span data-ttu-id="013b3-223">No</span><span class="sxs-lookup"><span data-stu-id="013b3-223">No</span></span> | <span data-ttu-id="013b3-224">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-224">N\A</span></span> | <span data-ttu-id="013b3-225">Да</span><span class="sxs-lookup"><span data-stu-id="013b3-225">Yes</span></span> | <span data-ttu-id="013b3-226">No</span><span class="sxs-lookup"><span data-stu-id="013b3-226">No</span></span> |
| <span data-ttu-id="013b3-227">**Аспекти на договор по проект (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="013b3-227">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="013b3-228">No</span><span class="sxs-lookup"><span data-stu-id="013b3-228">No</span></span> | <span data-ttu-id="013b3-229">No</span><span class="sxs-lookup"><span data-stu-id="013b3-229">No</span></span> | <span data-ttu-id="013b3-230">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-230">N\A</span></span> | <span data-ttu-id="013b3-231">No</span><span class="sxs-lookup"><span data-stu-id="013b3-231">No</span></span> | <span data-ttu-id="013b3-232">No</span><span class="sxs-lookup"><span data-stu-id="013b3-232">No</span></span> |
| <span data-ttu-id="013b3-233">**Интеграционен обект за взаимоотношения на проектни транзакции (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="013b3-233">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="013b3-234">No</span><span class="sxs-lookup"><span data-stu-id="013b3-234">No</span></span> | <span data-ttu-id="013b3-235">No</span><span class="sxs-lookup"><span data-stu-id="013b3-235">No</span></span> | <span data-ttu-id="013b3-236">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-236">N\A</span></span> | <span data-ttu-id="013b3-237">No</span><span class="sxs-lookup"><span data-stu-id="013b3-237">No</span></span> | <span data-ttu-id="013b3-238">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-238">N\A</span></span> |
| <span data-ttu-id="013b3-239">**Основни етапи на договора за интеграция на Project Operations (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="013b3-239">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="013b3-240">No</span><span class="sxs-lookup"><span data-stu-id="013b3-240">No</span></span> | <span data-ttu-id="013b3-241">No</span><span class="sxs-lookup"><span data-stu-id="013b3-241">No</span></span> | <span data-ttu-id="013b3-242">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-242">N\A</span></span> | <span data-ttu-id="013b3-243">No</span><span class="sxs-lookup"><span data-stu-id="013b3-243">No</span></span> | <span data-ttu-id="013b3-244">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-244">N\A</span></span> |
| <span data-ttu-id="013b3-245">**Обект за интеграция на Project Operations за оценки на разходите (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="013b3-245">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="013b3-246">No</span><span class="sxs-lookup"><span data-stu-id="013b3-246">No</span></span> | <span data-ttu-id="013b3-247">No</span><span class="sxs-lookup"><span data-stu-id="013b3-247">No</span></span> | <span data-ttu-id="013b3-248">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-248">N\A</span></span> | <span data-ttu-id="013b3-249">No</span><span class="sxs-lookup"><span data-stu-id="013b3-249">No</span></span> | <span data-ttu-id="013b3-250">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-250">N\A</span></span> |
| <span data-ttu-id="013b3-251">**Обект за експортиране на категории на разход по проект за интеграция на Project Operations (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="013b3-251">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="013b3-252">No</span><span class="sxs-lookup"><span data-stu-id="013b3-252">No</span></span> | <span data-ttu-id="013b3-253">No</span><span class="sxs-lookup"><span data-stu-id="013b3-253">No</span></span> | <span data-ttu-id="013b3-254">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-254">N\A</span></span> | <span data-ttu-id="013b3-255">No</span><span class="sxs-lookup"><span data-stu-id="013b3-255">No</span></span> | <span data-ttu-id="013b3-256">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-256">N\A</span></span> |
| <span data-ttu-id="013b3-257">**Обект за експортиране на Project Operations за интегриране на проектни разходи (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="013b3-257">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="013b3-258">Да</span><span class="sxs-lookup"><span data-stu-id="013b3-258">Yes</span></span> | <span data-ttu-id="013b3-259">No</span><span class="sxs-lookup"><span data-stu-id="013b3-259">No</span></span> | <span data-ttu-id="013b3-260">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-260">N\A</span></span> | <span data-ttu-id="013b3-261">No</span><span class="sxs-lookup"><span data-stu-id="013b3-261">No</span></span> | <span data-ttu-id="013b3-262">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-262">N\A</span></span> |
| <span data-ttu-id="013b3-263">**Обект за интеграция на Project Operations за оценки на часове (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="013b3-263">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="013b3-264">Да</span><span class="sxs-lookup"><span data-stu-id="013b3-264">Yes</span></span> | <span data-ttu-id="013b3-265">No</span><span class="sxs-lookup"><span data-stu-id="013b3-265">No</span></span> | <span data-ttu-id="013b3-266">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-266">N\A</span></span> | <span data-ttu-id="013b3-267">No</span><span class="sxs-lookup"><span data-stu-id="013b3-267">No</span></span> | <span data-ttu-id="013b3-268">Няма</span><span class="sxs-lookup"><span data-stu-id="013b3-268">N\A</span></span> |


4. <span data-ttu-id="013b3-269">За да опресните обекта, изберете името на картата и след това изберете **Опресняване на обекти**.</span><span class="sxs-lookup"><span data-stu-id="013b3-269">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![Обновяване на карта](./media/20RefreshMapping.png)

5. <span data-ttu-id="013b3-271">Изпълнете картата след завършване на опресняването.</span><span class="sxs-lookup"><span data-stu-id="013b3-271">After the refresh is complete, run the map.</span></span> <span data-ttu-id="013b3-272">Преди да активирате следващата карта, проверете дали картата в таблицата е в състояние на **Изпълнение**.</span><span class="sxs-lookup"><span data-stu-id="013b3-272">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="013b3-273">Изпълнението на карти с по-голям брой предпоставки може да отнеме известно време.</span><span class="sxs-lookup"><span data-stu-id="013b3-273">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="013b3-274">За да стартирате карта с предпоставки, активирайте превключвателя **Показване на свързани карти на обекти**.</span><span class="sxs-lookup"><span data-stu-id="013b3-274">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="013b3-275">Ако таблицата показва **Предварително първоначално синхронизиране** като **Не**, проверете дали флагът **Първоначално синхронизиране** е **Изключен** във всички необходими карти, преди да го стартирате.</span><span class="sxs-lookup"><span data-stu-id="013b3-275">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![Стартирайте карта](./media/21RunMap.png)

6. <span data-ttu-id="013b3-277">Проверете дали всички свързани с проекта карти са в работно състояние.</span><span class="sxs-lookup"><span data-stu-id="013b3-277">Validate all project related maps are in the running state.</span></span>

![Всички карти работят](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a><span data-ttu-id="013b3-279">Прилагане на конфигурационни данни в CDS за Project Operations (по избор)</span><span class="sxs-lookup"><span data-stu-id="013b3-279">Apply configuration data in CDS for Project Operations (optional)</span></span>

<span data-ttu-id="013b3-280">Ако сте приложили демонстрационни данни към средата на Finance, вижте [Настройка и прилагане на конфигурационни данни в Common Data Service за Project Operations](resource-apply-pro-setup-config-data.md), за да приложите демонстрационни данни към среда на CDS.</span><span class="sxs-lookup"><span data-stu-id="013b3-280">If you have applied demo data to the Finance environment, see [Set up and apply configuration data in the Common Data Service for Project Operations](resource-apply-pro-setup-config-data.md) to apply demo data to CDS environment.</span></span>


<span data-ttu-id="013b3-281">Средата на Project Operations вече е подготвена и конфигурирана.</span><span class="sxs-lookup"><span data-stu-id="013b3-281">Your Project Operations environment is now provisioned and configured.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]