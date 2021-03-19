---
title: Актуализирайте Project Operations във вашата финансова среда
description: Тази тема предоставя информация за това как да актуализирате Project Operations в средата си на Dynamics 365 Finance.
author: ruhercul
manager: tfehr
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: d68296ec59f0bd58f848154c90e02c58f275ab12
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291966"
---
# <a name="update-project-operations-in-your-finance-environment"></a><span data-ttu-id="dc5d8-103">Актуализирайте Project Operations във вашата финансова среда</span><span class="sxs-lookup"><span data-stu-id="dc5d8-103">Update Project Operations in your Finance environment</span></span>

<span data-ttu-id="dc5d8-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="dc5d8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="dc5d8-105">Тази тема предоставя информация за това как да актуализирате Dynamics 365 Project Operations в средата си на Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-105">This topic provides information about how to update Dynamics 365 Project Operations in your Dynamics 365 Finance environment.</span></span> <span data-ttu-id="dc5d8-106">Има три процедури, които са необходими за актуализиране на Project Operations до Update 5 (UR5):</span><span class="sxs-lookup"><span data-stu-id="dc5d8-106">There are three procedures that are required to update Project Operations to Update 5 (UR5):</span></span>

- [<span data-ttu-id="dc5d8-107">Импортирайте пакета във вашия проект за преглед</span><span class="sxs-lookup"><span data-stu-id="dc5d8-107">Import the package into your preview project</span></span>](#import)
- [<span data-ttu-id="dc5d8-108">Приложете актуализацията</span><span class="sxs-lookup"><span data-stu-id="dc5d8-108">Apply the update</span></span>](#apply)
- [<span data-ttu-id="dc5d8-109">Актуализирайте средата си на Dataverse</span><span class="sxs-lookup"><span data-stu-id="dc5d8-109">Update your Dataverse environment</span></span>](#update)

## <a name="import-the-package-into-your-lcs-project"></a><a name="import"></a><span data-ttu-id="dc5d8-110">Импортирайте пакета във вашия LCS проект</span><span class="sxs-lookup"><span data-stu-id="dc5d8-110">Import the package into your LCS project</span></span>

1. <span data-ttu-id="dc5d8-111">Влезте в [Lifecycle Services (LCS)](https://lcs.dynamics.com/) като собственик на проект или мениджър на среда.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-111">Sign in to [Lifecycle Services (LCS)](https://lcs.dynamics.com/) as a Project Owner or Environment manager.</span></span>
2. <span data-ttu-id="dc5d8-112">От списъка с проекти изберете вашия LCS проект.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-112">From the list of projects, select your LCS project.</span></span>
3. <span data-ttu-id="dc5d8-113">На страницата **Проект** в групата **Среда**, отворете средата, която искате да актуализирате.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-113">On the **Project** page, in the **Environments** group, open the environment that you want to update.</span></span>
4. <span data-ttu-id="dc5d8-114">Проверете дали средата работи.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-114">Verify that the environment is running.</span></span> <span data-ttu-id="dc5d8-115">Ако не е стартиран, стартирайте средата.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-115">If it isn't started, start the environment.</span></span>
5. <span data-ttu-id="dc5d8-116">В секцията **Ново издание** под **Налични актуализации** изберете **Преглед на актуализацията** за 10.0.15.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-116">In the **New release** section under **Available updates**, select **View update** for 10.0.15.</span></span>

![Бутон за преглед на актуализация](media/view-update.png)

6. <span data-ttu-id="dc5d8-118">На страницата **Двоични актуализации** изберете **Запазване на пакета**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-118">On the **Binary updates** page, select **Save package**.</span></span>
7. <span data-ttu-id="dc5d8-119">На страницата **Преглед и записване на актуализации** изберете **Записване на пакета**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-119">On the **Review and save updates** page, select **Save package**.</span></span>
8. <span data-ttu-id="dc5d8-120">На екрана **Записване на пакета в библиотеката с активи**, който се отваря, въведете името на пакета и след това изберете **Записване на пакета**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-120">On the **Save package to asset library** pane that opens, enter the package name and then select **Save package**.</span></span>
9. <span data-ttu-id="dc5d8-121">Когато LCS приключи запазването на пакета, се активира бутонът **Готово**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-121">When LCS has finished saving the package, the **Done** button is enabled.</span></span> <span data-ttu-id="dc5d8-122">Изберете **Готово**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-122">Select **Done**.</span></span> <span data-ttu-id="dc5d8-123">LCS ще провери пакета.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-123">LCS will verify the package.</span></span> <span data-ttu-id="dc5d8-124">Проверката може да отнеме няколко минути или до един час.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-124">Verification can take a few minutes or up to one hour.</span></span>


## <a name="apply-the-package-update"></a><a name="apply"></a><span data-ttu-id="dc5d8-125">Прилагане на актуализацията на пакет</span><span class="sxs-lookup"><span data-stu-id="dc5d8-125">Apply the package update</span></span>

1. <span data-ttu-id="dc5d8-126">В LCS, на страницата **Подробности за среда** изберете **Поддръжка** > **Прилагане на актуализации**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-126">In LCS, on the **Environment details** page, select **Maintain** > **Apply Updates**.</span></span>
2. <span data-ttu-id="dc5d8-127">От списъка изберете пакета, който сте запазили по-рано, и след това изберете **Прилагане**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-127">From the list, select the package that you saved earlier, and then select **Apply**.</span></span>
3. <span data-ttu-id="dc5d8-128">Изберете **Да**, за да потвърдите, че искате да разположите пакета.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-128">Select **Yes** to confirm that you want to deploy the package.</span></span>

![Потвърдете диалоговия прозорец за разполагане на пакети](media/confirm-package-deployment.png)

4. <span data-ttu-id="dc5d8-130">Изберете **Да**, за да потвърдите, че искате да актуализирате приложението.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-130">Select **Yes** to confirm that you want to update the application.</span></span>

![Потвърдете диалоговия прозорец за актуализиране на приложението](media/confirm-application-update.png)

<span data-ttu-id="dc5d8-132">Ще започне разгръщането и актуализацията на приложението.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-132">The deployment and application update will start.</span></span> 

<span data-ttu-id="dc5d8-133">На страницата **Подробности за среда** в горния десен ъгъл, състоянието на среда ще се актуализира до **Обслужване**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-133">On the **Environment details** page, in the top-right corner, the environment status will update to **Servicing**.</span></span> <span data-ttu-id="dc5d8-134">Приблизително два часа актуализацията ще бъде завършена.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-134">In approximately two hours, the update will be complete.</span></span> <span data-ttu-id="dc5d8-135">Информацията за изданието на приложението ще се актуализира до **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** и състоянието на околната среда ще се актуализира до **внедрена**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-135">The application release information will update to **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** and the environment status will update to **Deployed**.</span></span>


## <a name="update-your-dataverse-environment"></a><a name="update"></a><span data-ttu-id="dc5d8-136">Актуализирайте средата си на Dataverse</span><span class="sxs-lookup"><span data-stu-id="dc5d8-136">Update your Dataverse environment</span></span>

1. <span data-ttu-id="dc5d8-137">Влезте в [центъра за администриране на Power Platform](https://admin.powerplatform.com/).</span><span class="sxs-lookup"><span data-stu-id="dc5d8-137">Sign in to the [Power Platform admin center](https://admin.powerplatform.com/).</span></span>
2. <span data-ttu-id="dc5d8-138">В списъка намерете и отворете средата, която сте използвали за инсталиране на Project Operations.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-138">In the list, find and open the environment that you used to install Project Operations.</span></span>
3. <span data-ttu-id="dc5d8-139">На страницата **Среди** изберете **Ресурс** > **Приложения на Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-139">On the **Environments** page, select **Resource** > **Dynamics 365 apps**.</span></span>
4. <span data-ttu-id="dc5d8-140">Намерете в списъка **Microsoft Dynamics 365 Project Operations** и в колоната **Състояние** изберете **Налична актуализация**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-140">In the list, locate **Microsoft Dynamics 365 Project Operations**, and in the **Status** column, select **Update Available**.</span></span>
5. <span data-ttu-id="dc5d8-141">Изберете **Съгласен съм с Условията на услугата** и след това изберете **Актуализиране**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-141">Select the **I agree to the terms of service** check box, and then select **Update**.</span></span> <span data-ttu-id="dc5d8-142">Ще бъде инсталирана най-новата версия на решението.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-142">The latest version of the solution will be installed.</span></span>

<span data-ttu-id="dc5d8-143">След като инсталацията приключи, ще имате инсталирана версия 4.5.0.134.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-143">After the installation is complete, you'll have version 4.5.0.134 installed.</span></span>

## <a name="configure-new-features"></a><span data-ttu-id="dc5d8-144">Конфигуриране на нови функции</span><span class="sxs-lookup"><span data-stu-id="dc5d8-144">Configure new features</span></span>

### <a name="enable-dual-write-mapping"></a><span data-ttu-id="dc5d8-145">Активиране на нанасяне с двукратно записване</span><span class="sxs-lookup"><span data-stu-id="dc5d8-145">Enable dual-write mapping</span></span>

<span data-ttu-id="dc5d8-146">След като завършите актуализацията на средите на Finance и Dataverse, можете да активирате необходимите съпоставяния с двойно писане.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-146">After you complete the update on the Finance and Dataverse environments, you can enable the required dual-write mappings.</span></span> <span data-ttu-id="dc5d8-147">Изпълнете следните процедури, за да активирате нанасяния с двойно записване.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-147">Complete the following procedures to enable dual-write mappings.</span></span>

- [<span data-ttu-id="dc5d8-148">Актуализирайте настройките за защита в средата на Customer Engagement</span><span class="sxs-lookup"><span data-stu-id="dc5d8-148">Update security settings on Customer Engagement environment</span></span>](#security)
- [<span data-ttu-id="dc5d8-149">Обновяване на обекти на данни</span><span class="sxs-lookup"><span data-stu-id="dc5d8-149">Refresh data entities</span></span>](#refresh)
- [<span data-ttu-id="dc5d8-150">Актуализирайте и изпълнете нанасянията с двойно писане</span><span class="sxs-lookup"><span data-stu-id="dc5d8-150">Update and run the dual-write mappings</span></span>](#run)

### <a name="update-security-settings-on-the-dataverse-environment"></a><a name="security"></a><span data-ttu-id="dc5d8-151">Актуализирайте настройките за защита в средата на Dataverse</span><span class="sxs-lookup"><span data-stu-id="dc5d8-151">Update security settings on the Dataverse environment</span></span>

<span data-ttu-id="dc5d8-152">Следните актуализации на правата за защита за обекти се изискват като част от актуализацията на UR5.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-152">The following updates to the security privileges for entities are required as part of the update to UR5.</span></span>

1. <span data-ttu-id="dc5d8-153">В средата си на Dataverse отидете на **Настройки** и в групата **Система** изберете **Защита**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-153">In your Dataverse environment, go to **Settings**, and in the **System** group, select **Security**.</span></span>

![Настройки на среда на Dataverse](media/Picture21.png)

2. <span data-ttu-id="dc5d8-155">Изберете **Права за достъп**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-155">Select **Security Roles**.</span></span>
3. <span data-ttu-id="dc5d8-156">От списъка с роли изберете **потребител на приложение с двойно писане** и изберете раздела **Персонализирани обекти**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-156">From the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span> 
4. <span data-ttu-id="dc5d8-157">Проверете дали ролята имат разрешения **Четене** и **Добавяне към** за:</span><span class="sxs-lookup"><span data-stu-id="dc5d8-157">Verify that the role has **Read** and **Append To** permissions for:</span></span>

      - <span data-ttu-id="dc5d8-158">**Тип на обменната валута**</span><span class="sxs-lookup"><span data-stu-id="dc5d8-158">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="dc5d8-159">**Диаграма с акаунти**</span><span class="sxs-lookup"><span data-stu-id="dc5d8-159">**Chart Of Accounts**</span></span> 
      - <span data-ttu-id="dc5d8-160">**Финансов календар**</span><span class="sxs-lookup"><span data-stu-id="dc5d8-160">**Fiscal Calendar**</span></span> 
      - <span data-ttu-id="dc5d8-161">**Счетоводна книга**</span><span class="sxs-lookup"><span data-stu-id="dc5d8-161">**Ledger**</span></span>

5. <span data-ttu-id="dc5d8-162">След като ролята на защита бъде актуализирана, отидете на **Настройки** > **Защита** > **Екипи**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-162">After the security role is updated, go to **Settings** > **Security** > **Teams**.</span></span> <span data-ttu-id="dc5d8-163">Проверете дали ролята **потребител на приложение с двойно писане** е приложена към екипа.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-163">Verify that the **dual-write app user** role has been applied to the team.</span></span> 

### <a name="refresh-data-entities-from-the-update"></a><a name="refresh"></a><span data-ttu-id="dc5d8-164">Опреснете субектите на данни от актуализацията</span><span class="sxs-lookup"><span data-stu-id="dc5d8-164">Refresh data entities from the update</span></span>

1. <span data-ttu-id="dc5d8-165">Във вашата финансова среда отворете работното пространство **Управление на данни** и след това отворете страницата **Параметри на рамката**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-165">In your Finance environment, open the **Data management** workspace, and then open the **Framework parameters** page.</span></span>
2. <span data-ttu-id="dc5d8-166">На раздела **Настройки на обекта** изберете **Опресняване на списъка с обекти**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-166">On the **Entity settings** tab, select **Refresh entity list**.</span></span>
3. <span data-ttu-id="dc5d8-167">Изберете **Затваряне**, за да потвърдите опресняването на обекта.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-167">Select **Close** to confirm the entity refresh.</span></span>

 > [!NOTE]
 > <span data-ttu-id="dc5d8-168">Този процес ще отнеме от пет до 20 минути.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-168">This process will take approximately 20 minutes to complete.</span></span> <span data-ttu-id="dc5d8-169">Ще бъдете уведомени, когато опресняването приключи.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-169">You will be notified when the refresh is complete.</span></span>

### <a name="update-dual-write-mappings"></a><a name="run"></a><span data-ttu-id="dc5d8-170">Актуализиране на нанасяния с двойно записване</span><span class="sxs-lookup"><span data-stu-id="dc5d8-170">Update dual-write mappings</span></span>

1. <span data-ttu-id="dc5d8-171">В работното пространство **Управление на данни** изберете **Двойно писане**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-171">In the **Data management** workspace, select **Dual-write**.</span></span>
2. <span data-ttu-id="dc5d8-172">Изберете **Прилагане на решения** изберете двете решения от списъка и след това изберете **Приложи**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-172">Select **Apply solutions**, select both solutions in the list, and then select **Apply**.</span></span>
3. <span data-ttu-id="dc5d8-173">На страницата **Двойно писане** изберете следните таблични карти и след това изберете **Стоп**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-173">On the **Dual-write** page, select the following table maps, and then select **Stop**.</span></span>

    - <span data-ttu-id="dc5d8-174">**Действителни данни за интеграция на Project Operations (msdyn_actuals)**</span><span class="sxs-lookup"><span data-stu-id="dc5d8-174">**Project Operations integration actuals (msdyn_actuals)**</span></span>
    - <span data-ttu-id="dc5d8-175">**Категории разходи за проекти за интеграция на Project Operations (msdyn_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="dc5d8-175">**Project Operations integration project expense categories (msdyn_expensecategories)**</span></span>
    - <span data-ttu-id="dc5d8-176">**Обект на експортиране на разходи по проект на действителни данни за интеграция на Project Operations (msdyn_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="dc5d8-176">**Project Operations integration actuals project expenses export entity (msdyn_expenses)**</span></span>

4. <span data-ttu-id="dc5d8-177">На страницата **Версия на табличната карта** приложете нова версия на картата към всеки от трите обекта.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-177">On the **Table map version** page, apply a new version of the map to each of the three entities.</span></span>
5. <span data-ttu-id="dc5d8-178">На страницата **Двойно писане** страница, изберете изпълнение, за да рестартирате картите.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-178">On the **Dual-write** page, select run to restart the maps.</span></span>
6. <span data-ttu-id="dc5d8-179">От списъка с карти изберете картата **Счетоводна книга (msdyn_ledgers)** с всички предпоставки и изберете квадратчето **Първоначално синхронизиране**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-179">From the list of maps, select the **Ledger (msdyn_ledgers)** map with all prerequisites and select the **Initial sync** check box.</span></span> 
7. <span data-ttu-id="dc5d8-180">В полето **База за първоначална синхронизация** изберете **Приложения на Finance and Operations** и след това изберете **Изпълнение**.</span><span class="sxs-lookup"><span data-stu-id="dc5d8-180">In the **Master for initial sync** field, select **Finance and Operations apps** and then select **Run**.</span></span>
 
 ![Синхронизиране на карта на книга](media/DW6.png)
 


[!INCLUDE[footer-include](../includes/footer-banner.md)]