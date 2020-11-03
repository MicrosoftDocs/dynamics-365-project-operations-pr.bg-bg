---
title: Използване на добавката за Project Service за планиране на работата в Microsoft Project | MicrosoftDocs
description: Тази тема предоставя информация за това как да добавите, конфигурирате и използвате добавката Microsoft Project за Microsoft Project Service.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
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
ms.openlocfilehash: 1d988419ae5a9d57532902d2553cd7de147e27c1
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071950"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a><span data-ttu-id="b3699-103">Използвайте добавката Project Service Automation за планиране на работата в Microsoft Project</span><span class="sxs-lookup"><span data-stu-id="b3699-103">Use the Project Service Automation Add-in to plan your work in Microsoft Project</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] <span data-ttu-id="b3699-104">ви улеснява при извършване на планирането на проекти, включително прогнози.</span><span class="sxs-lookup"><span data-stu-id="b3699-104">makes it easier for you to do your project planning, including estimates.</span></span> <span data-ttu-id="b3699-105">Можете да определите работата, така че да са ясни разходите, усилията и стойността на продажбите при подаване на окончателното предложение.</span><span class="sxs-lookup"><span data-stu-id="b3699-105">You can define the work so that costs, effort, and sales value are clear as the final proposal is submitted.</span></span>  

 <span data-ttu-id="b3699-106">Сега можете да инсталирате [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] и да извършите работата по планирането в познатата среда на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-106">Now you can install the [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] and do your planning work in the familiar environment of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span> <span data-ttu-id="b3699-107">Използвайте стабилните възможностите за планиране и управление на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и след това актуализирайте плана на проекта в Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="b3699-107">Use the robust planning and management capabilities of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and then update your project plan in Project Service Automation.</span></span>  

> [!IMPORTANT]
> - <span data-ttu-id="b3699-108">За да използвате управлението на документи на SharePoint за съхранение на файловете на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] за проекти на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], администраторът на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] трябва да включи управлението на документи.</span><span class="sxs-lookup"><span data-stu-id="b3699-108">To use SharePoint document management to store your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] files for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] projects, your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] admin will need to turn on document management.</span></span> 
> - <span data-ttu-id="b3699-109">[!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] е съвместим само с [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.</span><span class="sxs-lookup"><span data-stu-id="b3699-109">The [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] is only compatible with [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.</span></span>  

## <a name="download-and-install-the-add-in"></a><span data-ttu-id="b3699-110">Изтеглете и инсталирайте добавката</span><span class="sxs-lookup"><span data-stu-id="b3699-110">Download and install the add-in</span></span>  
 <span data-ttu-id="b3699-111">Подгответе информацията за регистрация в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-111">Have your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] sign-in information ready.</span></span> <span data-ttu-id="b3699-112">Тази информация ви е необходима, за да се свържете от [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] с [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-112">You will need this information to connect from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

1.  <span data-ttu-id="b3699-113">От центъра за изтегляния изтеглете добавката за вашата поддържана версия на Project Service – [v2.X](https://go.microsoft.com/fwlink/?linkid=828268) или [v 3.4+](https://www.microsoft.com/download/details.aspx?id=57956).</span><span class="sxs-lookup"><span data-stu-id="b3699-113">From the Download Center, download the add-in for your supported version of Project Service, either [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) or [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).</span></span>  

2.  <span data-ttu-id="b3699-114">Щракнете върху връзката за изтегляне.</span><span class="sxs-lookup"><span data-stu-id="b3699-114">Click the download link.</span></span>  

3.  <span data-ttu-id="b3699-115">Когато изтеглянето приключи, щракнете върху **Да** за инсталиране на добавката.</span><span class="sxs-lookup"><span data-stu-id="b3699-115">When the download is complete, click **Yes** to install the add-in.</span></span>  

## <a name="configure-the-add-in"></a><span data-ttu-id="b3699-116">Конфигуриране на добавката</span><span class="sxs-lookup"><span data-stu-id="b3699-116">Configure the add-in</span></span>  

1. <span data-ttu-id="b3699-117">Отворете [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и щракнете върху раздел **Project Service**.</span><span class="sxs-lookup"><span data-stu-id="b3699-117">Open [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and click the **Project Service** tab.</span></span>  

2. <span data-ttu-id="b3699-118">Щракнете върху **свързване**.</span><span class="sxs-lookup"><span data-stu-id="b3699-118">Click **Connect**.</span></span>  

3. <span data-ttu-id="b3699-119">Въведете информацията си за влизане и след това щракнете върху **Влизане**.</span><span class="sxs-lookup"><span data-stu-id="b3699-119">Enter your sign-in information and then click **Sign in**.</span></span>  

   <span data-ttu-id="b3699-120">Вече можете да започнете да използвате добавката.</span><span class="sxs-lookup"><span data-stu-id="b3699-120">Now you can start using the add-in.</span></span>  

## <a name="read-from-a-template"></a><span data-ttu-id="b3699-121">Четене от шаблон</span><span class="sxs-lookup"><span data-stu-id="b3699-121">Read from a template</span></span>  
 <span data-ttu-id="b3699-122">Четете от шаблон, който сте създали в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] и сте копирали в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], за да започнете да планирате своя проект.</span><span class="sxs-lookup"><span data-stu-id="b3699-122">Read from a template that you created in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] and copied into [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to start your project planning.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="b3699-123">[Създаване на шаблон на проект (Project Service Automation)](../psa/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="b3699-123">[Create a project template (Project Service Automation)](../psa/create-project-template.md)</span></span>  

1.  <span data-ttu-id="b3699-124">От раздела **Project Service** щракнете върху **Четене** > **Шаблон на проект на Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="b3699-124">From the **Project Service** tab, click **Read** > **Project Service Automation Project Template**.</span></span>  

2.  <span data-ttu-id="b3699-125">Изберете шаблон на проект от списъка и след това щракнете върху **Отвори**.</span><span class="sxs-lookup"><span data-stu-id="b3699-125">Choose a project template from the list and then click **Open**.</span></span>  

    > [!NOTE]
    >  <span data-ttu-id="b3699-126">По подразбиране задачите, които са копирани от шаблона в проекта, са зададени като ръчно планирани.</span><span class="sxs-lookup"><span data-stu-id="b3699-126">By default, the tasks that are copied from the template into Project are set as manually scheduled.</span></span>  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a><span data-ttu-id="b3699-127">Присвояване на роли на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] на ресурси на проекти</span><span class="sxs-lookup"><span data-stu-id="b3699-127">Assign [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] roles to project resources</span></span>  

1.  <span data-ttu-id="b3699-128">Отворете проект и щракнете върху лентата **Задача**.</span><span class="sxs-lookup"><span data-stu-id="b3699-128">Open a project and click the **Task** ribbon.</span></span>  

2.  <span data-ttu-id="b3699-129">Щракнете върху менюто **Диаграма на Гант** и след това изберете **Лист на ресурсите**.</span><span class="sxs-lookup"><span data-stu-id="b3699-129">Click the **Gantt Chart** menu and then choose **Resource Sheet**.</span></span>  

3.  <span data-ttu-id="b3699-130">В листа на ресурсите, щракнете върху падащото меню **Роля на ресурс в Project Service** и изберете роля в Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="b3699-130">On the Resource Sheet, click the **Project Service Resource Role** drop-down menu and choose a Project Service Automation role.</span></span>  

## <a name="staff-your-project-with-resources"></a><span data-ttu-id="b3699-131">Осигурете ресурси за проекта си</span><span class="sxs-lookup"><span data-stu-id="b3699-131">Staff your project with resources</span></span>  

1.  <span data-ttu-id="b3699-132">От раздела Project Service изберете ред и щракнете върху **Търсене на ресурси**.</span><span class="sxs-lookup"><span data-stu-id="b3699-132">From the Project Service tab, select a row and click **Find Resources**.</span></span>  

2.  <span data-ttu-id="b3699-133">На екрана **Резервиране на ресурс** изберете ресурса, който искате да използвате за проекта.</span><span class="sxs-lookup"><span data-stu-id="b3699-133">On the **Book Resource** screen, select the resource that you want to use for the project.</span></span>  

3.  <span data-ttu-id="b3699-134">Щракнете върху **Резервирай** и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="b3699-134">Click **Book** and then click **OK**.</span></span>  

## <a name="publish-your-project"></a><span data-ttu-id="b3699-135">Публикуване на вашия проект</span><span class="sxs-lookup"><span data-stu-id="b3699-135">Publish your project</span></span>  
<span data-ttu-id="b3699-136">Когато приключи планирането на проекта, следващата стъпка е импортиране и публикуване на проекта в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-136">When your project planning is complete, the next step is to import and publish the project in to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

<span data-ttu-id="b3699-137">Проектът ще се импортира в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-137">The project will import into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> <span data-ttu-id="b3699-138">Прилагат се ценообразуването и процесът на генериране на екип.</span><span class="sxs-lookup"><span data-stu-id="b3699-138">The pricing and team generation process are applied.</span></span> <span data-ttu-id="b3699-139">Отворете проекта в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], за да проверите, че са генерирани екипът, оценките на проекта и съставната структура на работата.</span><span class="sxs-lookup"><span data-stu-id="b3699-139">Open the project in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to see that the team, project estimates, and work breakdown structure has been generated.</span></span> <span data-ttu-id="b3699-140">В таблицата по-долу е показано къде да се намерят резултатите:</span><span class="sxs-lookup"><span data-stu-id="b3699-140">The following table shows where to find the results:</span></span>


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="b3699-141">**Диаграма на Гант**</span><span class="sxs-lookup"><span data-stu-id="b3699-141">**Gantt Chart**</span></span>   | <span data-ttu-id="b3699-142">Импортиране в екрана на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Съставна структура на работата**.</span><span class="sxs-lookup"><span data-stu-id="b3699-142">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Work Breakdown Structure** screen.</span></span> |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="b3699-143">**Списък с ресурси**</span><span class="sxs-lookup"><span data-stu-id="b3699-143">**Resource Sheet**</span></span> |   <span data-ttu-id="b3699-144">Импортиране в екрана на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Членове на екипа на проект**.</span><span class="sxs-lookup"><span data-stu-id="b3699-144">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Team Members** screen.</span></span>   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="b3699-145">**Използване на употреба**</span><span class="sxs-lookup"><span data-stu-id="b3699-145">**Use Usage**</span></span>    |    <span data-ttu-id="b3699-146">Импортиране в екрана на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Оценки на проект**.</span><span class="sxs-lookup"><span data-stu-id="b3699-146">Omports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Estimates** screen.</span></span>     |

<span data-ttu-id="b3699-147">**За да импортирате и публикувате проекта**</span><span class="sxs-lookup"><span data-stu-id="b3699-147">**To import and publish your project**</span></span>  
1. <span data-ttu-id="b3699-148">От раздела **Project Service** щракнете върху **Публикуване** > **Нов проект на Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="b3699-148">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project**.</span></span>  

2. <span data-ttu-id="b3699-149">На диалоговия прозорец **Публикуване в нов проект в Project Service** въведете **Име на проект** и изберете **Клиент**.</span><span class="sxs-lookup"><span data-stu-id="b3699-149">On **Publish to a new project in Project Service** dialog box, enter the **Project Name** and select the **Customer**.</span></span>  

3. <span data-ttu-id="b3699-150">По желание проверете **Свързване на плана на проекта с Project Service Automation** , за да се свърже файлът на плана на проекта с Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="b3699-150">Optionally check the **Link project plan to Project Service Automation** to link the plan Project file to Project Service Automation.</span></span>  

4. <span data-ttu-id="b3699-151">Щракнете върху **Публикуване**.</span><span class="sxs-lookup"><span data-stu-id="b3699-151">Click **Publish**.</span></span>  

   <span data-ttu-id="b3699-152">Свързването на файла на проекта с [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] прави файла на проекта главен и задава съставната структура на работата в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] като само за четене.</span><span class="sxs-lookup"><span data-stu-id="b3699-152">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to read-only.</span></span>  <span data-ttu-id="b3699-153">За да направите промени в плана на проекта, трябва да ги направите в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да ги публикувате като актуализации в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-153">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

## <a name="edit-a-project-thats-been-imported"></a><span data-ttu-id="b3699-154">Редактиране на проект, който е импортиран</span><span class="sxs-lookup"><span data-stu-id="b3699-154">Edit a project that’s been imported</span></span>  
 <span data-ttu-id="b3699-155">За да направите промени на план на проект, който е импортиран в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], имате две опции:</span><span class="sxs-lookup"><span data-stu-id="b3699-155">To make changes to a project plan that's been imported into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you have two options:</span></span>  

- <span data-ttu-id="b3699-156">Отваряне на главния файл и редактиране в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-156">Open the master file and edit it in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

- <span data-ttu-id="b3699-157">Премахване на връзката на файла и редактиране директно в Project Service.</span><span class="sxs-lookup"><span data-stu-id="b3699-157">Unlink the file and edit it directly in Project Service.</span></span> <span data-ttu-id="b3699-158">По подразбиране проект, който е качен от [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], е заключен и може да се редактира само в проекта.</span><span class="sxs-lookup"><span data-stu-id="b3699-158">By default, a project that’s been uploaded from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] is locked and can only be edited in Project.</span></span> <span data-ttu-id="b3699-159">За да редактирате файла в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], връзката на файла трябва да се премахне.</span><span class="sxs-lookup"><span data-stu-id="b3699-159">To edit the file in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], the file has to be unlinked.</span></span>  

### <a name="edit-in-pn_microsoft_project"></a><span data-ttu-id="b3699-160">Редактиране в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span><span class="sxs-lookup"><span data-stu-id="b3699-160">Edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span></span>  

1. <span data-ttu-id="b3699-161">От главното меню щракнете върху **Project Service** > **Проекти**.</span><span class="sxs-lookup"><span data-stu-id="b3699-161">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="b3699-162">От списъка с проекти отворете този, който сте създали в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-162">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="b3699-163">Щракнете върху **Отвори в MS Project** от лентата.</span><span class="sxs-lookup"><span data-stu-id="b3699-163">Click **Open in MS Project** from the ribbon.</span></span> <span data-ttu-id="b3699-164">Така ще се отвори свързаният главен файл в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-164">This will open the linked master file in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a><span data-ttu-id="b3699-165">Премахване на връзката на файл и редактиране в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service</span><span class="sxs-lookup"><span data-stu-id="b3699-165">Unlink a file and edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service</span></span>  

1. <span data-ttu-id="b3699-166">От главното меню щракнете върху **Project Service** > **Проекти**.</span><span class="sxs-lookup"><span data-stu-id="b3699-166">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="b3699-167">От списъка с проекти отворете този, който сте създали в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-167">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="b3699-168">Щракнете върху **Премахни връзката с MS Project** от лентата.</span><span class="sxs-lookup"><span data-stu-id="b3699-168">Click **Unlink from MS Project** from the ribbon.</span></span>  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a><span data-ttu-id="b3699-169">Качване на файл на проект в SharePoint или групи на Office</span><span class="sxs-lookup"><span data-stu-id="b3699-169">Upload a Project file to SharePoint or Office Groups</span></span>  
 <span data-ttu-id="b3699-170">Можете да качите файла на проекта си в SharePoint и да го намерите под „Свързани документи” за проекта на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-170">You can upload your Project file to SharePoint and find it under the Associated Documents for your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  <span data-ttu-id="b3699-171">Администраторът трябва да конфигурира управление на документи на SharePoint и да го включи за обекта на проекта.</span><span class="sxs-lookup"><span data-stu-id="b3699-171">You need to have your administrator configure SharePoint document management and turn it on for the Project entity.</span></span> 

 <span data-ttu-id="b3699-172">Също така можете да качите файла на проекта на [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)], ако имате зададени групи на Office.</span><span class="sxs-lookup"><span data-stu-id="b3699-172">You can also upload your Project file to [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] if you have Office Groups set up.</span></span>

### <a name="upload-a-file-for-sharepoint"></a><span data-ttu-id="b3699-173">Качване на файл за SharePoint</span><span class="sxs-lookup"><span data-stu-id="b3699-173">Upload a file for SharePoint</span></span>  

1. <span data-ttu-id="b3699-174">От главното меню щракнете върху **Project Service** > **Качване**.</span><span class="sxs-lookup"><span data-stu-id="b3699-174">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="b3699-175">Изберете **Към документи на проект в Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="b3699-175">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="b3699-176">В диалоговия прозорец **Разрешаване на отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** изберете **Да** или **Не**.</span><span class="sxs-lookup"><span data-stu-id="b3699-176">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="b3699-177">Ако щракнете върху **Да** , ще можете да изберете бутона **Отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** в Project Service Automation, да стартирате [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да заредите файла на проекта от библиотеката с документи на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b3699-177">If you click **Yes** , you'll be able select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="b3699-178">Ако щракнете върху **Не** , връзката за бутона **Отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** няма да работи.</span><span class="sxs-lookup"><span data-stu-id="b3699-178">If you click **No** , the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="b3699-179">Файлът на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] може да се намери в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] под **Документи** за конкретния проект на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-179">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

### <a name="upload-a-file-for-office-groups"></a><span data-ttu-id="b3699-180">Качване на файл за групи на Office</span><span class="sxs-lookup"><span data-stu-id="b3699-180">Upload a file for Office Groups</span></span>  

1. <span data-ttu-id="b3699-181">От главното меню щракнете върху **Project Service** > **Качване**.</span><span class="sxs-lookup"><span data-stu-id="b3699-181">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="b3699-182">Изберете **Към документи на проект в Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="b3699-182">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="b3699-183">В диалоговия прозорец **Разрешаване на отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** изберете **Да** или **Не**.</span><span class="sxs-lookup"><span data-stu-id="b3699-183">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="b3699-184">Ако щракнете върху **Да** , ще можете да изберете бутона **Отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** в Project Service Automation, да стартирате [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да заредите файла на проекта от библиотеката с документи на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b3699-184">If you click **Yes** , you'll be able to select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="b3699-185">Ако щракнете върху **Не** , връзката за бутона **Отваряне в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** няма да работи.</span><span class="sxs-lookup"><span data-stu-id="b3699-185">If you click **No** , the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="b3699-186">Файлът на [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] може да се намери в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] под **Документи** за конкретния проект на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-186">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

## <a name="publish--your-project-as-a-template"></a><span data-ttu-id="b3699-187">Публикуване на вашия проект като шаблон</span><span class="sxs-lookup"><span data-stu-id="b3699-187">Publish  your project as a template</span></span>  
 <span data-ttu-id="b3699-188">Можете да запишете проекта си и да го използвате отново, като го запишете като шаблон на проект в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-188">You can save your project and reuse it by saving it as a project template in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  <span data-ttu-id="b3699-189">Шаблоните на проекти са планове на проекти за многократна употреба в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-189">Project templates are reusable project plans in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="b3699-190">[Създаване на шаблон на проект (Project Service Automation)](../psa/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="b3699-190">[Create a project template (Project Service Automation)](../psa/create-project-template.md)</span></span>  

1. <span data-ttu-id="b3699-191">От раздела **Project Service** щракнете върху **Публикуване** > **Нов шаблон на проект на Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="b3699-191">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project Template**.</span></span>  

2. <span data-ttu-id="b3699-192">На диалоговия прозорец **Публикуване в нов проект в шаблон на Project Service** въведете **Име на шаблона на проект**.</span><span class="sxs-lookup"><span data-stu-id="b3699-192">On the **Publish to a new project in Project Service template** dialog box, enter the **Project template name**.</span></span>  

3. <span data-ttu-id="b3699-193">По желание проверете **Свързване на плана на проекта с Project Service Automation** , за да се свърже файлът на проекта с [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-193">Optionally, check the **Link project plan to Project Service Automation** to link the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

4. <span data-ttu-id="b3699-194">Щракнете върху **Публикуване**.</span><span class="sxs-lookup"><span data-stu-id="b3699-194">Click **Publish**.</span></span>  

<span data-ttu-id="b3699-195">Свързването на файла на проекта с [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] прави файла на проекта главен и задава съставната структура на работата в шаблона на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] само за четене.</span><span class="sxs-lookup"><span data-stu-id="b3699-195">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] template to read-only.</span></span>  <span data-ttu-id="b3699-196">За да направите промени в плана на проекта, трябва да ги направите в [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] и да ги публикувате като актуализации в [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="b3699-196">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>

### <a name="see-also"></a><span data-ttu-id="b3699-197">Вижте също</span><span class="sxs-lookup"><span data-stu-id="b3699-197">See Also</span></span>  
 [<span data-ttu-id="b3699-198">Ръководство за мениджъри на проекти</span><span class="sxs-lookup"><span data-stu-id="b3699-198">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
