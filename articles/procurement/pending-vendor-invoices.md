---
title: Закупуване на нескладирани материали с помощта на фактури на доставчици в изчакване
description: Тази тема обяснява как да записвате чакащи фактури на доставчици.
author: sigitac
manager: tfehr
ms.date: 04/12/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7a706f419443dcdf92ce3b247d719943272907d0
ms.sourcegitcommit: 7468d668c48c1d87934aab9a034decd51e56dec6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/13/2021
ms.locfileid: "5880620"
---
# <a name="purchase-non-stocked-materials-using-a-pending-vendor-invoice"></a><span data-ttu-id="3bb22-103">Закупуване на нескладирани материали с помощта на фактури на доставчици в изчакване</span><span class="sxs-lookup"><span data-stu-id="3bb22-103">Purchase non-stocked materials using a pending vendor invoice</span></span>

<span data-ttu-id="3bb22-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="3bb22-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="3bb22-105">Тъй като дадена компания набавя нескладови материали за даден проект, разходите могат незабавно да бъдат записани спрямо проекта.</span><span class="sxs-lookup"><span data-stu-id="3bb22-105">As a company procures non-stocked materials for a project, the costs can be immediately recorded against the project.</span></span> 

<span data-ttu-id="3bb22-106">Например, Contoso Robotics US изпълнява проект за обновяване на оборудването и се нуждае от софтуерни лицензи.</span><span class="sxs-lookup"><span data-stu-id="3bb22-106">For example, Contoso Robotics US is performing an equipment renewal project and needs software licenses.</span></span> <span data-ttu-id="3bb22-107">Тези лицензи се доставят от доставчик на трета страна.</span><span class="sxs-lookup"><span data-stu-id="3bb22-107">These licenses are procured from a third-party vendor.</span></span>  <span data-ttu-id="3bb22-108">Използвайки Dynamics 365 Finance, служителят по задълженията записва изчакващ документ за фактура на доставчик и приписва разходите за лиценз директно към проекта за подновяване на оборудването.</span><span class="sxs-lookup"><span data-stu-id="3bb22-108">Using Dynamics 365 Finance, the Accounts payable clerk records a pending vendor invoice document and attributes the license costs directly against the equipment renewal project.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="3bb22-109">Преди да използвате функциите, описани в тази тема, прегледайте и приложете необходимите конфигурации.</span><span class="sxs-lookup"><span data-stu-id="3bb22-109">Before you use the functionality described in this topic, review and apply the required configurations.</span></span> <span data-ttu-id="3bb22-110">За повече информация вижте [Разрешаване на нескладовите материали и изчакващи фактура на доставчика](configure-materials-nonstocked.md).</span><span class="sxs-lookup"><span data-stu-id="3bb22-110">For more information, see [Enable non-stocked materials and pending vendor invoices](configure-materials-nonstocked.md).</span></span> 

## <a name="post-a-project-related-pending-vendor-invoice"></a><span data-ttu-id="3bb22-111">Публикувайте фактура на доставчик, свързана с проект</span><span class="sxs-lookup"><span data-stu-id="3bb22-111">Post a project-related pending vendor invoice</span></span> 

<span data-ttu-id="3bb22-112">Чакащите фактури на доставчици могат да бъдат записани на страницата **Чакащи фактури на доставчици** (**Задължения** > **Фактури** > **Чакащи фактури на доставчици**).</span><span class="sxs-lookup"><span data-stu-id="3bb22-112">Pending vendor invoices can be recorded on the **Pending vendor invoices** page (**Accounts payable** > **Invoices** > **Pending vendor invoices**).</span></span> <span data-ttu-id="3bb22-113">Изпълнете следните стъпки, за да публикувате фактура на висящ доставчик, свързана с проект:</span><span class="sxs-lookup"><span data-stu-id="3bb22-113">Complete the following steps to post a project-related pending vendor invoice:</span></span>

1. <span data-ttu-id="3bb22-114">Отидете на **Задължения** > **Фактури** и изберете **Създаване**.</span><span class="sxs-lookup"><span data-stu-id="3bb22-114">Go to **Accounts payable** > **Invoices** and select **New**.</span></span> 
2. <span data-ttu-id="3bb22-115">В полето **Сметка за фактура**, изберете доставчик и в **Брой** поле, въведете идентификацията на фактурата на доставчика.</span><span class="sxs-lookup"><span data-stu-id="3bb22-115">In the **Invoice account** field, select a vendor and in the **Number** field, enter the vendor invoice identification.</span></span>
3. <span data-ttu-id="3bb22-116">Добавете ред към фактурата на доставчика и в **Номер на артикул** поле, изберете артикула, който не е на склад, закупен от доставчика.</span><span class="sxs-lookup"><span data-stu-id="3bb22-116">Add a line to the vendor invoice and in the **Item number** field, select the non-stocked item purchased from the vendor.</span></span> 

    > [!NOTE]
    > <span data-ttu-id="3bb22-117">Редове за фактури на доставчици, които се основават на категория на поръчката, не могат да бъдат записани в проекта.</span><span class="sxs-lookup"><span data-stu-id="3bb22-117">Vendor invoice lines that are based on a procurement category can't be recorded against the project.</span></span> 
    
5. <span data-ttu-id="3bb22-118">Добавете закупеното количество.</span><span class="sxs-lookup"><span data-stu-id="3bb22-118">Add the quantity purchased.</span></span> <span data-ttu-id="3bb22-119">Системата ще попълни единичната цена въз основа на конфигурацията на цената на артикула, която не е на склад.</span><span class="sxs-lookup"><span data-stu-id="3bb22-119">The system will populate the unit price based on the non-stocked item price configuration.</span></span> 
6. <span data-ttu-id="3bb22-120">Проверете общата сума и други необходими подробности на линията.</span><span class="sxs-lookup"><span data-stu-id="3bb22-120">Verify the total amount and other required details on the line.</span></span>
7. <span data-ttu-id="3bb22-121">На линията с подробности, на раздела **Проект**, изберете идентификатора на проекта, в който ще бъде записан този елемент.</span><span class="sxs-lookup"><span data-stu-id="3bb22-121">On the line details, on the **Project** tab, select the ID of the project that this item will be recorded to.</span></span>
8. <span data-ttu-id="3bb22-122">По избор изберете номера на активността и актуализирайте категорията на проекта и свойството на реда.</span><span class="sxs-lookup"><span data-stu-id="3bb22-122">Optionally, select the activity number, and update the project category and line property.</span></span>
9. <span data-ttu-id="3bb22-123">Публикувайте изчакваща фактура на доставчик.</span><span class="sxs-lookup"><span data-stu-id="3bb22-123">Post pending vendor invoice.</span></span> <span data-ttu-id="3bb22-124">Когато фактурата е осчетоводена, системата записва:</span><span class="sxs-lookup"><span data-stu-id="3bb22-124">When the invoice is posted, the system records:</span></span>
    
    - <span data-ttu-id="3bb22-125">Сумата на баланса на доставчика.</span><span class="sxs-lookup"><span data-stu-id="3bb22-125">The vendor balance amount.</span></span>
    - <span data-ttu-id="3bb22-126">Сумата на данъка продажби.</span><span class="sxs-lookup"><span data-stu-id="3bb22-126">The sales tax amount.</span></span>
    - <span data-ttu-id="3bb22-127">Разходите по проекта се записват в сметката за интеграция на обществени поръчки.</span><span class="sxs-lookup"><span data-stu-id="3bb22-127">The cost against the project is recorded to the procurement integration account.</span></span>
    - <span data-ttu-id="3bb22-128">Действителната транзакция на проекта в Dataverse.</span><span class="sxs-lookup"><span data-stu-id="3bb22-128">The project actual transaction in Dataverse.</span></span> <span data-ttu-id="3bb22-129">Тази транзакция се обработва допълнително с помощта на [Списание за интеграция на Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="3bb22-129">This transaction is further processed using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="3bb22-130">Публикуването на този дневник премества сумата от сметката за интеграция на обществени поръчки в сметката за разходите по проекта.</span><span class="sxs-lookup"><span data-stu-id="3bb22-130">Posting this journal moves the amount from the procurement integration account to the project cost account.</span></span>
