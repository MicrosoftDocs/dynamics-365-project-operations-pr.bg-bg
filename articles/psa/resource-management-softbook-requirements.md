---
title: Изисквания за непотвърдени резервации
description: Тази тема предоставя информация за това как да изпълнявате изисквания за непотвърдени резервации.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 09f7acb95be014034cc03d7eed9d37363d430601
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147370"
---
# <a name="soft-book-requirements"></a><span data-ttu-id="1a04d-103">Изисквания за непотвърдени резервации</span><span class="sxs-lookup"><span data-stu-id="1a04d-103">Soft-book requirements</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="1a04d-104">Изискването за ресурс може да бъде с потвърдена резервация.</span><span class="sxs-lookup"><span data-stu-id="1a04d-104">A resource requirement can be hard-booked.</span></span> <span data-ttu-id="1a04d-105">Потвърдената резервация създава предложение, което консумира капацитет на ресурса.</span><span class="sxs-lookup"><span data-stu-id="1a04d-105">A hard booking creates a proposal that consumes a resource's capacity.</span></span> <span data-ttu-id="1a04d-106">След това предложението се изпраща обратно на заявителя за одобрение.</span><span class="sxs-lookup"><span data-stu-id="1a04d-106">The proposal is then sent back to the requester for approval.</span></span> <span data-ttu-id="1a04d-107">Непотвърдената резервация добавя временно ресурс към екип на проект и има различно състояние на таблото на графика, но не консумира капацитета на ресурса.</span><span class="sxs-lookup"><span data-stu-id="1a04d-107">A soft booking tentatively adds a resource to a project team and has a different status on the Schedule Board, but it doesn't consume the resource's capacity.</span></span> <span data-ttu-id="1a04d-108">За да направите непотвърдена резервация от таблото на графика, задайте полето **Състояние на резервацията** на **Непотвърдена**.</span><span class="sxs-lookup"><span data-stu-id="1a04d-108">To soft-book a resource from the Schedule Board, set the **Booking Status** field to **Soft**.</span></span>

![„Състояние на резервацията“ зададено на „Непотвърдена”](media/Resource-Management-image77.png)

<span data-ttu-id="1a04d-110">Когато разделът **Екип** е в изгледа **Именувани членове на екипа**, ресурсът се появява там.</span><span class="sxs-lookup"><span data-stu-id="1a04d-110">When the **Team** tab is in the **Named Team Members** view, the resource appears there.</span></span> <span data-ttu-id="1a04d-111">Часовете с непотвърдена резервация се отчитат в колоната с **Часове с непотвърдена резервация**.</span><span class="sxs-lookup"><span data-stu-id="1a04d-111">The soft-booked hours are reported in the **Soft Booked Hours** column.</span></span>

![Часове с непотвърден резервация в изгледа „Наименувани членове на екипа“](media/Resource-Management-image78.png)

<span data-ttu-id="1a04d-113">Членовете на екипа с непотвърдена резервация могат да бъдат присвоени към задачи.</span><span class="sxs-lookup"><span data-stu-id="1a04d-113">Soft-booked team members can be assigned to tasks.</span></span>

![Член на екипа с непотвърдена резервация, присвоен към задача](media/Resource-Management-image79.png)

<span data-ttu-id="1a04d-115">В раздела **Съгласуване** не се показват резервации за ресурс с непотвърдена резервация, тъй като разделът **Съгласуване** взема предвид само потвърдени резервации.</span><span class="sxs-lookup"><span data-stu-id="1a04d-115">On the **Reconciliation** tab, no bookings are shown for a soft-book resource, because the **Reconciliation** tab considers only hard-bookings.</span></span>

![Ресурс с непотвърдена резервация без резервации в раздела „Съгласуване“](media/Resource-Management-image80.png)

> [!NOTE]
> <span data-ttu-id="1a04d-117">Не можете да направите непотвърдена резервация за ресурс от изискване, което е генерирано от общ член на екипа.</span><span class="sxs-lookup"><span data-stu-id="1a04d-117">You can't soft-book a resource from a requirement that was generated from a generic team member.</span></span>

<span data-ttu-id="1a04d-118">На таблото на графика се използва различно оцветяване за непотвърдени резервации за ресурс.</span><span class="sxs-lookup"><span data-stu-id="1a04d-118">On the Schedule Board, a different coloring is used for soft bookings for a resource.</span></span>

![Непотвърдени резервация на таблото на графика](media/Resource-Management-image81.png)

<span data-ttu-id="1a04d-120">За да преобразувате непотвърдена резервация в потвърдена резервация, на таблото на графика щракнете с десния бутон върху непотвърдената резервация и след това изберете **Промяна на състоянието** \> **Потвърдена резервация** \> **Потвърдена**.</span><span class="sxs-lookup"><span data-stu-id="1a04d-120">To convert a soft booking to a hard booking, on the Schedule Board, right-click the soft booking, and then select **Change Status** \> **Hard Book** \> **Hard**.</span></span>

![Промяна на състоянието на резервация на потвърдена](media/Resource-Management-image82.png)

<span data-ttu-id="1a04d-122">Резервацията се променя и състоянието се променя в таблото на графика.</span><span class="sxs-lookup"><span data-stu-id="1a04d-122">The booking is changed, and the status is changed on the Schedule Board.</span></span> <span data-ttu-id="1a04d-123">Тъй като състоянието на резервацията вече **Потвърдена**, ресурсът се показва като резервиран и капацитетът и наличността му се коригират.</span><span class="sxs-lookup"><span data-stu-id="1a04d-123">Because the booking status is now **Hard**, the resource is shown as booked, and its capacity and availability are adjusted.</span></span>

<span data-ttu-id="1a04d-124">Можете да използвате същия метод, за да отмените потвърдена или непотвърдена резервация от таблото на графика.</span><span class="sxs-lookup"><span data-stu-id="1a04d-124">You can use the same method to cancel a hard booking or a soft booking from the Schedule Board.</span></span>

<span data-ttu-id="1a04d-125">За да преобразувате ресурс с непотвърдена резервация в такъв с потвърдена, в раздела **Екип** изберете ресурса, след което изберете **Потвърждаване.**</span><span class="sxs-lookup"><span data-stu-id="1a04d-125">To convert a resource that is soft-booked to hard-booked on the project's **Team** tab, select the resource, and then select **Confirm**.</span></span>

![Команда „Потвърждаване“](media/Resource-Management-image83.png)
