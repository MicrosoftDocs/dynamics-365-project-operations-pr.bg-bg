---
title: Отстраняване на неизправности при работа в мрежата на задачите
description: Тази тема предоставя информация за отстраняване на неизправности, необходима при работа в мрежата на задачите.
author: ruhercul
manager: tfehr
ms.date: 01/19/2021
ms.topic: article
ms.product: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 89bbad62c2a0a5693a57cf5c9a812ab644486469
ms.sourcegitcommit: c9edb4fc3042d97cb1245be627841e0a984dbdea
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/19/2021
ms.locfileid: "5031524"
---
# <a name="troubleshoot-working-in-the-task-grid"></a><span data-ttu-id="9eba1-103">Отстраняване на неизправности при работа в мрежата на задачите</span><span class="sxs-lookup"><span data-stu-id="9eba1-103">Troubleshoot working in the Task grid</span></span> 

<span data-ttu-id="9eba1-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="9eba1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="9eba1-105">Тази тема описва как да коригирате проблеми, които може да срещнете при работа с управление на разходите.</span><span class="sxs-lookup"><span data-stu-id="9eba1-105">This topic describes how to fix issues that you might encounter while working with cost management.</span></span>

## <a name="enable-cookies"></a><span data-ttu-id="9eba1-106">Разрешаване на бисквитки</span><span class="sxs-lookup"><span data-stu-id="9eba1-106">Enable cookies</span></span>

<span data-ttu-id="9eba1-107">Project Operations изисква бисквитките на трети страни да бъдат активирани, за да представят съставна структура на работата.</span><span class="sxs-lookup"><span data-stu-id="9eba1-107">Project Operations requires that third-party cookies be enabled in order to render the work breakdown structure.</span></span> <span data-ttu-id="9eba1-108">Когато бисквитките на трети страни не са активирани, вместо да виждате задачи, ще видите празна страница, когато изберете раздела **Задачи** на страницата **Проект**.</span><span class="sxs-lookup"><span data-stu-id="9eba1-108">When third-party cookies aren't enabled, instead of seeing tasks, you will see a blank page when you select the **Tasks** tab on the **Project** page.</span></span>

![Празен раздел, когато бисквитките на трети страни не са активирани](media/blankschedule.png)


### <a name="workaround"></a><span data-ttu-id="9eba1-110">Заобиколно решение</span><span class="sxs-lookup"><span data-stu-id="9eba1-110">Workaround</span></span>
<span data-ttu-id="9eba1-111">За Microsoft Edge или браузъри Google Chrome, следните процедури очертават как да актуализирате настройката на браузъра си, за да активирате бисквитки на трети страни.</span><span class="sxs-lookup"><span data-stu-id="9eba1-111">For Microsoft Edge or Google Chrome browsers, the following procedures outline how to update your browser setting to enable third-party cookies.</span></span>

#### <a name="microsoft-edge"></a><span data-ttu-id="9eba1-112">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="9eba1-112">Microsoft Edge</span></span>

1. <span data-ttu-id="9eba1-113">Отворете вашия браузър Edge.</span><span class="sxs-lookup"><span data-stu-id="9eba1-113">Open your Edge browser.</span></span>
2. <span data-ttu-id="9eba1-114">В горния десен ъгъл изберете **многоточието** (...) и след това **Настройки**.</span><span class="sxs-lookup"><span data-stu-id="9eba1-114">In the upper-right corner, select the **ellipsis** (...), and then select **Settings**.</span></span>
3. <span data-ttu-id="9eba1-115">Под **Бисквитки“ и разрешения за сайтове** изберете **Бисквитки“ и данни за сайтове**.</span><span class="sxs-lookup"><span data-stu-id="9eba1-115">Under **Cookies and site permissions**, select **Cookies and site data**.</span></span>
4. <span data-ttu-id="9eba1-116">Изключете **Блокирайте бисквитки на трети страни**.</span><span class="sxs-lookup"><span data-stu-id="9eba1-116">Turn off **Block third-party cookies**.</span></span>

#### <a name="google-chrome"></a><span data-ttu-id="9eba1-117">Google Chrome</span><span class="sxs-lookup"><span data-stu-id="9eba1-117">Google Chrome</span></span>

1. <span data-ttu-id="9eba1-118">Отворете вашия браузър Chrome.</span><span class="sxs-lookup"><span data-stu-id="9eba1-118">Open your Chrome browser.</span></span>
2. <span data-ttu-id="9eba1-119">В горния десен ъгъл изберете трите вертикални точки и след това **Настройки**.</span><span class="sxs-lookup"><span data-stu-id="9eba1-119">In the upper-right corner, select the three vertical dots, and then select **Settings**.</span></span>
3. <span data-ttu-id="9eba1-120">Под **Поверителност и защита** изберете **Бисквитки“ и други данни за сайтове**.</span><span class="sxs-lookup"><span data-stu-id="9eba1-120">Under **Privacy and security**, select **Cookies and other site data**.</span></span>
4. <span data-ttu-id="9eba1-121">Изберете **Разрешаване на всички бисквитки**.</span><span class="sxs-lookup"><span data-stu-id="9eba1-121">Select **Allow all cookies**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9eba1-122">Ако блокирате бисквитки на трети страни, всички бисквитки и данни за сайтове от други сайтове ще бъдат блокирани, дори ако сайтът е разрешен във вашия списък с изключения.</span><span class="sxs-lookup"><span data-stu-id="9eba1-122">If you block third-party cookies, all cookies and site data from other sites will be blocked, even if the site is allowed on your exceptions list.</span></span>

## <a name="pex-endpoint"></a><span data-ttu-id="9eba1-123">Крайна точка на PEX</span><span class="sxs-lookup"><span data-stu-id="9eba1-123">PEX Endpoint</span></span>

<span data-ttu-id="9eba1-124">Project Operations изисква проектният параметър да се позовава на крайната точка PEX.</span><span class="sxs-lookup"><span data-stu-id="9eba1-124">Project Operations requires that a project parameter reference the PEX Endpoint.</span></span> <span data-ttu-id="9eba1-125">Тази крайна точка е необходима за комуникация с услугата, използвана за визуализиране на структурата на разбивка на работата.</span><span class="sxs-lookup"><span data-stu-id="9eba1-125">This endpoint is required to communicate with the service used to render the work breakdown structure.</span></span> <span data-ttu-id="9eba1-126">Ако параметърът не е активиран, ще получите грешката „Параметърът на проекта не е валиден“.</span><span class="sxs-lookup"><span data-stu-id="9eba1-126">If the parameter isn't enabled, you will receive the error, "The project parameter is not valid".</span></span> 

### <a name="workaround"></a><span data-ttu-id="9eba1-127">Заобиколно решение</span><span class="sxs-lookup"><span data-stu-id="9eba1-127">Workaround</span></span>
 ![Поле PEX Endpoint на параметъра на проекта](media/projectparameter.png)

1. <span data-ttu-id="9eba1-129">Добавете полето **Крайна точка на PEX** към страницата **Параметри на проекта**.</span><span class="sxs-lookup"><span data-stu-id="9eba1-129">Add the **PEX Endpoint** field to the **Project Parameters** page.</span></span>
2. <span data-ttu-id="9eba1-130">Актуализирайте полето със следната стойност: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=\<id>&type=2`</span><span class="sxs-lookup"><span data-stu-id="9eba1-130">Update the field with the following value: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=\<id>&type=2`</span></span>
3. <span data-ttu-id="9eba1-131">Премахнете полето от страницата **Параметри на проекта**.</span><span class="sxs-lookup"><span data-stu-id="9eba1-131">Remove the field from the **Project Parameters** page.</span></span>

## <a name="privileges-for-project-for-the-web"></a><span data-ttu-id="9eba1-132">Привилегии за Проект за мрежата</span><span class="sxs-lookup"><span data-stu-id="9eba1-132">Privileges for Project for the Web</span></span>

<span data-ttu-id="9eba1-133">Project Operations разчита на външна услуга за планиране.</span><span class="sxs-lookup"><span data-stu-id="9eba1-133">Project Operations relies on an external scheduling service.</span></span> <span data-ttu-id="9eba1-134">Услугата изисква на потребителя да бъдат зададени няколко роли за четене и запис на обекти, свързани със структурата на разбивка на работата.</span><span class="sxs-lookup"><span data-stu-id="9eba1-134">The service requires that a user have several roles assigned to read and write to entities related to the work breakdown structure.</span></span> <span data-ttu-id="9eba1-135">Тези обекти включват проектни задачи, назначения на ресурси и зависимости на задачите.</span><span class="sxs-lookup"><span data-stu-id="9eba1-135">These entities include project tasks, resource assignments, and task dependencies.</span></span> <span data-ttu-id="9eba1-136">Ако потребителят не може да изобрази структурата на разбивка на работата, когато отиде в раздела **Задачи**, вероятно защото Проект за Project Operations не е активиран.</span><span class="sxs-lookup"><span data-stu-id="9eba1-136">If a user can't render the work breakdown structure when they go to the **Tasks** tab, it's probably because Project for Project Operations hasn't been enabled.</span></span> <span data-ttu-id="9eba1-137">Потребителят може да получи грешка права за достъп или грешка, свързана с отказ на достъп.</span><span class="sxs-lookup"><span data-stu-id="9eba1-137">A user might receive either a security role error, or an error related to a denial of access.</span></span>


## <a name="workaround"></a><span data-ttu-id="9eba1-138">Заобиколно решение</span><span class="sxs-lookup"><span data-stu-id="9eba1-138">Workaround</span></span>

1. <span data-ttu-id="9eba1-139">Отидете на **Настройки > Защита > Потребители > Потребители на приложение**.</span><span class="sxs-lookup"><span data-stu-id="9eba1-139">Go to **Setting > Security > Users > Application Users**.</span></span>  

   ![Четец на приложение](media/applicationuser.jpg)
   
2. <span data-ttu-id="9eba1-141">Щракнете двукратно върху потребителския запис на приложението, за да проверите следното:</span><span class="sxs-lookup"><span data-stu-id="9eba1-141">Double-click the application user record to verify the following:</span></span>

 - <span data-ttu-id="9eba1-142">Потребителят има достъп до проекта.</span><span class="sxs-lookup"><span data-stu-id="9eba1-142">The user has access to the project.</span></span> <span data-ttu-id="9eba1-143">Тази проверка обикновено се извършва, като се гарантира, че потребителят има роля на защита **Ръководител проект**.</span><span class="sxs-lookup"><span data-stu-id="9eba1-143">This verification is typically done by ensuring that the user has **Project Manager** security role.</span></span>
 - <span data-ttu-id="9eba1-144">Потребителят на приложението Microsoft Project съществува и е конфигуриран правилно.</span><span class="sxs-lookup"><span data-stu-id="9eba1-144">The Microsoft Project application user exists and is configured correctly.</span></span>
 
3. <span data-ttu-id="9eba1-145">Ако този потребител не съществува, можете да създадете нов запис на потребител.</span><span class="sxs-lookup"><span data-stu-id="9eba1-145">If this user doesn't exist, you can create a new user record.</span></span> <span data-ttu-id="9eba1-146">Изберете **Нови потребители**.</span><span class="sxs-lookup"><span data-stu-id="9eba1-146">Select **New Users**.</span></span> <span data-ttu-id="9eba1-147">Променете формуляра на записа на **Потребител на приложението** и след това добавете **ИД на приложението**.</span><span class="sxs-lookup"><span data-stu-id="9eba1-147">Change the entry form to **Application User**, and then add the **Application ID**.</span></span>

   ![Подробности за потребител на приложението](media/applicationuserdetails.jpg)

4. <span data-ttu-id="9eba1-149">Проверете дали потребителят е получил правилния лиценз и дали услугата е активирана в подробностите за лицензионните планове за услуги.</span><span class="sxs-lookup"><span data-stu-id="9eba1-149">Verify that the user has been assigned the correct license and that the service is enabled in the service plans details of the license.</span></span>
5. <span data-ttu-id="9eba1-150">Проверете дали потребителят може да отвори project.microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="9eba1-150">Verify that the user can open project.microsoft.com.</span></span>
6. <span data-ttu-id="9eba1-151">Проверете чрез параметрите на проекта, че системата сочи към правилната крайна точка на проекта.</span><span class="sxs-lookup"><span data-stu-id="9eba1-151">Verify through the project parameters that the system is pointing to the correct project endpoint.</span></span>
7. <span data-ttu-id="9eba1-152">Проверете дали потребителят на проектното приложение е създаден.</span><span class="sxs-lookup"><span data-stu-id="9eba1-152">Verify that the project application user is created.</span></span>
8. <span data-ttu-id="9eba1-153">Приложете следните роли на защита към потребителя:</span><span class="sxs-lookup"><span data-stu-id="9eba1-153">Apply the following security roles to the user:</span></span>

  - <span data-ttu-id="9eba1-154">Потребител на Dataverse</span><span class="sxs-lookup"><span data-stu-id="9eba1-154">Dataverse User</span></span>
  - <span data-ttu-id="9eba1-155">Система на Project Operations</span><span class="sxs-lookup"><span data-stu-id="9eba1-155">Project Operations System</span></span>
  - <span data-ttu-id="9eba1-156">Система на проекта</span><span class="sxs-lookup"><span data-stu-id="9eba1-156">Project System</span></span>

## <a name="error-when-updating-the-work-breakdown-structure"></a><span data-ttu-id="9eba1-157">Грешка при актуализиране на съставна структура на работата</span><span class="sxs-lookup"><span data-stu-id="9eba1-157">Error when updating the work breakdown structure</span></span>

<span data-ttu-id="9eba1-158">Когато се направят една или повече актуализации на съставна структура на работата, промените в крайна сметка се провалят и не се записват.</span><span class="sxs-lookup"><span data-stu-id="9eba1-158">When one or more updates are made to the work breakdown structure, the changes eventually fail and aren't saved.</span></span> <span data-ttu-id="9eba1-159">Възниква грешка в мрежата на графика, отбелязвайки, че „Скорошната промяна, която сте направили, не може да бъде запазена“.</span><span class="sxs-lookup"><span data-stu-id="9eba1-159">An error occurs in the schedule grid noting that “Recent change you’ve made couldn’t be saved.”</span></span>

### <a name="workaround"></a><span data-ttu-id="9eba1-160">Заобиколно решение</span><span class="sxs-lookup"><span data-stu-id="9eba1-160">Workaround</span></span>

1. <span data-ttu-id="9eba1-161">Проверете дали потребителят е получил правилния лиценз и дали услугата е активирана в подробностите за лицензионните планове за услуги.</span><span class="sxs-lookup"><span data-stu-id="9eba1-161">Verify that the user has been assigned the correct license and that the service is enabled in the service plans details of the license.</span></span>
2. <span data-ttu-id="9eba1-162">Проверете дали потребителят може да отвори project.microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="9eba1-162">Verify that the user can open project.microsoft.com.</span></span>
3. <span data-ttu-id="9eba1-163">Проверете дали системата сочи към правилната крайна точка на проекта.</span><span class="sxs-lookup"><span data-stu-id="9eba1-163">Verify that the system is pointing to the correct project endpoint,.</span></span>
4. <span data-ttu-id="9eba1-164">Проверете дали потребителят на проектното приложение е създаден.</span><span class="sxs-lookup"><span data-stu-id="9eba1-164">Verify that the Project Application user has been created.</span></span>
5. <span data-ttu-id="9eba1-165">Приложете следните роли на защита към потребителя:</span><span class="sxs-lookup"><span data-stu-id="9eba1-165">Apply the following security roles to the user:</span></span>
  
  - <span data-ttu-id="9eba1-166">Потребител на Dataverse или базов потребител</span><span class="sxs-lookup"><span data-stu-id="9eba1-166">Dataverse user or Base user</span></span>
  - <span data-ttu-id="9eba1-167">Система на Project Operations</span><span class="sxs-lookup"><span data-stu-id="9eba1-167">Project Operations System</span></span>
  - <span data-ttu-id="9eba1-168">Система на проекта</span><span class="sxs-lookup"><span data-stu-id="9eba1-168">Project System</span></span>
  - <span data-ttu-id="9eba1-169">Система за двойно записване на Project Operations (Тази роля се изисква, ако внедрявате базиран на ресурси / нескладиран сценарий на Project Operations.)</span><span class="sxs-lookup"><span data-stu-id="9eba1-169">Project Operations Dual Write System (This role is required if you are deploying the resource/non-stocked based scenario of Project Operations.)</span></span>
