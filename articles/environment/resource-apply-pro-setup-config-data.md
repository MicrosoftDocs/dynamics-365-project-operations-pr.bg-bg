---
title: Настройка и прилагане на конфигурационни данни в Common Data Service за Project Operations
description: Тази тема предоставя информация за настройка и прилагане на конфигурационни данни в Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d99ab4c7b2ebf6ba56b86a3e0151036c6247e484
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948750"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service-for-project-operations"></a><span data-ttu-id="b99f6-103">Настройка и прилагане на конфигурационни данни в Common Data Service за Project Operations</span><span class="sxs-lookup"><span data-stu-id="b99f6-103">Set up and apply configuration data in the Common Data Service for Project Operations</span></span>

<span data-ttu-id="b99f6-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="b99f6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="b99f6-105">Първоначална настройка и данни за конфигурация</span><span class="sxs-lookup"><span data-stu-id="b99f6-105">Install setup and configuration data</span></span>

1. <span data-ttu-id="b99f6-106">Изтеглете, деблокирайте и разархивирайте [Пакет за данни за настройка и конфигуриране](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span><span class="sxs-lookup"><span data-stu-id="b99f6-106">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="b99f6-107">Придвижете се до разархивираната папка и стартирайте изпълнимия файл, *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="b99f6-107">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="b99f6-108">На страница 1 на Common Data Service Съветник за миграция на конфигурация (CMT), изберете **Импортиране на данни** и след това изберете **Продължение**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-108">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Мигриране на конфигурация](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="b99f6-110">На страница 2 от съветника за CMT изберете **Office 365** като **Тип на внедряване**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-110">On Page 2 of the CMT Wizard, select **Office 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="b99f6-111">Изберете квадратчета за отметка **Показване на списък с наличните организации** и **Показване на напреднали**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-111">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="b99f6-112">Изберете региона на вашия наемател, въведете вашите идентификационни данни и изберете **Вход**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-112">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![Вход в конфигурация](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="b99f6-114">На страница 3 от списъка с организации на наемателя изберете организацията, в която искате да импортирате демонстрационните данни, и изберете **Вход**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-114">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="b99f6-115">На страница 4 изберете zip файла, *SampleSetupAndConfigData* от разопакованата папка.</span><span class="sxs-lookup"><span data-stu-id="b99f6-115">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![Избор на Zip файл](./media/3ZipFile.png)

![Избор на файл](./media/4SelectAFile.png)

9. <span data-ttu-id="b99f6-118">След като изберете zip файла, изберете **Импортиране на данни**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-118">After the zip file is selected, select **Import Data**.</span></span>

![Импортиране на данни](./media/5ImportData.png)

10. <span data-ttu-id="b99f6-120">Импортирането ще продължи приблизително две-десет минути в зависимост от скоростта на вашата мрежа.</span><span class="sxs-lookup"><span data-stu-id="b99f6-120">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="b99f6-121">След като импортирането завърши, излезте от съветника за CMT.</span><span class="sxs-lookup"><span data-stu-id="b99f6-121">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="b99f6-122">Проверете вашата организация за данни в следните 19 обекта:</span><span class="sxs-lookup"><span data-stu-id="b99f6-122">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="b99f6-123">Валута</span><span class="sxs-lookup"><span data-stu-id="b99f6-123">Currency</span></span>
  - <span data-ttu-id="b99f6-124">Организационна единица</span><span class="sxs-lookup"><span data-stu-id="b99f6-124">Organizational Unit</span></span>
  - <span data-ttu-id="b99f6-125">Контакт</span><span class="sxs-lookup"><span data-stu-id="b99f6-125">Contact</span></span>
  - <span data-ttu-id="b99f6-126">Данъчна група</span><span class="sxs-lookup"><span data-stu-id="b99f6-126">Tax Group</span></span>
  - <span data-ttu-id="b99f6-127">Клиентска група</span><span class="sxs-lookup"><span data-stu-id="b99f6-127">Customer Group</span></span>
  - <span data-ttu-id="b99f6-128">Единица</span><span class="sxs-lookup"><span data-stu-id="b99f6-128">Unit</span></span>
  - <span data-ttu-id="b99f6-129">Опаковъчна единица</span><span class="sxs-lookup"><span data-stu-id="b99f6-129">Unit Group</span></span>
  - <span data-ttu-id="b99f6-130">Ценова листа</span><span class="sxs-lookup"><span data-stu-id="b99f6-130">Price List</span></span>
  - <span data-ttu-id="b99f6-131">Ценова листа на параметър на проекта</span><span class="sxs-lookup"><span data-stu-id="b99f6-131">Project Parameter Price List</span></span>
  - <span data-ttu-id="b99f6-132">Честота на фактура</span><span class="sxs-lookup"><span data-stu-id="b99f6-132">Invoice Frequency</span></span>
  - <span data-ttu-id="b99f6-133">Категория налични ресурси</span><span class="sxs-lookup"><span data-stu-id="b99f6-133">Bookable Resource Category</span></span>
  - <span data-ttu-id="b99f6-134">Категория на трансакция</span><span class="sxs-lookup"><span data-stu-id="b99f6-134">Transaction Category</span></span>
  - <span data-ttu-id="b99f6-135">Категория на разхода</span><span class="sxs-lookup"><span data-stu-id="b99f6-135">Expense Category</span></span>
  - <span data-ttu-id="b99f6-136">Цена на роля</span><span class="sxs-lookup"><span data-stu-id="b99f6-136">Role Price</span></span>
  - <span data-ttu-id="b99f6-137">Цена на категория транзакция</span><span class="sxs-lookup"><span data-stu-id="b99f6-137">Transaction Category Price</span></span>
  - <span data-ttu-id="b99f6-138">Характеристика</span><span class="sxs-lookup"><span data-stu-id="b99f6-138">Characteristic</span></span>
  - <span data-ttu-id="b99f6-139">Наличен ресурс</span><span class="sxs-lookup"><span data-stu-id="b99f6-139">Bookable Resource</span></span>
  - <span data-ttu-id="b99f6-140">Асоциация на категория налични ресурси</span><span class="sxs-lookup"><span data-stu-id="b99f6-140">Bookable resource category Assn</span></span>
  - <span data-ttu-id="b99f6-141">Характеристика на наличен ресурс</span><span class="sxs-lookup"><span data-stu-id="b99f6-141">Bookable Resource Characteristic</span></span>

![Пълно импортиране](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="b99f6-143">Актуализиране на конфигурациите на Project Operations</span><span class="sxs-lookup"><span data-stu-id="b99f6-143">Update Project Operations configurations</span></span>

1. <span data-ttu-id="b99f6-144">Навигиране до средата на CE.</span><span class="sxs-lookup"><span data-stu-id="b99f6-144">Navigate to the CE environment.</span></span> <span data-ttu-id="b99f6-145">Можете да я намерите, като отворите [Административен център на Power Platform](https://admin.powerplatform.microsoft.com/environments), изберете среда и след това изберете **Отворена среда**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-145">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![Отваряне на средата](./media/7OpenEnvironment.png)

2. <span data-ttu-id="b99f6-147">Отидете на **Проекти** > **Ресурси** и след това изберете **Създаване**, за да създадете резервируем ресурс за вашия потребител.</span><span class="sxs-lookup"><span data-stu-id="b99f6-147">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![Налични ресурси](./media/8BookableResources.png)

3. <span data-ttu-id="b99f6-149">На раздела **Общи** изберете своя администратор.</span><span class="sxs-lookup"><span data-stu-id="b99f6-149">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="b99f6-150">Уверете се, че часовата зона съвпада с тази, в която се намирате.</span><span class="sxs-lookup"><span data-stu-id="b99f6-150">Verify that the time zone matches the one you are in.</span></span> 

![Нов наличен ресурс](./media/9NewBookableResource.png)

4. <span data-ttu-id="b99f6-152">В раздела **Планиране** в полето **Фирма** изберете фирмата **USPM** и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-152">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![Раздел за планиране](./media/10SchedulingTab.png)

5. <span data-ttu-id="b99f6-154">Изберете раздела **Работни часове**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-154">Select the **Work hours** tab.</span></span>  

![Работно време](./media/11WorkHours.png)

6. <span data-ttu-id="b99f6-156">Щракнете двукратно върху която и да е стойност в календара и изберете **редактиране** > **Всички събития от поредицата**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-156">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![Работен календар](./media/12WorkCalendar.png)

7. <span data-ttu-id="b99f6-158">Сменете работното време на осем (8) работен ден, маркирайте почивните дни като неработни дни и се уверете, че часовата зона съвпада с вашата.</span><span class="sxs-lookup"><span data-stu-id="b99f6-158">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="b99f6-159">Изберете **Записване и затваряне**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-159">Select **Save and close**.</span></span>

![Актуализиране на календар](./media/13UpdateCalendar.png)

9. <span data-ttu-id="b99f6-161">Отидете на **Настройки** > **Шаблони на календара** и изберете **Създаване**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-161">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![Шаблони на календар](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="b99f6-163">Въведете име, изберете ресурса на шаблона, който сте създали, и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-163">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![Записване на Шаблон на календар](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="b99f6-165">Отидете на **Параметри** и щракнете двукратно върху записа.</span><span class="sxs-lookup"><span data-stu-id="b99f6-165">Go to **Parameters** and double-click the record.</span></span> 
 
 ![Параметри на проекта](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="b99f6-167">Актуализирайте следните полета:</span><span class="sxs-lookup"><span data-stu-id="b99f6-167">Update the following fields:</span></span>

 - <span data-ttu-id="b99f6-168">**Фирма по подразбиране**: USPM</span><span class="sxs-lookup"><span data-stu-id="b99f6-168">**Default company**: USPM</span></span>
 - <span data-ttu-id="b99f6-169">**Организационна единица по подразбиране**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="b99f6-169">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="b99f6-170">**Честота на фактурите**: Седми и последен ден</span><span class="sxs-lookup"><span data-stu-id="b99f6-170">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="b99f6-171">**Шаблон за работен час**: Преминете към шаблона, който сте създали.</span><span class="sxs-lookup"><span data-stu-id="b99f6-171">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="b99f6-172">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="b99f6-172">Select **Save**.</span></span> 

![Актуализирани параметри на проекта](./media/17UpdatedProjectParameters.png)
