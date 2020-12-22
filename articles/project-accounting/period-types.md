---
title: Типове периоди
description: Тази тема предоставя информация за начина на задаване на типове периоди за оценка на приход.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6bcd988fbd074c66d64f7e327b4329d3de27e950
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531359"
---
# <a name="period-types"></a><span data-ttu-id="c4455-103">Типове периоди</span><span class="sxs-lookup"><span data-stu-id="c4455-103">Period types</span></span>

<span data-ttu-id="c4455-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="c4455-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="c4455-105">Типът на периода определя колко често се изчисляват приходите от даден проект.</span><span class="sxs-lookup"><span data-stu-id="c4455-105">A period type defines how frequently revenue on a project is estimated.</span></span> <span data-ttu-id="c4455-106">Тази тема предоставя информация за начина на задаване на типове периоди за оценка на приход.</span><span class="sxs-lookup"><span data-stu-id="c4455-106">This topic provides information about how to set up period types for revenue estimation.</span></span> 

## <a name="create-and-work-with-period-types"></a><span data-ttu-id="c4455-107">Създаване и работа с типове периоди</span><span class="sxs-lookup"><span data-stu-id="c4455-107">Create and work with period types</span></span>
<span data-ttu-id="c4455-108">За да създавате и работите с типове периоди, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="c4455-108">To create and work with period types, complete the following steps:</span></span>

1. <span data-ttu-id="c4455-109">В средата на Dynamics 365 Finance отидете на **Управление на проекти и счетоводство** > **Настройка** > **Оценки** > **Типове периоди**.</span><span class="sxs-lookup"><span data-stu-id="c4455-109">In your Dynamics 365 Finance environment, go to **Project management and accounting** > **Setup** > **Estimates** > **Period types**.</span></span>
2. <span data-ttu-id="c4455-110">Изберете **Нов**, за да създадете нов тип период.</span><span class="sxs-lookup"><span data-stu-id="c4455-110">Select **New** to create new period type.</span></span> <span data-ttu-id="c4455-111">Въведете име и описание.</span><span class="sxs-lookup"><span data-stu-id="c4455-111">Enter a name and description.</span></span>
3. <span data-ttu-id="c4455-112">В полето **Честота** задайте стойност:</span><span class="sxs-lookup"><span data-stu-id="c4455-112">In the **Frequency** field, select a value:</span></span>

    - <span data-ttu-id="c4455-113">Ако изберете **Седмично**, **На две седмици**, **Два пъти месечно**, **Месечно**, **На ден**, **На тримесечие** или **Годишно**, календарът ще се използва за генериране на периоди.</span><span class="sxs-lookup"><span data-stu-id="c4455-113">If you select **Week**, **Bi-weekly**, **Semi-monthly**, **Month**, **Day**, **Quarter**, or **Year**, the calendar will be used to generate the periods.</span></span> 
    - <span data-ttu-id="c4455-114">Ако изберете **Период на книга**, периодите на главната книга от конфигурацията на главната книга ще се използват за генериране на периоди.</span><span class="sxs-lookup"><span data-stu-id="c4455-114">If you select **Ledger period**, ledger periods from the General ledger configuration will be used to generate periods.</span></span>
    - <span data-ttu-id="c4455-115">Ако изберете **Неограничено**, можете да посочите персонализирани периоди.</span><span class="sxs-lookup"><span data-stu-id="c4455-115">If you select **Unlimited**, you can specify custom periods.</span></span>
4. <span data-ttu-id="c4455-116">Изберете запис от тип период и след това изберете **Генериране на периоди**, за да създадете периоди за типа период.</span><span class="sxs-lookup"><span data-stu-id="c4455-116">Select the period type record and then select **Generate periods** to create periods for the period type.</span></span> <span data-ttu-id="c4455-117">Въз основа на избраната от вас честота на периода може да имате възможност да посочите начална дата или броя на периодите, които да генерирате.</span><span class="sxs-lookup"><span data-stu-id="c4455-117">Based on the period frequency that you selected, you might have the option to specify a start date or the number of periods to generate.</span></span>
5. <span data-ttu-id="c4455-118">Изберете **Периоди** за преглед на генерираните периоди.</span><span class="sxs-lookup"><span data-stu-id="c4455-118">Select **Periods** to review generated periods.</span></span>

