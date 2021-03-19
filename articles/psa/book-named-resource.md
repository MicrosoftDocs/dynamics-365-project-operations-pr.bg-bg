---
title: Резервиране на наименувани ресурси от изисквания за ресурси
description: Тази тема предоставя информация за резервиране на ресурси за изискване за общ ресурс.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
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
ms.openlocfilehash: 50858d4fc55285b2e91117c6cbfb2419931b4197
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291021"
---
# <a name="book-named-resources-from-resource-requirements"></a><span data-ttu-id="83155-103">Резервиране на наименувани ресурси от изисквания за ресурси</span><span class="sxs-lookup"><span data-stu-id="83155-103">Book named resources from resource requirements</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="83155-104">Можете да резервирате наименуван ресурс, за да замените общ ресурс, който има изискване за ресурс.</span><span class="sxs-lookup"><span data-stu-id="83155-104">You can book a named resource to replace generic resource that has a resource requirement.</span></span>

1. <span data-ttu-id="83155-105">В Project Service Automation (PSA), на страницата **Проекти**, щракнете върху раздела **Екип**.</span><span class="sxs-lookup"><span data-stu-id="83155-105">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab.</span></span>
2. <span data-ttu-id="83155-106">Изберете общия ресурс, който има изискване за ресурс, от списъка и след това щракнете върху **Резервиране**.</span><span class="sxs-lookup"><span data-stu-id="83155-106">Select the generic resource that has a resource requirement from the list and then click **Book**.</span></span> <span data-ttu-id="83155-107">Или отворете изискването за ресурс и след това щракнете върху **Резервиране**.</span><span class="sxs-lookup"><span data-stu-id="83155-107">Or, open the resource requirement and then click **Book**.</span></span>


![Резервиране на общ член на екипа](media/RM-how-to-14.png)


3. <span data-ttu-id="83155-109">На страницата **Асистент за планиране** изберете наименуван ресурс, за да го резервирате за екипа на проекта, и след това щракнете върху **Резервиране**.</span><span class="sxs-lookup"><span data-stu-id="83155-109">On the **Schedule Assistant** page, select a named resource to book onto your project team and then click **Book**.</span></span>

![Резервиране на общ член на екипа с помощта на асистента за планиране](media/RM-how-to-15.png)

<span data-ttu-id="83155-111">Когато резервацията бъде завършена и изпълнена от наименуван ресурс, общият ресурс се заменя с наименувания ресурс.</span><span class="sxs-lookup"><span data-stu-id="83155-111">When the booking is complete and fulfilled by a named resource, the generic resource is replaced with the named resource.</span></span>

![Наименуван член на екипа заменя общ член на екипа](media/RM-how-to-16.png)

<span data-ttu-id="83155-113">Присвояванията в графика също се актуализират с наименуваните ресурси.</span><span class="sxs-lookup"><span data-stu-id="83155-113">The assignments on the schedule are updated with the named resource as well.</span></span>

![Наименуван член на екипа, присвоен на задачи по проекта](media/RM-how-to-17.png)

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a><span data-ttu-id="83155-115">Изпълнение на общ ресурс с няколко наименувани ресурса</span><span class="sxs-lookup"><span data-stu-id="83155-115">Fulfill a generic resource with multiple named resources</span></span>
<span data-ttu-id="83155-116">Изпълнението на изискване за общ ресурс с множество наименувани ресурси е подобно на присвояването на един наименуван ресурс.</span><span class="sxs-lookup"><span data-stu-id="83155-116">Fulfilling a requirement for a generic resource with multiple named resources is similar to assigning a single named resource.</span></span> <span data-ttu-id="83155-117">Например има задача с продължителност от пет дни и 120 часа усилия.</span><span class="sxs-lookup"><span data-stu-id="83155-117">For example, there is a task with a duration of five days and 120 hours of effort.</span></span> <span data-ttu-id="83155-118">Тази задача не може да бъде изпълнена от един ресурс, който работи на обикновен осемчасов ден пет дни в седмицата.</span><span class="sxs-lookup"><span data-stu-id="83155-118">This task can't be completed by one resource that works a typical eight-hour day over a five day week.</span></span> 

![Задача, която се нуждае от 120 часа усилия за пет дни](media/RM-how-to-21.png)

<span data-ttu-id="83155-120">Изискването е за 120 часа инженер по роботика за пет дни, което е 24 часа на ден.</span><span class="sxs-lookup"><span data-stu-id="83155-120">The requirement is for 120 hours of robotics engineering over five days, which is 24 hours per day.</span></span>

![Изискване за ден](media/RM-how-to-22.png)

<span data-ttu-id="83155-122">Това е пример, когато са необходими множество наименувани ресурси за изпълнение на заявка за общ ресурс.</span><span class="sxs-lookup"><span data-stu-id="83155-122">This is an example of when multiple named resources are needed to fulfill a generic resource request.</span></span> <span data-ttu-id="83155-123">Ще трябва да резервирате множество ресурси, за да изпълните изискването.</span><span class="sxs-lookup"><span data-stu-id="83155-123">You will need to book multiple resources to fulfill the requirement.</span></span>

![Резервиране на множество ресурси за изпълнение на изискването](media/RM-how-to-23.png)

<span data-ttu-id="83155-125">Основната разлика в този сценарий е, че общият ресурс остава в екипа, присвоен на задачата, и резервираните наименувани членове на екипа от ресурси не се присвояват като част от позицията.</span><span class="sxs-lookup"><span data-stu-id="83155-125">The main difference in this scenario is that the generic resource remains on the team assigned to the task, and the booked named resource team members are not assigned as part of the position.</span></span> <span data-ttu-id="83155-126">Мениджърът на проекти може да присвои работата според нуждите на наименуваните ресурси.</span><span class="sxs-lookup"><span data-stu-id="83155-126">The project manager can assign the work as appropriate to the named resources.</span></span> <span data-ttu-id="83155-127">Изгледът **Съгласуване** може да помогне на мениджър на проект с разбивка на резервациите на множество ресурси на няколко присвоявания на задачи.</span><span class="sxs-lookup"><span data-stu-id="83155-127">The **Reconciliation** view can assist a project manager in breaking up the bookings across multiple resources to task assignments.</span></span> <span data-ttu-id="83155-128">Това не се извършва автоматично, защото в сценарий, който е по-сложен от примера по-горе, като например такъв, в който имате пакет от задачи, съставляващи изискването, намерението на мениджъра на проекта как иска да присвои, трябва да се предположи от системата.</span><span class="sxs-lookup"><span data-stu-id="83155-128">This is not done automatically because in any scenario more complicated than the simple example above, such as where you have a bundle of tasks making up the requirement, the intent of how the project manager wants to assign, needs to be assumed by the system.</span></span> <span data-ttu-id="83155-129">Тъй като системата не може да разбере намеренията, предположенията вероятно ще се различават от тях и ще се получи неправилен или непредвидим резултат.</span><span class="sxs-lookup"><span data-stu-id="83155-129">Because the system can't understand intent, chances are that the assumptions will be different than intended and an incorrect or unpredictable result will happen.</span></span> <span data-ttu-id="83155-130">Предвидимият резултат е, че общият ресурс остава присвоен, докато мениджърът на проекта нарочно присвоява създава присвоявания с помощта на изгледа **Съгласуване**.</span><span class="sxs-lookup"><span data-stu-id="83155-130">The predictable outcome is that the generic resource remains assigned until the project manager deliberately creates assignments, with the assistance of the **Reconciliation** view.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]