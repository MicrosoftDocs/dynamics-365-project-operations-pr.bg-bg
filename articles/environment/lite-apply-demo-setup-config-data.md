---
title: Прилагане на демонстрационни данни за настройка и конфигурация – олекотено
description: Тази тема предоставя информация за това как да приложите демонстрационни данни за настройка конфигурационни в Project Operations.
author: sigitac
manager: Annbe
ms.date: 11/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5cfc270c07a568d692f6cd180b9c367ae185044c
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401250"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="05551-103">Прилагане на демонстрационни данни за настройка и конфигурация за Project Operations – олекотено</span><span class="sxs-lookup"><span data-stu-id="05551-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="05551-104">_\*\*Леко внедряване – фактуриране на сделка към проформа_</span><span class="sxs-lookup"><span data-stu-id="05551-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05551-105">Предварителни изисквания</span><span class="sxs-lookup"><span data-stu-id="05551-105">Prerequisites</span></span>

<span data-ttu-id="05551-106">Преди да започнете конфигурацията, трябва да имате среда на Common Data Service (CDS), осигурена за Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="05551-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="05551-107">Инструкции</span><span class="sxs-lookup"><span data-stu-id="05551-107">Instructions</span></span>

1. <span data-ttu-id="05551-108">Изтеглете [Пакет с основни данни](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="05551-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="05551-109">Придвижете се до папката *ProjOpsDemoDataSetupAndMaster - Integrated CMT* и стартирайте изпълнимия файл *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="05551-109">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="05551-110">На страница 1 на Common Data Service Съветник за миграция на конфигурация (CMT), изберете **Импортиране на данни** и след това изберете **Продължение**.</span><span class="sxs-lookup"><span data-stu-id="05551-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Мигриране на конфигурация](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="05551-112">На страница 2 от съветника за CMT изберете **Microsoft 365** като **Тип на внедряване**.</span><span class="sxs-lookup"><span data-stu-id="05551-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="05551-113">Изберете квадратчета за отметка **Показване на списък с наличните организации** и **Показване на напреднали**.</span><span class="sxs-lookup"><span data-stu-id="05551-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="05551-114">Изберете региона на вашия наемател, въведете вашите идентификационни данни и след това изберете **Вход**.</span><span class="sxs-lookup"><span data-stu-id="05551-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![Вход в конфигурация](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="05551-116">На страница 3 от списъка с организации на клиента изберете организацията, в която искате да импортирате демонстрационните данни, и изберете **Вход**.</span><span class="sxs-lookup"><span data-stu-id="05551-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="05551-117">На страница 4 изберете zip файла *MasterAndSetupData* от разопакованата папка *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span><span class="sxs-lookup"><span data-stu-id="05551-117">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![Zip файл](./media/3ZipFile.png)

![Избор на файл](./media/4SelectAFile.png)

9. <span data-ttu-id="05551-120">След като изберете zip файла, изберете **Импортиране на данни**.</span><span class="sxs-lookup"><span data-stu-id="05551-120">After the zip file is selected, select **Import Data**.</span></span>

![Импортиране на данни](./media/5ImportData.png)

10. <span data-ttu-id="05551-122">Импортирането ще продължи приблизително две-десет минути в зависимост от скоростта на вашата мрежа.</span><span class="sxs-lookup"><span data-stu-id="05551-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="05551-123">След като завърши, излезте от съветника за CMT.</span><span class="sxs-lookup"><span data-stu-id="05551-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="05551-124">Проверете вашата организация за данни в следните 20 обекта:</span><span class="sxs-lookup"><span data-stu-id="05551-124">Check your organization for data in the following 20 entities:</span></span>

-   <span data-ttu-id="05551-125">Валута</span><span class="sxs-lookup"><span data-stu-id="05551-125">Currency</span></span>
-   <span data-ttu-id="05551-126">Клиент</span><span class="sxs-lookup"><span data-stu-id="05551-126">Account</span></span>
-   <span data-ttu-id="05551-127">Организационна единица</span><span class="sxs-lookup"><span data-stu-id="05551-127">Organizational Unit</span></span>
-   <span data-ttu-id="05551-128">Контакт</span><span class="sxs-lookup"><span data-stu-id="05551-128">Contact</span></span>
-   <span data-ttu-id="05551-129">Данъчна група</span><span class="sxs-lookup"><span data-stu-id="05551-129">Tax Group</span></span>
-   <span data-ttu-id="05551-130">Клиентска група</span><span class="sxs-lookup"><span data-stu-id="05551-130">Customer Group</span></span>
-   <span data-ttu-id="05551-131">Единица</span><span class="sxs-lookup"><span data-stu-id="05551-131">Unit</span></span>
-   <span data-ttu-id="05551-132">Опаковъчна единица</span><span class="sxs-lookup"><span data-stu-id="05551-132">Unit Group</span></span>
-   <span data-ttu-id="05551-133">Ценова листа</span><span class="sxs-lookup"><span data-stu-id="05551-133">Price List</span></span>
-   <span data-ttu-id="05551-134">Ценова листа на параметър на проекта</span><span class="sxs-lookup"><span data-stu-id="05551-134">Project Parameter Price List</span></span> 
-   <span data-ttu-id="05551-135">Честота на фактура</span><span class="sxs-lookup"><span data-stu-id="05551-135">Invoice Frequency</span></span>
-   <span data-ttu-id="05551-136">Категория налични ресурси</span><span class="sxs-lookup"><span data-stu-id="05551-136">Bookable Resource Category</span></span>
-   <span data-ttu-id="05551-137">Категория на трансакция</span><span class="sxs-lookup"><span data-stu-id="05551-137">Transaction Category</span></span>
-   <span data-ttu-id="05551-138">Категория на разхода</span><span class="sxs-lookup"><span data-stu-id="05551-138">Expense Category</span></span>
-   <span data-ttu-id="05551-139">Цена на роля</span><span class="sxs-lookup"><span data-stu-id="05551-139">Role Price</span></span>
-   <span data-ttu-id="05551-140">Цена на категория транзакция</span><span class="sxs-lookup"><span data-stu-id="05551-140">Transaction Category Price</span></span>
-   <span data-ttu-id="05551-141">Характеристика</span><span class="sxs-lookup"><span data-stu-id="05551-141">Characteristic</span></span>
-   <span data-ttu-id="05551-142">Наличен ресурс</span><span class="sxs-lookup"><span data-stu-id="05551-142">Bookable Resource</span></span>
-   <span data-ttu-id="05551-143">Асоциация на категория налични ресурси</span><span class="sxs-lookup"><span data-stu-id="05551-143">Bookable resource category Assn</span></span>
-   <span data-ttu-id="05551-144">Характеристика на наличен ресурс</span><span class="sxs-lookup"><span data-stu-id="05551-144">Bookable Resource Characteristic</span></span>

![Пълно импортиране](./media/6CompleteImport.png)
