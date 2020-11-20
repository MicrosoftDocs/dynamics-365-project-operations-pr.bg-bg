---
title: Дневни разходи
description: Тази тема предоставя информация за правилата за дневни, които се използват в управлението на разходите.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 8d723b49e9556401c364b323cf58eaaf44906275
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128495"
---
# <a name="per-diems"></a><span data-ttu-id="66320-103">Дневни разходи</span><span class="sxs-lookup"><span data-stu-id="66320-103">Per diems</span></span>

<span data-ttu-id="66320-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="66320-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="66320-105">Дневната надбавка е надбавка, която се изплаща на работник, който пътува по работа.</span><span class="sxs-lookup"><span data-stu-id="66320-105">A per diem is an allowance that is paid to a worker who is traveling for work.</span></span> <span data-ttu-id="66320-106">В управлението на разходите можете да създадете правила за дневни за различни ситуации при пътуване.</span><span class="sxs-lookup"><span data-stu-id="66320-106">In Expense management, you can create per diem rules for  various travel situations.</span></span> <span data-ttu-id="66320-107">Тарифите за дневни могат да се основават на времето на годината, местоположението на пътуването или и двете.</span><span class="sxs-lookup"><span data-stu-id="66320-107">Per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="66320-108">Когато създавате правило за дневни, можете да посочите, че процент от дневния размер ще бъде удържан, ако работникът получи безплатни ястия или услуги.</span><span class="sxs-lookup"><span data-stu-id="66320-108">When you create a per diem  rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="66320-109">Можете също така да зададете минимален и максимален брой часове, които дневната ставка може да се прилага за пътуването на работник.</span><span class="sxs-lookup"><span data-stu-id="66320-109">You can also set a minimum and maximum number of hours that the per diem rate can apply to a worker's travel.</span></span>

## <a name="configuration"></a><span data-ttu-id="66320-110">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="66320-110">Configuration</span></span> 

1. <span data-ttu-id="66320-111">За да добавите дневни места, отидете на **Настройка** > **Изчисления и кодове** > **Местоположения за дневни**.</span><span class="sxs-lookup"><span data-stu-id="66320-111">To add per diem locations, go to **Set up** > **Calculations and codes** > **Per diem locations**.</span></span>
2. <span data-ttu-id="66320-112">За всяко от добавените по-горе местоположения изберете тарифа за дневни и валута, която е валидна между конкретна начална и крайна дата за хотел, храна и други разходи.</span><span class="sxs-lookup"><span data-stu-id="66320-112">For each of the locations added above, select a per diem rate and currency that is valid between a specific start and end date for hotel, meals, and other expenses.</span></span> <span data-ttu-id="66320-113">Тарифите за дневни и валути са конфигурирани в **Настройка** > **Изчисления и кодове** > **Дневни**.</span><span class="sxs-lookup"><span data-stu-id="66320-113">Per diem rates and currencies are configured under **Set up** > **Calculations and codes** > **Per diems**.</span></span>
3. <span data-ttu-id="66320-114">На страницата **Места за дневни** конфигурирайте нива на дневни ставки.</span><span class="sxs-lookup"><span data-stu-id="66320-114">On the **Per diem locations** page, configure per diem rate tiers.</span></span> <span data-ttu-id="66320-115">Дневните ставки ви позволяват да дефинирате процентното разпределение на дневната надбавка за хотел, храна и други разходи.</span><span class="sxs-lookup"><span data-stu-id="66320-115">Per diem rate tiers allow you to define the percentage split of a daily allowance for hotel, meal, and other expenses.</span></span> 
4. <span data-ttu-id="66320-116">За да посочите намаление на процента на хранене за закуска, обяд или вечеря, актуализирайте полетата на страницата **Параметри за управление на разходите** на раздела **Дневни**.</span><span class="sxs-lookup"><span data-stu-id="66320-116">To specify the meal percentage reduction for breakfast, lunch, or dinner, update the fields on the **Expense management parameters** page on the **Per diem** tab.</span></span> 
    
## <a name="submit-expenses-using-per-diem"></a><span data-ttu-id="66320-117">Подайте разходи с помощта на дневни</span><span class="sxs-lookup"><span data-stu-id="66320-117">Submit expenses using per diem</span></span>
<span data-ttu-id="66320-118">За да представите разходи за използване на дневни, използвайте категория на разходите **Дневни**, когато създавате отчет за разходите.</span><span class="sxs-lookup"><span data-stu-id="66320-118">To submit expenses utilizing per diems, use the **Per diem** expense category when you create an expense report.</span></span> <span data-ttu-id="66320-119">Влезте в **Дневни от датата**, **Дневни до днешна дата** и **Място за дневни**.</span><span class="sxs-lookup"><span data-stu-id="66320-119">Enter the **Per diem from date**, **Per diem to date**,  and the **Per diem location**.</span></span> <span data-ttu-id="66320-120">Сумата ще бъде изчислена на базата на дневните ставки за избраното място и намаляването на храненето ще бъде изчислено въз основа на нивата на дневни ставки.</span><span class="sxs-lookup"><span data-stu-id="66320-120">The amount will be calculated based on the per diem rates for the selected location and meal reduction will be calculated based on the per diem rate tiers.</span></span>
