---
title: Настройване и прилагане на конфигурационни данни в Common Data Service
description: Тази тема предоставя информация за настройка и прилагане на конфигурационни данни в Project Operations.
author: sigitac
ms.date: 05/10/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 2ea00df6112fb69b61f1889463424fdfee79aec9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001278"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a><span data-ttu-id="f46dd-103">Настройване и прилагане на конфигурационни данни в Common Data Service</span><span class="sxs-lookup"><span data-stu-id="f46dd-103">Set up and apply configuration data in the Common Data Service</span></span> 

<span data-ttu-id="f46dd-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="f46dd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="f46dd-105">Предварителни изисквания</span><span class="sxs-lookup"><span data-stu-id="f46dd-105">Prerequisites</span></span>

<span data-ttu-id="f46dd-106">Преди да започнете да конфигурирате данни в Common Data Service (CDS), трябва да са изпълнени следните предварителни изисквания:</span><span class="sxs-lookup"><span data-stu-id="f46dd-106">Before you begin to configure data in the Common Data Service (CDS), the following prerequisites must be met:</span></span>

1.  <span data-ttu-id="f46dd-107">Осигурете среда на CDS среда и среда на Dynamics 365 Finance за Project Operations.</span><span class="sxs-lookup"><span data-stu-id="f46dd-107">Provision a CDS environment and a Dynamics 365 Finance environment for Project Operations.</span></span>
2.  <span data-ttu-id="f46dd-108">Информацията за юридически лица от Dynamics 365 Finance се споделя в средата на CDS.</span><span class="sxs-lookup"><span data-stu-id="f46dd-108">Legal entity information from Dynamics 365 Finance is shared to the CDS environment.</span></span> <span data-ttu-id="f46dd-109">Това означава, че обектът **Фирма** в CDS има следните фирмени записи:</span><span class="sxs-lookup"><span data-stu-id="f46dd-109">This means that the **Company** entity in CDS has the following company records:</span></span>
  - <span data-ttu-id="f46dd-110">THPM</span><span class="sxs-lookup"><span data-stu-id="f46dd-110">THPM</span></span>
  - <span data-ttu-id="f46dd-111">USPM</span><span class="sxs-lookup"><span data-stu-id="f46dd-111">USPM</span></span>
  - <span data-ttu-id="f46dd-112">GBPM</span><span class="sxs-lookup"><span data-stu-id="f46dd-112">GBPM</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="f46dd-113">Първоначална настройка и данни за конфигурация</span><span class="sxs-lookup"><span data-stu-id="f46dd-113">Install setup and configuration data</span></span>

1. <span data-ttu-id="f46dd-114">Изтеглете, деблокирайте и разархивирайте [Пакет за данни за настройка и конфигуриране](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip).</span><span class="sxs-lookup"><span data-stu-id="f46dd-114">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip).</span></span>
2. <span data-ttu-id="f46dd-115">Придвижете се до разархивираната папка и стартирайте изпълнимия файл, *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="f46dd-115">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="f46dd-116">На страница 1 на Common Data Service Съветник за миграция на конфигурация (CMT), изберете **Импортиране на данни** и след това изберете **Продължение**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-116">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Мигриране на конфигурация](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="f46dd-118">На страница 2 от съветника за CMT изберете **Microsoft 365** като **Тип на внедряване**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-118">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="f46dd-119">Изберете квадратчета за отметка **Показване на списък с наличните организации** и **Показване на напреднали**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-119">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="f46dd-120">Изберете региона на вашия наемател, въведете вашите идентификационни данни и изберете **Вход**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-120">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![Вход в конфигурация](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="f46dd-122">На страница 3 от списъка с организации на наемателя изберете организацията, в която искате да импортирате демонстрационните данни, и изберете **Вход**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-122">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="f46dd-123">На страница 4 изберете zip файла, *SampleSetupAndConfigData* от разопакованата папка.</span><span class="sxs-lookup"><span data-stu-id="f46dd-123">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![Избор на Zip файл](./media/3ZipFile.png)

![Избор на файл](./media/4SelectAFile.png)

9. <span data-ttu-id="f46dd-126">След като изберете zip файла, изберете **Импортиране на данни**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-126">After the zip file is selected, select **Import Data**.</span></span>

![Импортиране на данни](./media/5ImportData.png)

10. <span data-ttu-id="f46dd-128">Импортирането ще продължи приблизително две-десет минути в зависимост от скоростта на вашата мрежа.</span><span class="sxs-lookup"><span data-stu-id="f46dd-128">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="f46dd-129">След като импортирането завърши, излезте от съветника за CMT.</span><span class="sxs-lookup"><span data-stu-id="f46dd-129">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="f46dd-130">Проверете вашата организация за данни в следните 26 обекта:</span><span class="sxs-lookup"><span data-stu-id="f46dd-130">Check your organization for data in the following 26 entities:</span></span>

  - <span data-ttu-id="f46dd-131">Валута</span><span class="sxs-lookup"><span data-stu-id="f46dd-131">Currency</span></span>
  - <span data-ttu-id="f46dd-132">Диаграма с акаунти</span><span class="sxs-lookup"><span data-stu-id="f46dd-132">Chart of Accounts</span></span>
  - <span data-ttu-id="f46dd-133">Финансов календар</span><span class="sxs-lookup"><span data-stu-id="f46dd-133">Fiscal Calendar</span></span>
  - <span data-ttu-id="f46dd-134">Типове обменни курсове на валута</span><span class="sxs-lookup"><span data-stu-id="f46dd-134">Currency Exchange Rate Types</span></span>
  - <span data-ttu-id="f46dd-135">Ден за плащане</span><span class="sxs-lookup"><span data-stu-id="f46dd-135">Payment Day</span></span>
  - <span data-ttu-id="f46dd-136">График на плащане</span><span class="sxs-lookup"><span data-stu-id="f46dd-136">Payment Schedule</span></span>
  - <span data-ttu-id="f46dd-137">Условие за плащане</span><span class="sxs-lookup"><span data-stu-id="f46dd-137">Payment Term</span></span>
  - <span data-ttu-id="f46dd-138">Организационна единица</span><span class="sxs-lookup"><span data-stu-id="f46dd-138">Organizational Unit</span></span>
  - <span data-ttu-id="f46dd-139">Контакт</span><span class="sxs-lookup"><span data-stu-id="f46dd-139">Contact</span></span>
  - <span data-ttu-id="f46dd-140">Данъчна група</span><span class="sxs-lookup"><span data-stu-id="f46dd-140">Tax Group</span></span>
  - <span data-ttu-id="f46dd-141">Клиентска група</span><span class="sxs-lookup"><span data-stu-id="f46dd-141">Customer Group</span></span>
  - <span data-ttu-id="f46dd-142">Група доставчици</span><span class="sxs-lookup"><span data-stu-id="f46dd-142">Vendor Group</span></span>
  - <span data-ttu-id="f46dd-143">Единица</span><span class="sxs-lookup"><span data-stu-id="f46dd-143">Unit</span></span>
  - <span data-ttu-id="f46dd-144">Опаковъчна единица</span><span class="sxs-lookup"><span data-stu-id="f46dd-144">Unit Group</span></span>
  - <span data-ttu-id="f46dd-145">Ценова листа</span><span class="sxs-lookup"><span data-stu-id="f46dd-145">Price List</span></span>
  - <span data-ttu-id="f46dd-146">Ценова листа на параметър на проекта</span><span class="sxs-lookup"><span data-stu-id="f46dd-146">Project Parameter Price List</span></span>
  - <span data-ttu-id="f46dd-147">Честота на фактура</span><span class="sxs-lookup"><span data-stu-id="f46dd-147">Invoice Frequency</span></span>
  - <span data-ttu-id="f46dd-148">Категория налични ресурси</span><span class="sxs-lookup"><span data-stu-id="f46dd-148">Bookable Resource Category</span></span>
  - <span data-ttu-id="f46dd-149">Категория на трансакция</span><span class="sxs-lookup"><span data-stu-id="f46dd-149">Transaction Category</span></span>
  - <span data-ttu-id="f46dd-150">Категория на разхода</span><span class="sxs-lookup"><span data-stu-id="f46dd-150">Expense Category</span></span>
  - <span data-ttu-id="f46dd-151">Цена на роля</span><span class="sxs-lookup"><span data-stu-id="f46dd-151">Role Price</span></span>
  - <span data-ttu-id="f46dd-152">Цена на категория транзакция</span><span class="sxs-lookup"><span data-stu-id="f46dd-152">Transaction Category Price</span></span>
  - <span data-ttu-id="f46dd-153">Характеристика</span><span class="sxs-lookup"><span data-stu-id="f46dd-153">Characteristic</span></span>
  - <span data-ttu-id="f46dd-154">Наличен ресурс</span><span class="sxs-lookup"><span data-stu-id="f46dd-154">Bookable Resource</span></span>
  - <span data-ttu-id="f46dd-155">Асоциация на категория налични ресурси</span><span class="sxs-lookup"><span data-stu-id="f46dd-155">Bookable resource category Assn</span></span>
  - <span data-ttu-id="f46dd-156">Характеристика на наличен ресурс</span><span class="sxs-lookup"><span data-stu-id="f46dd-156">Bookable Resource Characteristic</span></span>

![Пълно импортиране](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="f46dd-158">Актуализиране на конфигурациите на Project Operations</span><span class="sxs-lookup"><span data-stu-id="f46dd-158">Update Project Operations configurations</span></span>

1. <span data-ttu-id="f46dd-159">Навигиране до средата на CE.</span><span class="sxs-lookup"><span data-stu-id="f46dd-159">Navigate to the CE environment.</span></span> <span data-ttu-id="f46dd-160">Можете да я намерите, като отворите [Административен център на Power Platform](https://admin.powerplatform.microsoft.com/environments), изберете среда и след това изберете **Отворена среда**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-160">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![Отваряне на средата](./media/7OpenEnvironment.png)

2. <span data-ttu-id="f46dd-162">Отидете на **Проекти** > **Ресурси** и след това изберете **Създаване**, за да създадете резервируем ресурс за вашия потребител.</span><span class="sxs-lookup"><span data-stu-id="f46dd-162">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![Налични ресурси](./media/8BookableResources.png)

3. <span data-ttu-id="f46dd-164">На раздела **Общи** изберете своя администратор.</span><span class="sxs-lookup"><span data-stu-id="f46dd-164">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="f46dd-165">Уверете се, че часовата зона съвпада с тази, в която се намирате.</span><span class="sxs-lookup"><span data-stu-id="f46dd-165">Verify that the time zone matches the one you are in.</span></span> 

![Нов наличен ресурс](./media/9NewBookableResource.png)

4. <span data-ttu-id="f46dd-167">В раздела **Планиране** в полето **Фирма** изберете фирмата **USPM** и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-167">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![Раздел за планиране](./media/10SchedulingTab.png)

5. <span data-ttu-id="f46dd-169">Изберете раздела **Работни часове**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-169">Select the **Work hours** tab.</span></span>  

![Работно време](./media/11WorkHours.png)

6. <span data-ttu-id="f46dd-171">Щракнете двукратно върху която и да е стойност в календара и изберете **редактиране** > **Всички събития от поредицата**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-171">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![Работен календар](./media/12WorkCalendar.png)

7. <span data-ttu-id="f46dd-173">Сменете работното време на осем (8) работен ден, маркирайте почивните дни като неработни дни и се уверете, че часовата зона съвпада с вашата.</span><span class="sxs-lookup"><span data-stu-id="f46dd-173">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="f46dd-174">Изберете **Записване и затваряне**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-174">Select **Save and close**.</span></span>

![Актуализиране на календар](./media/13UpdateCalendar.png)

9. <span data-ttu-id="f46dd-176">Отидете на **Настройки** > **Шаблони на календара** и изберете **Създаване**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-176">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![Шаблони на календар](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="f46dd-178">Въведете име, изберете ресурса на шаблона, който сте създали, и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-178">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![Записване на Шаблон на календар](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="f46dd-180">Отидете на **Параметри** и щракнете двукратно върху записа.</span><span class="sxs-lookup"><span data-stu-id="f46dd-180">Go to **Parameters** and double-click the record.</span></span> 
 
 ![Параметри на проекта](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="f46dd-182">Актуализирайте следните полета:</span><span class="sxs-lookup"><span data-stu-id="f46dd-182">Update the following fields:</span></span>

 - <span data-ttu-id="f46dd-183">**Фирма по подразбиране**: USPM</span><span class="sxs-lookup"><span data-stu-id="f46dd-183">**Default company**: USPM</span></span>
 - <span data-ttu-id="f46dd-184">**Организационна единица по подразбиране**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="f46dd-184">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="f46dd-185">**Честота на фактурите**: Седми и последен ден</span><span class="sxs-lookup"><span data-stu-id="f46dd-185">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="f46dd-186">**Шаблон за работен час**: Преминете към шаблона, който сте създали.</span><span class="sxs-lookup"><span data-stu-id="f46dd-186">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="f46dd-187">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="f46dd-187">Select **Save**.</span></span> 

![Актуализирани параметри на проекта](./media/17UpdatedProjectParameters.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
