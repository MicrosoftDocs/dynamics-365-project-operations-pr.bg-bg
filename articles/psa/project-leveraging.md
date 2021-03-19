---
title: Прогнозни оценки за продажби и проекти
description: Тази тема предоставя информация за това как да се възползвате от графика и прогнозите в процеса на продажби.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: 87dc72b76ec4f88684ef2c702718e1ab631ff936
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5283895"
---
# <a name="sales-estimates-and-projects"></a><span data-ttu-id="7b176-103">Прогнозни оценки за продажби и проекти</span><span class="sxs-lookup"><span data-stu-id="7b176-103">Sales estimates and projects</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="7b176-104">По време на процеса на продажби можете да създавате прогнозни оценки за продажби, като свържете проект към оферта за продажба.</span><span class="sxs-lookup"><span data-stu-id="7b176-104">During the sales process, you can create sales estimates by linking a project to a sales quote.</span></span> <span data-ttu-id="7b176-105">По този начин може да се появи еднозначна прогнозна оценка по време на процеса на продажба, за да се възползвате от възможностите за планиране и оценка на проекта.</span><span class="sxs-lookup"><span data-stu-id="7b176-105">In this way, deterministic estimation can occur during the sales process, to take advantage of project scheduling and estimation capabilities.</span></span> <span data-ttu-id="7b176-106">Ако продажбата е одобрена, графикът, използван за целите на прогнозната оценка на продажбите, може да се използва като основа за по-нататъшно уточняване на плана на проекта.</span><span class="sxs-lookup"><span data-stu-id="7b176-106">If the sale goes through, the schedule that was used for sales estimation purposes can be used as the basis for further refinement of the project plan.</span></span>

## <a name="linking-a-project-to-a-quote-line"></a><span data-ttu-id="7b176-107">Свързване на проект към ред на оферта</span><span class="sxs-lookup"><span data-stu-id="7b176-107">Linking a project to a quote line</span></span>

<span data-ttu-id="7b176-108">Когато създавате ред на оферта, базирана на проект, можете да създадете нов проект или да свържете съществуващ проект на страницата **Ред на оферта**.</span><span class="sxs-lookup"><span data-stu-id="7b176-108">When you create a project-based quote line, you can create a new project or associate an existing project pn the **Quote Line** page.</span></span> 

> ![Формуляр „Ред на оферта“](media/project-8.png)
 
<span data-ttu-id="7b176-110">Когато създавате нов проект от подробностите от реда на офертата, можете да се възползвате от шаблоните на проекти.</span><span class="sxs-lookup"><span data-stu-id="7b176-110">When you create a new project from the quote line details, you can take advantage of project templates.</span></span> <span data-ttu-id="7b176-111">Шаблоните на проекти са примерни проекти, които представляват стандартни проектни планове и финансови прогнозни оценки, които са типични за дадена организация.</span><span class="sxs-lookup"><span data-stu-id="7b176-111">Project templates are model projects that represent standard project plans and financial estimates that are typical in an organization.</span></span> <span data-ttu-id="7b176-112">Те могат също така да представляват копия от проектни планове и прогнозни оценки от минали проекти.</span><span class="sxs-lookup"><span data-stu-id="7b176-112">They can also represent copies of project plans and estimates from past projects.</span></span>

> ![Подробности за ред на оферта](media/project-9.png)
  
<span data-ttu-id="7b176-114">Когато създавате от офертата, проектът автоматично се свързва с реда за офертата.</span><span class="sxs-lookup"><span data-stu-id="7b176-114">When you create the project from the quote, the project is automatically associated with the quote line.</span></span>

## <a name="components-of-estimates-in-a-project"></a><span data-ttu-id="7b176-115">Компоненти на прогнозни оценки в проект</span><span class="sxs-lookup"><span data-stu-id="7b176-115">Components of estimates in a project</span></span>

<span data-ttu-id="7b176-116">Графикът ви позволява да разделяте работата на задачи, да поддържате йерархия на задачите, да определяте какви ресурси са необходими за изпълнение на задача и да присвоявате прогнозна оценка на усилието, което е необходимо за изпълнение на задача.</span><span class="sxs-lookup"><span data-stu-id="7b176-116">A schedule lets you divide work into tasks, maintain a hierarchy of tasks, determine what resources are required to complete a task, and assign an estimate of the effort that is required to complete a task.</span></span>

<span data-ttu-id="7b176-117">Можете да дефинирате прогнозните оценки на работните усилия и графиците, като използвате полетата в раздела **График** на страницата **Проект**.</span><span class="sxs-lookup"><span data-stu-id="7b176-117">You can define the work effort and schedule estimates by using the fields on the **Schedule** tab of the **Project** page.</span></span> <span data-ttu-id="7b176-118">Тъй като ценовата листа е свързана с проекта, финансовите оценки се изчисляват чрез използване на разходите и продажните цени, които са дефинирани в ценовата листа.</span><span class="sxs-lookup"><span data-stu-id="7b176-118">Because a price list is associated with the project, financial estimates are calculated by using cost and sales prices that are defined in the price list.</span></span>

## <a name="importing-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="7b176-119">Импортиране на оценки от проект в оферта</span><span class="sxs-lookup"><span data-stu-id="7b176-119">Importing estimates from a project into a quote</span></span>

<span data-ttu-id="7b176-120">След като дефинирате прогнозни оценки за проект, можете да ги импортирате в реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="7b176-120">After you define project estimates, you can import them into the quote line.</span></span> <span data-ttu-id="7b176-121">На страницата **Подробности на ред на оферта** изберете **Импортиране от прогнозни оценки** в лентата, за да обобщите прогнозните оценки за проекта по тип на транзакция, роля или ниво на задача.</span><span class="sxs-lookup"><span data-stu-id="7b176-121">On the **Quote Line Details** page, select **Import from estimates** on the ribbon to summarize project estimates by transaction type, role, or task level.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]