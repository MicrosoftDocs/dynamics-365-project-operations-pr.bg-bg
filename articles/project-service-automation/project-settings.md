---
title: Настройки на проекти
description: Тази тема предоставя информация за настройките за управление на проекти.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 7c5be6ff-8f92-4dfc-9f9d-4abc76f96638
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 843192092598fd713b3bc59bf90c5362d0dad8b4
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749260"
---
# <a name="project-settings"></a><span data-ttu-id="142e7-103">Настройки на проекти</span><span class="sxs-lookup"><span data-stu-id="142e7-103">Project settings</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="142e7-104">Използвайте следните настройки за достъп до функциите за планиране на проекти.</span><span class="sxs-lookup"><span data-stu-id="142e7-104">Use the following settings to access the project planning features.</span></span>

## <a name="work-template"></a><span data-ttu-id="142e7-105">Работен шаблон</span><span class="sxs-lookup"><span data-stu-id="142e7-105">Work template</span></span>

<span data-ttu-id="142e7-106">За да създадете график на проект, създайте шаблон на календар на проект, който определя броя на работни часове на ден и всички неработни дни.</span><span class="sxs-lookup"><span data-stu-id="142e7-106">To create a project schedule, you create a project calendar template that defines the number of working hours per day and any business closures.</span></span> <span data-ttu-id="142e7-107">За да създадете шаблон за календар на проект, свържете работен шаблон с полето **Шаблон на календар** за проекта.</span><span class="sxs-lookup"><span data-stu-id="142e7-107">To create a project calendar template, you associate a work template with the **Calendar template** field for the project.</span></span> <span data-ttu-id="142e7-108">Изпълнете следните стъпки, за да създадете работен шаблон.</span><span class="sxs-lookup"><span data-stu-id="142e7-108">Follow these steps to create a work template.</span></span>

1. <span data-ttu-id="142e7-109">В PSA, в левия навигационен екран, щракнете върху **Ресурси**.</span><span class="sxs-lookup"><span data-stu-id="142e7-109">In PSA, in the left navigation pane, click **Resources**.</span></span> 
2. <span data-ttu-id="142e7-110">На страницата със списъка **Ресурси** отворете потребителски запис и след това изберете **Показване на работните часове**.</span><span class="sxs-lookup"><span data-stu-id="142e7-110">On the **Resources** list page, open a user record, and then select **Show Work Hours**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="142e7-111">Уверете се, че сте разрешили изскачащи прозорци на страницата на браузъра.</span><span class="sxs-lookup"><span data-stu-id="142e7-111">Make sure that you allow pop-ups on the browser page.</span></span> <span data-ttu-id="142e7-112">Това ви позволява да видите работните часове, зададени за ресурса.</span><span class="sxs-lookup"><span data-stu-id="142e7-112">This lets you see the work hours set for the resource.</span></span>
  
3. <span data-ttu-id="142e7-113">В раздела **Месечен изглед** щракнете върху **Настройване**.</span><span class="sxs-lookup"><span data-stu-id="142e7-113">On the **Monthly View** tab, click **Set Up**.</span></span> <span data-ttu-id="142e7-114">Показва се списък с три опции:</span><span class="sxs-lookup"><span data-stu-id="142e7-114">A list of three options appears:</span></span> 

  - <span data-ttu-id="142e7-115">Нов седмичен график</span><span class="sxs-lookup"><span data-stu-id="142e7-115">New Weekly Schedule</span></span>
  - <span data-ttu-id="142e7-116">Седмичен график за един ден</span><span class="sxs-lookup"><span data-stu-id="142e7-116">Work Schedule for One Day</span></span>
  - <span data-ttu-id="142e7-117">Почивка</span><span class="sxs-lookup"><span data-stu-id="142e7-117">Time Off</span></span>

> ![Настройване на опции](media/project-13.png)

4. <span data-ttu-id="142e7-119">Изберете **Нов седмичен график** и след това задайте опциите за този график на ресурс.</span><span class="sxs-lookup"><span data-stu-id="142e7-119">Select **New Weekly Schedule**, and then set the options for this resource schedule.</span></span> <span data-ttu-id="142e7-120">Можете да зададете повтарящ се седмичен график, дневни часови параметри, неработни дни и др.</span><span class="sxs-lookup"><span data-stu-id="142e7-120">You can set a recurring weekly schedule, daily hour parameters, business closures, and more.</span></span>
5. <span data-ttu-id="142e7-121">Задайте диапазон от дати, изберете **Запиши** и след това щракнете върху **Затваряне**.</span><span class="sxs-lookup"><span data-stu-id="142e7-121">Set the date range, select **Save**, and then click **Close**.</span></span> 
6. <span data-ttu-id="142e7-122">Върнете се на страницата със списъка **Ресурси** и изберете ресурса, за който задавате работните часове.</span><span class="sxs-lookup"><span data-stu-id="142e7-122">Go back to the **Resources** list page, and select the resource that you set the work hours for.</span></span> 
7. <span data-ttu-id="142e7-123">Изберете **Задаване на календара като**, за да зададете работния шаблон.</span><span class="sxs-lookup"><span data-stu-id="142e7-123">Select **Set Calendar As** to set the work template.</span></span> 
8. <span data-ttu-id="142e7-124">В диалоговия прозорец **Работен шаблон** въведете името за работния шаблон и след това изберете **Прилагане**.</span><span class="sxs-lookup"><span data-stu-id="142e7-124">In the **Work Template** dialog box, enter a name for the work template, and then select **Apply**.</span></span> 

<span data-ttu-id="142e7-125">Сега можете да свържете работния шаблон с шаблон на календар на проект.</span><span class="sxs-lookup"><span data-stu-id="142e7-125">You can now associate the work template with a project calendar template.</span></span>

## <a name="resource-roles"></a><span data-ttu-id="142e7-126">Роли на ресурси</span><span class="sxs-lookup"><span data-stu-id="142e7-126">Resource roles</span></span>

<span data-ttu-id="142e7-127">Терминът *роля на ресурс* се отнася до набор от умения, компетенции и сертификати, които дадено лице трябва да притежава, за да изпълни определен набор от задачи по даден проект.</span><span class="sxs-lookup"><span data-stu-id="142e7-127">The term *resource role* refers to the set of skills, competencies, and certifications that a person must have to perform a specific set of tasks on a project.</span></span> <span data-ttu-id="142e7-128">PSA ви позволява да остойностявате и фактурирате времето на ресурс въз основа на ролята, с която е свързан ресурсът.</span><span class="sxs-lookup"><span data-stu-id="142e7-128">PSA lets you cost and bill a resource's time based on the role that the resource is associated with.</span></span> <span data-ttu-id="142e7-129">Всяка организация трябва да настрои тези роли с помощта на лявата навигация в менюто на **Project Service**.</span><span class="sxs-lookup"><span data-stu-id="142e7-129">Every organization must set up these roles by using the left navigation on the **Project Service** menu.</span></span>

<span data-ttu-id="142e7-130">Всяка организация трябва да настрои тези роли в страницата **Активни категории ресурси**.</span><span class="sxs-lookup"><span data-stu-id="142e7-130">Every organization must set up these roles on the **Active Resource Categories** page.</span></span> <span data-ttu-id="142e7-131">За да отворите тази страница, в левия навигационен екран изберете **Роли на ресурси**.</span><span class="sxs-lookup"><span data-stu-id="142e7-131">To open this page, in the left navigation pane, select **Resource Roles**.</span></span>

## <a name="price-lists"></a><span data-ttu-id="142e7-132">Ценови листи</span><span class="sxs-lookup"><span data-stu-id="142e7-132">Price lists</span></span>

<span data-ttu-id="142e7-133">Ценовите листи ви позволяват да задавате разходите и продажните цени за роли на ресурси, категории разходи, продукти и други елементи в дадена организация.</span><span class="sxs-lookup"><span data-stu-id="142e7-133">Price lists let you set cost and sales prices for resource roles, expense categories, products, and other elements in an organization.</span></span> <span data-ttu-id="142e7-134">Преди да настроите финансови прогнозни оценки за работата, която трябва да бъде извършена за проект, трябва да създадете поддържаща ценова листа за разходи и продажби.</span><span class="sxs-lookup"><span data-stu-id="142e7-134">Before you set financial estimates for the work that must be delivered for a project, you should create a backing cost and sales price list.</span></span> <span data-ttu-id="142e7-135">В секцията с параметри трябва също да настроите ценова листа за разходи и продажби по подразбиране, която се отнася за всички проекти, които са създадени в организацията.</span><span class="sxs-lookup"><span data-stu-id="142e7-135">In the parameters section, you should also set up a default cost and sales price list that applies to all projects that are created in the organization.</span></span> <span data-ttu-id="142e7-136">На страницата **Активни параметри на проекта** се уверете, че сте настроили ценова листа за разходи и продажби.</span><span class="sxs-lookup"><span data-stu-id="142e7-136">On the **Active Project Parameters** page, make sure that you set up a default cost and sales price list.</span></span>
