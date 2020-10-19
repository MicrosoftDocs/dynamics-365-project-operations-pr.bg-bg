---
title: Прилагане на демонстрационни данни за настройка и конфигурация
description: Тази тема предоставя информация за това как да приложите демонстрационни данни за настройка конфигурационни в Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 42e02f393e89d20b2a462645f519a3792bee8f2f
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948747"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations-lite-deployment---deal-to-proforma-invoicing"></a><span data-ttu-id="10378-103">Приложете демонстрационни данни за настройка и конфигурация за внедряване на Project Operations lite - сключете сделка за проформа фактуриране</span><span class="sxs-lookup"><span data-stu-id="10378-103">Apply demo setup and configuration data for Project Operations lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="10378-104">_\*\*Леко внедряване – фактуриране на сделка към проформа_</span><span class="sxs-lookup"><span data-stu-id="10378-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

1. <span data-ttu-id="10378-105">Изтеглете [Пакет с основни данни](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="10378-105">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="10378-106">Придвижете се до папката *ProjOpsDemoDataSetupAndMaster - Integrated CMT* и стартирайте изпълнимия файл *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="10378-106">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="10378-107">На страница 1 на Common Data Service Съветник за миграция на конфигурация (CMT), изберете **Импортиране на данни** и след това изберете **Продължение**.</span><span class="sxs-lookup"><span data-stu-id="10378-107">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Мигриране на конфигурация](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="10378-109">На страница 2 от съветника за CMT изберете **Office 365** като **Тип на внедряване**.</span><span class="sxs-lookup"><span data-stu-id="10378-109">On Page 2 of the CMT Wizard, select **Office 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="10378-110">Изберете квадратчета за отметка **Показване на списък с наличните организации** и **Показване на напреднали**.</span><span class="sxs-lookup"><span data-stu-id="10378-110">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="10378-111">Изберете региона на вашия наемател, въведете вашите идентификационни данни и след това изберете **Вход**.</span><span class="sxs-lookup"><span data-stu-id="10378-111">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![Вход в конфигурация](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="10378-113">На страница 3 от списъка с организации на клиента изберете организацията, в която искате да импортирате демонстрационните данни, и изберете **Вход**.</span><span class="sxs-lookup"><span data-stu-id="10378-113">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="10378-114">На страница 4 изберете zip файла *MasterAndSetupData* от разопакованата папка *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span><span class="sxs-lookup"><span data-stu-id="10378-114">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![Zip файл](./media/3ZipFile.png)

![Избор на файл](./media/4SelectAFile.png)

9. <span data-ttu-id="10378-117">След като изберете zip файла, изберете **Импортиране на данни**.</span><span class="sxs-lookup"><span data-stu-id="10378-117">After the zip file is selected, select **Import Data**.</span></span>

![Импортиране на данни](./media/5ImportData.png)

10. <span data-ttu-id="10378-119">Импортирането ще продължи приблизително две-десет минути в зависимост от скоростта на вашата мрежа.</span><span class="sxs-lookup"><span data-stu-id="10378-119">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="10378-120">След като завърши, излезте от съветника за CMT.</span><span class="sxs-lookup"><span data-stu-id="10378-120">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="10378-121">Проверете вашата организация за данни в следните 20 обекта:</span><span class="sxs-lookup"><span data-stu-id="10378-121">Check your organization for data in the following 20 entities:</span></span>

- <span data-ttu-id="10378-122">Валута</span><span class="sxs-lookup"><span data-stu-id="10378-122">Currency</span></span>
- <span data-ttu-id="10378-123">Организационна единица</span><span class="sxs-lookup"><span data-stu-id="10378-123">Organizational Unit</span></span>
- <span data-ttu-id="10378-124">Контакт</span><span class="sxs-lookup"><span data-stu-id="10378-124">Contact</span></span>
- <span data-ttu-id="10378-125">Данъчна група</span><span class="sxs-lookup"><span data-stu-id="10378-125">Tax Group</span></span>
- <span data-ttu-id="10378-126">Клиентска група</span><span class="sxs-lookup"><span data-stu-id="10378-126">Customer Group</span></span>
- <span data-ttu-id="10378-127">Единица</span><span class="sxs-lookup"><span data-stu-id="10378-127">Unit</span></span>
- <span data-ttu-id="10378-128">Опаковъчна единица</span><span class="sxs-lookup"><span data-stu-id="10378-128">Unit Group</span></span>
- <span data-ttu-id="10378-129">Ценова листа</span><span class="sxs-lookup"><span data-stu-id="10378-129">Price List</span></span>
- <span data-ttu-id="10378-130">Ценова листа на параметър на проекта</span><span class="sxs-lookup"><span data-stu-id="10378-130">Project Parameter Price List</span></span>
- <span data-ttu-id="10378-131">Честота на фактура</span><span class="sxs-lookup"><span data-stu-id="10378-131">Invoice Frequency</span></span>
- <span data-ttu-id="10378-132">Подробни данни за честота на фактура</span><span class="sxs-lookup"><span data-stu-id="10378-132">Invoice Frequency Detail</span></span>
- <span data-ttu-id="10378-133">Категория налични ресурси</span><span class="sxs-lookup"><span data-stu-id="10378-133">Bookable Resource Category</span></span>
- <span data-ttu-id="10378-134">Категория на трансакция</span><span class="sxs-lookup"><span data-stu-id="10378-134">Transaction Category</span></span>
- <span data-ttu-id="10378-135">Категория на разхода</span><span class="sxs-lookup"><span data-stu-id="10378-135">Expense Category</span></span>
- <span data-ttu-id="10378-136">Цена на роля</span><span class="sxs-lookup"><span data-stu-id="10378-136">Role Price</span></span>
- <span data-ttu-id="10378-137">Цена на категория транзакция</span><span class="sxs-lookup"><span data-stu-id="10378-137">Transaction Category Price</span></span>
- <span data-ttu-id="10378-138">Характеристика</span><span class="sxs-lookup"><span data-stu-id="10378-138">Characteristic</span></span>
- <span data-ttu-id="10378-139">Наличен ресурс</span><span class="sxs-lookup"><span data-stu-id="10378-139">Bookable Resource</span></span>
- <span data-ttu-id="10378-140">Асоциация на категория налични ресурси</span><span class="sxs-lookup"><span data-stu-id="10378-140">Bookable resource category Assn</span></span>
- <span data-ttu-id="10378-141">Характеристика на наличен ресурс</span><span class="sxs-lookup"><span data-stu-id="10378-141">Bookable Resource Characteristic</span></span>

![Пълно импортиране](./media/6CompleteImport.png)
