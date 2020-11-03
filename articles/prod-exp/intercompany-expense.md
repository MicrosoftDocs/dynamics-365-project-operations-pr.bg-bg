---
title: Междуфирмени разходи
description: Работник, който е нает от едно юридическо лице в организация, може да изпълнява работа за друго юридическо лице в същата организация. В тази ситуация можете да използвате функцията за вътрешнофирмени разходи, за да разпределите разходите на работника към юридическото лице, за което е извършена работата.
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
ms.openlocfilehash: 0967f23e4e1f8e0431c55d4d54554e7e90e2451c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071971"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="e050b-104">Междуфирмени разходи</span><span class="sxs-lookup"><span data-stu-id="e050b-104">Intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="e050b-105">Работник, който е нает от едно юридическо лице в организация, може да изпълнява работа за друго юридическо лице в същата организация.</span><span class="sxs-lookup"><span data-stu-id="e050b-105">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="e050b-106">В тази ситуация можете да използвате функцията за вътрешнофирмени разходи, за да разпределите разходите на работника към юридическото лице, за което е извършена работата.</span><span class="sxs-lookup"><span data-stu-id="e050b-106">In this situation, you can use the intercompany expense feature to assign the worker’s expenses to the legal entity for which the work was performed.</span></span> <span data-ttu-id="e050b-107">Юридическото лице, което наема работника, се нарича наемащо юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="e050b-107">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="e050b-108">Юридическото лице, за което работникът прави разходи, се нарича юридическо лице-заемател.</span><span class="sxs-lookup"><span data-stu-id="e050b-108">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="e050b-109">Преди работникът да може да създаде и представи разходи за работа, извършена за различно юридическо лице, в наемащото се юридическо лице, на **Параметри за управление на разходите** страница, изберете **Разрешаване на вътрешнофирмени разходни линии** опция.</span><span class="sxs-lookup"><span data-stu-id="e050b-109">Before a worker can create and submit expenses for work that is performed for a different legal entity, in the loaning legal entity, on the **Expense management parameters** page, select the **Allow intercompany expense lines** option.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="e050b-110">Данъчно осчетоводяване за вътрешнофирмени разходи</span><span class="sxs-lookup"><span data-stu-id="e050b-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="e050b-111">Ако искате да използвате данъчни групи, които са свързани със заемащото (източник) юридическо лице вместо заемното (целевото) юридическо лице във вашия отчет за разходите, ще трябва да конфигурирате това в настройката на данъка върху продажбите в Главната книга.</span><span class="sxs-lookup"><span data-stu-id="e050b-111">If you want to use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you will need to configure this in the General ledger sales tax set up.</span></span> <span data-ttu-id="e050b-112">Когато параметърът на главната книга, **Юридическо лице за междуфирмено данъчно осчетоводяване** е зададено на **Източник** и **Прилагайте правилата за данъчно облагане на продажбите** е зададено на **Не** , ще се използва данъчната комбинация за наемащото юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="e050b-112">When the General ledger parameter, **Legal entity for intercompany tax posting** is set to **Source** and **Apply sales tax taxation rules** is set to **No** , the tax combination for the loaning legal entity will be used.</span></span> <span data-ttu-id="e050b-113">Когато същият параметър е зададен на **Дестинация** , ще се използва данъчната комбинация за заемане на юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="e050b-113">When the same parameter is set to **Destination** , the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="e050b-114">За юридически лица в САЩ, когато параметърът е зададен на **Източник** , **Вземане на данък върху продажбите** полето също трябва да бъде конфигурирано на новото **Групи за осчетоводяване на книга** страница.</span><span class="sxs-lookup"><span data-stu-id="e050b-114">For legal entities in the United States, when the parameter is set to **Source** , the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="e050b-115">Счетоводният механизъм ще използва информацията от това поле за счетоводно записване, свързано с данъци.</span><span class="sxs-lookup"><span data-stu-id="e050b-115">The accounting engine will use the information from this field for tax related accounting entry.</span></span>   
<span data-ttu-id="e050b-116">Поведението е последователно за разходни линии, публикувани със или без проект.</span><span class="sxs-lookup"><span data-stu-id="e050b-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  
