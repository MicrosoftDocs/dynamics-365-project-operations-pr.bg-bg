---
title: Управление на оферти по проект
description: Тази тема предоставя информация за офертите по проекти.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 3c33adabbd03cca19ae5e7f401f08a716e9242b2
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177813"
---
# <a name="manage-project-quotes"></a><span data-ttu-id="4b957-103">Управление на оферти по проект</span><span class="sxs-lookup"><span data-stu-id="4b957-103">Manage project quotes</span></span>

<span data-ttu-id="4b957-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="4b957-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="4b957-105">В Dynamics 365 Project Operations офертите по проекти са създадени, за да помогнат за изграждането на предложения за работа по проекти.</span><span class="sxs-lookup"><span data-stu-id="4b957-105">In Dynamics 365 Project Operations, project quotes are designed to help build proposals for project work.</span></span> <span data-ttu-id="4b957-106">Структурата на оферта по проект в Project Operations е структурирана за предложения по проект със следните компоненти:</span><span class="sxs-lookup"><span data-stu-id="4b957-106">The structure of a project quote in Project Operations is structured for project proposals with the following components:</span></span>

  - <span data-ttu-id="4b957-107">Редове на оферта, които идентифицират отделните компоненти на работата, които ще се представят като компоненти от високо ниво.</span><span class="sxs-lookup"><span data-stu-id="4b957-107">Quote lines that identify the discrete components of work that will be presented as high-level components.</span></span>
  - <span data-ttu-id="4b957-108">Подробности за ред на оферта, които идентифицират и оценяват работата за всеки компонент от високо ниво или ред на оферта.</span><span class="sxs-lookup"><span data-stu-id="4b957-108">Quote line details that identify and estimate the work for each high-level component or quote line.</span></span> <span data-ttu-id="4b957-109">Графикът или прогнозите за дати и финансовите аспекти на работата са обвързани с този ред на оферта.</span><span class="sxs-lookup"><span data-stu-id="4b957-109">Schedule or date estimates and the financial aspects for the work are tied to that quote line.</span></span>
  - <span data-ttu-id="4b957-110">Моделите за договаряне и платимите компоненти са настроени за всеки ред на оферта.</span><span class="sxs-lookup"><span data-stu-id="4b957-110">Contracting models and chargeable components are set up for each quote line.</span></span> <span data-ttu-id="4b957-111">Тази настройка помага да се оцени разпределението на приходите, разходите и рентабилността за всеки ред на офертата и общата оферта.</span><span class="sxs-lookup"><span data-stu-id="4b957-111">This set up helps estimate the spread of revenue, spend, and profitability for each quote line and the overall quote.</span></span>

## <a name="view-all-project-based-quotes"></a><span data-ttu-id="4b957-112">Преглед на всички базирани на проект оферти</span><span class="sxs-lookup"><span data-stu-id="4b957-112">View all project-based quotes</span></span>

<span data-ttu-id="4b957-113">Списък с всички оферти по проект може да се прегледа от страницата със списъка **Оферти**.</span><span class="sxs-lookup"><span data-stu-id="4b957-113">A list of all the project quotes can be seen from the **Quotes** list page.</span></span> 

1. <span data-ttu-id="4b957-114">Отидете в **Продажби** > **Оферти**.</span><span class="sxs-lookup"><span data-stu-id="4b957-114">Go to **Sales** > **Quotes**.</span></span> <span data-ttu-id="4b957-115">Показва се списък с всички оферти по проект в системата.</span><span class="sxs-lookup"><span data-stu-id="4b957-115">A list of all your project quotes in the system are shown.</span></span> 
2. <span data-ttu-id="4b957-116">Използвайте **Превключвател на изгледи**, за да изберете други филтрирани изгледи на офертите.</span><span class="sxs-lookup"><span data-stu-id="4b957-116">Use the **View Switcher** to select other filtered views of the quotes.</span></span> <span data-ttu-id="4b957-117">Като използвате персонализирани критерии за филтриране, можете да конфигурирате свои собствени изгледи и опции за навигация.</span><span class="sxs-lookup"><span data-stu-id="4b957-117">Using custom filter criteria, you can configure your own views and navigation options.</span></span>

<span data-ttu-id="4b957-118">Оферти могат да се създават или изтриват от тази страница със списък или от страниците с подробности.</span><span class="sxs-lookup"><span data-stu-id="4b957-118">Quotes can be created or deleted from this list page or detail pages.</span></span>
