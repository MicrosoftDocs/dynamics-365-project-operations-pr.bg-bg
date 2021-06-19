---
title: Общ преглед на междуфирмено фактуриране
description: Тази тема предоставя информация и примери за междуфирмено фактуриране за проекти.
author: sigitac
ms.date: 11/19/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 42af89105f8325f1c94df6d2133d2c329facf2b3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6002628"
---
# <a name="intercompany-invoicing-overview"></a><span data-ttu-id="ca9de-103">Общ преглед на междуфирмено фактуриране</span><span class="sxs-lookup"><span data-stu-id="ca9de-103">Intercompany invoicing overview</span></span>

<span data-ttu-id="ca9de-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="ca9de-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="ca9de-105">Във вашата организация може да има множество подразделения, дъщерни дружества и други юридически лица, които прехвърлят продукти и услуги помежду си за проекти.</span><span class="sxs-lookup"><span data-stu-id="ca9de-105">Your organization might have multiple divisions, subsidiaries, and other legal entities that transfer products and services to each other for projects.</span></span> <span data-ttu-id="ca9de-106">Юридическото лице, което предоставя услугата или продукта, се нарича *кредитиращо юридическо лице*.</span><span class="sxs-lookup"><span data-stu-id="ca9de-106">The legal entity that provides the service or product is called the *lending legal entity*.</span></span> <span data-ttu-id="ca9de-107">Юридическото лице, което получава услугата или продукта, се нарича *получаващо юридическо лице*.</span><span class="sxs-lookup"><span data-stu-id="ca9de-107">The legal entity that receives the service or product is called the *borrowing legal entity*.</span></span>

<span data-ttu-id="ca9de-108">Следващата илюстрация показва типичен сценарий, при който две юридически лица, Contoso Robotics САЩ (заемащото юридическо лице) и Contoso Robotics ОК (кредитиращото юридическо лице) споделят ресурси, за да доставят проект за клиента Adventure works.</span><span class="sxs-lookup"><span data-stu-id="ca9de-108">The following illustration shows a typical scenario where two legal entities, Contoso Robotics USA (the borrowing legal entity) and Contoso Robotics UK (the lending legal entity) share resources to deliver a project for the customer, Adventure works.</span></span> <span data-ttu-id="ca9de-109">За този сценарий Contoso Robotics САЩ има договор за доставка на работата на Adventure Works.</span><span class="sxs-lookup"><span data-stu-id="ca9de-109">For this scenario, Contoso Robotics USA is contracted to deliver the work to Adventure Works.</span></span>

![Междуфирмено фактуриране](./media/IntercompanyScenario.png) 

<span data-ttu-id="ca9de-111">Dynamics 365 Project Operations използва следния поток за обработка на междуфирмени трансакции:</span><span class="sxs-lookup"><span data-stu-id="ca9de-111">Dynamics 365 Project Operations uses the following flow to process intercompany transactions:</span></span>

1. <span data-ttu-id="ca9de-112">Ресурсите от кредитиращото юридическо лице отчитат междуфирмените трансакции на време или разход, като резервират време и разходи по проекти в получаващото юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="ca9de-112">Resources from the lending legal entity record intercompany time or expense transactions by booking time and expense against projects in the borrowing legal entity.</span></span>
2. <span data-ttu-id="ca9de-113">Разходите за време и разход се записват в кредитиращата фирма, като се използва ценовата листа за себестойност на получаващата фирма.</span><span class="sxs-lookup"><span data-stu-id="ca9de-113">Time and expense costs are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
3. <span data-ttu-id="ca9de-114">Междуфирмените нефактурирани трансакции за продажби се записват в кредитиращата фирма, като се използва ценовата листа за себестойност на получаващата фирма.</span><span class="sxs-lookup"><span data-stu-id="ca9de-114">Intercompany unbilled sale transactions are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
4. <span data-ttu-id="ca9de-115">Нефактурираните приходи се записват в получаващата фирма, като се използва ценовата листа за продажби на договора по проект.</span><span class="sxs-lookup"><span data-stu-id="ca9de-115">Unbilled revenue is recorded in the borrowing company using the project contract sales price list.</span></span> <span data-ttu-id="ca9de-116">Може да се издаде фактура на клиента след записването на нефактурираните приходи.</span><span class="sxs-lookup"><span data-stu-id="ca9de-116">The customer can be billed when unbilled revenue is recorded.</span></span> <span data-ttu-id="ca9de-117">Не е необходимо клиентът да чака, докато обработката на междуфирмените фактури завърши.</span><span class="sxs-lookup"><span data-stu-id="ca9de-117">The customer doesn't have to wait until intercompany invoice processing is complete.</span></span>
5. <span data-ttu-id="ca9de-118">Междуфирмените клиентски фактури се създават периодично в кредитиращата фирма.</span><span class="sxs-lookup"><span data-stu-id="ca9de-118">Intercompany customer invoices are created on a periodic basis in the lending company.</span></span> <span data-ttu-id="ca9de-119">Фактурите се създават ръчно или чрез периодичен автоматизиран процес.</span><span class="sxs-lookup"><span data-stu-id="ca9de-119">The invoices are created manually or by using a periodic automated process.</span></span> <span data-ttu-id="ca9de-120">Може да се създаде една фактура за всяко получаващо юридическо лице или са се създадат отделни фактури по проект.</span><span class="sxs-lookup"><span data-stu-id="ca9de-120">A single invoice can be created for each borrowing legal entity or separate invoices can be created by project.</span></span>
6. <span data-ttu-id="ca9de-121">Когато междуфирмена клиентска фактура се публикува в кредитиращото юридическо лице, се създава съответната чакаща фактура на доставчик в получаващото юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="ca9de-121">When the intercompany customer invoice is posted in the lending legal entity, the corresponding pending vendor invoice is created in the borrowing legal entity.</span></span> <span data-ttu-id="ca9de-122">Разходите в чакащата фактура на доставчика ще бъдат записани в подкнигата на проекта, когато фактурата бъде публикувана.</span><span class="sxs-lookup"><span data-stu-id="ca9de-122">The costs in the pending vendor invoice will be recorded to the project subledger when the invoice is posted.</span></span>

<span data-ttu-id="ca9de-123">Следващата диаграма илюстрира междуфирменото фактуриране, тъй като се отнася до счетоводни събития и очаквани публикувания в главната книга.</span><span class="sxs-lookup"><span data-stu-id="ca9de-123">The following diagram illustrates intercompany invoicing as it relates to accounting events and expected postings to the general ledger.</span></span>

![Междуфирмен поток](./media/IntercompanyFlow.png)

## <a name="additional-resources"></a><span data-ttu-id="ca9de-125">Допълнителни ресурси</span><span class="sxs-lookup"><span data-stu-id="ca9de-125">Additional resources</span></span>

- [<span data-ttu-id="ca9de-126">Конфигуриране на междуфирмено фактуриране</span><span class="sxs-lookup"><span data-stu-id="ca9de-126">Configure intercompany invoicing</span></span>](configure-intercompany-invoicing.md)
- [<span data-ttu-id="ca9de-127">Запис на междуфирмени трансакции</span><span class="sxs-lookup"><span data-stu-id="ca9de-127">Record intercompany transactions</span></span>](create-intercompany-transactions.md)
- [<span data-ttu-id="ca9de-128">Създаване на междуфирмени фактури за клиенти и доставчици</span><span class="sxs-lookup"><span data-stu-id="ca9de-128">Create intercompany customer and vendor invoices</span></span>](create-intercompany-customer-vendor-invoices.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]