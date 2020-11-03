---
title: Конфигуриране на допълнителни настройки на параметри
description: Как се конфигурират допълнителни настройки на параметри в Project Service
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 24a4fe83471da916fb91cfe20e739279c08d8e5e
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071820"
---
# <a name="configure-additional-parameter-settings-project-service"></a><span data-ttu-id="388bc-103">Конфигуриране на допълнителни настройки на параметри (Project Service)</span><span class="sxs-lookup"><span data-stu-id="388bc-103">Configure additional parameter settings (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="388bc-104">След като сте конфигурирали елементите в предишните теми, трябва да зададете допълнителни параметри на проекта за използване в проектите ви.</span><span class="sxs-lookup"><span data-stu-id="388bc-104">Once you’ve configured the items in previous topics, you need to set additional project parameters to use for your projects.</span></span> <span data-ttu-id="388bc-105">При първата инсталация на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] сте създали настройка за параметър първо да се създадат всички записи, нужни за работата на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="388bc-105">When you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you created a parameters setting to first create all the records required for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to work.</span></span> <span data-ttu-id="388bc-106">Сега е време да се върнете и да конфигурирате допълнителни полета за тези настройки.</span><span class="sxs-lookup"><span data-stu-id="388bc-106">Now it’s time to go back and configure additional fields for these settings.</span></span>  
  
 <span data-ttu-id="388bc-107">Трябва да конфигурирате следните настройки:</span><span class="sxs-lookup"><span data-stu-id="388bc-107">You’ll need to have configured the following settings:</span></span>  
  
-   <span data-ttu-id="388bc-108">Организационна единица</span><span class="sxs-lookup"><span data-stu-id="388bc-108">Organizational unit</span></span>  
  
-   <span data-ttu-id="388bc-109">Честота на фактура</span><span class="sxs-lookup"><span data-stu-id="388bc-109">Invoice frequency</span></span>  
  
-   <span data-ttu-id="388bc-110">Шаблони за работно време</span><span class="sxs-lookup"><span data-stu-id="388bc-110">Work hours template</span></span>  
  
-   <span data-ttu-id="388bc-111">Ценова листа</span><span class="sxs-lookup"><span data-stu-id="388bc-111">Price list</span></span>  
 
<span data-ttu-id="388bc-112">В тази стъпка ще укажете и какъв тип разпределение на ресурсите искате:</span><span class="sxs-lookup"><span data-stu-id="388bc-112">In this step, you’ll also indicate what type of resource allocation you want:</span></span>  
  
- <span data-ttu-id="388bc-113">**Централен**.</span><span class="sxs-lookup"><span data-stu-id="388bc-113">**Central**.</span></span> <span data-ttu-id="388bc-114">Само управителите на ресурси могат да разпределят ресурси на проекти.</span><span class="sxs-lookup"><span data-stu-id="388bc-114">Only resource managers can allocate resources to projects.</span></span>  
  
- <span data-ttu-id="388bc-115">**Хибриден**.</span><span class="sxs-lookup"><span data-stu-id="388bc-115">**Hybrid**.</span></span> <span data-ttu-id="388bc-116">Управители на ресурси, управители на проекти и главни счетоводители могат да разпределят ресурси на проекти.</span><span class="sxs-lookup"><span data-stu-id="388bc-116">Resource managers, project managers, and account managers can allocate resources to projects.</span></span>  
  
 
<span data-ttu-id="388bc-117">За да зададете параметри на проект:</span><span class="sxs-lookup"><span data-stu-id="388bc-117">To set project parameters:</span></span>  
  
1. <span data-ttu-id="388bc-118">Отидете на **Project Service > Параметри**.</span><span class="sxs-lookup"><span data-stu-id="388bc-118">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="388bc-119">Щракнете върху настройката на параметри, която искате да конфигурирате (тази, която сте създали, когато сте инсталирали за първи път [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), или щракнете върху **Нова** , за да създадете нова.</span><span class="sxs-lookup"><span data-stu-id="388bc-119">Click the parameters setting you want to configure (the one you created when you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), or click **New** to create a new one.</span></span>  
  
3. <span data-ttu-id="388bc-120">В зоната **Общи** , задайте всички опции за параметрите на вашия проект.</span><span class="sxs-lookup"><span data-stu-id="388bc-120">In the **General** area, set all the options for your project parameters.</span></span>  
  
4. <span data-ttu-id="388bc-121">В зоната **Ценова листа** щракнете върху **+** , за да добавите ценова листа, изберете ценова листа в падащия списък **Ценова листа на параметър на проект** и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="388bc-121">In the **Price List** area, click **+** to add a price list, select a price list in the **Project Parameter Price List** drop-down list, and then click **Save**.</span></span>  
  
5. <span data-ttu-id="388bc-122">Щракнете върху бутона **Записване** в долния десен ъгъл на екрана.</span><span class="sxs-lookup"><span data-stu-id="388bc-122">Click the **Save** button in the bottom right corner of the screen.</span></span>  

> [!NOTE]
> <span data-ttu-id="388bc-123">Записът на параметрите на проекта трябва да се поддържа, за да може Project Service да функционира правилно.</span><span class="sxs-lookup"><span data-stu-id="388bc-123">The project parameter record must be maintained for Project Service to function correcly.</span></span> <span data-ttu-id="388bc-124">Този запис не трябва да се изтрива.</span><span class="sxs-lookup"><span data-stu-id="388bc-124">This record should not be deleted.</span></span>

### <a name="see-also"></a><span data-ttu-id="388bc-125">Вижте също</span><span class="sxs-lookup"><span data-stu-id="388bc-125">See Also</span></span>  
 [<span data-ttu-id="388bc-126">Задаване на ресурси</span><span class="sxs-lookup"><span data-stu-id="388bc-126">Set up resources</span></span>](../psa/set-up-resources.md)
