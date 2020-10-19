---
title: Резервации спрямо задания
description: Тази тема предоставя информация за разликите между резервациите на ресурси и назначенията на ресурси.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fa99783e52dbcdeaf80bbfd03df0f458f86b5e99
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/28/2020
ms.locfileid: "3895998"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="9e135-103">Резервации спрямо задания</span><span class="sxs-lookup"><span data-stu-id="9e135-103">Bookings vs assignments</span></span>

<span data-ttu-id="9e135-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="9e135-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="9e135-105">Резервациите са потвърдено или непотвърдено разпределение на ресурси за даден проект.</span><span class="sxs-lookup"><span data-stu-id="9e135-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="9e135-106">Потвърдените резервации консумират капацитет на ресурса.</span><span class="sxs-lookup"><span data-stu-id="9e135-106">Hard bookings consume a resource's capacity.</span></span> 

<span data-ttu-id="9e135-107">Присвояванията са присвояването на ресурси на задачи по проекта в графика на проекта.</span><span class="sxs-lookup"><span data-stu-id="9e135-107">Assignments are the assignment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="9e135-108">Ресурсите могат да бъдат реални или общи.</span><span class="sxs-lookup"><span data-stu-id="9e135-108">The resources can be real or generic.</span></span> 

<span data-ttu-id="9e135-109">В идеалния случай за реални ресурси резервациите и присвояванията трябва да са съгласувани, защото не се различават.</span><span class="sxs-lookup"><span data-stu-id="9e135-109">Ideally, for real resources, the bookings and assignments should agree, because they don't differ.</span></span> <span data-ttu-id="9e135-110">Microsoft Dynamics Project Operations обаче не налага това споразумение.</span><span class="sxs-lookup"><span data-stu-id="9e135-110">However, Microsoft Dynamics Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="9e135-111">Изгледът **Съгласуване** показва на мениджъра на проекта местата, където резервациите на ресурса и присвояванията не са съгласувани.</span><span class="sxs-lookup"><span data-stu-id="9e135-111">The **Reconciliation** view shows a project manager places where a resource's bookings and assignments don't agree.</span></span>
