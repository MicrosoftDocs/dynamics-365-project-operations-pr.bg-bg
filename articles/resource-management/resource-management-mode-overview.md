---
title: Общ преглед на режими на управление на ресурси
description: Тази тема предоставя информация за функционалността за управление на ресурс в Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 94db65a2ddbdc6a7226c70907bcce4c45b4a3923
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000873"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="9d490-103">Общ преглед на режими на управление на ресурси</span><span class="sxs-lookup"><span data-stu-id="9d490-103">Resource management modes overview</span></span>

<span data-ttu-id="9d490-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="9d490-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="9d490-105">Dynamics 365 Project Operations поддържа два режима, за да можете да изпълните цялостния процес на резервация.</span><span class="sxs-lookup"><span data-stu-id="9d490-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="9d490-106">Режимът на управление се определя като параметър на проекта и може да бъде модифициран, ако вашият бизнес се нуждае от промяна.</span><span class="sxs-lookup"><span data-stu-id="9d490-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="9d490-107">Централен режим</span><span class="sxs-lookup"><span data-stu-id="9d490-107">Central mode</span></span>
<span data-ttu-id="9d490-108">За организации, които централизират разпределението на ресурси за проекти, централният режим осигурява начин да се гарантира, че мениджърите на проекти могат да определят изискванията за ресурси на ниво проект.</span><span class="sxs-lookup"><span data-stu-id="9d490-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="9d490-109">Изпълнението на изискванията за ресурси се делегира на мениджър на ресурси.</span><span class="sxs-lookup"><span data-stu-id="9d490-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="9d490-110">Мениджърите на проекти могат да приемат или отхвърлят ресурси, предложени от Мениджъра на ресурси.</span><span class="sxs-lookup"><span data-stu-id="9d490-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![Централен режим](./media/resource-management-central.png)

<span data-ttu-id="9d490-112">За да управлявате ресурси с централния режим, вижте:</span><span class="sxs-lookup"><span data-stu-id="9d490-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="9d490-113">Присвояване на общи налични ресурси на задача и генериране на изисквания за ресурси</span><span class="sxs-lookup"><span data-stu-id="9d490-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="9d490-114">Резервиране на наименувани ресурси от изисквания за ресурси</span><span class="sxs-lookup"><span data-stu-id="9d490-114">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="9d490-115">Подаване на заявка за ресурс</span><span class="sxs-lookup"><span data-stu-id="9d490-115">Submit a resource request</span></span>](/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="9d490-116">Изпълнете заявка за ресурс</span><span class="sxs-lookup"><span data-stu-id="9d490-116">Fulfill a resource request</span></span>](/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="9d490-117">Приемане или отхвърляне на предложен ресурс по проект от заявка за ресурс</span><span class="sxs-lookup"><span data-stu-id="9d490-117">Accept or reject a proposed project resource from a resource request</span></span>](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="9d490-118">Хибриден режим</span><span class="sxs-lookup"><span data-stu-id="9d490-118">Hybrid mode</span></span>
<span data-ttu-id="9d490-119">За организации, които изискват гъвкавост при разпределението на ресурсите, хибридният режим дава възможност както на ръководителите на проекти, така и на мениджърите на ресурси да резервират ресурси.</span><span class="sxs-lookup"><span data-stu-id="9d490-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![Хибриден режим](./media/resource-management-hybrid.png)

<span data-ttu-id="9d490-121">В допълнение към процеса на поддържан централен режим, вижте следните теми за управление на всички други поддържани потоци на резервации в хибриден режим:</span><span class="sxs-lookup"><span data-stu-id="9d490-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="9d490-122">Резервиране на ресурс директно към проект:</span><span class="sxs-lookup"><span data-stu-id="9d490-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="9d490-123">Резервиране на наименувани налични ресурси в екип по проект и присвояване на задачи</span><span class="sxs-lookup"><span data-stu-id="9d490-123">Book named bookable resources to a project team and assign tasks</span></span>](/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="9d490-124">Резервиране на ресурс от изискване за ресурси:</span><span class="sxs-lookup"><span data-stu-id="9d490-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="9d490-125">Присвояване на общи налични ресурси на задача и генериране на изисквания за ресурси</span><span class="sxs-lookup"><span data-stu-id="9d490-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="9d490-126">Резервиране на наименувани ресурси от изисквания за ресурси</span><span class="sxs-lookup"><span data-stu-id="9d490-126">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]