---
title: Изпълнение на общите изисквания за ресурси
description: Тази тема предоставя информация за това как да резервирате ресурси за изискване за общ ресурс.
author: ruhercul
ms.date: 09/23/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: e36875a0d5dcb24d9669e2ea989c6fc7db7bcd7c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005823"
---
# <a name="generic-resource-requirement-fulfillment"></a><span data-ttu-id="3aaf2-103">Изпълнение на общите изисквания за ресурси</span><span class="sxs-lookup"><span data-stu-id="3aaf2-103">Generic resource requirement fulfillment</span></span>

<span data-ttu-id="3aaf2-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="3aaf2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="3aaf2-105">Можете да резервирате наименуван ресурс, за да замените общ ресурс, който има изискване за ресурс.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-105">You can book a named resource to replace generic resource that has a resource requirement.</span></span>

1. <span data-ttu-id="3aaf2-106">На страницата **Проекти** изберете раздела **Екип**.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-106">On the **Projects** page, select the **Team** tab.</span></span>
2. <span data-ttu-id="3aaf2-107">Изберете общия ресурс, който има изискване за ресурс, от списъка и след това изберете **Резервиране**.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-107">Select the generic resource that has a resource requirement from the list, and then select **Book**.</span></span> <span data-ttu-id="3aaf2-108">Или отворете изискването за ресурс и след това изберете **Резервиране**.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-108">Or, open the resource requirement and then select **Book**.</span></span>
3. <span data-ttu-id="3aaf2-109">На страницата **Асистент за планиране** изберете наименуван ресурс, за да го резервирате за екипа на проекта, и след това изберете **Резервиране**.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-109">On the **Schedule Assistant** page, select a named resource to book onto your project team and then select **Book**.</span></span>

<span data-ttu-id="3aaf2-110">Когато резервацията бъде завършена и изпълнена от наименуван ресурс, общият ресурс се заменя с наименувания ресурс.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-110">When the booking is complete and fulfilled by a named resource, the generic resource is replaced with the named resource.</span></span>

<span data-ttu-id="3aaf2-111">Присвояванията в графика също се актуализират с наименуваните ресурси.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-111">The assignments on the schedule are updated with the named resource as well.</span></span>

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a><span data-ttu-id="3aaf2-112">Изпълнение на общ ресурс с няколко наименувани ресурса</span><span class="sxs-lookup"><span data-stu-id="3aaf2-112">Fulfill a generic resource with multiple named resources</span></span>
<span data-ttu-id="3aaf2-113">Изпълнението на изискване за общ ресурс с множество наименувани ресурси е подобно на присвояването на един наименуван ресурс.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-113">Fulfilling a requirement for a generic resource with multiple named resources is similar to assigning a single named resource.</span></span> <span data-ttu-id="3aaf2-114">Например има задача с продължителност от пет дни и 120 часа усилия.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-114">For example, there is a task with a duration of five days and 120 hours of effort.</span></span> <span data-ttu-id="3aaf2-115">Тази задача не може да бъде изпълнена от един ресурс, който работи на обикновен осемчасов ден пет дни в седмицата.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-115">This task can't be completed by one resource that works a typical eight-hour day over a five-day week.</span></span> 

<span data-ttu-id="3aaf2-116">Изискването е за 120 часа инженер по роботика за пет дни, което е 24 часа на ден.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-116">The requirement is for 120 hours of robotics engineering over five days, which is 24 hours per day.</span></span>

<span data-ttu-id="3aaf2-117">Това е пример, когато са необходими множество наименувани ресурси за изпълнение на заявка за общ ресурс.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-117">This is an example of when multiple named resources are needed to fulfill a generic resource request.</span></span> <span data-ttu-id="3aaf2-118">Ще трябва да резервирате множество ресурси, за да изпълните изискването.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-118">You will need to book multiple resources to fulfill the requirement.</span></span>

<span data-ttu-id="3aaf2-119">Основната разлика в този сценарий е, че общият ресурс остава в екипа, присвоен на задачата, и резервираните наименувани членове на екипа от ресурси не се присвояват като част от позицията.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-119">The main difference in this scenario is that the generic resource remains on the team assigned to the task, and the booked named resource team members are not assigned as part of the position.</span></span> <span data-ttu-id="3aaf2-120">Мениджърът на проекти може да присвои работата според нуждите на наименуваните ресурси.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-120">The project manager can assign the work as appropriate to the named resources.</span></span> <span data-ttu-id="3aaf2-121">Изгледът **Съгласуване** може да помогне на мениджър на проект с разбивка на резервациите на множество ресурси на няколко присвоявания на задачи.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-121">The **Reconciliation** view can assist a project manager in breaking up the bookings across multiple resources to task assignments.</span></span> <span data-ttu-id="3aaf2-122">Това не се извършва автоматично, защото в сценарий, който е по-сложен от примера по-горе, като например такъв, в който имате пакет от задачи, съставляващи изискването или намерението на мениджъра на проекта как иска да присвои, трябва да се предположи от системата.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-122">This is not done automatically because in any scenario more complicated than the simple example above, such as where you have a bundle of tasks making up the requirement or the intent of how the project manager wants to assign, needs to be assumed by the system.</span></span> <span data-ttu-id="3aaf2-123">Тъй като системата не може да разбере намеренията, предположенията вероятно ще се различават от тях и ще възникне неправилен или непредвидим резултат.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-123">Because the system can't understand intent, it's likely that the assumptions will be different than intended and an incorrect or unpredictable result will occur.</span></span> <span data-ttu-id="3aaf2-124">Предвидимият резултат е, че общият ресурс остава присвоен, докато мениджърът на проекта нарочно присвоява създава присвоявания с помощта на изгледа **Съгласуване**.</span><span class="sxs-lookup"><span data-stu-id="3aaf2-124">The predictable outcome is that the generic resource remains assigned until the project manager deliberately creates assignments, with the assistance of the **Reconciliation** view.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]