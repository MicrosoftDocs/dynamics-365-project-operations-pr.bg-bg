---
title: Интеграция на Microsoft Project Client
description: Планирането и поддържането на график на проекта може да бъде сложно, така че ръководителите на проекти трябва да използват инструменти, които да им помогнат да управляват тази задача. Интеграцията с Microsoft Project Client осигурява поддръжка за отваряне и управление на структурна разбивка на работата на проекта.
author: Yowelle
ms.date: 06/16/2021
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjWbsTemplate
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-04
ms.dyn365.ops.version: 7.2999999999999998
ms.openlocfilehash: b312ec5b1f4e6a98a2cbf1667b2f55b758b2d613
ms.sourcegitcommit: 3a4b181be08ef0428104d72b54a3e61ac2782f14
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/17/2021
ms.locfileid: "6269822"
---
# <a name="microsoft-project-client-integration"></a><span data-ttu-id="65373-104">Интеграция на Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="65373-104">Microsoft Project client integration</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="65373-105">Планирането и поддържането на график на проекта може да бъде сложно, така че ръководителите на проекти трябва да използват инструменти, които да им помогнат да управляват тази задача.</span><span class="sxs-lookup"><span data-stu-id="65373-105">Planning and maintaining a project schedule can be complex, so project managers need to use tools that help them manage this task.</span></span> <span data-ttu-id="65373-106">Интеграцията с Microsoft Project Client осигурява поддръжка за отваряне и управление на структурна разбивка на работата на проекта.</span><span class="sxs-lookup"><span data-stu-id="65373-106">Integration with Microsoft Project Client provides support to open and manage a project work breakdown structure.</span></span> <span data-ttu-id="65373-107">Ръководителят на проекта може да публикува всички промени обратно в Dynamics 365 Finance съставна структура на работата по проекта.</span><span class="sxs-lookup"><span data-stu-id="65373-107">The project manager can publish any changes back to the Dynamics 365 Finance project work breakdown structure.</span></span>

> [!NOTE]
> <span data-ttu-id="65373-108">Ако използвате юлската актуализация (версия 10.0.4), трябва да инсталирате KB 4054797 и 4055884.</span><span class="sxs-lookup"><span data-stu-id="65373-108">If you are using the July update (version 10.0.4), you must install KB 4054797 and 4055884.</span></span>

## <a name="configure-the-microsoft-project-client-add-in"></a><span data-ttu-id="65373-109">Конфигурирайте добавката Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="65373-109">Configure the Microsoft Project Client add-in</span></span>
<span data-ttu-id="65373-110">За да активирате интеграцията с Microsoft Project Client, се изисква добавка Microsoft Dynamics 365 да бъде инсталирана в приложението на потребителя Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="65373-110">To enable the integration with Microsoft Project Client, a Microsoft Dynamics 365 add-in is required to be installed in the user’s client Microsoft Project application.</span></span> <span data-ttu-id="65373-111">Това става чрез отваряне на **Работно пространство за управление на проекти**.</span><span class="sxs-lookup"><span data-stu-id="65373-111">This is done by opening the **Project management workspace**.</span></span>

<span data-ttu-id="65373-112">• Щракнете **Конфигурирайте клиентска добавка за проект** от **Връзки** > раздел **Настройка** на работното пространство.</span><span class="sxs-lookup"><span data-stu-id="65373-112">•   Click **Configure project client add-in** from the **Links** > **Setup** section of the workspace.</span></span>

<span data-ttu-id="65373-113">• Щракнете **Отворете**, след това щракнете **Изпълнение**, когато бъдете подканени.</span><span class="sxs-lookup"><span data-stu-id="65373-113">•   Click **Open**, then click **Run** when prompted.</span></span>

## <a name="open-and-edit-an-existing-draft-work-breakdown-structure-in-microsoft-project-client"></a><span data-ttu-id="65373-114">Отворете и редактирайте съществуваща структура на разбивка на чернови в Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="65373-114">Open and edit an existing draft work breakdown structure in Microsoft Project Client</span></span>
<span data-ttu-id="65373-115">Ако проект в Dynamics 365 Finance вече има създадена структура на разбивка на работата, структурата на разбивка на работата може да бъде отворена в приложението Microsoft Project Client, ако структурата на разбивка на работата е в състояние на чернови.</span><span class="sxs-lookup"><span data-stu-id="65373-115">If a project in Dynamics 365 Finance already has a work breakdown structure created, the work breakdown structure can be opened in the Microsoft Project Client application if the work breakdown structure is in a draft status.</span></span> <span data-ttu-id="65373-116">За да отворите от страницата **Проект** щракнете върху връзката **Отворете в Microsoft Project** от раздела **План**. Тази страница може да се отвори и от приложението Microsoft Project Client, като щракнете върху **Отворете** в раздела **Microsoft Dynamics 365**. Изберете **Юридическо лице** и **Проект** от списъка.</span><span class="sxs-lookup"><span data-stu-id="65373-116">To open from the **Project** page, click **Open in Microsoft Project** link from the **Plan** tab. This page can also be opened from within the Microsoft Project Client application by clicking **Open** in the **Microsoft Dynamics 365** tab. Select the **Legal entity** and **Project** from the list.</span></span>

> [!NOTE]
> <span data-ttu-id="65373-117">Ако използвате Internet Explorer като браузър, ще трябва да щракнете **Записване** за ръчно отваряне от мястото, на което се изтегля файлът.</span><span class="sxs-lookup"><span data-stu-id="65373-117">If you're using Internet Explorer as your browser, you will need to click **Save** to manually open from the location that the file is downloaded to.</span></span> <span data-ttu-id="65373-118">Или щракнете **Запазете и отворете**, за да отворите файла в Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="65373-118">Or, click **Save and open** to open the file in Microsoft Project Client.</span></span> <span data-ttu-id="65373-119">Не преименувайте името на файла, когато записвате.</span><span class="sxs-lookup"><span data-stu-id="65373-119">Do not rename the file name when saving.</span></span>

<span data-ttu-id="65373-120">Преди да редактирате файла с помощта на Microsoft Project Client, трябва да го проверите. Щракнете върху **Разгледайте** в раздела **Microsoft Dynamics 365**. Това ще попречи на други потребители да редактират структурата на разбивка на работата от Finance едновременно.</span><span class="sxs-lookup"><span data-stu-id="65373-120">Before making any edits to the file using Microsoft Project Client, you need to check it out. Click **Check out** in the **Microsoft Dynamics 365** tab. This will prevent other users from editing the work breakdown structure from within Finance at the same time.</span></span> <span data-ttu-id="65373-121">За да публикувате структурата на разбивка на работата след завършване на редакции, щракнете върху **Вкарване** на **Microsoft Dynamics 365** раздел.</span><span class="sxs-lookup"><span data-stu-id="65373-121">To publish the work breakdown structure after completing any edits, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

<span data-ttu-id="65373-122">Ако екип по проект вече е добавен към проекта във Finance, списъкът с ресурси ще се попълни с членовете на екипа.</span><span class="sxs-lookup"><span data-stu-id="65373-122">If a project team has already been added to the project in Finance, the resource list will be populated with the team members.</span></span> <span data-ttu-id="65373-123">Ако екипът на проекта все още не е добавен към проекта, можете да изберете ресурси и да изградите екипа в рамките на Microsoft Project Client, като щракнете върху бутона **Ресурси** на раздела **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="65373-123">If a project team has not yet been added to the project, you can select resources and build the team within Microsoft Project Client by clicking the **Resources** button on the **Microsoft Dynamics 365** tab.</span></span> 

<span data-ttu-id="65373-124">Следните данни ще бъдат синхронизирани обратно във Finance като част от процеса на чекиране:</span><span class="sxs-lookup"><span data-stu-id="65373-124">The following data will be synced back to Finance as part of the check-in process:</span></span>

<span data-ttu-id="65373-125">•   Име на задача</span><span class="sxs-lookup"><span data-stu-id="65373-125">•   Task name</span></span>

<span data-ttu-id="65373-126">•   Начална дата</span><span class="sxs-lookup"><span data-stu-id="65373-126">•   Start date</span></span>

<span data-ttu-id="65373-127">•   Дата на приключване</span><span class="sxs-lookup"><span data-stu-id="65373-127">•   Finish date</span></span>

<span data-ttu-id="65373-128">•   Предшественици</span><span class="sxs-lookup"><span data-stu-id="65373-128">•   Predecessors</span></span>

<span data-ttu-id="65373-129">•   Имена на ресурси</span><span class="sxs-lookup"><span data-stu-id="65373-129">•   Resource names</span></span>

<span data-ttu-id="65373-130">•   Категория</span><span class="sxs-lookup"><span data-stu-id="65373-130">•   Category</span></span>

<span data-ttu-id="65373-131">•   Категория ресурси</span><span class="sxs-lookup"><span data-stu-id="65373-131">•   Resource category</span></span>

<span data-ttu-id="65373-132">•   Работно време</span><span class="sxs-lookup"><span data-stu-id="65373-132">•   Work hours</span></span>

<span data-ttu-id="65373-133">•   Бележки</span><span class="sxs-lookup"><span data-stu-id="65373-133">•   Notes</span></span>

<span data-ttu-id="65373-134">•   Приоритет</span><span class="sxs-lookup"><span data-stu-id="65373-134">•   Priority</span></span>

> [!NOTE]
> <span data-ttu-id="65373-135">Ако добавите други колони към вашия файл на Microsoft Project Client, те няма да бъдат записани във файла и няма да бъдат показани, когато файлът бъде отворен отново.</span><span class="sxs-lookup"><span data-stu-id="65373-135">If you add any other columns to your Microsoft Project Client file, they will not be saved to the file and will not be displayed when the file is opened again.</span></span>

## <a name="create-the-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="65373-136">Създайте структура на разбивка на работата за съществуващ проект с помощта на Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="65373-136">Create the work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="65373-137">Зад а създадете нова съставна структура на работата с помощта на Microsoft Project Client, следвайте тези стъпки:</span><span class="sxs-lookup"><span data-stu-id="65373-137">To create a new work breakdown structure using Microsoft Project Client, follow these steps:</span></span>


1.  <span data-ttu-id="65373-138">Отворете на Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="65373-138">Open Microsoft Project Client.</span></span>

2.  <span data-ttu-id="65373-139">В раздела **Microsoft Dynamics 365** щракнете върху **Отваряне**.</span><span class="sxs-lookup"><span data-stu-id="65373-139">On the **Microsoft Dynamics 365** tab, click **Open**.</span></span>

3.  <span data-ttu-id="65373-140">Изберете **Юридически обект** за проекта.</span><span class="sxs-lookup"><span data-stu-id="65373-140">Select the **Legal entity** for the project.</span></span>

4.  <span data-ttu-id="65373-141">Изберете **проекта**.</span><span class="sxs-lookup"><span data-stu-id="65373-141">Select the **Project**.</span></span>

5.  <span data-ttu-id="65373-142">Щракнете върху **Извличане** на раздела **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="65373-142">Click **Check out** on the **Microsoft Dynamics 365** tab.</span></span>

6.  <span data-ttu-id="65373-143">Когато сте готови да публикувате във Finance, щракнете **Вкарване** на раздела **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="65373-143">When ready to publish to Finance, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

## <a name="replace-the-existing-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="65373-144">Заменете съществуващата съставна структура на работата за съществуващ проект с помощта на Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="65373-144">Replace the existing work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="65373-145">За да създадете нова съставна структура на работата с помощта на Microsoft Project Client и да замените съществуваща съставна структура на работата за съществуващ проект, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="65373-145">To create a new work breakdown structure using Microsoft Project Client and replace an existing work breakdown structure for an existing project, follow these steps:</span></span>

1.  <span data-ttu-id="65373-146">Отворете Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="65373-146">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="65373-147">Създайте график в Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="65373-147">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="65373-148">В раздела **Microsoft Dynamics 365** щракнете върху **Запазите промените** > **Заменете съществуващия проект**.</span><span class="sxs-lookup"><span data-stu-id="65373-148">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Replace existing project**.</span></span>

4.  <span data-ttu-id="65373-149">Изберете **Юридически обект** за проекта.</span><span class="sxs-lookup"><span data-stu-id="65373-149">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="65373-150">Изберете **проекта**.</span><span class="sxs-lookup"><span data-stu-id="65373-150">Select the **Project**.</span></span>

6.  <span data-ttu-id="65373-151">Щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="65373-151">Click **OK**.</span></span>

## <a name="create-a-new-project-from-within-microsoft-project-client"></a><span data-ttu-id="65373-152">Създайте нов проект от Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="65373-152">Create a new project from within Microsoft Project Client</span></span>


1.  <span data-ttu-id="65373-153">Отворете Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="65373-153">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="65373-154">Създайте график в Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="65373-154">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="65373-155">В раздела **Microsoft Dynamics 365** щракнете върху **Запазите промените** > **Записване в нов проект**.</span><span class="sxs-lookup"><span data-stu-id="65373-155">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Save to new Project**.</span></span>

4.  <span data-ttu-id="65373-156">Изберете **Юридически обект** за проекта.</span><span class="sxs-lookup"><span data-stu-id="65373-156">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="65373-157">Въведете **ИД на проекта**, ако е необходимо.</span><span class="sxs-lookup"><span data-stu-id="65373-157">Enter the **Project ID**, if necessary.</span></span>

6.  <span data-ttu-id="65373-158">Въведете **Име на проекта**.</span><span class="sxs-lookup"><span data-stu-id="65373-158">Enter the **Project name**.</span></span>

7.  <span data-ttu-id="65373-159">Изберете **Тип на проекта**, **Проектна група** и **ИД на договор за проект**.</span><span class="sxs-lookup"><span data-stu-id="65373-159">Select the **Project type**, **Project group** and the **Project contract ID**.</span></span> <span data-ttu-id="65373-160">Като алтернатива можете да създадете нов договор за проект, като щракнете върху **Създаване**.</span><span class="sxs-lookup"><span data-stu-id="65373-160">Alternatively, you can create a new project contract by clicking **New**.</span></span>

8.  <span data-ttu-id="65373-161">Изберете **Календар**, който да се използва за ресурси.</span><span class="sxs-lookup"><span data-stu-id="65373-161">Select the **Calendar** to be used for resourcing.</span></span>

11. <span data-ttu-id="65373-162">Щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="65373-162">Click **OK**.</span></span>

> [!NOTE]
> <span data-ttu-id="65373-163">Добавката за клиент на проект не поддържа следните знаци във формата на ИД на проекта:</span><span class="sxs-lookup"><span data-stu-id="65373-163">The Project Client add-in doesn’t support the following characters in the project ID format:</span></span>
> 
>   - <span data-ttu-id="65373-164">Долна черта</span><span class="sxs-lookup"><span data-stu-id="65373-164">Underscore</span></span>
>   - <span data-ttu-id="65373-165">Точка</span><span class="sxs-lookup"><span data-stu-id="65373-165">Period</span></span>
>   - <span data-ttu-id="65373-166">Интервал</span><span class="sxs-lookup"><span data-stu-id="65373-166">Space</span></span>
>   - <span data-ttu-id="65373-167">Наклонена черта</span><span class="sxs-lookup"><span data-stu-id="65373-167">Slash</span></span>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
