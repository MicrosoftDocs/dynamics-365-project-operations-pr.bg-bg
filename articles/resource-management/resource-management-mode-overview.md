---
title: Общ преглед на режими на управление на ресурси
description: Тази тема предоставя информация за функционалността Управление на ресурс Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 4a8e605109e48b50da68abeee989f8ac8d3d659c
ms.sourcegitcommit: cf79185c8c84c55fbae55f9cfc1b17840e072b49
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/01/2020
ms.locfileid: "3930078"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="92b86-103">Общ преглед на режими на управление на ресурси</span><span class="sxs-lookup"><span data-stu-id="92b86-103">Resource management modes overview</span></span>

<span data-ttu-id="92b86-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="92b86-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="92b86-105">Dynamics 365 Project Operations поддържа два режима, за да можете да изпълните цялостния процес на резервация.</span><span class="sxs-lookup"><span data-stu-id="92b86-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="92b86-106">Режимът на управление се определя като параметър на проекта и може да бъде модифициран, ако вашият бизнес се нуждае от промяна.</span><span class="sxs-lookup"><span data-stu-id="92b86-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="92b86-107">Централен режим</span><span class="sxs-lookup"><span data-stu-id="92b86-107">Central mode</span></span>
<span data-ttu-id="92b86-108">За организации, които централизират разпределението на ресурси за проекти, централният режим осигурява начин да се гарантира, че мениджърите на проекти могат да определят изискванията за ресурси на ниво проект.</span><span class="sxs-lookup"><span data-stu-id="92b86-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="92b86-109">Изпълнението на изискванията за ресурси се делегира на мениджър на ресурси.</span><span class="sxs-lookup"><span data-stu-id="92b86-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="92b86-110">Мениджърите на проекти могат да приемат или отхвърлят ресурси, предложени от Мениджъра на ресурси.</span><span class="sxs-lookup"><span data-stu-id="92b86-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![Централен режим](./media/resource-management-central.png)

<span data-ttu-id="92b86-112">За да управлявате ресурси с централния режим, вижте:</span><span class="sxs-lookup"><span data-stu-id="92b86-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="92b86-113">Присвояване на общи налични ресурси на задача и генериране на изисквания за ресурси</span><span class="sxs-lookup"><span data-stu-id="92b86-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="92b86-114">Резервиране на наименувани ресурси от изисквания за ресурси</span><span class="sxs-lookup"><span data-stu-id="92b86-114">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="92b86-115">Подаване на заявка за ресурс</span><span class="sxs-lookup"><span data-stu-id="92b86-115">Submit a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="92b86-116">Изпълнете заявка за ресурс</span><span class="sxs-lookup"><span data-stu-id="92b86-116">Fulfill a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="92b86-117">Приемане или отхвърляне на предложен ресурс по проект от заявка за ресурс</span><span class="sxs-lookup"><span data-stu-id="92b86-117">Accept or reject a proposed project resource from a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="92b86-118">Хибриден режим</span><span class="sxs-lookup"><span data-stu-id="92b86-118">Hybrid mode</span></span>
<span data-ttu-id="92b86-119">За организации, които изискват гъвкавост при разпределението на ресурсите, хибридният режим дава възможност както на ръководителите на проекти, така и на мениджърите на ресурси да резервират ресурси.</span><span class="sxs-lookup"><span data-stu-id="92b86-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![Хибриден режим](./media/resource-management-hybrid.png)

<span data-ttu-id="92b86-121">В допълнение към процеса на поддържан централен режим, вижте следните теми за управление на всички други поддържани потоци на резервации в хибриден режим:</span><span class="sxs-lookup"><span data-stu-id="92b86-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="92b86-122">Резервиране на ресурс директно към проект:</span><span class="sxs-lookup"><span data-stu-id="92b86-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="92b86-123">Резервиране на наименувани налични ресурси в екип по проект и присвояване на задачи</span><span class="sxs-lookup"><span data-stu-id="92b86-123">Book named bookable resources to a project team and assign tasks</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="92b86-124">Резервиране на ресурс от изискване за ресурси:</span><span class="sxs-lookup"><span data-stu-id="92b86-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="92b86-125">Присвояване на общи налични ресурси на задача и генериране на изисквания за ресурси</span><span class="sxs-lookup"><span data-stu-id="92b86-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="92b86-126">Резервиране на наименувани ресурси от изисквания за ресурси</span><span class="sxs-lookup"><span data-stu-id="92b86-126">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
