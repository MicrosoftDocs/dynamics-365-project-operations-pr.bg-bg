---
title: Определяне на календари на проекти
description: Тази тема предоставя информация за използването на календар на проекта за проследяване на графика на проекта.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 1d44a2d0d8c13fb9e93b9a6da15fb3a7ce8d764c
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897978"
---
# <a name="define-project-calendars"></a><span data-ttu-id="10a02-103">Определяне на календари на проекти</span><span class="sxs-lookup"><span data-stu-id="10a02-103">Define project calendars</span></span>

<span data-ttu-id="10a02-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="10a02-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="10a02-105">За да създадете график на проект, създайте шаблон на календар на проект, който определя броя на работни часове на ден и всички неработни дни.</span><span class="sxs-lookup"><span data-stu-id="10a02-105">To create a project schedule, you create a project calendar template that defines the number of working hours per day and any business closures.</span></span> <span data-ttu-id="10a02-106">За да създадете шаблон за календар на проект, свържете работен шаблон с полето **Шаблон на календар** за проекта.</span><span class="sxs-lookup"><span data-stu-id="10a02-106">To create a project calendar template, you associate a work template with the **Calendar template** field for the project.</span></span> <span data-ttu-id="10a02-107">Изпълнете следните стъпки, за да създадете работен шаблон.</span><span class="sxs-lookup"><span data-stu-id="10a02-107">Follow these steps to create a work template.</span></span>

1. <span data-ttu-id="10a02-108">Изберете **Ресурси** в левия прозорец за навигация.</span><span class="sxs-lookup"><span data-stu-id="10a02-108">In the left navigation pane, select **Resources**.</span></span> 
2. <span data-ttu-id="10a02-109">На страницата със списъка **Ресурси** отворете потребителски запис и след това изберете **Показване на работните часове**.</span><span class="sxs-lookup"><span data-stu-id="10a02-109">On the **Resources** list page, open a user record, and then select **Show Work Hours**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="10a02-110">Уверете се, че сте разрешили изскачащи прозорци на страницата на браузъра.</span><span class="sxs-lookup"><span data-stu-id="10a02-110">Make sure that you allow pop-ups on the browser page.</span></span> <span data-ttu-id="10a02-111">Това ви позволява да видите работните часове, зададени за ресурса.</span><span class="sxs-lookup"><span data-stu-id="10a02-111">This lets you see the work hours set for the resource.</span></span>
  
3. <span data-ttu-id="10a02-112">В раздела **Месечен изглед** изберете **Настройване**.</span><span class="sxs-lookup"><span data-stu-id="10a02-112">On the **Monthly View** tab, select **Set Up**.</span></span> <span data-ttu-id="10a02-113">Показва се списък с три опции:</span><span class="sxs-lookup"><span data-stu-id="10a02-113">A list of three options appears:</span></span> 

  - <span data-ttu-id="10a02-114">Нов седмичен график</span><span class="sxs-lookup"><span data-stu-id="10a02-114">New Weekly Schedule</span></span>
  - <span data-ttu-id="10a02-115">Седмичен график за един ден</span><span class="sxs-lookup"><span data-stu-id="10a02-115">Work Schedule for One Day</span></span>
  - <span data-ttu-id="10a02-116">Неработно време</span><span class="sxs-lookup"><span data-stu-id="10a02-116">Time Off</span></span>

4. <span data-ttu-id="10a02-117">Изберете **Нов седмичен график** и след това задайте опциите за този график на ресурс.</span><span class="sxs-lookup"><span data-stu-id="10a02-117">Select **New Weekly Schedule**, and then set the options for this resource schedule.</span></span> <span data-ttu-id="10a02-118">Можете да зададете повтарящ се седмичен график, дневни часови параметри, неработни дни и др.</span><span class="sxs-lookup"><span data-stu-id="10a02-118">You can set a recurring weekly schedule, daily hour parameters, business closures, and more.</span></span>
5. <span data-ttu-id="10a02-119">Задайте диапазон от дати, изберете **Запиши** и след това изберете **Затваряне**.</span><span class="sxs-lookup"><span data-stu-id="10a02-119">Set the date range, select **Save**, and then select **Close**.</span></span> 
6. <span data-ttu-id="10a02-120">Върнете се на страницата със списъка **Ресурси** и изберете ресурса, за който задавате работните часове.</span><span class="sxs-lookup"><span data-stu-id="10a02-120">Go back to the **Resources** list page, and select the resource that you set the work hours for.</span></span> 
7. <span data-ttu-id="10a02-121">Изберете **Задаване на календара като**, за да зададете работния шаблон.</span><span class="sxs-lookup"><span data-stu-id="10a02-121">Select **Set Calendar As** to set the work template.</span></span> 
8. <span data-ttu-id="10a02-122">В диалоговия прозорец **Работен шаблон** въведете името за работния шаблон и след това изберете **Прилагане**.</span><span class="sxs-lookup"><span data-stu-id="10a02-122">In the **Work Template** dialog box, enter a name for the work template, and then select **Apply**.</span></span> 

<span data-ttu-id="10a02-123">Сега можете да свържете работния шаблон с шаблон на календар на проект.</span><span class="sxs-lookup"><span data-stu-id="10a02-123">You can now associate the work template with a project calendar template.</span></span>
