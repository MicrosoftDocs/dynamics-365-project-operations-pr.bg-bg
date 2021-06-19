---
title: Проектни поръчки за продажби за времеви и материални проекти
description: Тази тема обяснява как да създавате поръчки за продажби, базирани на проекти, за времеви и материални проекти.
author: Yowelle
ms.date: 04/05/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2019-04-05
ms.dyn365.ops.version: AX 10.0.2
ms.openlocfilehash: dec9bc700d18f71ec7c9e976b38cb8cbb41f21b5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6009648"
---
# <a name="project-sales-orders-for-time-and-material-projects"></a><span data-ttu-id="e60b8-103">Проектни поръчки за продажби за времеви и материални проекти</span><span class="sxs-lookup"><span data-stu-id="e60b8-103">Project sales orders for time and material projects</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="e60b8-104">Тази тема описва как да създадете поръчка за продажба за проект.</span><span class="sxs-lookup"><span data-stu-id="e60b8-104">This topic describes how to create a sales order for a project.</span></span> <span data-ttu-id="e60b8-105">Поръчки за продажби могат да се създават само за проекти от типа **време и материал**.</span><span class="sxs-lookup"><span data-stu-id="e60b8-105">Sales orders can only be created for projects of type **time and material**.</span></span>

<span data-ttu-id="e60b8-106">Ако проектът за време и материал има множество източници на финансиране по договора за проект, трябва да активирате **Разрешаване на поръчки за продажба за проекти с множество източници на финансиране** параметър на страницата **Управление на проекти и счетоводни параметри**.</span><span class="sxs-lookup"><span data-stu-id="e60b8-106">If a time and material project has multiple funding sources on the project contract, you must enable the **Allow sales orders for projects with multiple funding sources** parameter on the **Project management and accounting parameters** page.</span></span> 

> [!NOTE]
> - <span data-ttu-id="e60b8-107">Налична е поддръжка за поръчки за продажба на проекти с множество източници на финансиране, започвайки с версия 10.0.2 и по-нова.</span><span class="sxs-lookup"><span data-stu-id="e60b8-107">Support for project sales orders with multiple funding sources is available starting with application release 10.0.2 and higher.</span></span>
> - <span data-ttu-id="e60b8-108">Параметърът за активиране на поддръжката за поръчки за продажби на проекти с множество източници на финансиране ще бъде премахнат през април 2020 г., след което функционалността винаги ще бъде активирана.</span><span class="sxs-lookup"><span data-stu-id="e60b8-108">The parameter to enable the support for project sales orders with multiple funding sources will be removed in the April 2020 release wave, after which the functionality will always be enabled.</span></span>

<span data-ttu-id="e60b8-109">Можете да създавате поръчки за продажби, базирани на проекти, по два начина:</span><span class="sxs-lookup"><span data-stu-id="e60b8-109">You can create project-based sales orders in two ways:</span></span>

- <span data-ttu-id="e60b8-110">Отидете на самия проект.</span><span class="sxs-lookup"><span data-stu-id="e60b8-110">Go to the project itself.</span></span> <span data-ttu-id="e60b8-111">В екрана за действие изберете **Управление > Задачи за артикули > Поръчка за продажба**.</span><span class="sxs-lookup"><span data-stu-id="e60b8-111">On the Action Pane, select **Manage > Item tasks > Sales order**.</span></span> <span data-ttu-id="e60b8-112">Информацията за проекта по подразбиране ще бъде поръчка за продажба от проекта.</span><span class="sxs-lookup"><span data-stu-id="e60b8-112">The project information will default to the sales order from the project.</span></span> <span data-ttu-id="e60b8-113">Ако проектният договор има повече от един източник на финансиране, ще трябва да изберете източника на финансиране, за да настроите клиента за поръчката за продажба.</span><span class="sxs-lookup"><span data-stu-id="e60b8-113">If the project contract has more than one funding source, you will need to select the funding source to set the customer for the sales order.</span></span> <span data-ttu-id="e60b8-114">Ако има само един източник на финансиране за проекта, клиентът ще бъде настроен автоматично.</span><span class="sxs-lookup"><span data-stu-id="e60b8-114">If there is only one funding source for the project, the customer will be automatically set.</span></span>
- <span data-ttu-id="e60b8-115">Отидете на **Всички поръчки за продажба** страница със списък и създайте нова поръчка за продажба.</span><span class="sxs-lookup"><span data-stu-id="e60b8-115">Go to the **All sales order** list page and create a new sales order.</span></span> <span data-ttu-id="e60b8-116">Ще трябва да изберете проекта за поръчка за продажба.</span><span class="sxs-lookup"><span data-stu-id="e60b8-116">You will need to select the project for the sales order.</span></span> <span data-ttu-id="e60b8-117">След като проектът бъде избран, клиентът ще бъде настроен от източника на финансиране или ще трябва да изберете източника на финансиране, ако договорът за проект има множество източници на финансиране.</span><span class="sxs-lookup"><span data-stu-id="e60b8-117">After the project is selected, the customer will be set from the funding source or you will need to select the funding source if the project contract has multiple funding sources.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]