---
title: Настройване и прилагане на конфигурационни данни в Common Data Service
description: Тази тема предоставя информация за настройка и прилагане на конфигурационни данни в Project Operations.
author: sigitac
manager: Annbe
ms.date: 11/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7742e81316b217066f9f3b8d5c23aa64f1a7efc4
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642215"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a><span data-ttu-id="6ccd5-103">Настройване и прилагане на конфигурационни данни в Common Data Service</span><span class="sxs-lookup"><span data-stu-id="6ccd5-103">Set up and apply configuration data in the Common Data Service</span></span> 

<span data-ttu-id="6ccd5-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="6ccd5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="6ccd5-105">Предварителни изисквания</span><span class="sxs-lookup"><span data-stu-id="6ccd5-105">Prerequisites</span></span>

<span data-ttu-id="6ccd5-106">Преди да започнете да конфигурирате данни в Common Data Service (CDS), трябва да са изпълнени следните предварителни условия:</span><span class="sxs-lookup"><span data-stu-id="6ccd5-106">Before you beging to configure data in the Common Data Service (CDS), the following prerequisites must be met:</span></span>

1.  <span data-ttu-id="6ccd5-107">Осигурете среда на CDS среда и среда на Dynamics 365 Finance за Project Operations.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-107">Provision a CDS environment and a Dynamics 365 Finance environment for Project Operations.</span></span>
2.  <span data-ttu-id="6ccd5-108">Информацията за юридически лица от Dynamics 365 Finance се споделя в средата на CDS.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-108">Legal entity information from Dynamics 365 Finance is shared to the CDS environment.</span></span> <span data-ttu-id="6ccd5-109">Това означава, че обектът **Фирма** в CDS има следните фирмени записи:</span><span class="sxs-lookup"><span data-stu-id="6ccd5-109">This means that the **Company** entity in CDS has the following company records:</span></span>
  - <span data-ttu-id="6ccd5-110">THPM</span><span class="sxs-lookup"><span data-stu-id="6ccd5-110">THPM</span></span>
  - <span data-ttu-id="6ccd5-111">USPM</span><span class="sxs-lookup"><span data-stu-id="6ccd5-111">USPM</span></span>
  - <span data-ttu-id="6ccd5-112">GBPM</span><span class="sxs-lookup"><span data-stu-id="6ccd5-112">GBPM</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="6ccd5-113">Първоначална настройка и данни за конфигурация</span><span class="sxs-lookup"><span data-stu-id="6ccd5-113">Install setup and configuration data</span></span>

1. <span data-ttu-id="6ccd5-114">Изтеглете, деблокирайте и разархивирайте [Пакет за данни за настройка и конфигуриране](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span><span class="sxs-lookup"><span data-stu-id="6ccd5-114">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="6ccd5-115">Придвижете се до разархивираната папка и стартирайте изпълнимия файл, *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-115">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="6ccd5-116">На страница 1 на Common Data Service Съветник за миграция на конфигурация (CMT), изберете **Импортиране на данни** и след това изберете **Продължение**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-116">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Мигриране на конфигурация](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="6ccd5-118">На страница 2 от съветника за CMT изберете **Microsoft 365** като **Тип на внедряване**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-118">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="6ccd5-119">Изберете квадратчета за отметка **Показване на списък с наличните организации** и **Показване на напреднали**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-119">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="6ccd5-120">Изберете региона на вашия наемател, въведете вашите идентификационни данни и изберете **Вход**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-120">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![Вход в конфигурация](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="6ccd5-122">На страница 3 от списъка с организации на наемателя изберете организацията, в която искате да импортирате демонстрационните данни, и изберете **Вход**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-122">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="6ccd5-123">На страница 4 изберете zip файла, *SampleSetupAndConfigData* от разопакованата папка.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-123">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![Избор на Zip файл](./media/3ZipFile.png)

![Избор на файл](./media/4SelectAFile.png)

9. <span data-ttu-id="6ccd5-126">След като изберете zip файла, изберете **Импортиране на данни**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-126">After the zip file is selected, select **Import Data**.</span></span>

![Импортиране на данни](./media/5ImportData.png)

10. <span data-ttu-id="6ccd5-128">Импортирането ще продължи приблизително две-десет минути в зависимост от скоростта на вашата мрежа.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-128">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="6ccd5-129">След като импортирането завърши, излезте от съветника за CMT.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-129">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="6ccd5-130">Проверете вашата организация за данни в следните 19 обекта:</span><span class="sxs-lookup"><span data-stu-id="6ccd5-130">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="6ccd5-131">Валута</span><span class="sxs-lookup"><span data-stu-id="6ccd5-131">Currency</span></span>
  - <span data-ttu-id="6ccd5-132">Организационна единица</span><span class="sxs-lookup"><span data-stu-id="6ccd5-132">Organizational Unit</span></span>
  - <span data-ttu-id="6ccd5-133">Контакт</span><span class="sxs-lookup"><span data-stu-id="6ccd5-133">Contact</span></span>
  - <span data-ttu-id="6ccd5-134">Данъчна група</span><span class="sxs-lookup"><span data-stu-id="6ccd5-134">Tax Group</span></span>
  - <span data-ttu-id="6ccd5-135">Клиентска група</span><span class="sxs-lookup"><span data-stu-id="6ccd5-135">Customer Group</span></span>
  - <span data-ttu-id="6ccd5-136">Единица</span><span class="sxs-lookup"><span data-stu-id="6ccd5-136">Unit</span></span>
  - <span data-ttu-id="6ccd5-137">Опаковъчна единица</span><span class="sxs-lookup"><span data-stu-id="6ccd5-137">Unit Group</span></span>
  - <span data-ttu-id="6ccd5-138">Ценова листа</span><span class="sxs-lookup"><span data-stu-id="6ccd5-138">Price List</span></span>
  - <span data-ttu-id="6ccd5-139">Ценова листа на параметър на проекта</span><span class="sxs-lookup"><span data-stu-id="6ccd5-139">Project Parameter Price List</span></span>
  - <span data-ttu-id="6ccd5-140">Честота на фактура</span><span class="sxs-lookup"><span data-stu-id="6ccd5-140">Invoice Frequency</span></span>
  - <span data-ttu-id="6ccd5-141">Категория налични ресурси</span><span class="sxs-lookup"><span data-stu-id="6ccd5-141">Bookable Resource Category</span></span>
  - <span data-ttu-id="6ccd5-142">Категория на трансакция</span><span class="sxs-lookup"><span data-stu-id="6ccd5-142">Transaction Category</span></span>
  - <span data-ttu-id="6ccd5-143">Категория на разхода</span><span class="sxs-lookup"><span data-stu-id="6ccd5-143">Expense Category</span></span>
  - <span data-ttu-id="6ccd5-144">Цена на роля</span><span class="sxs-lookup"><span data-stu-id="6ccd5-144">Role Price</span></span>
  - <span data-ttu-id="6ccd5-145">Цена на категория транзакция</span><span class="sxs-lookup"><span data-stu-id="6ccd5-145">Transaction Category Price</span></span>
  - <span data-ttu-id="6ccd5-146">Характеристика</span><span class="sxs-lookup"><span data-stu-id="6ccd5-146">Characteristic</span></span>
  - <span data-ttu-id="6ccd5-147">Наличен ресурс</span><span class="sxs-lookup"><span data-stu-id="6ccd5-147">Bookable Resource</span></span>
  - <span data-ttu-id="6ccd5-148">Асоциация на категория налични ресурси</span><span class="sxs-lookup"><span data-stu-id="6ccd5-148">Bookable resource category Assn</span></span>
  - <span data-ttu-id="6ccd5-149">Характеристика на наличен ресурс</span><span class="sxs-lookup"><span data-stu-id="6ccd5-149">Bookable Resource Characteristic</span></span>

![Пълно импортиране](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="6ccd5-151">Актуализиране на конфигурациите на Project Operations</span><span class="sxs-lookup"><span data-stu-id="6ccd5-151">Update Project Operations configurations</span></span>

1. <span data-ttu-id="6ccd5-152">Навигиране до средата на CE.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-152">Navigate to the CE environment.</span></span> <span data-ttu-id="6ccd5-153">Можете да я намерите, като отворите [Административен център на Power Platform](https://admin.powerplatform.microsoft.com/environments), изберете среда и след това изберете **Отворена среда**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-153">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![Отваряне на средата](./media/7OpenEnvironment.png)

2. <span data-ttu-id="6ccd5-155">Отидете на **Проекти** > **Ресурси** и след това изберете **Създаване**, за да създадете резервируем ресурс за вашия потребител.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-155">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![Налични ресурси](./media/8BookableResources.png)

3. <span data-ttu-id="6ccd5-157">На раздела **Общи** изберете своя администратор.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-157">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="6ccd5-158">Уверете се, че часовата зона съвпада с тази, в която се намирате.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-158">Verify that the time zone matches the one you are in.</span></span> 

![Нов наличен ресурс](./media/9NewBookableResource.png)

4. <span data-ttu-id="6ccd5-160">В раздела **Планиране** в полето **Фирма** изберете фирмата **USPM** и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-160">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![Раздел за планиране](./media/10SchedulingTab.png)

5. <span data-ttu-id="6ccd5-162">Изберете раздела **Работни часове**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-162">Select the **Work hours** tab.</span></span>  

![Работно време](./media/11WorkHours.png)

6. <span data-ttu-id="6ccd5-164">Щракнете двукратно върху която и да е стойност в календара и изберете **редактиране** > **Всички събития от поредицата**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-164">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![Работен календар](./media/12WorkCalendar.png)

7. <span data-ttu-id="6ccd5-166">Сменете работното време на осем (8) работен ден, маркирайте почивните дни като неработни дни и се уверете, че часовата зона съвпада с вашата.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-166">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="6ccd5-167">Изберете **Записване и затваряне**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-167">Select **Save and close**.</span></span>

![Актуализиране на календар](./media/13UpdateCalendar.png)

9. <span data-ttu-id="6ccd5-169">Отидете на **Настройки** > **Шаблони на календара** и изберете **Създаване**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-169">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![Шаблони на календар](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="6ccd5-171">Въведете име, изберете ресурса на шаблона, който сте създали, и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-171">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![Записване на Шаблон на календар](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="6ccd5-173">Отидете на **Параметри** и щракнете двукратно върху записа.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-173">Go to **Parameters** and double-click the record.</span></span> 
 
 ![Параметри на проекта](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="6ccd5-175">Актуализирайте следните полета:</span><span class="sxs-lookup"><span data-stu-id="6ccd5-175">Update the following fields:</span></span>

 - <span data-ttu-id="6ccd5-176">**Фирма по подразбиране**: USPM</span><span class="sxs-lookup"><span data-stu-id="6ccd5-176">**Default company**: USPM</span></span>
 - <span data-ttu-id="6ccd5-177">**Организационна единица по подразбиране**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="6ccd5-177">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="6ccd5-178">**Честота на фактурите**: Седми и последен ден</span><span class="sxs-lookup"><span data-stu-id="6ccd5-178">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="6ccd5-179">**Шаблон за работен час**: Преминете към шаблона, който сте създали.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-179">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="6ccd5-180">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="6ccd5-180">Select **Save**.</span></span> 

![Актуализирани параметри на проекта](./media/17UpdatedProjectParameters.png)
