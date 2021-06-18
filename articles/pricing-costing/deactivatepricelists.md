---
title: Дезактивиране на ценови листи
description: Тази тема обяснява как да деактивирате или премахнете неизползвани или стари ценови листи.
author: rumant
ms.date: 03/19/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Professional Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: d5d6cf6b4b097c08edca5a3235ed1b438a0eae2d
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001323"
---
# <a name="deactivate-price-lists"></a><span data-ttu-id="8902d-103">Дезактивиране на ценови листи</span><span class="sxs-lookup"><span data-stu-id="8902d-103">Deactivate price lists</span></span> 

<span data-ttu-id="8902d-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="8902d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8902d-105">За да премахнете стари или неизползвани ценови листи от Dynamics 365 Project Operations, има две стъпки, които трябва да изпълните.</span><span class="sxs-lookup"><span data-stu-id="8902d-105">To remove old or unused price lists from Dynamics 365 Project Operations, there are two steps you must complete.</span></span> 

1. <span data-ttu-id="8902d-106">Премахнете или изтрийте ценовата листа от конкретни страници.</span><span class="sxs-lookup"><span data-stu-id="8902d-106">Remove or delete the price list from specific pages.</span></span>
2. <span data-ttu-id="8902d-107">Деактивирайте или изтрийте ценовата листа от Активните ценови листи на страницата **Ценови списъци**.</span><span class="sxs-lookup"><span data-stu-id="8902d-107">Deactivate or delete the price list from the Active price lists on the **Price Lists** page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="8902d-108">Трябва да изпълните двете стъпки, за да премахнете напълно ценовата листа.</span><span class="sxs-lookup"><span data-stu-id="8902d-108">You must complete both steps to fully remove a price list.</span></span> <span data-ttu-id="8902d-109">Само изпълнението на стъпка 2, която е директно изтриване или деактивиране на ценовата листа от изгледа Активни ценови списъци, не е достатъчно.</span><span class="sxs-lookup"><span data-stu-id="8902d-109">Only performing step 2, which is to directly delete or deactivate the price list from the Active Price Lists view, is not sufficient.</span></span> <span data-ttu-id="8902d-110">Трябва също да изтриете свързването на този ценоразпис от всички места, споменати в стъпка 1.</span><span class="sxs-lookup"><span data-stu-id="8902d-110">You must also delete the association of this price list from all the places mentioned in step 1.</span></span>

## <a name="delete-the-price-list-from-specific-pages"></a><span data-ttu-id="8902d-111">Изтриване на ценовата листа от конкретни страници</span><span class="sxs-lookup"><span data-stu-id="8902d-111">Delete the price list from specific pages</span></span>
1. <span data-ttu-id="8902d-112">За да изтриете ценова листа от Project Operations, отидете на следните страници:</span><span class="sxs-lookup"><span data-stu-id="8902d-112">To delete a price list from Project Operations, go to the following pages:</span></span>  

      - <span data-ttu-id="8902d-113">Страница **Параметри на проект** > раздел **Ценови листи**</span><span class="sxs-lookup"><span data-stu-id="8902d-113">**Project parameters** page > **Price Lists** tab</span></span>
      - <span data-ttu-id="8902d-114">Страница **Организационно звено** > мрежа **Ценови списъци**</span><span class="sxs-lookup"><span data-stu-id="8902d-114">**Organizational Unit** page > **Price Lists** grid</span></span>
      - <span data-ttu-id="8902d-115">Страница **Сметка** > мрежа **Проектни ценови списъци**</span><span class="sxs-lookup"><span data-stu-id="8902d-115">**Account** page > **Project Price Lists** grid</span></span>
      - <span data-ttu-id="8902d-116">Страница **Оферти по проекти** > мрежа **Проектни ценови листи**: Това се отнася за всички активни проектни оферти.</span><span class="sxs-lookup"><span data-stu-id="8902d-116">**Project Quotes** page > **Project Price Lists** grid: This applies to all active project quotes.</span></span>
      - <span data-ttu-id="8902d-117">Страница **Договори по проекти** > мрежа **Проектни ценови листи**: Това се отнася за всички активни проектни договори.</span><span class="sxs-lookup"><span data-stu-id="8902d-117">**Project Contracts** page > **Project Price Lists** grid: This applies to all active project contracts.</span></span>

 2. <span data-ttu-id="8902d-118">За всяка страница трябва да изберете ценовата листа, която искате да изтриете, и след това да изберете **Изтрий**.</span><span class="sxs-lookup"><span data-stu-id="8902d-118">For each page, you need to select the price list that you want to delete, and then select **Delete**.</span></span> 
 
## <a name="delete-or-deactivate-the-price-list-from-the-price-lists-page"></a><span data-ttu-id="8902d-119">Изтрийте или дезактивирайте ценовата листа от страницата Ценови листи</span><span class="sxs-lookup"><span data-stu-id="8902d-119">Delete or deactivate the price list from the Price Lists page</span></span>
 
1. <span data-ttu-id="8902d-120">За да изтриете ценоразпис от активните ценови листи, отидете на **Продажби** > **Клиенти** > **Ценови листи**.</span><span class="sxs-lookup"><span data-stu-id="8902d-120">To delete a price list from the active price lists, go to **Sales** > **Customers** > **Price Lists**.</span></span> 
2. <span data-ttu-id="8902d-121">Изберете ценовата листа, която искате да изтриете и след това изберете **Изтриване**.</span><span class="sxs-lookup"><span data-stu-id="8902d-121">Select the price list that you want to delete and then select **Delete**.</span></span> <span data-ttu-id="8902d-122">Ако ценовата листа е посочена за всякакви съществуващи транзакции, няма да можете да я изтриете.</span><span class="sxs-lookup"><span data-stu-id="8902d-122">If the price list is referenced on any existing transactions, you won't be able to delete it.</span></span> <span data-ttu-id="8902d-123">Ако това се случи, можете да деактивирате ценовата листа, така че да не се показва в никакви изгледи.</span><span class="sxs-lookup"><span data-stu-id="8902d-123">If this happens, you can deactivate the price list so that it doesn't appear in any views.</span></span> 
3. <span data-ttu-id="8902d-124">За да деактивирате ценовата листа, изберете ценовата листа отново и след това изберете **Дезактивирайте**.</span><span class="sxs-lookup"><span data-stu-id="8902d-124">To deactivate the price list, select the price list again, and then select **Deactivate**.</span></span>   
