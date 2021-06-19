---
title: Набори от одобрения
description: Тази тема предоставя информация за набора от одобрения, заявките и поднаборите на тези операции.
author: stsporen
manager: tfehr
ms.date: 05/28/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: ac73313420029ece740d0bdb9c21c7abaa9defc6
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116858"
---
# <a name="approval-sets"></a><span data-ttu-id="3f171-103">Набори от одобрения</span><span class="sxs-lookup"><span data-stu-id="3f171-103">Approval sets</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="3f171-104">Наборът от одобрения групира заявките за одобрение заедно в по-малки поднабори от операции.</span><span class="sxs-lookup"><span data-stu-id="3f171-104">Approval sets group approval requests together into smaller subsets of operations.</span></span> <span data-ttu-id="3f171-105">Това групиране позволява обработката на одобренията по ред на проекта и позволява повторен опит и последователност.</span><span class="sxs-lookup"><span data-stu-id="3f171-105">This grouping allows approvals to be processed in order by Project and allows for retrying and sequencing.</span></span> <span data-ttu-id="3f171-106">Групирането подобрява надеждността и проследимостта на обработката на одобрения за големи обеми одобрения.</span><span class="sxs-lookup"><span data-stu-id="3f171-106">Grouping improves the reliability and traceability of approval processing for large volumes of approvals.</span></span>

<span data-ttu-id="3f171-107">Наборите от одобрения показват цялостното състояние на обработка на свързаните записи.</span><span class="sxs-lookup"><span data-stu-id="3f171-107">Approval sets indicate the overall processing state of their related records.</span></span> <span data-ttu-id="3f171-108">Когато запис за одобрение се обработва с помощта на набор от одобрения, записът се премества от **Подадени** в **Одобрени** и се премахва връзката с набора от одобрения.</span><span class="sxs-lookup"><span data-stu-id="3f171-108">When an approval record is processed using an approval set, the record moves from **Submitted** to **Approved**, and is unlinked from the approval set.</span></span> <span data-ttu-id="3f171-109">Ако подаването на записа за одобрение е неуспешно, той остава в състояние **Подаден** и наборът от одобрения се маркира като неуспешен.</span><span class="sxs-lookup"><span data-stu-id="3f171-109">If a record fails when it is submitted for approval, the record remains in a status of **Submitted** and the approval set is marked as failed.</span></span> <span data-ttu-id="3f171-110">Наборът от одобрения регистрира съобщението за грешка за неуспеха.</span><span class="sxs-lookup"><span data-stu-id="3f171-110">The approval set logs the error message of the failure.</span></span>

## <a name="processing-approvals-and-approval-sets"></a><span data-ttu-id="3f171-111">Обработка на одобрения и набори от одобрения</span><span class="sxs-lookup"><span data-stu-id="3f171-111">Processing approvals and approval sets</span></span>
<span data-ttu-id="3f171-112">Одобренията, които са в опашка за обработка, са видими в изгледа **Обработка на одобрения**.</span><span class="sxs-lookup"><span data-stu-id="3f171-112">Approvals that are queued for processing are visible in the **Processing Approvals** view.</span></span> <span data-ttu-id="3f171-113">Системата се опитва да обработва всички записи многократно асинхронно, включително повторни опити за одобрение, ако предишните опити са неуспешни.</span><span class="sxs-lookup"><span data-stu-id="3f171-113">The system tries to process all the entries multiple times asynchronously, including retrying an approval if previous attempts failed.</span></span>

<span data-ttu-id="3f171-114">Полето **Жизнен цикъл на набор от одобрения** записва броя на останалите опити за обработка на набора, преди той да бъде маркиран като неуспешен.</span><span class="sxs-lookup"><span data-stu-id="3f171-114">The **Approval Set Lifetime** field records the number of attempts left to process the set before it's marked as failed.</span></span>

## <a name="failed-approvals-and-approval-sets"></a><span data-ttu-id="3f171-115">Неуспешни одобрения и набори от одобрения</span><span class="sxs-lookup"><span data-stu-id="3f171-115">Failed approvals and approval sets</span></span>
<span data-ttu-id="3f171-116">Изгледът **Неуспешни одобрения** изброява всички одобрения, които изискват намеса на потребителя.</span><span class="sxs-lookup"><span data-stu-id="3f171-116">The **Failed Approvals** view lists all approvals that require user intervention.</span></span> <span data-ttu-id="3f171-117">Отворете свързаните регистрационни файлове на набора от одобрения, за да идентифицирате причината за неуспеха.</span><span class="sxs-lookup"><span data-stu-id="3f171-117">Open the associated approval set logs to identify the cause of the failure.</span></span>
<span data-ttu-id="3f171-118">Избирането на **Повторен опит** добавя към изчислението на жизнения цикъл на набора от одобрения, премества набора от одобрения обратно в състояние на **Обработка** и се опитва да обработи останалите записи.</span><span class="sxs-lookup"><span data-stu-id="3f171-118">Selecting **Retry** adds to the approval set lifetime count, moves the approval set back to a status of **Processing**, and attempts to process the remaining records.</span></span>

## <a name="configure-approval-sets"></a><span data-ttu-id="3f171-119">Конфигуриране на набори от одобрения</span><span class="sxs-lookup"><span data-stu-id="3f171-119">Configure approval sets</span></span>

###  <a name="enable-the-approval-sets-feature"></a><span data-ttu-id="3f171-120">Активиране на функцията за набори от одобрения</span><span class="sxs-lookup"><span data-stu-id="3f171-120">Enable the Approval sets feature</span></span>
<span data-ttu-id="3f171-121">Преди да активирате функцията за набори от одобрения, проверете дали в момента няма обработвани одобрения.</span><span class="sxs-lookup"><span data-stu-id="3f171-121">Before you enable the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="3f171-122">Отидете на страницата **Параметри на проект** и изберете **Контрол на функцията** > **Активиране на съвременни одобрения**.</span><span class="sxs-lookup"><span data-stu-id="3f171-122">Go to the **Project parameters** page and select **Feature Control** > **Enable Modern Approvals**.</span></span>

### <a name="turn-off-the-approval-sets-feature"></a><span data-ttu-id="3f171-123">Изключване на функцията за набори от одобрения</span><span class="sxs-lookup"><span data-stu-id="3f171-123">Turn off the Approval sets feature</span></span>
<span data-ttu-id="3f171-124">Преди да изключите функцията за набори от одобрения, проверете дали в момента няма обработвани одобрения.</span><span class="sxs-lookup"><span data-stu-id="3f171-124">Before you turn off the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="3f171-125">Отидете на страницата **Параметри на проект** и изберете **Контрол на функцията** > **Дезактивиране на съвременни одобрения**.</span><span class="sxs-lookup"><span data-stu-id="3f171-125">Go to the **Project Parameters** page and select **Feature Control** > **Disable Modern Approvals**.</span></span>

### <a name="configuring-the-asynchronous-threshold"></a><span data-ttu-id="3f171-126">Конфигуриране на асинхронния праг</span><span class="sxs-lookup"><span data-stu-id="3f171-126">Configuring the asynchronous threshold</span></span> 
<span data-ttu-id="3f171-127">При създаване на набори от одобрения обработката се премества във фонов режим, когато избраният брой записи за одобрение надвишава посочения праг.</span><span class="sxs-lookup"><span data-stu-id="3f171-127">When approval sets are created, processing moves to the background when the selected number of records for approval exceeds the indicated threshold.</span></span> <span data-ttu-id="3f171-128">Използвайте полето **Асинхронен праг** за конфигуриране кога обработката на одобрение трябва да се изпълнява синхронно или асинхронно.</span><span class="sxs-lookup"><span data-stu-id="3f171-128">Use the **Asynchronous Threshold** field to configure when approval processing should be run synchronously or asynchronously.</span></span>
<span data-ttu-id="3f171-129">Валидните стойности са:</span><span class="sxs-lookup"><span data-stu-id="3f171-129">Valid values are:</span></span>

  - <span data-ttu-id="3f171-130">Нула: Всички заявки трябва да се обработват асинхронно.</span><span class="sxs-lookup"><span data-stu-id="3f171-130">Zero: All requests should be processed asynchronously.</span></span> 
  - <span data-ttu-id="3f171-131">Числа, по-големи от нула: Одобренията се обработват асинхронно само когато подаденият брой одобрения надвишава тази стойност.</span><span class="sxs-lookup"><span data-stu-id="3f171-131">Numbers greater than zero: Approvals are processed asynchronously only when the submitted number of approvals exceeds this value.</span></span>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
