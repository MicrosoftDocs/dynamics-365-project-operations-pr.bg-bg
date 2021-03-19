---
title: Резервации спрямо задания
description: Тази тема предоставя информация за разликите между резервациите на ресурси и назначенията на ресурси.
author: ruhercul
manager: Annbe
ms.date: 01/08/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 3aaf8dcbae0a5762879c2b1223eba3bdc33af1a7
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279890"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="07fca-103">Резервации спрямо задания</span><span class="sxs-lookup"><span data-stu-id="07fca-103">Bookings vs assignments</span></span>

<span data-ttu-id="07fca-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="07fca-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="07fca-105">Резервациите са потвърдено или непотвърдено разпределение на ресурси за даден проект.</span><span class="sxs-lookup"><span data-stu-id="07fca-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="07fca-106">Потвърдените резервации консумират капацитет на ресурса.</span><span class="sxs-lookup"><span data-stu-id="07fca-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="07fca-107">Резервациите представляват организационни концепции за екипите, така че те да могат да разберат как ще бъдат ангажирани ресурси в разнообразни проекти.</span><span class="sxs-lookup"><span data-stu-id="07fca-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="07fca-108">Dynamics 365 Project Operations счита резервациите за концепция на ниво проект.</span><span class="sxs-lookup"><span data-stu-id="07fca-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="07fca-109">За разлика от резервациите присвояванията представляват ангажимент на ресурси към задачи по проекта в графика на проекта.</span><span class="sxs-lookup"><span data-stu-id="07fca-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="07fca-110">Ресурсите могат да бъдат наименувани или общи.</span><span class="sxs-lookup"><span data-stu-id="07fca-110">The resources can be named or generic.</span></span>  <span data-ttu-id="07fca-111">Когато изискването за ресурс се извлича от заданията на проектната задача, Project Operations използва контурите на усилията на заданието за ресурси, за да изгради контурите на подробностите за изискванията за ресурси.</span><span class="sxs-lookup"><span data-stu-id="07fca-111">When a resource requirement is derived from the project task assignments, Project Operations uses the effort contours of the resources assignment to build the contours of the resource requirement details.</span></span> <span data-ttu-id="07fca-112">Обаче препратка към заданията за ресурси не се поддържа.</span><span class="sxs-lookup"><span data-stu-id="07fca-112">However, a refence to the resource assignments isn't maintained.</span></span> <span data-ttu-id="07fca-113">Актуализациите на резервациите, получени от изискването за ресурс, не актуализират никакви назначения на ресурси.</span><span class="sxs-lookup"><span data-stu-id="07fca-113">Updates to the bookings derived from the resource requirement don't update any resource assignments.</span></span>

<span data-ttu-id="07fca-114">Обикновено сборът на резервациите за ресурс ще се равнява на сборът от присвояванията на ресурса към една или много задачи.</span><span class="sxs-lookup"><span data-stu-id="07fca-114">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="07fca-115">Project Operations обаче не налага това споразумение.</span><span class="sxs-lookup"><span data-stu-id="07fca-115">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="07fca-116">Изгледът **Съгласуване** показва на мениджъра на проекта местата, където резервациите на ресурса и присвояванията не са съгласувани.</span><span class="sxs-lookup"><span data-stu-id="07fca-116">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]