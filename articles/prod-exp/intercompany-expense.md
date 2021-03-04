---
title: Междуфирмени разходи
description: Тази тема предоставя информация за това как да се използват вътрешнофирмени разходи за разпределяне на разходите на работник на юридическото лице, за което е извършена работата.
author: ShylaThompson
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 553ddbe622210169db8de4aa506dcf1ea1e9d5ef
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960819"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="d2ffa-103">Междуфирмени разходи</span><span class="sxs-lookup"><span data-stu-id="d2ffa-103">Intercompany expenses</span></span>

<span data-ttu-id="d2ffa-104">Работник, който е нает от едно юридическо лице в организация, може да изпълнява работа за друго юридическо лице в същата организация.</span><span class="sxs-lookup"><span data-stu-id="d2ffa-104">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="d2ffa-105">Можете да използвате вътрешнофирмени разходи за разпределяне на разходите на работник на юридическото лице, за което е извършена работата.</span><span class="sxs-lookup"><span data-stu-id="d2ffa-105">You can use intercompany expenses to assign the worker’s expenses to the legal entity for which the  work was performed.</span></span> <span data-ttu-id="d2ffa-106">Юридическото лице, което наема работника, се нарича наемащо юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="d2ffa-106">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="d2ffa-107">Юридическото лице, за което работникът прави разходи, се нарича юридическо лице-заемател.</span><span class="sxs-lookup"><span data-stu-id="d2ffa-107">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="d2ffa-108">Преди даден работник да може да създава и подава междуфирмени разходи, трябва да активирате междуфирмени разходни редове.</span><span class="sxs-lookup"><span data-stu-id="d2ffa-108">Before a worker can create and submit intercompany expenses, you must enable intercompany expense lines.</span></span> <span data-ttu-id="d2ffa-109">В отдаденото под наем юридическо лице, на страница **Параметри за управление на разходите** изберете **Разрешаване на вътрешнофирмени разходни линии**.</span><span class="sxs-lookup"><span data-stu-id="d2ffa-109">In the loaning legal entity, on the **Expense management parameters** page, select **Allow intercompany expense lines**.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="d2ffa-110">Данъчно осчетоводяване за вътрешнофирмени разходи</span><span class="sxs-lookup"><span data-stu-id="d2ffa-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="d2ffa-111">Преди да можете да използвате данъчни групи, които са свързани със заемащото (източник) юридическо лице вместо заемното (местоназначението) юридическо лице във вашия отчет за разходите, трябва да активирате функционалността в настройката на данъка върху продажбите в Главната книга.</span><span class="sxs-lookup"><span data-stu-id="d2ffa-111">Before you can use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you must enable the functionality in the General ledger sales tax setup.</span></span> <span data-ttu-id="d2ffa-112">Когато **Юридическо лице за междуфирмено данъчно осчетоводяване** параметърът е зададен на **Източник** и **Прилагайте правилата за данъчно облагане на продажбите** е зададено на **Не**, се използва данъчната комбинация за наемащото юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="d2ffa-112">When the **Legal entity for intercompany tax posting** parameter is set to **Source** and **Apply sales tax taxation rules** is set to **No**, the tax combination for the loaning legal entity is used.</span></span> <span data-ttu-id="d2ffa-113">Когато същият параметър е зададен на **Дестинация**, ще се използва данъчната комбинация за заемане на юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="d2ffa-113">When the same parameter is set to **Destination**, the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="d2ffa-114">За юридически лица в САЩ, когато параметърът е зададен на **Източник**, **Вземане на данък върху продажбите** полето също трябва да бъде конфигурирано на новото **Групи за осчетоводяване на книга** страница.</span><span class="sxs-lookup"><span data-stu-id="d2ffa-114">For legal entities in the United States, when the parameter is set to **Source**, the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="d2ffa-115">Счетоводният механизъм ще използва информацията от това поле за счетоводно записване, свързано с данъци.</span><span class="sxs-lookup"><span data-stu-id="d2ffa-115">The accounting engine will use the information from this field for tax-related accounting entry.</span></span>   
<span data-ttu-id="d2ffa-116">Поведението е последователно за разходни линии, публикувани със или без проект.</span><span class="sxs-lookup"><span data-stu-id="d2ffa-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  
