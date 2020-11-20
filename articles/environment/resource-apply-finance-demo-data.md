---
title: Прилагане на демонстрационни данни към среда, хоствана в облак на Finance
description: Тази тема обяснява как да приложите демо данни от Project Operations към среда, хоствана в облак на Dynamics 365 Finance.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a7cdbd2847ce45972aadd0d1a2d4f26270727ad9
ms.sourcegitcommit: d33ef0ae39f90fe3b0f6b4524f483e8052057361
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/03/2020
ms.locfileid: "4365225"
---
# <a name="apply-demo-data-to-a-finance-cloud-hosted-environment"></a><span data-ttu-id="22c94-103">Прилагане на демонстрационни данни към среда, хоствана в облак на Finance</span><span class="sxs-lookup"><span data-stu-id="22c94-103">Apply demo data to a Finance Cloud-hosted environment</span></span>

<span data-ttu-id="22c94-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="22c94-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="22c94-105">Тази тема е приложима само за Microsoft Dynamics 365 Finance, версия 10.0.13 и може да се изпълнява само в среда, хоствана в облак.</span><span class="sxs-lookup"><span data-stu-id="22c94-105">This topic is only applicable only Microsoft Dynamics 365 Finance version 10.0.13 and can be performed only on a Cloud-hosted environment.</span></span> <span data-ttu-id="22c94-106">Изпълнете стъпките в тази тема **ПРЕДИ** да прилагате качествени актуализации за околната среда.</span><span class="sxs-lookup"><span data-stu-id="22c94-106">Complete the steps in this topic **BEFORE** you apply quality updates to the environment.</span></span>

1. <span data-ttu-id="22c94-107">Във вашия LCS проект отворете страницата **Подробности за среда**.</span><span class="sxs-lookup"><span data-stu-id="22c94-107">In your LCS project, open the **Environment details** page.</span></span> <span data-ttu-id="22c94-108">Забележете, че включва подробности, необходими за свързване с околната среда чрез протокол за отдалечен работен плот (RDP).</span><span class="sxs-lookup"><span data-stu-id="22c94-108">Notice that it includes the details needed to connect to the environment by using Remote Desktop Protocol (RDP).</span></span>

![Подробности за среди на ](./media/1EnvironmentDetails.png)

<span data-ttu-id="22c94-110">Първият набор от подчертани идентификационни данни са идентификационните данни на локалния акаунт и съдържат хипервръзка към връзката с отдалечен работен плот.</span><span class="sxs-lookup"><span data-stu-id="22c94-110">The first set of highlighted credentials are the local account credentials and contain a hyperlink to the remote desktop connection.</span></span> <span data-ttu-id="22c94-111">Идентификационните данни включват потребителско име и парола за администратор на околната среда.</span><span class="sxs-lookup"><span data-stu-id="22c94-111">The credentials include the environment admin username and password.</span></span> <span data-ttu-id="22c94-112">Вторият набор от идентификационни данни се използва за влизане в SQL Server в тази среда.</span><span class="sxs-lookup"><span data-stu-id="22c94-112">The second set of credentials are used to log in to SQL Server in this environment.</span></span>

2. <span data-ttu-id="22c94-113">Свържете се с околната среда чрез хипервръзката в **Локални акаунти** и използвайте **Идентификационни данни на локален акаунт** за удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="22c94-113">Remote to the environment by the hyperlink in **Local Accounts**, and use the **Local Account credentials** to authenticate.</span></span>
3. <span data-ttu-id="22c94-114">Отидете на **Интернет информационни услуги** > **Анкети за приложения** > **AOSService** и спрете услугата.</span><span class="sxs-lookup"><span data-stu-id="22c94-114">Go to **Internet Information Services** > **Application Pools** > **AOSService** and stop the service.</span></span> <span data-ttu-id="22c94-115">В този момент спирате услугата, за да можете да продължите да подменяте SQL базата данни.</span><span class="sxs-lookup"><span data-stu-id="22c94-115">You are stopping the service at this point so that you can continue to replace the SQL database.</span></span>

![Спиране на AOS](./media/2StopAOS.png)

4. <span data-ttu-id="22c94-117">Отидете на **Услуги** и спрете следните два елемента:</span><span class="sxs-lookup"><span data-stu-id="22c94-117">Go to **Services** and stop the following two items:</span></span>

- <span data-ttu-id="22c94-118">Microsoft Dynamics 365 Unified Operations: Служба за управление на партиди</span><span class="sxs-lookup"><span data-stu-id="22c94-118">Microsoft Dynamics 365 Unified Operations: Batch Management Service</span></span>
- <span data-ttu-id="22c94-119">Microsoft Dynamics 365 Unified Operations: Рамка за експортиране и импортиране на данни</span><span class="sxs-lookup"><span data-stu-id="22c94-119">Microsoft Dynamics 365 Unified Operations: Data Import Export Framework</span></span>

![Спиране на услуги](./media/3StopServices.png)

5. <span data-ttu-id="22c94-121">Отворете студиото за управление на Microsoft SQL Server.</span><span class="sxs-lookup"><span data-stu-id="22c94-121">Open Microsoft SQL Server Management Studio.</span></span> <span data-ttu-id="22c94-122">Влезте с идентификационни данни на SQL сървър и използвайте потребителя и паролата на axdbadmin от страницата LCS **Подробности за средите**.</span><span class="sxs-lookup"><span data-stu-id="22c94-122">Log in with SQL server credentials and use the axdbadmin user and password from the LCS **Environments details** page.</span></span>

![SQL Server Management Studio](./media/4SSMS.png)

6. <span data-ttu-id="22c94-124">В Object Explorer **Бази данни** и намерете **AXDB**.</span><span class="sxs-lookup"><span data-stu-id="22c94-124">In Object Explorer, **Databases** and locate **AXDB**.</span></span> <span data-ttu-id="22c94-125">Ще замените базата данни с нова база данни, която се намира в [Център за изтегляне](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span><span class="sxs-lookup"><span data-stu-id="22c94-125">You will replace database with a new database that is located in the [Download Center](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span></span> 
7. <span data-ttu-id="22c94-126">Копирайте zip файла във виртуалната машина, в която сте отдалечени, и извлечете zip съдържанието.</span><span class="sxs-lookup"><span data-stu-id="22c94-126">Copy the zip file to the VM you are remoted into and extract zip contents.</span></span>
8. <span data-ttu-id="22c94-127">В SQL Server Management Studio щракнете с десния бутон върху **AxDB** и след това изберете **Задачи** > **Възстанови** > **База данни**.</span><span class="sxs-lookup"><span data-stu-id="22c94-127">In SQL Server Management Studio, right-click **AxDB**, and then select **Tasks** > **Restore** > **Database**.</span></span>

![Възстановяване на база данни](./media/5RestoreDatabase.png)

9. <span data-ttu-id="22c94-129">Изберете **Изходно устройство** и отидете до файла, извлечен от zip, който сте копирали.</span><span class="sxs-lookup"><span data-stu-id="22c94-129">Select **Source Device** and navigate to the file extracted from zip you copied.</span></span>

![Изходни устройства](./media/6SourceDevice.png)

10. <span data-ttu-id="22c94-131">Изберете **Опции** и след това изберете **Презапишете съществуващата база данни** и **Затворете съществуващите връзки към целевата база данни**.</span><span class="sxs-lookup"><span data-stu-id="22c94-131">Select **Options**, and then select **Overwrite the existing database** and **Close existing connections to destination database**.</span></span> 
11. <span data-ttu-id="22c94-132">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="22c94-132">Select **OK**.</span></span>

![Възстановяване на настройки](./media/7RestoreSetting.png)

<span data-ttu-id="22c94-134">Ще получите потвърждение, че възстановяването на AXDB е успешно.</span><span class="sxs-lookup"><span data-stu-id="22c94-134">You will receive confirmation that the AXDB restore was successful.</span></span> <span data-ttu-id="22c94-135">След като получите това потвърждение, можете да затворите SQL Services Management Studio.</span><span class="sxs-lookup"><span data-stu-id="22c94-135">After you receive this confirmation, you can close SQL Services Management Studio.</span></span>

12. <span data-ttu-id="22c94-136">Отидете обратно на **Интернет информационни услуги** > **Анкети за приложения** > **AOSService** и стартирайте AOSService.</span><span class="sxs-lookup"><span data-stu-id="22c94-136">Go back to **Internet Information Services** > **Application Pools** > **AOSService** and start the AOSService.</span></span>
13. <span data-ttu-id="22c94-137">Отидете на **Услуги** и стартирайте двете услуги, които сте спрели по-рано.</span><span class="sxs-lookup"><span data-stu-id="22c94-137">Go to **Services** and start the two services you stopped earlier.</span></span>

14. <span data-ttu-id="22c94-138">Намерете инструмента AdminUserProvisioning на тази VM.</span><span class="sxs-lookup"><span data-stu-id="22c94-138">Locate the AdminUserProvisioning tool on this VM.</span></span> <span data-ttu-id="22c94-139">Погледнете под K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span><span class="sxs-lookup"><span data-stu-id="22c94-139">Look under, K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span></span>
15. <span data-ttu-id="22c94-140">Стартирайте .ext файла, като използвате вашия потребителски адрес в полето **Имейл адрес**.</span><span class="sxs-lookup"><span data-stu-id="22c94-140">Run the .ext file using your user address in the **Email Address** field.</span></span> 
16. <span data-ttu-id="22c94-141">Изберете **Подаване**.</span><span class="sxs-lookup"><span data-stu-id="22c94-141">Select **Submit**.</span></span>

![Осигуряване на потребител администратор](./media/8AdminUserProvisioning.png)

<span data-ttu-id="22c94-143">Това отнема няколко минути.</span><span class="sxs-lookup"><span data-stu-id="22c94-143">This takes a couple of minutes to complete.</span></span> <span data-ttu-id="22c94-144">Трябва да получите съобщение за потвърждение, че потребителят на администратор е успешно актуализиран.</span><span class="sxs-lookup"><span data-stu-id="22c94-144">You should receive a confirmation message that the Admin user was successfully updated.</span></span>

17. <span data-ttu-id="22c94-145">И накрая, стартирайте командния ред като администратор и изпълнете iisreset</span><span class="sxs-lookup"><span data-stu-id="22c94-145">Lastly, run Command Prompt as Administrator and perform iisreset</span></span>

![Нулиране на IIS](./media/9IISReset.png)

18. <span data-ttu-id="22c94-147">Затворете сесията на отдалечения работен плот и използвайте средата LCS **Подробности за среда**, за да влезете в средата, за да потвърдите, че работи както се очаква.</span><span class="sxs-lookup"><span data-stu-id="22c94-147">Close the remote desktop session and use the LCS **Environment details** page to log in to the environment to confirm it is working as expected.</span></span>

![Finance and Operations](./media/10FinanceAndOperations.png)
