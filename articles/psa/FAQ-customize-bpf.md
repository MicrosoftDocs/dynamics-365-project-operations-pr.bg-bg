---
title: Как да персонализирам потока на бизнес процес „Етапи на проект”?
description: Общ преглед на това как да персонализирате потока на бизнес процес „Етапи на проект”.
ms.custom:
- dyn365-projectservice
ms.date: 10/11/2018
ms.topic: article
author: JohnPBurrows
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 2e6c60fe67aea908013077bde40c2faeabc2f39e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993133"
---
# <a name="how-do-i-customize-the-project-stages-business-process-flow"></a><span data-ttu-id="dbe02-103">Как да персонализирам потока на бизнес процес „Етапи на проект”?</span><span class="sxs-lookup"><span data-stu-id="dbe02-103">How do I customize the Project Stages business process flow?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-2-4x-9-0-platform](../includes/cc-applies-to-psa-app-2-4x-9-0-platform.md)]
[!INCLUDE[cc-applies-to-psa-app-1x-8-2-platform](../includes/cc-applies-to-psa-app-1x-8-2-platform.md)]

<span data-ttu-id="dbe02-104">Има известно ограничение в по-ранни версии на приложението Project Service, което изисква имената на етапите на потока на бизнес процес „Етапи на проект” трябва да съвпадат точно с очакваните английски имена (**Quote**, **Plan**, **Close**).</span><span class="sxs-lookup"><span data-stu-id="dbe02-104">There's a known limitation in earlier versions of the Project Service application that the names of the stages in the Project Stages business process flow must exactly match the expected English names (**Quote**, **Plan**, **Close**).</span></span> <span data-ttu-id="dbe02-105">В противен случай бизнес логиката, която разчита на английските имена на етапи, няма да работи според очакваното.</span><span class="sxs-lookup"><span data-stu-id="dbe02-105">Otherwise, the business logic, which relies on the English stage names, doesn't work as expected.</span></span> <span data-ttu-id="dbe02-106">Ето защо вие не виждате познати действия като **Превключване на процес** или **Редактиране на процес** налични във формуляра на проекта, освен това персонализирането на потока на бизнес процес не се насърчава.</span><span class="sxs-lookup"><span data-stu-id="dbe02-106">That's why you don't see familiar actions such as **Switch Process** or **Edit Process** available on the project form, and customizing the business process flow isn't encouraged.</span></span> 

<span data-ttu-id="dbe02-107">Това ограничение е било адресирано във версия 2.4.5.48 и по-нова.</span><span class="sxs-lookup"><span data-stu-id="dbe02-107">This limitation has been addressed in version 2.4.5.48 and later.</span></span> <span data-ttu-id="dbe02-108">Тази статия предоставя предложени заобиколни решения, ако имате нужда да персонализирате потока на бизнес процес по подразбиране за по-ранни версии.</span><span class="sxs-lookup"><span data-stu-id="dbe02-108">This article provides suggested workarounds if you need to customize the default business process flow for earlier versions.</span></span>  

## <a name="business-logic-requires-an-exact-match-with-english-stage-names"></a><span data-ttu-id="dbe02-109">Бизнес логиката изисква точно съвпадение с английските имена на етап</span><span class="sxs-lookup"><span data-stu-id="dbe02-109">Business logic requires an exact match with English stage names</span></span>

<span data-ttu-id="dbe02-110">Потокът на бизнес процес „Етапи на проект” включва бизнес логика, която управлява следните поведения в приложението:</span><span class="sxs-lookup"><span data-stu-id="dbe02-110">The Project Stages business process flow includes business logic that drives the following behaviors in the app:</span></span>
- <span data-ttu-id="dbe02-111">Когато проектът е свързан с оферта, кодът задава потока на бизнес процес на етап **Quote**.</span><span class="sxs-lookup"><span data-stu-id="dbe02-111">When the project is associated with a quote, the code sets the business process flow to the **Quote** stage.</span></span>
- <span data-ttu-id="dbe02-112">Когато проектът е свързан с договор, кодът задава потока на бизнес процес на етап **Plan**.</span><span class="sxs-lookup"><span data-stu-id="dbe02-112">When the project is associated with a contract, the code sets the business process flow to the **Plan** stage.</span></span>
- <span data-ttu-id="dbe02-113">Когато потокът на бизнес процес е придвижен до етап **Close**, записът на проекта се дезактивира.</span><span class="sxs-lookup"><span data-stu-id="dbe02-113">When the business process flow is advanced to the **Close** stage, the project record is deactivated.</span></span> <span data-ttu-id="dbe02-114">Когато проектът е дезактивиран, формулярът на проекта и съставната структура на работата (WBS) се задават на състояние само за четене, именуваните резервации на ресурс се освобождават и всички свързани ценови листи се дезактивират.</span><span class="sxs-lookup"><span data-stu-id="dbe02-114">When the project is deactivated, the project form and work breakdown structure (WBS) are set to read-only, the named resource bookings are released, and any associated price lists are deactivated.</span></span>

<span data-ttu-id="dbe02-115">Тази бизнес логика се основава на английските имена на етапи на проекта.</span><span class="sxs-lookup"><span data-stu-id="dbe02-115">This business logic relies on the English names for the project stages.</span></span> <span data-ttu-id="dbe02-116">Тази зависимост от английските имена на етапи е основната причина за това персонализирането на потока на бизнес процес на „Етапи на проект” да не се насърчава, както и за това да не виждате обикновени действия на потока на бизнес процес, като **Превключване на процес** или **Редактиране на процес** в обекта на проекта.</span><span class="sxs-lookup"><span data-stu-id="dbe02-116">This dependency on the English stage names is the main reason why customization of the Project Stages business process flow isn't encouraged, as well as why you don’t see the common business process flow actions like **Switch Process** or **Edit Process** on the project entity.</span></span>

## <a name="what-happens-if-the-stage-names-dont-match-the-english-names"></a><span data-ttu-id="dbe02-117">Какво става, ако имената на етап не съвпадат с английските имена?</span><span class="sxs-lookup"><span data-stu-id="dbe02-117">What happens if the stage names don't match the English names?</span></span>

<span data-ttu-id="dbe02-118">В приложението Project Service, версия 1.x на платформата 8.2, когато имената на етапи в потока на бизнес процес не отговарят точно на английските имена на етап, бизнес логиката, която задава правилния етап за оферта или договор, или такава, която затваря проект, се пропуска.</span><span class="sxs-lookup"><span data-stu-id="dbe02-118">In the Project Service app version 1.x on the 8.2 platform, when the stage names in the business process flow don’t match the English stage names exactly, the business logic that sets the right stage for quotes or contracts, or that closes the project, is skipped.</span></span> <span data-ttu-id="dbe02-119">Съобщения за грешки не се показват.</span><span class="sxs-lookup"><span data-stu-id="dbe02-119">No error messages are displayed.</span></span> <span data-ttu-id="dbe02-120">По тази причина изглежда, че можете да персонализирате потока на бизнес процес „Етапи на проект”.</span><span class="sxs-lookup"><span data-stu-id="dbe02-120">Therefore it appears that you are able to customize the Project Stages business process flow.</span></span> <span data-ttu-id="dbe02-121">Няма да видите обаче никой от автоматичните процеси да работи за оферти, договори и затваряне на проект.</span><span class="sxs-lookup"><span data-stu-id="dbe02-121">However, you won’t see any of the automatic processes working for quotes, contracts, and project close.</span></span>

<span data-ttu-id="dbe02-122">В приложението Project Service, версия 2.4.4.30 или по-стара на платформа 9.0 има значителна архитектурна промяна на потока на бизнес процес, която изисква пренаписване на бизнес логиката на потока на бизнес процес.</span><span class="sxs-lookup"><span data-stu-id="dbe02-122">In the Project Service app version 2.4.4.30 or earlier on the 9.0 platform, there was a significant architectural change to business process flows, which required a re-write of the business process flow business logic.</span></span> <span data-ttu-id="dbe02-123">В резултат на това, ако имената на етап от процеса не съответстват на очакваните английски имена, ще получите съобщение за грешка.</span><span class="sxs-lookup"><span data-stu-id="dbe02-123">As a result, if the process stage names don’t match the expected English names, you do receive an error message.</span></span> 

<span data-ttu-id="dbe02-124">По тази причина, ако искате да персонализирате потока на бизнес процес „Етапи на проект” за обекта на проекта, можете само да добавите напълно нови етапи към потока на бизнес процес по подразбиране за обекта на проект, като запазите етапите **Quote**, **Plan** и **Close**, както са си.</span><span class="sxs-lookup"><span data-stu-id="dbe02-124">Therefore, if you want to customize the Project Stages business process flow for the project entity, you can only add brand new stages to the default business process flow for the project entity, while keeping the **Quote**, **Plan**, and **Close** stages as-is.</span></span> <span data-ttu-id="dbe02-125">Това ограничение гарантира, че няма да получите грешки от бизнес логиката, която очаква английски имена на етап в потока на бизнес процес.</span><span class="sxs-lookup"><span data-stu-id="dbe02-125">This restriction ensures that you don’t get errors from the business logic that expects the English stage names in the business process flow.</span></span>

<span data-ttu-id="dbe02-126">Във версия 2.4.5.48 или по-нова бизнес логиката, описана в тази статия, е премахната от потока на бизнес процес по подразбиране за обекта на проекта.</span><span class="sxs-lookup"><span data-stu-id="dbe02-126">In version 2.4.5.48 or later, the business logic described in this article has been removed from the default business process flow for the project entity.</span></span> <span data-ttu-id="dbe02-127">Надстройката до тази версия или по-нова ще ви позволи да персонализирате или подмените потока на бизнес процес по подразбиране с ваш такъв.</span><span class="sxs-lookup"><span data-stu-id="dbe02-127">Upgrading to that version or later will let you customize or replace the default business process flow with one of your own.</span></span> 

## <a name="workarounds-for-earlier-versions"></a><span data-ttu-id="dbe02-128">Заобиколни решения за по-ранни версии</span><span class="sxs-lookup"><span data-stu-id="dbe02-128">Workarounds for earlier versions</span></span>

<span data-ttu-id="dbe02-129">Ако надстройката не е опция, можете да персонализирате потока на бизнес процес „Етапи на проект” за обекта на проекта по един от следните начини:</span><span class="sxs-lookup"><span data-stu-id="dbe02-129">If upgrading isn't an option, you can customize the Project Stages business process flow for the project entity in one of these two ways:</span></span>

1. <span data-ttu-id="dbe02-130">Добавете допълнителни етапи към конфигурацията по подразбиране, като запазите английските имена на етап за **Quote**, **Plan** и **Close**.</span><span class="sxs-lookup"><span data-stu-id="dbe02-130">Add additional stages to the default configuration, while retaining the English stage names for **Quote**, **Plan**, and **Close**.</span></span>


![Екранна снимка на добавянето на етапи към конфигурацията по подразбиране](media/FAQ-Customize-BPF-1.png)
 
2. <span data-ttu-id="dbe02-132">Създайте свой собствен поток на бизнес процес и го направете основен поток на бизнес процес за обекта на проекта, което ще ви позволи да имате всяко желано име на етап.</span><span class="sxs-lookup"><span data-stu-id="dbe02-132">Create your own business process flow and make it the primary business process flow for the project entity, which lets you have any stage names you want.</span></span> <span data-ttu-id="dbe02-133">Ако обаче искате да използвате същите стандартни етапи на проект **Quote**, **Plan** и **Close**, трябва да направите някои персонализации, които са предизвикани от вашите персонализирани имена на етапи.</span><span class="sxs-lookup"><span data-stu-id="dbe02-133">However, if you want to use the same standard project stages **Quote**, **Plan**, and **Close**, you need to do some customizations that are driven off your custom stage names.</span></span> <span data-ttu-id="dbe02-134">По-сложната логика е в затварянето на проекта, което все още можете да задействате, като просто дезактивирате записа на проекта.</span><span class="sxs-lookup"><span data-stu-id="dbe02-134">The more complex logic is in the closing of the project, which you can still trigger by just deactivating the project record.</span></span>

![Персонализиране на BPF](media/FAQ-Customize-BPF-2.png)

### <a name="additional-considerations-for-project-service-app-version-24430-or-earlier-on-platform-90"></a><span data-ttu-id="dbe02-136">Допълнителни съображения за приложение Project Service, версия 2.4.4.30 или по-нова на платформа 9.0</span><span class="sxs-lookup"><span data-stu-id="dbe02-136">Additional considerations for Project Service app version 2.4.4.30 or earlier on platform 9.0</span></span>

<span data-ttu-id="dbe02-137">В Project Service, версия 2.4.4.30 или по-нова на платформа 9.0 при персонализиран поток на бизнес процес полето **Име на етап** в обекта на проект, използвано в диаграмата **Проект по етап** и изгледите на списък на проекта, няма да се актуализира, защото е сдвоено с потока на бизнес процес „Етапи на проект”.</span><span class="sxs-lookup"><span data-stu-id="dbe02-137">In Project Service 2.4.4.30 or earlier on platform 9.0, with a custom business process flow the **Stage Name** field on the project entity used in the **Project By Stage** chart and project list views won’t update, because it’s coupled to the default Project Stages business process flow.</span></span> <span data-ttu-id="dbe02-138">Можете да решите този проблем чрез следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="dbe02-138">You can address this issue with the following steps:</span></span>

- <span data-ttu-id="dbe02-139">Добавете персонализирано поле, за да уловите текущия етап на поток на бизнес процес, който се актуализира, докато потребителят преминава през персонализирания поток на бизнес процес.</span><span class="sxs-lookup"><span data-stu-id="dbe02-139">Add a custom field to capture the current business process flow stage that is updated as the user advances through the custom business process flow.</span></span>

- <span data-ttu-id="dbe02-140">Променете диаграмата **Проект по етап**, за да работи с персонализираното ви поле вместо конфигурацията по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="dbe02-140">Modify the **Project By Stage** chart to work with your custom field instead of the default configuration.</span></span>

### <a name="steps-to-create-your-own-business-process-flow-for-the-project-entity"></a><span data-ttu-id="dbe02-141">Стъпки за създаване на собствен поток на бизнес процес за обекта на процеса</span><span class="sxs-lookup"><span data-stu-id="dbe02-141">Steps to create your own business process flow for the project entity</span></span>

<span data-ttu-id="dbe02-142">За да създадете свой собствен поток на бизнес процес за обекта на проекта, направете следното:</span><span class="sxs-lookup"><span data-stu-id="dbe02-142">To create your own business process flow for the project entity do the following:</span></span>

1. <span data-ttu-id="dbe02-143">Отидете в **Настройки** > **Център за процеси**.</span><span class="sxs-lookup"><span data-stu-id="dbe02-143">Go to **Settings** > **Process Center**.</span></span> <span data-ttu-id="dbe02-144">Не копирайте потока на бизнес процес „Етапи на проект”, защото това ще копира и бизнес логиката на Project Service.</span><span class="sxs-lookup"><span data-stu-id="dbe02-144">Don’t copy the Project Stages business process flow because that also copies the Project Service business logic.</span></span>

  ![Създаване на процес](media/FAQ-Customize-BPF-3.png)

2. <span data-ttu-id="dbe02-146">Използвайте дизайнера на процеси, за да създадете желаните имена на етапи.</span><span class="sxs-lookup"><span data-stu-id="dbe02-146">Use the Process Designer to create the stage names you want.</span></span> <span data-ttu-id="dbe02-147">Ако искате същата функционалност като етапите по подразбиране за **Оферта**, **План** и **Затваряне**, ще трябва да я създадете според вашите персонализирани имена на етапи на поток на бизнес процес.</span><span class="sxs-lookup"><span data-stu-id="dbe02-147">If you want the same functionality as the default stages for **Quote**, **Plan**, and **Close**, you’ll have to create that based on your custom business process flow’s stage names.</span></span>

   ![Екранна снимка на дизайнера на процеси, използван за персонализиране на BPF](media/FAQ-Customize-BPF-4.png) 

3. <span data-ttu-id="dbe02-149">В дизайнера на процеси щракнете върху **Подреждане на поток на процес**, за да направите персонализирания поток на бизнес процес основен поток на бизнес процес за обекта на проекта, като го преместите над потока на бизнес процес „Етапи на проект” в горната част на списъка.</span><span class="sxs-lookup"><span data-stu-id="dbe02-149">In the Process Designer, click **Order Process Flow** to make the custom business process flow the primary business process flow for the project entity by moving it above the Project Stages business process flow to the top of the list.</span></span>


   [<span data-ttu-id="dbe02-150">Екранна снимка на използване на подреждане на поток на процес</span><span class="sxs-lookup"><span data-stu-id="dbe02-150">Screenshot of using Order Process Flow</span></span>](media/FAQ-Customize-BPF-5-720.png)

### <a name="the-following-steps-apply-to-project-service-app-24430-or-earlier-on-the-90-platform"></a><span data-ttu-id="dbe02-151">Следващите стъпки се прилагат за приложението Project Service, версия 2.4.4.30 или по-стара на платформа 9.0</span><span class="sxs-lookup"><span data-stu-id="dbe02-151">The following steps apply to Project Service app 2.4.4.30 or earlier on the 9.0 platform</span></span>

4. <span data-ttu-id="dbe02-152">Добавете ново потребителско поле към обекта на проекта, за да уловите персонализираните етапи във вашия персонализиран поток на бизнес процес.</span><span class="sxs-lookup"><span data-stu-id="dbe02-152">Add a new custom field to the project entity to capture the custom stages in your custom business process flow.</span></span> <span data-ttu-id="dbe02-153">Ще трябва да добавите бизнес логика (добавка/работен процес), за да актуализирате това поле, когато етапът на персонализирания поток на бизнес процес се актуализира.</span><span class="sxs-lookup"><span data-stu-id="dbe02-153">You’ll need to add business logic (plugin/workflow) to update this field when the stage on the custom business process flow is updated.</span></span>

   ![Екранна снимка на персонализиране на обекта на проекта](media/FAQ-Customize-BPF-6-720.png)

5. <span data-ttu-id="dbe02-155">Променете диаграмата **Проект по етап**, за да използвате своето ново персонализирано поле за етапи.</span><span class="sxs-lookup"><span data-stu-id="dbe02-155">Modify the **Project By Stage** chart to use your new custom field for stages.</span></span>

   ![Екранна снимка на използването на диаграмата „Проект по етап”](media/FAQ-Customize-BPF-7-720.png)

6. <span data-ttu-id="dbe02-157">Променете всички изгледи за обекта на проекта, за да включите своето ново персонализирано поле за етапи.</span><span class="sxs-lookup"><span data-stu-id="dbe02-157">Modify any views for the project entity to include your new custom field for stages.</span></span>

   ![Екранна снимка на промяната на изгледи в обекта на проекта](media/FAQ-Customize-BPF-8-720.png)



[!INCLUDE[footer-include](../includes/footer-banner.md)]