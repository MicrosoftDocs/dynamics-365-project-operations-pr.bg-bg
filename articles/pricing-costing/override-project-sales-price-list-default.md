---
title: Заместване на ценовите листи за продажби по проект
description: Тази тема предоставя информация за създаването на персонализирани ценови листи за продажби.
author: rumant
manager: Annbe
ms.date: 10/22/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: c97dca8685c2db7d256017cf4442416feb0e005b
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130835"
---
# <a name="override-project-sales-price-lists"></a><span data-ttu-id="91b5f-103">Заместване на ценовите листи за продажби по проект</span><span class="sxs-lookup"><span data-stu-id="91b5f-103">Override project sales price lists</span></span>

<span data-ttu-id="91b5f-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="91b5f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

## <a name="customer-specific-project-price-lists"></a><span data-ttu-id="91b5f-105">Ценови листи по проект, специфични за клиента</span><span class="sxs-lookup"><span data-stu-id="91b5f-105">Customer-specific project price lists</span></span>

<span data-ttu-id="91b5f-106">Може да се зададат специфични за клиента споразумения за цени като ценови листи по проект в запис на клиент в Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="91b5f-106">Customer-specific price agreements can be set up as project price lists on an account record in Dynamics 365 Project Operations.</span></span>

<span data-ttu-id="91b5f-107">За да създадете ценова листа, специфична за клиент, по проект, в областта **Продажби** отидете на записа на клиента.</span><span class="sxs-lookup"><span data-stu-id="91b5f-107">To set up a customer-specific project price list, in the **Sales** area, navigate to the account record.</span></span>

1. <span data-ttu-id="91b5f-108">Отворете страницата със списъка **Клиенти**.</span><span class="sxs-lookup"><span data-stu-id="91b5f-108">Open the **Accounts** list page.</span></span>
2. <span data-ttu-id="91b5f-109">Намерете и щракнете двукратно върху клиентски запис, за да отворите страницата с подробности **Клиент**.</span><span class="sxs-lookup"><span data-stu-id="91b5f-109">Locate and double-click a customer record to open the **Account** details page.</span></span>
3. <span data-ttu-id="91b5f-110">В раздела **Ценови листи по проект** изберете \*\*+ Нова ценова листа по проект^^.</span><span class="sxs-lookup"><span data-stu-id="91b5f-110">On the **Project Price lists** tab, select \*\*+ New Project Price List^^.</span></span>
4. <span data-ttu-id="91b5f-111">На страницата **Нова ценова листа по проект** изберете ценова листа от падащото меню.</span><span class="sxs-lookup"><span data-stu-id="91b5f-111">On the **New Project Price List** page, select a price list from the drop-down.</span></span> <span data-ttu-id="91b5f-112">Включени са само ценови листи, които имат зададен контекст **Продажби** и чиято валута съвпада с валутата на клиента.</span><span class="sxs-lookup"><span data-stu-id="91b5f-112">Only price lists that have the context set to **Sales** and whose currency matches the account currency are included.</span></span>
5. <span data-ttu-id="91b5f-113">Задайте име на връзката и след това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="91b5f-113">Name the association, and then select **Save**.</span></span> <span data-ttu-id="91b5f-114">Създава се ценова листа по проект, специфична за клиента.</span><span class="sxs-lookup"><span data-stu-id="91b5f-114">A customer-specific project price list is created.</span></span> <span data-ttu-id="91b5f-115">Тази ценова листа ще се използва за задаване на цени по проект по подразбиране в оферти и договори по проект,създадени за този клиент, когато датата на създаване на офертата или договора по проект попада в рамките на валидната дата в ценовата листа.</span><span class="sxs-lookup"><span data-stu-id="91b5f-115">This price list will be used to default project prices on project quotes or contracts created for this customer where the created date of the quote or project contract falls within the date effectivity of the price list.</span></span>

## <a name="custom-pricing-on-project-quotes"></a><span data-ttu-id="91b5f-116">Персонализирано ценообразуване в оферти по проект</span><span class="sxs-lookup"><span data-stu-id="91b5f-116">Custom pricing on project quotes</span></span>

<span data-ttu-id="91b5f-117">В офертите по проект може да има ценообразуване по проект, което започва със стандартна ценова листа по подразбиране, която по подразбиране е от клиента или от параметрите на проекта.</span><span class="sxs-lookup"><span data-stu-id="91b5f-117">On project quotes, you can have project pricing that starts with a default standard price list that defaults from the customer or from the project parameters.</span></span>

<span data-ttu-id="91b5f-118">Когато се нуждаете от персонализирано ценообразуване за свързана с проекта работа по определена оферта, можете да го получите от свързания обект на ценовите листи по проекта.</span><span class="sxs-lookup"><span data-stu-id="91b5f-118">When you need custom pricing for project-related work on a particular quote, you can get that from the project price lists associated entity.</span></span>

<span data-ttu-id="91b5f-119">Изпълнете следните стъпки, за да настроите специфично за офертата ценообразуване по проекта.</span><span class="sxs-lookup"><span data-stu-id="91b5f-119">Complete the following steps to set up quote-specific project pricing.</span></span>

1. <span data-ttu-id="91b5f-120">Отворете офертата по проекта и изберете раздела **Ценови листи по проект**.</span><span class="sxs-lookup"><span data-stu-id="91b5f-120">Open the project quote and select the **Project Price Lists** tab.</span></span>
2. <span data-ttu-id="91b5f-121">В подмрежата изберете **Създаване на персонализирано ценообразуване**.</span><span class="sxs-lookup"><span data-stu-id="91b5f-121">In the subgrid, select **Create custom pricing**.</span></span>

<span data-ttu-id="91b5f-122">Всички ценови листи по проект, които са прикачени към офертата, се копират в новите ценови листи.</span><span class="sxs-lookup"><span data-stu-id="91b5f-122">All the project price lists that are attached to the quote are copied to new price lists.</span></span> <span data-ttu-id="91b5f-123">Имената на новите ценови листи отразяват името на офертата с клеймо за дата и час, показващо кога са създадени тези ценови листи.</span><span class="sxs-lookup"><span data-stu-id="91b5f-123">The names of the new price lists reflect the name of quote with a date-time stamp for when these price lists were created.</span></span>

<span data-ttu-id="91b5f-124">Можете да използвате всяка от тези ценови листи и да актуализирате цените за труд (цена на роля) и разходи (цена на категория).</span><span class="sxs-lookup"><span data-stu-id="91b5f-124">You can use each of those price lists and make updates to labor (role price) and expense (category price) prices.</span></span> <span data-ttu-id="91b5f-125">Тези цени ще бъдат приложими само за тази оферта по проект.</span><span class="sxs-lookup"><span data-stu-id="91b5f-125">These prices will only be applicable to this project quote.</span></span>

## <a name="price-lists-on-a-project-contract"></a><span data-ttu-id="91b5f-126">Ценови листи в договор по проект</span><span class="sxs-lookup"><span data-stu-id="91b5f-126">Price lists on a project contract</span></span>

<span data-ttu-id="91b5f-127">При договор по проект ценообразуването по проект винаги по подразбиране е като персонализирана ценова листа с името на договора и клеймо с датата и часа на създаване, добавено към името.</span><span class="sxs-lookup"><span data-stu-id="91b5f-127">On a project contract, project pricing always defaults as a custom price list with the name of contract and the created date time stamp appended to the name.</span></span> <span data-ttu-id="91b5f-128">Това е вярно независимо дали договорът е създаден при спечелване на офертата или е създаден от нулата.</span><span class="sxs-lookup"><span data-stu-id="91b5f-128">This is true whether the contract was created when the quote was won or if the contract was created from scratch.</span></span> <span data-ttu-id="91b5f-129">Ако е необходимо, можете да премахнете тази асоциация към персонализираната ценова листа и вместо това да свържете стандартна ценова листа към договор по проект.</span><span class="sxs-lookup"><span data-stu-id="91b5f-129">If needed, you can remove this association to the custom price list and associate a standard price list to the project contract instead.</span></span>

<span data-ttu-id="91b5f-130">Когато свържете стандартна ценова листа към ценовите листи по проекта в офертата или договора, всички промени, които направите на цените в ценовата листа, ще се отразят на всички оферти и договори, които използват ценовата листа.</span><span class="sxs-lookup"><span data-stu-id="91b5f-130">When you associate a standard price list to the project price lists on quote or contract, any changes made to the prices in the price list will impact all quotes and contracts that use the price list.</span></span>
