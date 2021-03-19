---
title: ЧЗВ за управление на ресурси
description: Тази тема дава отговори на често задавани въпроси за управлението на ресурси.
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
ms.openlocfilehash: 20562b98ccc8451ab57dd42fb8c2f9f303811dbe
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5283130"
---
# <a name="resource-management-faq"></a><span data-ttu-id="bb345-103">ЧЗВ за управление на ресурси</span><span class="sxs-lookup"><span data-stu-id="bb345-103">Resource management FAQ</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

## <a name="what-is-the-difference-between-a-team-member-and-a-resource-requirement"></a><span data-ttu-id="bb345-104">Каква е разликата между член на екипа и изискване за ресурс?</span><span class="sxs-lookup"><span data-stu-id="bb345-104">What is the difference between a team member and a resource requirement?</span></span>

<span data-ttu-id="bb345-105">Член на екипа на проект може да бъде присвоен на задачи, резервиран или резервиран над капацитета и зададен като одобряващ.</span><span class="sxs-lookup"><span data-stu-id="bb345-105">A project team member can be assigned to tasks, booked or overbooked, and set as an approver.</span></span> <span data-ttu-id="bb345-106">Изискване за ресурс може да съществува без член на екипа на проект, като чернова на бележка за търсене.</span><span class="sxs-lookup"><span data-stu-id="bb345-106">A resource requirement can exist without a project team member, as a draft note of demand.</span></span> 

## <a name="what-is-the-difference-between-proposed-and-soft-booked-hours"></a><span data-ttu-id="bb345-107">Каква е разликата между предложените и непотвърдените часове?</span><span class="sxs-lookup"><span data-stu-id="bb345-107">What is the difference between proposed and soft-booked hours?</span></span>

<span data-ttu-id="bb345-108">Предложените часове и непотвърдените часове се различават по видимост.</span><span class="sxs-lookup"><span data-stu-id="bb345-108">Proposed hours and soft-booked hours differ in visibility.</span></span> <span data-ttu-id="bb345-109">Предложените часове са видими само за мениджъри на ресурси и мениджъра на проекта, който е инициирал търсенето с помощта на заявка за ресурс.</span><span class="sxs-lookup"><span data-stu-id="bb345-109">Proposed hours are visible only to resource managers and the project manager who initiated the demand by using a resource request.</span></span> <span data-ttu-id="bb345-110">Непотвърдените часове са видими за всеки, който има достъп до таблото на графика.</span><span class="sxs-lookup"><span data-stu-id="bb345-110">Soft-booked hours are visible to anyone who has access to the Schedule Board.</span></span>

## <a name="how-can-i-see-the-soft-booked-hours-for-resources-on-a-team"></a><span data-ttu-id="bb345-111">Как мога да видя непотвърдените часове за ресурси в екип?</span><span class="sxs-lookup"><span data-stu-id="bb345-111">How can I see the soft-booked hours for resources on a team?</span></span>

<span data-ttu-id="bb345-112">Непотвърдени резервации можете да направите, когато резервирате изискване за ресурс.</span><span class="sxs-lookup"><span data-stu-id="bb345-112">Soft bookings can made when you book a resource requirement.</span></span> <span data-ttu-id="bb345-113">Ресурси, които имат непотвърдена резервация в екип на проект, се показват като членове на екипа, които имат непотвърдени часове.</span><span class="sxs-lookup"><span data-stu-id="bb345-113">Resources that are soft-booked on a project team appear as team members who have soft-booked hours.</span></span> <span data-ttu-id="bb345-114">Те се показват също и на таблото на графика.</span><span class="sxs-lookup"><span data-stu-id="bb345-114">They also appear on the Schedule Board.</span></span>

## <a name="how-do-i-change-the-required-hours-and-the-start-and-end-dates-for-a-resource-generic-or-named-that-i-booked"></a><span data-ttu-id="bb345-115">Как да променя необходимите часове, както и началната и крайната дата, за ресурс (общ или наименуван), които съм резервирал?</span><span class="sxs-lookup"><span data-stu-id="bb345-115">How do I change the required hours, and the start and end dates, for a resource (generic or named) that I booked?</span></span>

<span data-ttu-id="bb345-116">След като ресурсите са резервирани, изберете **Поддръжка на резервации**, за да направите всички необходими промени.</span><span class="sxs-lookup"><span data-stu-id="bb345-116">After resources are booked, select **Maintain Bookings** to make any changes that are required.</span></span>

## <a name="what-resources-types-does-project-service-automation-support"></a><span data-ttu-id="bb345-117">Какви типове ресурси поддържа Project Service Automation?</span><span class="sxs-lookup"><span data-stu-id="bb345-117">What resources types does Project Service Automation support?</span></span>

<span data-ttu-id="bb345-118">**Потребител** и **Контакт** са единствените типове ресурси, които се поддържат в Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="bb345-118">**User** and **Contact** are the only resource types that are supported in Dynamics 365 Project Service Automation.</span></span> <span data-ttu-id="bb345-119">Въпреки че можете да създавате други видове ресурси (например **Оборудване** и **Група**), за тях не се поддържа случай на използване „от край до край“.</span><span class="sxs-lookup"><span data-stu-id="bb345-119">Although you can create other types of resources (for example, **Equipment** and **Group**), no end-to-end use case is supported for them.</span></span>

## <a name="what-is-the-difference-between-an-assignment-and-a-booking"></a><span data-ttu-id="bb345-120">Каква е разликата между присвояване и резервация?</span><span class="sxs-lookup"><span data-stu-id="bb345-120">What is the difference between an assignment and a booking?</span></span>

<span data-ttu-id="bb345-121">Присвояванията са присвояването на ресурси на задачи по проекта в графика на проекта.</span><span class="sxs-lookup"><span data-stu-id="bb345-121">Assignments are the assignment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="bb345-122">Ресурсите могат да бъдат реални или общи ресурси.</span><span class="sxs-lookup"><span data-stu-id="bb345-122">The resources can be either real or generic resources.</span></span> <span data-ttu-id="bb345-123">Резервациите са потвърдено или непотвърдено разпределение на ресурси за даден проект.</span><span class="sxs-lookup"><span data-stu-id="bb345-123">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="bb345-124">Потвърдените резервации консумират капацитет на ресурса.</span><span class="sxs-lookup"><span data-stu-id="bb345-124">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="bb345-125">В идеалния случай за реални ресурси резервациите и присвояванията трябва да са съгласувани, защото не се различават.</span><span class="sxs-lookup"><span data-stu-id="bb345-125">Ideally, for real resources, the bookings and assignments should agree, because they don't differ.</span></span> <span data-ttu-id="bb345-126">PSA обаче не прилага това съгласуване.</span><span class="sxs-lookup"><span data-stu-id="bb345-126">However, PSA doesn't enforce this agreement.</span></span> <span data-ttu-id="bb345-127">Изгледът „Съгласуване“ показва на мениджъра на проекта местата, където резервациите на ресурса и присвояванията не са съгласувани.</span><span class="sxs-lookup"><span data-stu-id="bb345-127">The Reconciliation view shows a project manager places where a resource's bookings and assignments don't agree.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]