---
title: Предоставяне на оценки за работата за проект по време на процеса на продажба
description: Как се предоставят оценки за работата за проект по време на процеса на продажба в Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: e9382127b2ce0b157d681fc77d67200ba9c5e59d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147955"
---
# <a name="provide-work-estimates-for-a-project-during-the-sales-process-project-service"></a><span data-ttu-id="1acc7-103">Предоставяне на оценки за работата за проект по време на процеса на продажба (Project Service)</span><span class="sxs-lookup"><span data-stu-id="1acc7-103">Provide work estimates for a project during the sales process (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="1acc7-104">По време на процеса на продажба можете да изготвите оценки за продажби от самото начало с редове за оферти.</span><span class="sxs-lookup"><span data-stu-id="1acc7-104">During the sales process, you can work out sales estimates from the ground up with quote lines.</span></span> <span data-ttu-id="1acc7-105">Възможностите на услугата за проекти [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]в [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] осигуряват по-научен и причинно-следствен начин за оформяне на оценки за продажбите чрез разбивка на елементите от работата и свързване на съответните атрибути, които допринасят за оценките за проекта в съставна структура на работата.</span><span class="sxs-lookup"><span data-stu-id="1acc7-105">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] provide a more scientific and deterministic way of coming up with sales estimates by breaking down work items and associating relevant attributes that contribute toward the estimates for the project in the work breakdown structure.</span></span>  
  
 <span data-ttu-id="1acc7-106">След като спечелите продажбата, можете да използвате свързаната съставна структура на работата плана на проекта си, като го прецизирате според нуждите за успешно завършване на проекта ви.</span><span class="sxs-lookup"><span data-stu-id="1acc7-106">Once you win the sale, you can use the associated work breakdown structure in your project plan, refining it as necessary for successful completion of your project.</span></span>  
  
## <a name="link-a-project-to-a-quote-line"></a><span data-ttu-id="1acc7-107">Свързване на проект към ред за оферта</span><span class="sxs-lookup"><span data-stu-id="1acc7-107">Link a project to a quote line</span></span>  
 <span data-ttu-id="1acc7-108">Когато създавате оферта, базирана на проект, можете да създадете нов проект от реда на офертата.</span><span class="sxs-lookup"><span data-stu-id="1acc7-108">When creating a project-based quote line, you can create a new project from the quote line.</span></span> <span data-ttu-id="1acc7-109">След това можете да използвате шаблони шаблони за проект, които са или предварително конфигурирани стандартни планове за проект и финансови оценки, обичайни за организацията ви, или копие от план на проект и оценки от минал проект.</span><span class="sxs-lookup"><span data-stu-id="1acc7-109">You can then use project templates, which are either pre-configured standard project plans and financial estimates common to your organization, or a copy of a project plan and estimates from a past project.</span></span> <span data-ttu-id="1acc7-110">Когато създавате даден проект, избирането на шаблон на проект предоставя основа за прецизиране на плана на проекта, оценките и изискванията за роли.</span><span class="sxs-lookup"><span data-stu-id="1acc7-110">When you create a project, choosing a project template provides a basis to refine the project plan, estimates, and role requirements.</span></span> <span data-ttu-id="1acc7-111">Чрез създаването на проекта ви от офертата, проектът автоматично се свързва с реда за оферта.</span><span class="sxs-lookup"><span data-stu-id="1acc7-111">By creating your project from the quote, the project is automatically associated with the quote line.</span></span>  
  
## <a name="project-estimate-components"></a><span data-ttu-id="1acc7-112">Компоненти на оценката на проекта</span><span class="sxs-lookup"><span data-stu-id="1acc7-112">Project estimate components</span></span>  
 <span data-ttu-id="1acc7-113">Съставната структура на работата в даден проект предоставя начин за разбиване на работата на задачи, поддържане на йерархия на задачите и присвояване на оценка на усилията, необходими за завършването на всяка задача.</span><span class="sxs-lookup"><span data-stu-id="1acc7-113">The work breakdown structure in a project provides a way to break down work into tasks, maintain a hierarchy of tasks, and assign an estimate of effort required to complete each task.</span></span> <span data-ttu-id="1acc7-114">Можете също да свържете роли към задача, за да определите оценка на типа ресурси, необходим за завършване на задача, както и график.</span><span class="sxs-lookup"><span data-stu-id="1acc7-114">You can also associate roles to a task to indicate an estimate of the type of resource required to complete a task and a schedule.</span></span>  
  
 <span data-ttu-id="1acc7-115">Съставната структура на работата ви помага да определите оценките за усилията за работата и графика.</span><span class="sxs-lookup"><span data-stu-id="1acc7-115">The work breakdown structure helps you determine work effort and schedule estimates.</span></span> <span data-ttu-id="1acc7-116">По подразбиране проектът използва ценовата листа по подразбиране, която сте дефинирали по-рано.</span><span class="sxs-lookup"><span data-stu-id="1acc7-116">By default, the project uses default price lists that you defined earlier.</span></span> <span data-ttu-id="1acc7-117">Разходите и продажните цени, определени в ценовите листи, помагат за определянето на оценките за разбивката на работата по проекта.</span><span class="sxs-lookup"><span data-stu-id="1acc7-117">The cost and sales prices defined in the price lists help determine financial estimates for the project’s work breakdown.</span></span>  
  
 <span data-ttu-id="1acc7-118">Ако вашият проект е свързан с оферта, и офертата има ценова листа, различна от тази по подразбиране, за финансовите оценки се използва ценовата листа на офертата.</span><span class="sxs-lookup"><span data-stu-id="1acc7-118">If your project is associated with a quote, and the quote has a different price list from the default, the quote’s price list is used for financial estimates.</span></span>  
  
## <a name="import-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="1acc7-119">Импортиране на оценки от проект в оферта</span><span class="sxs-lookup"><span data-stu-id="1acc7-119">Import estimates from a project into a quote</span></span>  
 <span data-ttu-id="1acc7-120">След като имате оценки за проект в проекта, можете да импортирате тези оценки в реда на офертата:</span><span class="sxs-lookup"><span data-stu-id="1acc7-120">Once you have project estimates in the project, you can import these estimates into the quote line:</span></span>  
  
-   <span data-ttu-id="1acc7-121">В **Подробности за ред на оферта** щракнете върху **Импортиране от оценки**.</span><span class="sxs-lookup"><span data-stu-id="1acc7-121">In **Quote Line Details**, click **Import from estimates**.</span></span> 

-   <span data-ttu-id="1acc7-122">Изберете дали да импортирате оценките на проекта обобщени по тип на транзакция, роля или ниво на възел в съставната структура на работата.</span><span class="sxs-lookup"><span data-stu-id="1acc7-122">Select whether to import project estimates summarized by transaction type, role, or work breakdown structure node level.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="1acc7-123">Вижте също</span><span class="sxs-lookup"><span data-stu-id="1acc7-123">See Also</span></span>  
 [<span data-ttu-id="1acc7-124">Ръководство за мениджъри на проекти</span><span class="sxs-lookup"><span data-stu-id="1acc7-124">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
