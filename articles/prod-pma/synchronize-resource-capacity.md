---
title: Синхронизиране на производителност на ресурс
description: Тази тема предоставя информация за това как да синхронизирате капацитета на ресурса в календари и проекти.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 8bde3c434680f0651293cbce13ecdce945c3a743
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997498"
---
# <a name="synchronize-resource-capacity"></a><span data-ttu-id="49b01-103">Синхронизиране на производителност на ресурс</span><span class="sxs-lookup"><span data-stu-id="49b01-103">Synchronize resource capacity</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="49b01-104">Процесите за синхронизиране на ресурси помагат да се гарантира, че информацията за календара и основния календар се влива в планирането на ресурсите на проекта.</span><span class="sxs-lookup"><span data-stu-id="49b01-104">The processes for resource synchronization help guarantee that information for the calendar and base calendar trickles down into project resource scheduling.</span></span> <span data-ttu-id="49b01-105">Ако календарът е променен, процесите правят необходимите актуализации на планирането на ресурсите на проекта.</span><span class="sxs-lookup"><span data-stu-id="49b01-105">If the calendar is changed, the processes make the required updates to the scheduling of project resources.</span></span> <span data-ttu-id="49b01-106">Процесите помагат и за подобряване на производителността, тъй като информацията за ресурсите на календара се синхронизира предварително.</span><span class="sxs-lookup"><span data-stu-id="49b01-106">The processes also help improve performance, because the calendar's resource information is synchronized in advance.</span></span> <span data-ttu-id="49b01-107">Следователно актуализациите на информацията за планиране на ресурси се извършват по-бързо.</span><span class="sxs-lookup"><span data-stu-id="49b01-107">Therefore, updates to resource scheduling information occur more quickly.</span></span> <span data-ttu-id="49b01-108">Препоръчваме ви да планирате процесите като пакет, вместо като един по един.</span><span class="sxs-lookup"><span data-stu-id="49b01-108">We recommend that you schedule the processes as a batch instead of one at a time.</span></span> <span data-ttu-id="49b01-109">В противен случай съществува риск някой да забрави включените дати, когато информацията е била синхронизирана за последен път.</span><span class="sxs-lookup"><span data-stu-id="49b01-109">Otherwise, there is a risk that someone will forget the inclusive dates when the information was last synchronized.</span></span> <span data-ttu-id="49b01-110">Ако не се използват включени дати, могат да възникнат пропуски по време на синхронизирането на датите.</span><span class="sxs-lookup"><span data-stu-id="49b01-110">If inclusive dates aren't used, gaps can occur during date synchronization.</span></span>

![Синхронизация на календар](./media/projectresourcing04-1024x471.jpg)

## <a name="synchronize-resource-capacity-roll-ups"></a><span data-ttu-id="49b01-112">Синхронизация на сборове на капацитет на ресурс</span><span class="sxs-lookup"><span data-stu-id="49b01-112">Synchronize resource capacity roll-ups</span></span>

<span data-ttu-id="49b01-113">Процесът на синхронизация е предназначен да синхронизира цялата информация за календара на ресурсите.</span><span class="sxs-lookup"><span data-stu-id="49b01-113">The synchronization process is designed to synchronize all resource calendar information.</span></span> <span data-ttu-id="49b01-114">Тази информация включва основна информация за календара за всякакви промени в таблицата за капацитет на ресурсите на проекта.</span><span class="sxs-lookup"><span data-stu-id="49b01-114">This information includes base calendar information about any changes to the project's Resource calendar capacity table.</span></span> <span data-ttu-id="49b01-115">Ако в проекта се добавят нови ресурси, синхронизацията помага да се гарантира, че актуализираната информация за календара е налична.</span><span class="sxs-lookup"><span data-stu-id="49b01-115">If new resources are added in the project, synchronization helps guarantee that the updated calendar information is available.</span></span> <span data-ttu-id="49b01-116">Тази синхронизация може да се направи по всяко време.</span><span class="sxs-lookup"><span data-stu-id="49b01-116">This synchronization can be done at any time.</span></span>

<span data-ttu-id="49b01-117">Ние препоръчваме да използвате партида.</span><span class="sxs-lookup"><span data-stu-id="49b01-117">We recommend that you use a batch.</span></span> <span data-ttu-id="49b01-118">Опциите са налични по време на синхронизиране на резервации за капацитет.</span><span class="sxs-lookup"><span data-stu-id="49b01-118">The options are available during synchronization of capacity reservations.</span></span>

1. <span data-ttu-id="49b01-119">Изберете **Управление на проекти и счетоводство** &gt; **Периодични** &gt; **Синхронизация на капацитета** &gt; **Синхронизирайте обобщените капацитети на ресурсите**.</span><span class="sxs-lookup"><span data-stu-id="49b01-119">Select **Project management and accounting** &gt; **Periodic** &gt; **Capacity synchronization** &gt; **Synchronize resources capacity roll-ups**.</span></span>
2. <span data-ttu-id="49b01-120">Задайте опциите в следната таблица.</span><span class="sxs-lookup"><span data-stu-id="49b01-120">Set the options in the following table.</span></span>

    | <span data-ttu-id="49b01-121">Опция</span><span class="sxs-lookup"><span data-stu-id="49b01-121">Option</span></span>      | <span data-ttu-id="49b01-122">Описание</span><span class="sxs-lookup"><span data-stu-id="49b01-122">Description</span></span> |
    |-------------|-------------|
    | <span data-ttu-id="49b01-123">Код на периода</span><span class="sxs-lookup"><span data-stu-id="49b01-123">Period code</span></span> | <span data-ttu-id="49b01-124">По желание изберете кода на интервала за дата на главната книга, за да зададете началната и крайната дата за процеса на синхронизиране за събиране на капацитета на ресурсите.</span><span class="sxs-lookup"><span data-stu-id="49b01-124">Optionally select the General ledger date interval code to set the start and end dates for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="49b01-125">Начална дата</span><span class="sxs-lookup"><span data-stu-id="49b01-125">Start date</span></span>  | <span data-ttu-id="49b01-126">Въведете началната дата за процеса на синхронизиране за събирания на капацитета на ресурсите.</span><span class="sxs-lookup"><span data-stu-id="49b01-126">Enter the start date for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="49b01-127">Крайна дата</span><span class="sxs-lookup"><span data-stu-id="49b01-127">End date</span></span>    | <span data-ttu-id="49b01-128">Въведете крайна дата за процеса на синхронизиране за събирания на капацитета на ресурсите.</span><span class="sxs-lookup"><span data-stu-id="49b01-128">Enter the end date for the synchronization process for resource capacity roll-ups.</span></span> |

<span data-ttu-id="49b01-129">[![Процес на синхронизация](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span><span class="sxs-lookup"><span data-stu-id="49b01-129">[![Synchronization process](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]