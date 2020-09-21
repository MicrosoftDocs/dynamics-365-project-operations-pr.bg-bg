---
title: Присвояване на общи налични ресурси на задача и екип на проект
description: Тази тема предоставя информация за резервиране на общи ресурси за задачи и екипи на проекти.
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: f461fbd3-1fce-4aeb-a896-a6d14453a5a4
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 82478e2cf97ab03e80e9f5fbb662b3603d5905b9
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749380"
---
# <a name="assign-generic-bookable-resources-to-a-task-and-generate-resource-requirements"></a><span data-ttu-id="6f0a4-103">Присвояване на общи налични ресурси на задача и генериране на изисквания за ресурси</span><span class="sxs-lookup"><span data-stu-id="6f0a4-103">Assign generic bookable resources to a task and generate resource requirements</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="6f0a4-104">Освен резервиране и присвояване на наименувани или реални ресурси на вашия проект, можете да присвоите общи ресурси на задачи по проекта.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-104">In addition to booking and assigning named or real resources to your project, you can assign generic resources to project tasks.</span></span> <span data-ttu-id="6f0a4-105">Тези ресурси могат да служат като контейнери за наименувани ресурси, докато не сте готови да осигурите персонал за вашия проект с наименувани ресурси.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-105">These resources can serve as placeholders for named resources until you are ready to staff your project with named resources.</span></span> 

1. <span data-ttu-id="6f0a4-106">В Project Service Automation (PSA) отворете страницата **Проект** и в раздела **График** въведете името на позицията на общия ресурс в клетката **Ресурс** на графика.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-106">In Project Service Automation (PSA), open the **Project** page and on the **Schedule** tab, enter the position name of the generic resource in the **Resource** cell of the schedule.</span></span> <span data-ttu-id="6f0a4-107">Или щракнете върху иконата **Ресурс** в клетката, за да отворите инструмента за избор на ресурси, и след това въведете името на общия ресурс, който искате да създадете.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-107">Or, click the **Resource** icon in the cell to open the resource picker and then enter the name of the generic resource that you want to create.</span></span>

![Създаване и присвояване на общ член на екипа](media/RM-how-to-9.png)

<span data-ttu-id="6f0a4-109">Това ще отвори панела **Бързо създаване: член на екипа на проект**.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-109">This will open the **Quick Create: Project Team Member** panel.</span></span> 

2. <span data-ttu-id="6f0a4-110">Въведете ролята и организационната единица на члена на екипа общ ресурс и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-110">Enter the role and organization unit of the generic resource team member and then click **Save**.</span></span>

![Бързо създаване на общ член на екип](media/RM-how-to-10.png)

3. <span data-ttu-id="6f0a4-112">След като сте създали новия член на екипа общ ресурс, той се присвоява на задачата.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-112">After you have created the new generic resource team member, it is assigned to the task.</span></span> <span data-ttu-id="6f0a4-113">Можете да продължите да присвоявате този общ ресурс на други задачи в графика на задачите.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-113">You can continue to assign that generic resource to other tasks in the task schedule.</span></span>

![Присвояване на съществуващ общ член на екипа на задачи](media/RM-how-to-11.png)

4. <span data-ttu-id="6f0a4-115">След като сте присвоили общия ресурс, можете да генерирате изискване за ресурс и да го изпълните, като направите директна резервация или подадете заявка за ресурс до мениджър на ресурси.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-115">After you have assigned the generic resource, you can generate a resource requirement and fulfill it by directly booking or submitting a resource request to a resource manager.</span></span>

![Генериране на изискване за общ член на екипа](media/RM-how-to-12.png)

<span data-ttu-id="6f0a4-117">В мрежата на члена на екипа, освен че можете да използвате инструмента за избор на ресурси, както е споменато по-горе, можете да добавите общи ресурси директно.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-117">On the team member grid, in addition to being able to use the resource picker as mentioned above, you can add generic resources directly.</span></span> <span data-ttu-id="6f0a4-118">Ресурсите се добавят с изискване за ресурс, което се базира на началната/крайната дата и метода на разпределение, посочен в панела **Бързо създаване: член на екипа на проект**.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-118">The resources are added with a resource requirement that is based on the start/end dates and allocation method specified in the **Quick Create: Project Team Member** panel.</span></span>

<span data-ttu-id="6f0a4-119">Можете да видите разликата, ако добавите общия член на екипа директно и след това присвоите повече задачи на общия ресурс, отколкото са часовете, които трябва да бъдат покрити от него.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-119">You can see a difference if you add the generic team member directly and then assign more tasks to the generic resource than they have required hours to cover.</span></span> <span data-ttu-id="6f0a4-120">Щракнете върху **Генериране на изискване**, за да генериране отново изискването за балансиране на необходимите часове спрямо задачите.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-120">Click **Generate Requirement** to regenerate the requirement to balance the required hours against assignments.</span></span>

<span data-ttu-id="6f0a4-121">Можете също така да щракнете върху връзката **Изискване за ресурс** в мрежата на екипа, за да отворите изискването и да добавите умения, предпочитани ресурси и т. н.</span><span class="sxs-lookup"><span data-stu-id="6f0a4-121">You can also click the **Resource requirement** link in the team grid to open the requirement and add skills, preferred resources, etc.</span></span>

![Изискване за ресурс](media/RM-how-to-13.png)

