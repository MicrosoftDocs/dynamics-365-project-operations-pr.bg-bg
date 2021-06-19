---
title: Управление на договори по проекти
description: Тази тема предоставя информация за прегледа на базирани на проект договори.
author: rumant
ms.date: 10/26/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5e2f182f66bd1f4fe57d19e4bf82525ac8b84c29
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003078"
---
# <a name="manage-project-contracts"></a><span data-ttu-id="d0c38-103">Управление на договори по проекти</span><span class="sxs-lookup"><span data-stu-id="d0c38-103">Manage project contracts</span></span>

<span data-ttu-id="d0c38-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="d0c38-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d0c38-105">Договорите по проект в Dynamics 365 Project Operations улавят и управляват договорените ангажименти и подробности за фактуриране на проект.</span><span class="sxs-lookup"><span data-stu-id="d0c38-105">Project contracts in Dynamics 365 Project Operations capture and manage the contractually agreed on commitments and billing details of a project.</span></span> <span data-ttu-id="d0c38-106">Структурата на договор по проект в Project Operations е съобразена с базирана на проект работа със следните компоненти:</span><span class="sxs-lookup"><span data-stu-id="d0c38-106">The structure of a project contract in Project Operations is tailored to project-based work with the following components:</span></span>

- <span data-ttu-id="d0c38-107">Аспекти на договор, които идентифицират отделните компоненти на работата, които ще се представят като компоненти на фактура по договор.</span><span class="sxs-lookup"><span data-stu-id="d0c38-107">Contract lines that identify the discrete components of work that will be presented as high-level components on a project invoice.</span></span>
- <span data-ttu-id="d0c38-108">Подробности за аспекти на договор, които идентифицират и оценяват работата за всеки компонент от високо ниво или аспекти на договор.</span><span class="sxs-lookup"><span data-stu-id="d0c38-108">Contract line details that identify and estimate the work for each high-level component or contract line.</span></span> <span data-ttu-id="d0c38-109">Оценката включва графика и финансовите аспекти на работата, обвързани с аспектите на договора.</span><span class="sxs-lookup"><span data-stu-id="d0c38-109">The estimate includes the schedule and the financial aspects for the work tied to the contract line.</span></span>
- <span data-ttu-id="d0c38-110">Моделите за договаряне и платимите компоненти се настройват за всеки ред на договора, който съдържа споразумението за фактуриране за всеки аспект на договора и цялостния договор.</span><span class="sxs-lookup"><span data-stu-id="d0c38-110">Contracting models and chargeable components are set up for each contract line that holds the billing arrangement for each contract line and the overall contract.</span></span>

## <a name="view-all-project-based-contracts"></a><span data-ttu-id="d0c38-111">Преглед на всички базирани на проект договори</span><span class="sxs-lookup"><span data-stu-id="d0c38-111">View all project-based contracts</span></span>

<span data-ttu-id="d0c38-112">Списък с всички договори по проект може да се прегледа на страницата със списъка **Договори**.</span><span class="sxs-lookup"><span data-stu-id="d0c38-112">A list of all project contracts can be seen on the **Contracts** list page.</span></span> 

1. <span data-ttu-id="d0c38-113">Отидете на **Продажби** > **Договори**.</span><span class="sxs-lookup"><span data-stu-id="d0c38-113">Go to **Sales** > **Contracts**.</span></span> <span data-ttu-id="d0c38-114">Показва се списък с всички договори по проект в системата.</span><span class="sxs-lookup"><span data-stu-id="d0c38-114">A list of all your project Contracts in the system are shown.</span></span> 
2. <span data-ttu-id="d0c38-115">Изберете **Превключвател на изгледи** (стрелката за падащо меню до името на изгледа), за да изберете други филтрирани изгледи.</span><span class="sxs-lookup"><span data-stu-id="d0c38-115">Select the **View switcher** (the drop-down arrow next to the name of the view) to select other filtered views.</span></span> <span data-ttu-id="d0c38-116">Можете да създадете свои собствени изгледи с персонализирани критерии за филтриране.</span><span class="sxs-lookup"><span data-stu-id="d0c38-116">You can create your own views with custom filter criteria.</span></span>

<span data-ttu-id="d0c38-117">Договорите могат да се създават или изтриват от тази страница със списък или от страниците с подробности.</span><span class="sxs-lookup"><span data-stu-id="d0c38-117">Contracts can be created or deleted from this list page or detail pages.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]