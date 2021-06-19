---
title: Типове периоди
description: Тази тема предоставя информация за начина на задаване на типове периоди за оценка на приход.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 07cc9cde5fab10accb1fd6efede58926918f614c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013473"
---
# <a name="period-types"></a><span data-ttu-id="d5ad5-103">Типове периоди</span><span class="sxs-lookup"><span data-stu-id="d5ad5-103">Period types</span></span>

<span data-ttu-id="d5ad5-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="d5ad5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="d5ad5-105">Типът на периода определя колко често се изчисляват приходите от даден проект.</span><span class="sxs-lookup"><span data-stu-id="d5ad5-105">A period type defines how frequently revenue on a project is estimated.</span></span> <span data-ttu-id="d5ad5-106">Тази тема предоставя информация за начина на задаване на типове периоди за оценка на приход.</span><span class="sxs-lookup"><span data-stu-id="d5ad5-106">This topic provides information about how to set up period types for revenue estimation.</span></span> 

## <a name="create-and-work-with-period-types"></a><span data-ttu-id="d5ad5-107">Създаване и работа с типове периоди</span><span class="sxs-lookup"><span data-stu-id="d5ad5-107">Create and work with period types</span></span>
<span data-ttu-id="d5ad5-108">За да създавате и работите с типове периоди, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="d5ad5-108">To create and work with period types, complete the following steps:</span></span>

1. <span data-ttu-id="d5ad5-109">В средата на Dynamics 365 Finance отидете на **Управление на проекти и счетоводство** > **Настройка** > **Оценки** > **Типове периоди**.</span><span class="sxs-lookup"><span data-stu-id="d5ad5-109">In your Dynamics 365 Finance environment, go to **Project management and accounting** > **Setup** > **Estimates** > **Period types**.</span></span>
2. <span data-ttu-id="d5ad5-110">Изберете **Нов**, за да създадете нов тип период.</span><span class="sxs-lookup"><span data-stu-id="d5ad5-110">Select **New** to create new period type.</span></span> <span data-ttu-id="d5ad5-111">Въведете име и описание.</span><span class="sxs-lookup"><span data-stu-id="d5ad5-111">Enter a name and description.</span></span>
3. <span data-ttu-id="d5ad5-112">В полето **Честота** задайте стойност:</span><span class="sxs-lookup"><span data-stu-id="d5ad5-112">In the **Frequency** field, select a value:</span></span>

    - <span data-ttu-id="d5ad5-113">Ако изберете **Седмично**, **На две седмици**, **Два пъти месечно**, **Месечно**, **На ден**, **На тримесечие** или **Годишно**, календарът ще се използва за генериране на периоди.</span><span class="sxs-lookup"><span data-stu-id="d5ad5-113">If you select **Week**, **Bi-weekly**, **Semi-monthly**, **Month**, **Day**, **Quarter**, or **Year**, the calendar will be used to generate the periods.</span></span> 
    - <span data-ttu-id="d5ad5-114">Ако изберете **Период на книга**, периодите на главната книга от конфигурацията на главната книга ще се използват за генериране на периоди.</span><span class="sxs-lookup"><span data-stu-id="d5ad5-114">If you select **Ledger period**, ledger periods from the General ledger configuration will be used to generate periods.</span></span>
    - <span data-ttu-id="d5ad5-115">Ако изберете **Неограничено**, можете да посочите персонализирани периоди.</span><span class="sxs-lookup"><span data-stu-id="d5ad5-115">If you select **Unlimited**, you can specify custom periods.</span></span>
4. <span data-ttu-id="d5ad5-116">Изберете запис от тип период и след това изберете **Генериране на периоди**, за да създадете периоди за типа период.</span><span class="sxs-lookup"><span data-stu-id="d5ad5-116">Select the period type record and then select **Generate periods** to create periods for the period type.</span></span> <span data-ttu-id="d5ad5-117">Въз основа на избраната от вас честота на периода може да имате възможност да посочите начална дата или броя на периодите, които да генерирате.</span><span class="sxs-lookup"><span data-stu-id="d5ad5-117">Based on the period frequency that you selected, you might have the option to specify a start date or the number of periods to generate.</span></span>
5. <span data-ttu-id="d5ad5-118">Изберете **Периоди** за преглед на генерираните периоди.</span><span class="sxs-lookup"><span data-stu-id="d5ad5-118">Select **Periods** to review generated periods.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]