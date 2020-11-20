---
title: Резервации спрямо задания
description: Тази тема предоставя информация за разликите между резервациите на ресурси и назначенията на ресурси.
author: ruhercul
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 8fe6937dfdfe137f28917c16da1d7dc6155284ae
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130205"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="a3ec5-103">Резервации спрямо задания</span><span class="sxs-lookup"><span data-stu-id="a3ec5-103">Bookings vs assignments</span></span>

<span data-ttu-id="a3ec5-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="a3ec5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a3ec5-105">Резервациите са потвърдено или непотвърдено разпределение на ресурси за даден проект.</span><span class="sxs-lookup"><span data-stu-id="a3ec5-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="a3ec5-106">Потвърдените резервации консумират капацитет на ресурса.</span><span class="sxs-lookup"><span data-stu-id="a3ec5-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="a3ec5-107">Резервациите представляват организационни концепции за екипите, така че те да могат да разберат как ще бъдат ангажирани ресурси в разнообразни проекти.</span><span class="sxs-lookup"><span data-stu-id="a3ec5-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="a3ec5-108">Dynamics 365 Project Operations счита резервациите за концепция на ниво проект.</span><span class="sxs-lookup"><span data-stu-id="a3ec5-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="a3ec5-109">За разлика от резервациите присвояванията представляват ангажимент на ресурси към задачи по проекта в графика на проекта.</span><span class="sxs-lookup"><span data-stu-id="a3ec5-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="a3ec5-110">Ресурсите могат да бъдат наименувани или общи.</span><span class="sxs-lookup"><span data-stu-id="a3ec5-110">The resources can be named or generic.</span></span> 

<span data-ttu-id="a3ec5-111">Обикновено сборът на резервациите за ресурс ще се равнява на сборът от присвояванията на ресурса към една или много задачи.</span><span class="sxs-lookup"><span data-stu-id="a3ec5-111">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="a3ec5-112">Project Operations обаче не налага това споразумение.</span><span class="sxs-lookup"><span data-stu-id="a3ec5-112">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="a3ec5-113">Изгледът **Съгласуване** показва на мениджъра на проекта местата, където резервациите на ресурса и присвояванията не са съгласувани.</span><span class="sxs-lookup"><span data-stu-id="a3ec5-113">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>
