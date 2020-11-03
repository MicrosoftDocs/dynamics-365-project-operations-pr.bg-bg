---
title: Създаване на модели на прогноза за бюджети на проекти
description: Тази тема описва как да създадете прогнозен модел за оставащите бюджети.
author: Yowelle
manager: AnnBe
ms.date: 04/24/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 32a436d240f5535ff15f8bc3b8ba9be2d1d4da17
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071956"
---
# <a name="create-forecast-models-for-project-budgets"></a><span data-ttu-id="c7d7e-103">Създаване на модели на прогноза за бюджети на проекти</span><span class="sxs-lookup"><span data-stu-id="c7d7e-103">Create forecast models for project budgets</span></span> 

[!include [banner](../includes/banner.md)]

<span data-ttu-id="c7d7e-104">Тази тема описва как да създадете прогнозен модел за оставащите бюджети.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-104">This topic describes how to create a forecast model for remaining budgets.</span></span> <span data-ttu-id="c7d7e-105">Проект, който е обект на бюджетен контрол, използва два вида бюджети: оригинален и оставащ.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-105">A project that is subject to budget control uses two types of budgets: original and remaining.</span></span> <span data-ttu-id="c7d7e-106">Когато създавате бюджет на проект, трябва да посочите оригиналните и останалите модели за прогнозиране на бюджета, които са създадени на страницата **Прогнозни модели**.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-106">When you create a project budget, you must specify the original and remaining budget forecast models that were created in the **Forecast models** page.</span></span> <span data-ttu-id="c7d7e-107">Бюджетите на проекти въз основа на посочените модели се създават, когато ангажирате бюджета на проекта.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-107">Project budgets based on the specified models are created when you commit the project budget.</span></span>

> [!NOTE]
> <span data-ttu-id="c7d7e-108">Прогнозен модел, който се използва за контрол на бюджета, не може да има подмодел или да се използва като подмодел.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-108">A forecast model that is used for budget control can’t have a submodel or be used as a submodel.</span></span>

1. <span data-ttu-id="c7d7e-109">Изберете **Управление на проекти и счетоводство** > **Настройвам** > **Прогнози**  > **Прогнозни модели**.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-109">Select **Project management and accounting** > **Setup** > **Forecasts**  > **Forecast models**.</span></span>
2. <span data-ttu-id="c7d7e-110">Изберете **Създаване** , за да създадете нов прогнозен модел и след това въведете идентификационен номер на модела и име за новия модел.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-110">Select **New** to create a new forecast model, and then enter a model ID number and name for the new model.</span></span> 
3. <span data-ttu-id="c7d7e-111">Задайте опцията **Спряна** на **Да** за предотвратяване на промени в прогнозните редове за прогнозния модел.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-111">Set the **Stopped** option to **Yes** to prevent any changes to the forecast lines for the forecast model.</span></span> 
4. <span data-ttu-id="c7d7e-112">Ако прогнозните редове, с които е свързан моделът, трябва да генерират прогнози за паричния поток в главната книга, задайте **Включете в прогнозите за паричния поток** на **Да.**</span><span class="sxs-lookup"><span data-stu-id="c7d7e-112">If the forecast lines that the model is associated with should generate cash flow forecasts in the general ledger, set **Include in Cash flow forecasts** to **Yes.**</span></span> 
5. <span data-ttu-id="c7d7e-113">За да използвате датата на проекта като дата на фактурата, задайте **Дата на фактура за прогноза** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-113">To use the project date as the invoice date, set **Forecast Invoice date** to **Yes**.</span></span> 
6. <span data-ttu-id="c7d7e-114">В полето **Тип бюджет** изберете един от следните типове модели:</span><span class="sxs-lookup"><span data-stu-id="c7d7e-114">In the **Budget type** field, select one of the following model types:</span></span>

   - <span data-ttu-id="c7d7e-115">**Първоначален бюджет** : Използвайте първоначалните бюджетни суми, които са поети, когато първоначалният бюджет е създаден и одобрен.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-115">**Original budget** : Use the original budget amounts that are committed when the initial budget is created and approved.</span></span>
   - <span data-ttu-id="c7d7e-116">**Оставащ бюджет** : Използвайте останалите бюджетни суми през целия живот на проекта.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-116">**Remaining budget** : Use the remaining budget amounts during the life of the project.</span></span> <span data-ttu-id="c7d7e-117">Салдата в този прогнозен модел се намаляват от реални транзакции и се увеличават или намаляват от ревизии на бюджета.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-117">The balances in this forecast model are reduced by actual transactions and increased or decreased by budget revisions.</span></span>
   - <span data-ttu-id="c7d7e-118">**Пренасяне напред** : Използвайте пренесените бюджетни суми за проекта.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-118">**Carry-forward** : Use the carry-forward budget amounts for the project.</span></span> <span data-ttu-id="c7d7e-119">Пренасочването е незадължителен процес, който може да се стартира за прехвърляне на неизползвани бюджетни суми от един финансова година в друг.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-119">Carry-forward is an optional process that can be run to transfer unused budget amounts from one fiscal year to another.</span></span>

7. <span data-ttu-id="c7d7e-120">Задайте следните опции, както е нужно:</span><span class="sxs-lookup"><span data-stu-id="c7d7e-120">Set the following options as required:</span></span>

   - <span data-ttu-id="c7d7e-121">Активирайте **Дата на фактура на прогноза** , за да използвате датата на проекта като дата на фактурата.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-121">Enable **Forecast invoice date** to use the project date as the invoice date.</span></span>
   - <span data-ttu-id="c7d7e-122">Активиране на **Прогноза с WIP** за прогнозиране въз основа на незавършено производство (WIP) и след това изберете вида на WIP.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-122">Enable **Forecast with WIP** to forecast based on work in progress (WIP), and then select the type of WIP.</span></span> 
   - <span data-ttu-id="c7d7e-123">Можете да запазите подразбирания **Тип бюджет** като **Няма** или въведете нов тип.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-123">You can keep the default **Budget type** as **None** or enter a new type.</span></span> <span data-ttu-id="c7d7e-124">Типът на бюджета не може да бъде променен, след като промените запис.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-124">The budget type can't be changed after you change a record.</span></span>     
    > [!NOTE]
    > <span data-ttu-id="c7d7e-125">Ако промените типа бюджет по подразбиране, всички други опции ще станат недостъпни за актуализации и не можете да използвате повторно този модел на прогноза.</span><span class="sxs-lookup"><span data-stu-id="c7d7e-125">If you change the default budget type, all other options will become unavailable for updates, and you can't reuse this forecast model.</span></span> 
   


 

