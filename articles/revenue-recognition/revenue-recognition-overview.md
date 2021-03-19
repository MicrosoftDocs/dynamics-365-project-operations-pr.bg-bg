---
title: Общ преглед на признаването на приходите
description: Тази тема предоставя информация за признаването на приходите в Project Operations.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5e77a0442f634a50f8099fadec42ff400fee0e81
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278855"
---
# <a name="revenue-recognition-overview"></a><span data-ttu-id="b0c1e-103">Общ преглед на признаването на приходите</span><span class="sxs-lookup"><span data-stu-id="b0c1e-103">Revenue recognition overview</span></span>

<span data-ttu-id="b0c1e-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="b0c1e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="b0c1e-105">В Dynamics 365 Project Operations принципите за признаване на приходите варират в зависимост от избрания метод за фактуриране за проект или част от проекта.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-105">In Dynamics 365 Project Operations, revenue recognition principles vary based on the selected billing method for a project or portion of the project.</span></span> <span data-ttu-id="b0c1e-106">Тази тема предоставя информация за признаването на приходите в Project Operations.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-106">This topic provides information about revenue recognition in Project Operations.</span></span>

## <a name="transactions-accounted-using-time-and-material-billing-method"></a><span data-ttu-id="b0c1e-107">Трансакции, отчетени с метода за фактуриране на време и материали</span><span class="sxs-lookup"><span data-stu-id="b0c1e-107">Transactions accounted using time and material billing method</span></span>

- <span data-ttu-id="b0c1e-108">Признаването на разходи и приходи е свързано.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-108">Cost and revenue recognition are connected.</span></span> <span data-ttu-id="b0c1e-109">Разходите за трансакции и нефактурираните продажби се публикуват с помощта на [журнала за интеграция на Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="b0c1e-109">Transaction cost and unbilled sales are posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span>
- <span data-ttu-id="b0c1e-110">Профилът на разходите и приходите на проекта определя дали трансакциите на нефактурирани продажби се публикуват в главната книга.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-110">Project cost and revenue profile determine if unbilled sales transactions are posted to the general ledger.</span></span> <span data-ttu-id="b0c1e-111">Ако е избрано **Натрупан приход** системата използва сметките **Стойност на продажбите на WIP** и **Стройност на продажбите за натрупан приход** при публикуването.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-111">If **Accrue revenue** is selected, the system uses the **WIP sales value** and the **Accrued revenue sales value** accounts during posting.</span></span> <span data-ttu-id="b0c1e-112">По-долу е даден пример за този метод.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-112">The following is an example of this method.</span></span>  

  | <span data-ttu-id="b0c1e-113">Тип на трансакция</span><span class="sxs-lookup"><span data-stu-id="b0c1e-113">Transaction type</span></span> | <span data-ttu-id="b0c1e-114">Дебит/кредит</span><span class="sxs-lookup"><span data-stu-id="b0c1e-114">Debit/Credit</span></span> | <span data-ttu-id="b0c1e-115">Количество</span><span class="sxs-lookup"><span data-stu-id="b0c1e-115">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="b0c1e-116">Стойност на продажбите на WIP</span><span class="sxs-lookup"><span data-stu-id="b0c1e-116">WIP Sales value</span></span> | <span data-ttu-id="b0c1e-117">Дебит</span><span class="sxs-lookup"><span data-stu-id="b0c1e-117">Debit</span></span> | <span data-ttu-id="b0c1e-118">100</span><span class="sxs-lookup"><span data-stu-id="b0c1e-118">100</span></span> |
  | <span data-ttu-id="b0c1e-119">Стойност на продажбите на начислени приходи</span><span class="sxs-lookup"><span data-stu-id="b0c1e-119">Accrued revenue sales value</span></span> | <span data-ttu-id="b0c1e-120">Кредит</span><span class="sxs-lookup"><span data-stu-id="b0c1e-120">Credit</span></span> | <span data-ttu-id="b0c1e-121">100</span><span class="sxs-lookup"><span data-stu-id="b0c1e-121">100</span></span> |

- <span data-ttu-id="b0c1e-122">Приходите се признават при фактуриране.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-122">Revenue is recognized during invoicing.</span></span> <span data-ttu-id="b0c1e-123">Системата използва сметката **Фактуриран приход** при публикуването.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-123">The system uses the **Invoiced revenue** account during posting.</span></span> <span data-ttu-id="b0c1e-124">По-долу е даден пример за този метод.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-124">The following is an example of this method.</span></span>  

  | <span data-ttu-id="b0c1e-125">Тип на трансакция</span><span class="sxs-lookup"><span data-stu-id="b0c1e-125">Transaction type</span></span> | <span data-ttu-id="b0c1e-126">Дебит/кредит</span><span class="sxs-lookup"><span data-stu-id="b0c1e-126">Debit/Credit</span></span> | <span data-ttu-id="b0c1e-127">Количество</span><span class="sxs-lookup"><span data-stu-id="b0c1e-127">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="b0c1e-128">Баланс на клиент</span><span class="sxs-lookup"><span data-stu-id="b0c1e-128">Customer balance</span></span> | <span data-ttu-id="b0c1e-129">Дебит</span><span class="sxs-lookup"><span data-stu-id="b0c1e-129">Debit</span></span> | <span data-ttu-id="b0c1e-130">120</span><span class="sxs-lookup"><span data-stu-id="b0c1e-130">120</span></span> |
  | <span data-ttu-id="b0c1e-131">Дължим данък върху продажбите</span><span class="sxs-lookup"><span data-stu-id="b0c1e-131">Sales tax payable</span></span> | <span data-ttu-id="b0c1e-132">Кредит</span><span class="sxs-lookup"><span data-stu-id="b0c1e-132">Credit</span></span> | <span data-ttu-id="b0c1e-133">20</span><span class="sxs-lookup"><span data-stu-id="b0c1e-133">20</span></span> |
  | <span data-ttu-id="b0c1e-134">Фактуриран приход</span><span class="sxs-lookup"><span data-stu-id="b0c1e-134">Invoiced Revenue</span></span> | <span data-ttu-id="b0c1e-135">Кредит</span><span class="sxs-lookup"><span data-stu-id="b0c1e-135">Credit</span></span> | <span data-ttu-id="b0c1e-136">100</span><span class="sxs-lookup"><span data-stu-id="b0c1e-136">100</span></span> |

- <span data-ttu-id="b0c1e-137">Ако приходите са натрупани при публикуване на нефактурираните продажби, системата ще възстанови начисления приход при фактуриране.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-137">If revenue was accrued when the unbilled sales are posted, the system will reverse the accrued revenue at invoicing.</span></span>

  | <span data-ttu-id="b0c1e-138">Тип на трансакция</span><span class="sxs-lookup"><span data-stu-id="b0c1e-138">Transaction type</span></span> | <span data-ttu-id="b0c1e-139">Дебит/кредит</span><span class="sxs-lookup"><span data-stu-id="b0c1e-139">Debit/Credit</span></span> | <span data-ttu-id="b0c1e-140">Количество</span><span class="sxs-lookup"><span data-stu-id="b0c1e-140">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="b0c1e-141">Стойност на продажбите на WIP</span><span class="sxs-lookup"><span data-stu-id="b0c1e-141">WIP Sales value</span></span> | <span data-ttu-id="b0c1e-142">Кредит</span><span class="sxs-lookup"><span data-stu-id="b0c1e-142">Credit</span></span> | <span data-ttu-id="b0c1e-143">100</span><span class="sxs-lookup"><span data-stu-id="b0c1e-143">100</span></span> |
  | <span data-ttu-id="b0c1e-144">Стойност на продажбите на начислени приходи</span><span class="sxs-lookup"><span data-stu-id="b0c1e-144">Accrued revenue sales value</span></span> | <span data-ttu-id="b0c1e-145">Дебит</span><span class="sxs-lookup"><span data-stu-id="b0c1e-145">Debit</span></span> | <span data-ttu-id="b0c1e-146">100</span><span class="sxs-lookup"><span data-stu-id="b0c1e-146">100</span></span> |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a><span data-ttu-id="b0c1e-147">Трансакции, отчетени с метода за фактуриране с фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="b0c1e-147">Transactions accounted using the fixed price billing method</span></span>

- <span data-ttu-id="b0c1e-148">Признаването на разходи и приходи е отделно.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-148">Cost and revenue recognition are separate.</span></span> <span data-ttu-id="b0c1e-149">Разходите за трансакции се публикуват с помощта на [журнала за интеграция на Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="b0c1e-149">Transaction cost is posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="b0c1e-150">Не се създават трансакции за нефактурирани продажби.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-150">Unbilled sales transactions aren't created.</span></span>
- <span data-ttu-id="b0c1e-151">Приходите могат да се признаят по време на фактурирането, ако профилът на разходите и приходите на проекта е със зададен **Принцип, използван за изчисления на завършеност на проекта** на **Няма WIP**.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-151">Revenue can be recognized during invoicing if the project cost and revenue profile have **Principle used for project completion calculations** set to **No WIP**.</span></span> <span data-ttu-id="b0c1e-152">Използвайте този метод само за краткосрочни, опростени проекти.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-152">Only use this method for short term, simple projects.</span></span>
- <span data-ttu-id="b0c1e-153">Приходите могат да се признаят, като се използват прогнози за приход с фиксирана цена с метода **Завършен договор** или **Признаване на приход за процент на завършеност**.</span><span class="sxs-lookup"><span data-stu-id="b0c1e-153">Revenue can be recognized using fixed price revenue estimates, with either the **Completed contract** or **Percent completion revenue recognition** method.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="b0c1e-154">Допълнителни ресурси</span><span class="sxs-lookup"><span data-stu-id="b0c1e-154">Additional resources</span></span>
[<span data-ttu-id="b0c1e-155">Статия за конфигуриране на счетоводство за проекти с възможност за фактуриране</span><span class="sxs-lookup"><span data-stu-id="b0c1e-155">Configure accounting for billable projects article</span></span>](../project-accounting/configure-accounting-billable-projects.md)

[<span data-ttu-id="b0c1e-156">Проекти за прогнози за приходи с фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="b0c1e-156">Fixed price revenue estimate projects</span></span>](rev-rec-percentage-completion-method.md)

[<span data-ttu-id="b0c1e-157">Управление на прогнози за приходи</span><span class="sxs-lookup"><span data-stu-id="b0c1e-157">Manage revenue estimates</span></span>](rev-rec-completed-contract-method.md)

[<span data-ttu-id="b0c1e-158">Методи за разходи за завършване</span><span class="sxs-lookup"><span data-stu-id="b0c1e-158">Cost to complete methods</span></span>](cost-complete-methods.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]