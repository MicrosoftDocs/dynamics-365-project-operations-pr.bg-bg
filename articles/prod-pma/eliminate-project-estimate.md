---
title: Премахване на оценка на проект
description: Тази тема предоставя информация за премахване на прогнозна оценка на проекта, след като тя е завършена.
author: Yowelle
manager: AnnBe
ms.date: 05/26/2020
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
ms.openlocfilehash: 8bda8a7357e883b948449b2a19bea476996dde3c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071873"
---
# <a name="eliminate-a-project-estimate"></a><span data-ttu-id="b5678-103">Премахване на оценка на проект</span><span class="sxs-lookup"><span data-stu-id="b5678-103">Eliminate a project estimate</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="b5678-104">Прогнозните оценки за проект предоставят финансов поглед за прогнозната и планираната работа за проекта.</span><span class="sxs-lookup"><span data-stu-id="b5678-104">Project estimates provide the financial view for work that is estimated and scheduled for a project.</span></span> <span data-ttu-id="b5678-105">За да работите с разчети за даден проект, трябва да прикачите проекта към разчетен проект.</span><span class="sxs-lookup"><span data-stu-id="b5678-105">To work with estimates for a project, you must attach the project to an estimate project.</span></span> <span data-ttu-id="b5678-106">Приблизителният проект винаги се основава на съществуващ проект, но множество проекти могат да се отнасят до един проект за оценка.</span><span class="sxs-lookup"><span data-stu-id="b5678-106">An estimate project is always based on an existing project, however multiple projects can refer to a single estimate project.</span></span> <span data-ttu-id="b5678-107">Към прогнозни проекти могат да се прикачат само проекти с фиксирана цена и инвестиционни проекти и тези проекти трябва да принадлежат към същата проектна група като прогнозния проект.</span><span class="sxs-lookup"><span data-stu-id="b5678-107">Only fixed-price and investment projects can be attached to estimate projects, and those projects must belong to the same project group as the estimate project.</span></span>

<span data-ttu-id="b5678-108">За да се елиминира проект за оценка, той трябва да бъде завършен.</span><span class="sxs-lookup"><span data-stu-id="b5678-108">To eliminate an estimate project, it must be complete.</span></span> <span data-ttu-id="b5678-109">Следващите стъпки обясняват как да премахнете приблизителна оценка.</span><span class="sxs-lookup"><span data-stu-id="b5678-109">The following steps explain how to eliminate an estimate.</span></span>

1. <span data-ttu-id="b5678-110">Отидете на **Управление на проекти и счетоводство** > **Всички проекти** и отворете проекта.</span><span class="sxs-lookup"><span data-stu-id="b5678-110">Go to **Project management and accounting** > **All Projects** and open the project.</span></span> 
2. <span data-ttu-id="b5678-111">На раздела **Управление** изберете **Оценки** и на **Оценете** страница изберете **Елиминиране**.</span><span class="sxs-lookup"><span data-stu-id="b5678-111">On the **Manage** tab, select **Estimates** , and on the **Estimate** page select **Eliminate**.</span></span>
3. <span data-ttu-id="b5678-112">На **Премахване на прогнозата** страницата на раздела **Общи** задайте следните опции:</span><span class="sxs-lookup"><span data-stu-id="b5678-112">On the **Eliminate estimate** page on the **General** tab, set the following options:</span></span>

   - <span data-ttu-id="b5678-113">**Код на периода** : Изберете кода на периода, за да изберете подходящите прогнозни проекти.</span><span class="sxs-lookup"><span data-stu-id="b5678-113">**Period code** : Select the period code to choose the appropriate estimate projects.</span></span> 
   - <span data-ttu-id="b5678-114">**Приблизителна дата** : Изберете подходящата прогнозна дата за елиминиране.</span><span class="sxs-lookup"><span data-stu-id="b5678-114">**Estimate date** : Select the appropriate estimate date for elimination.</span></span>
   - <span data-ttu-id="b5678-115">**Елиминирайте с WIP предупреждения** : Активирайте тази опция, за да предоставите известие, когато прогноза, свързана с незавършено производство (WIP), ще бъде премахната.</span><span class="sxs-lookup"><span data-stu-id="b5678-115">**Eliminate with WIP warnings** : Enable this option to provide notification when an estimate that is associated with a work in progress (WIP) will be eliminated.</span></span> <span data-ttu-id="b5678-116">Когато тази опция не е активирана, елиминирането не може да продължи, ако съществуват непрогнозни транзакции.</span><span class="sxs-lookup"><span data-stu-id="b5678-116">When this option is not enabled, elimination can’t continue if any non-estimated transactions exist.</span></span> 
   > [!NOTE]
   > <span data-ttu-id="b5678-117">Тази опция е налична само когато елиминирането се прилага към проект за оценка.</span><span class="sxs-lookup"><span data-stu-id="b5678-117">This option is available only when elimination is applied to an estimate project.</span></span> <span data-ttu-id="b5678-118">Не е налично, ако използвате периодични публикации.</span><span class="sxs-lookup"><span data-stu-id="b5678-118">It is not available if you are using periodic postings.</span></span> <span data-ttu-id="b5678-119">Тази настройка работи с настройките на **Оценете** в раздела **Параметри на проекта** страница в **Позволява елиминиране, когато съществуват непрогнозни транзакции** полева група.</span><span class="sxs-lookup"><span data-stu-id="b5678-119">This setting works with the settings on the **Estimate** tab on the **Project parameters** page, in the **Allow elimination when non-estimated transactions exist** field group.</span></span>
   - <span data-ttu-id="b5678-120">**Задайте етап на Готово** : Активирайте тази опция, за да зададете етапа на прогнозния проект на **Готово** след като стартирате елиминацията.</span><span class="sxs-lookup"><span data-stu-id="b5678-120">**Set stage to Finished** : Enable this option to set the estimate project’s stage to **Finished** after you run the elimination.</span></span>
   - <span data-ttu-id="b5678-121">**Отпечатайте списък с прогнози** : Изберете информацията, която да бъде включена при отпечатване на списъка с прогнози.</span><span class="sxs-lookup"><span data-stu-id="b5678-121">**Print estimate list** : Select the information to be included when the estimate list is printed.</span></span>
   - <span data-ttu-id="b5678-122">**Покажи Infolog** : Активирайте тази опция, за да се покаже Infolog.</span><span class="sxs-lookup"><span data-stu-id="b5678-122">**Show Infolog** : Enable this option to display the Infolog.</span></span>
   - <span data-ttu-id="b5678-123">**Дата на изпращане** : Изберете датата на осчетоводяване на регистъра на прогнозата.</span><span class="sxs-lookup"><span data-stu-id="b5678-123">**Posting date** : Choose the ledger posting date of the estimate.</span></span>

4.  <span data-ttu-id="b5678-124">Изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="b5678-124">Select **OK**.</span></span>
5. <span data-ttu-id="b5678-125">След завършване на процеса на елиминиране, проектът за елиминирана оценка се показва с отрицателна стойност.</span><span class="sxs-lookup"><span data-stu-id="b5678-125">After the elimination process is complete, the eliminated estimate project is displayed with a negative value.</span></span> 

<span data-ttu-id="b5678-126">Ако не сте възнамерявали да премахнете прогноза, можете да изберете елиминираната оценка и да изберете **Обратно елиминиране**.</span><span class="sxs-lookup"><span data-stu-id="b5678-126">If you did not intend to eliminate an estimate, you can select the eliminated estimate and select **Reverse elimination**.</span></span>   
