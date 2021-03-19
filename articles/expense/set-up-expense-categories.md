---
title: Настройване на категории разходи
description: Тази тема предоставя информация за това как да настроите категории разходи и споделени категории за отчети за разходите.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 1589cf82626e744d35f31fef8e8437a5ad71360d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276110"
---
# <a name="set-up-expense-categories"></a><span data-ttu-id="3ea6b-103">Настройване на категории разходи</span><span class="sxs-lookup"><span data-stu-id="3ea6b-103">Set up expense categories</span></span>

<span data-ttu-id="3ea6b-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="3ea6b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="3ea6b-105">Когато служителите създават отчети за разходите, всеки разход, който записват, трябва да бъде свързан с категория разходи.</span><span class="sxs-lookup"><span data-stu-id="3ea6b-105">When employees create expense reports, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="3ea6b-106">Категориите на разходите се извличат от споделени категории, които могат да се споделят между юридическите лица във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="3ea6b-106">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="3ea6b-107">В зависимост от начина, по който е дефинирана вашата организация, тези категории разходи могат да се споделят и в други области.</span><span class="sxs-lookup"><span data-stu-id="3ea6b-107">Depending on how your organization is defined, these expense categories can also be shared in other areas.</span></span> <span data-ttu-id="3ea6b-108">Въз основа на дефиницията на вашата организация и насоки от екипа за внедряване, трябва да определите дали категориите, които се използват в управлението на разходите, ще се използват само в управлението на разходите или трябва да се споделят в други области.</span><span class="sxs-lookup"><span data-stu-id="3ea6b-108">Based on the definition of your organization and guidance from the implementation team, you must determine whether the categories that are used in Expense management will be used only in Expense management or should be shared in other areas.</span></span>

> [!NOTE]
> <span data-ttu-id="3ea6b-109">Тези категории могат да се споделят между управление на проекти и счетоводство и управление на разходите, или между управление на проекти и счетоводство и производство.</span><span class="sxs-lookup"><span data-stu-id="3ea6b-109">These categories can be shared between Project management and accounting and Expense management, or between Project management and accounting and Production.</span></span> <span data-ttu-id="3ea6b-110">Те обаче не могат да се споделят между управлението на разходите и производството.</span><span class="sxs-lookup"><span data-stu-id="3ea6b-110">However, they can't be shared between Expense management and Production.</span></span>

<span data-ttu-id="3ea6b-111">Преди да започнете процеса на настройка, трябва да се вземат следните решения за всяка категория разходи:</span><span class="sxs-lookup"><span data-stu-id="3ea6b-111">Before you can begin the setup process, the following decisions must be made for each expense category:</span></span>

- <span data-ttu-id="3ea6b-112">Каква е категорията на разхода?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-112">What is the expense category?</span></span> <span data-ttu-id="3ea6b-113">Примерите включват категории за полети, хотел или пробег.</span><span class="sxs-lookup"><span data-stu-id="3ea6b-113">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="3ea6b-114">Може ли категорията на разходите да се използва и в управлението на проекти и счетоводството?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-114">Can the expense category also be used in Project management and accounting?</span></span> <span data-ttu-id="3ea6b-115">Ако може, вие също трябва да вземете следните решения:</span><span class="sxs-lookup"><span data-stu-id="3ea6b-115">If it can, you must also make the following decisions:</span></span>

    - <span data-ttu-id="3ea6b-116">Кои сметки за разходи ще бъдат използвани за следните разходи?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-116">Which cost accounts will be used for the following expenses?</span></span>

        - <span data-ttu-id="3ea6b-117">Разход</span><span class="sxs-lookup"><span data-stu-id="3ea6b-117">Cost</span></span>
        - <span data-ttu-id="3ea6b-118">Разпределение на изплащания</span><span class="sxs-lookup"><span data-stu-id="3ea6b-118">Payroll allocation</span></span>
        - <span data-ttu-id="3ea6b-119">Стойност на разход за WIP</span><span class="sxs-lookup"><span data-stu-id="3ea6b-119">WIP-cost value</span></span>
        - <span data-ttu-id="3ea6b-120">Елемент на разходите</span><span class="sxs-lookup"><span data-stu-id="3ea6b-120">Cost-item</span></span>
        - <span data-ttu-id="3ea6b-121">Елемент на стойност на елемент на WIP</span><span class="sxs-lookup"><span data-stu-id="3ea6b-121">WIP-cost value-item</span></span>
        - <span data-ttu-id="3ea6b-122">Натрупана загуба</span><span class="sxs-lookup"><span data-stu-id="3ea6b-122">Accrued loss</span></span>
        - <span data-ttu-id="3ea6b-123">WIP - натрупана загуба</span><span class="sxs-lookup"><span data-stu-id="3ea6b-123">WIP-accrued loss</span></span>

    - <span data-ttu-id="3ea6b-124">Кои сметки за приходи ще бъдат използвани за следните източници на приходи?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-124">Which revenue accounts will be used for the following sources of revenue?</span></span>

        - <span data-ttu-id="3ea6b-125">Фактурирани приходи</span><span class="sxs-lookup"><span data-stu-id="3ea6b-125">Invoiced revenue</span></span>
        - <span data-ttu-id="3ea6b-126">Начислени приходи - Стойност на продажби</span><span class="sxs-lookup"><span data-stu-id="3ea6b-126">Accrued revenue-sales value</span></span>
        - <span data-ttu-id="3ea6b-127">WIP-продажбена стойност</span><span class="sxs-lookup"><span data-stu-id="3ea6b-127">WIP-sales value</span></span>
        - <span data-ttu-id="3ea6b-128">Натрупани приходи-производство</span><span class="sxs-lookup"><span data-stu-id="3ea6b-128">Accrued revenue-production</span></span>
        - <span data-ttu-id="3ea6b-129">WIP-Продукция</span><span class="sxs-lookup"><span data-stu-id="3ea6b-129">WIP-production</span></span>
        - <span data-ttu-id="3ea6b-130">Натрупани приходи-приход</span><span class="sxs-lookup"><span data-stu-id="3ea6b-130">Accrued revenue-profit</span></span>
        - <span data-ttu-id="3ea6b-131">WIP-приход</span><span class="sxs-lookup"><span data-stu-id="3ea6b-131">WIP-profit</span></span>
        - <span data-ttu-id="3ea6b-132">Натрупани приходи-абонамент</span><span class="sxs-lookup"><span data-stu-id="3ea6b-132">Accrued revenue-subscription</span></span>
        - <span data-ttu-id="3ea6b-133">WIP-Абонамент</span><span class="sxs-lookup"><span data-stu-id="3ea6b-133">WIP-subscription</span></span>

- <span data-ttu-id="3ea6b-134">Какъв е типът на разхода?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-134">What is the expense type?</span></span>
- <span data-ttu-id="3ea6b-135">Какъв е методът на плащане по подразбиране за категорията разходи?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-135">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="3ea6b-136">Трябва ли разходите в категорията на разходите да бъдат детайлизирани?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-136">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="3ea6b-137">Какъв е основният акаунт по подразбиране за категорията разходи?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-137">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="3ea6b-138">Каква е групата по данък върху продажбите по подразбиране за категорията на разходите?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-138">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="3ea6b-139">Разрешени ли са допълнителни методи на плащане за разходната категория?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-139">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="3ea6b-140">Ако да, какви са те?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-140">If so, what are they?</span></span>
- <span data-ttu-id="3ea6b-141">Има ли подкатегории в тази категория разходи?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-141">Are there subcategories in this expense category?</span></span> <span data-ttu-id="3ea6b-142">Ако има подкатегории, вие също трябва да вземете следните решения:</span><span class="sxs-lookup"><span data-stu-id="3ea6b-142">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="3ea6b-143">Изключена ли е някоя от подкатегориите от събирането на данъци?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-143">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="3ea6b-144">Каква е групата за данък върху продажбите на артикули в подкатегориите?</span><span class="sxs-lookup"><span data-stu-id="3ea6b-144">What is the item sales tax group of the subcategories?</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]