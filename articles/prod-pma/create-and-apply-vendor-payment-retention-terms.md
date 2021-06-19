---
title: Създаване и прилагане на условия за запазване на плащания на доставчик
description: Тази тема предоставя информация за това как да настроите и поддържате условия за задържане на плащания от доставчици.
author: Yowelle
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
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
ms.openlocfilehash: 09bb30f55ee8e1f24634e9d8b7dea95bd3dbd24f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006300"
---
# <a name="create-and-apply-vendor-payment-retention-terms"></a><span data-ttu-id="32f76-103">Създаване и прилагане на условия за запазване на плащания на доставчик</span><span class="sxs-lookup"><span data-stu-id="32f76-103">Create and apply vendor payment retention terms</span></span>

[!include [banner](../includes/banner.md)] 

<span data-ttu-id="32f76-104">Настройването на условия за задържане на плащания от доставчици за проект е полезно, когато вашата организация иска да запази част от плащанията, извършени към доставчик.</span><span class="sxs-lookup"><span data-stu-id="32f76-104">Setting up vendor payment retention terms for a project is useful when your organization wants to retain part of the payments made to a vendor.</span></span> <span data-ttu-id="32f76-105">Например, когато искате да задържите плащане на доставчик, докато доставените продукти отговарят на вашите очаквания.</span><span class="sxs-lookup"><span data-stu-id="32f76-105">For example, when you want to hold payment to a vendor until the products delivered meet your expectations.</span></span> <span data-ttu-id="32f76-106">Условията за задържане на плащане на доставчик могат да бъдат определени, когато договаряте договор за доставчик.</span><span class="sxs-lookup"><span data-stu-id="32f76-106">Vendor payment retention terms can be specified when you negotiate a vendor contract.</span></span>

## <a name="create-vendor-payment-retention-terms"></a><span data-ttu-id="32f76-107">Създаване на условия за запазване на плащания на доставчик</span><span class="sxs-lookup"><span data-stu-id="32f76-107">Create vendor payment retention terms</span></span>

<span data-ttu-id="32f76-108">Можете да въведете процента на плащане от доставчика за задържане и процента от предварително задържаните суми, които трябва да бъдат освободени.</span><span class="sxs-lookup"><span data-stu-id="32f76-108">You can enter the percentage of vendor payment for retention and the percentage of the previously retained amounts to be released.</span></span> <span data-ttu-id="32f76-109">Сумите се запазват автоматично във фактурите на доставчика, докато договорът достигне определеното състояние на завършеност.</span><span class="sxs-lookup"><span data-stu-id="32f76-109">Amounts are automatically retained on vendor invoices until the contract reaches the specified state of completion.</span></span> <span data-ttu-id="32f76-110">След като настроите условията за запазване, можете да ги приложите към всеки проект за този доставчик.</span><span class="sxs-lookup"><span data-stu-id="32f76-110">After you set up the retention terms, you can apply them to any project for that vendor.</span></span>

<span data-ttu-id="32f76-111">Използвайте следните стъпки, за да настроите и поддържате условия за задържане на плащания от доставчици.</span><span class="sxs-lookup"><span data-stu-id="32f76-111">Use the following steps to set up and maintain retention terms for vendor payments.</span></span> 

1. <span data-ttu-id="32f76-112">Отидете на **Управление на проекти и счетоводство** > **Задържане** > **Условия за задържане на плащане от доставчика**.</span><span class="sxs-lookup"><span data-stu-id="32f76-112">Go to **Project management and accounting** > **Retention** > **Vendor payment retention terms**.</span></span>
2. <span data-ttu-id="32f76-113">Изберете **Ново**, за да добавите нов срок за запазване на доставчика.</span><span class="sxs-lookup"><span data-stu-id="32f76-113">Select **New** to add a new vendor retention term.</span></span> <span data-ttu-id="32f76-114">Стойността на **ИД на правило** за новия термин се въвежда автоматично.</span><span class="sxs-lookup"><span data-stu-id="32f76-114">The **Rule ID** value for the new term is automatically entered.</span></span> 
3. <span data-ttu-id="32f76-115">Въведете кратко описание в полето **Описание** и на **Условия** FastTab, изберете **Добавяне на ред** да въведете термични стойности за следното:</span><span class="sxs-lookup"><span data-stu-id="32f76-115">Enter a brief description in the **Description** field, and on the **Terms** FastTab, select **Add line** to enter term values for the following:</span></span>

   - <span data-ttu-id="32f76-116">**Процент доставени единици**: Въведете процент на завършеност за срока.</span><span class="sxs-lookup"><span data-stu-id="32f76-116">**Percentage of units delivered**: Enter a percentage of completion for the term.</span></span> <span data-ttu-id="32f76-117">Сумите се запазват автоматично във фактурите на доставчика, докато етапът на завършване на проект не стане равен на указания процент.</span><span class="sxs-lookup"><span data-stu-id="32f76-117">Amounts are automatically retained on vendor invoices until the project stage of completion is equal to the specified percentage.</span></span> <span data-ttu-id="32f76-118">Например, ако въведете 50,00, сумите се запазват, докато проектът не бъде завършен на 50 процента.</span><span class="sxs-lookup"><span data-stu-id="32f76-118">For example, if you enter 50.00, amounts are retained until the project is 50 percent completed.</span></span>
   - <span data-ttu-id="32f76-119">**Процент за запазване**: Въведете процент от сумата на фактурата на доставчика, която трябва да бъде запазена.</span><span class="sxs-lookup"><span data-stu-id="32f76-119">**Percentage to retain**: Enter a percentage of the vendor invoice amount to be retained.</span></span> <span data-ttu-id="32f76-120">Например, ако въведете 10,00, тогава 10 процента от сумата във фактура на доставчик се запазва, докато проектът достигне процента на завършеност, както е зададено в **Процент на доставените единици поле**.</span><span class="sxs-lookup"><span data-stu-id="32f76-120">For example, if you enter 10.00, then 10 percent of the amount on a vendor invoice is retained until the project reaches the percentage of completion as set in the **Percentage of units delivered field**.</span></span>
   - <span data-ttu-id="32f76-121">**Процент за освобождаване**: Изберете **Добавяне на ред** да въведете процент от всички задържани по-рано суми, които да бъдат освободени за избраното ниво на завършеност на проекта.</span><span class="sxs-lookup"><span data-stu-id="32f76-121">**Percentage to release**: Select **Add line** to enter a percentage of any previously retained amounts to be released for the selected level of project completion.</span></span>

> [!NOTE]
> <span data-ttu-id="32f76-122">Ако имате повече от един етап за различни нива на завършеност на проекта, въведете отделна линия за срок на запазване на доставчика за всяко правило за запазване.</span><span class="sxs-lookup"><span data-stu-id="32f76-122">If you have more than one milestone for different levels of project completion, enter a separate vendor retention term line for each retention rule.</span></span> <span data-ttu-id="32f76-123">Всеки ред може да посочи различен процент на задържане и различен процент на освобождаване за всяко определено ниво на завършеност на проекта.</span><span class="sxs-lookup"><span data-stu-id="32f76-123">Each line can specify a different retention percentage and a different release percentage for each designated level of project completion.</span></span>

<span data-ttu-id="32f76-124">След като създадете правила за запазване на доставчик за даден доставчик, можете да приложите правилата към проект.</span><span class="sxs-lookup"><span data-stu-id="32f76-124">After you create vendor retention terms for a vendor, you can apply the terms to a project.</span></span>

## <a name="apply-vendor-retention-terms-to-a-project"></a><span data-ttu-id="32f76-125">Приложете условия за задържане на доставчици към проект</span><span class="sxs-lookup"><span data-stu-id="32f76-125">Apply vendor retention terms to a project</span></span>

1. <span data-ttu-id="32f76-126">Отидете на **Управление на проекти и счетоводство** > **Проекти** > **Всички проекти** и отворете проект от страницата със списъка с проекти.</span><span class="sxs-lookup"><span data-stu-id="32f76-126">Go to **Project management and accounting** > **Projects** > **All projects** and open a project from the project list page.</span></span>
2. <span data-ttu-id="32f76-127">На **Споразумения с доставчици** FastTab, изберете **Добавяне на ред**.</span><span class="sxs-lookup"><span data-stu-id="32f76-127">On the **Vendor agreements** FastTab, select **Add line**.</span></span>
3. <span data-ttu-id="32f76-128">В полето **Код на акаунт** изберете едно от следните опции:</span><span class="sxs-lookup"><span data-stu-id="32f76-128">In the **Account code field**, select one of the following options:</span></span> 

   - <span data-ttu-id="32f76-129">**Таблица**: Правилата за запазване на доставчик се прилагат за един доставчик.</span><span class="sxs-lookup"><span data-stu-id="32f76-129">**Table**: The vendor retention terms apply to a single vendor.</span></span>
   - <span data-ttu-id="32f76-130">**Група**: Правилата за запазване на доставчик се прилагат за всички доставчици в група доставчици.</span><span class="sxs-lookup"><span data-stu-id="32f76-130">**Group**: The vendor retention terms apply to all vendors in a vendor group.</span></span>
   - <span data-ttu-id="32f76-131">**Всички**: Правилата за запазване на доставчик се прилагат за всички доставчици.</span><span class="sxs-lookup"><span data-stu-id="32f76-131">**All**: The vendor retention terms apply to all vendors.</span></span>

4. <span data-ttu-id="32f76-132">В **Поле на доставчика / групата на доставчика**, изберете доставчика или групата доставчици, за които се прилагат условията за задържане на доставчика.</span><span class="sxs-lookup"><span data-stu-id="32f76-132">In the **Vendor/Vendor group field**, select the vendor or vendor group to which the vendor retention terms apply.</span></span> <span data-ttu-id="32f76-133">Ако сте избрали **всичко** в предишната стъпка това поле не е налично.</span><span class="sxs-lookup"><span data-stu-id="32f76-133">If you selected **All** in the previous step, this field is unavailable.</span></span>
5. <span data-ttu-id="32f76-134">В полето **Условия за задържане на доставчика** изберете условията за запазване, които сте създали в предишната процедура.</span><span class="sxs-lookup"><span data-stu-id="32f76-134">In the **Vendor retention terms** field, select the retention terms that you created in the previous procedure.</span></span>
6. <span data-ttu-id="32f76-135">Ако проектът има и условия за плащане при плащане (PWP), настроени за доставчика, въведете праговия процент за проекта в полето **Процент на прага на PWP**.</span><span class="sxs-lookup"><span data-stu-id="32f76-135">If the project also has pay-when-paid (PWP) terms set up for the vendor, enter the threshold percentage for the project in the **PWP threshold percentage** field.</span></span>

<span data-ttu-id="32f76-136">Условията за задържане на доставчика се показват и в поръчките за покупка, които създавате за доставчика.</span><span class="sxs-lookup"><span data-stu-id="32f76-136">The vendor retention terms are also displayed on purchase orders that you create for the vendor.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]