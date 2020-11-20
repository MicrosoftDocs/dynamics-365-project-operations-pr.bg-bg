---
title: Създаване на ръчна проформа фактура – олекотено
description: Тази тема предоставя информация за създаване на ръчна проформа фактура в Project Operations.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 87ef090454b2a7ab997e7c21d8d10badc31c8235
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176373"
---
# <a name="create-a-manual-proforma-invoice---lite"></a><span data-ttu-id="25d7f-103">Създаване на ръчна проформа фактура – олекотено</span><span class="sxs-lookup"><span data-stu-id="25d7f-103">Create a manual proforma invoice - lite</span></span>

<span data-ttu-id="25d7f-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="25d7f-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="25d7f-105">В Dynamics 365 Project Operations проформа фактурите могат да се създават ръчно, ако е необходимо.</span><span class="sxs-lookup"><span data-stu-id="25d7f-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="25d7f-106">Можете ръчно да създадете проформа фактура от **Договори за проекти** страница от списъка или от **Договор за проект** страница с подробности.</span><span class="sxs-lookup"><span data-stu-id="25d7f-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="25d7f-107">Страница със списък на договори по проекта</span><span class="sxs-lookup"><span data-stu-id="25d7f-107">Project Contracts list page</span></span>

<span data-ttu-id="25d7f-108">От страница със списък **Договори за проекти**, изберете един или повече договори за проекти и създайте фактури за всички избрани записи.</span><span class="sxs-lookup"><span data-stu-id="25d7f-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="25d7f-109">Системата проверява кой от избраните договори за проекти има **Готови за фактуриране** изоставане, датирано преди днешната дата.</span><span class="sxs-lookup"><span data-stu-id="25d7f-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog  dated before today's date.</span></span> <span data-ttu-id="25d7f-110">От тези договори системата създава проекти на проформа фактури.</span><span class="sxs-lookup"><span data-stu-id="25d7f-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="25d7f-111">Ако проектният договор има множество клиенти, може да има една фактура, създадена на клиент, и няколко фактури за договор за проект.</span><span class="sxs-lookup"><span data-stu-id="25d7f-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="25d7f-112">Всички създадени фактури по проекта са достъпни в **Фактура** страница в секцията **Таксуване** на област **Продажби**.</span><span class="sxs-lookup"><span data-stu-id="25d7f-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="25d7f-113">Страница с подробности за договор по проект</span><span class="sxs-lookup"><span data-stu-id="25d7f-113">Project Contract details page</span></span>

<span data-ttu-id="25d7f-114">Проформа фактура също може да бъде създадена от страница с подробности **Договор за проект**, която създава фактура за конкретния договор за проект.</span><span class="sxs-lookup"><span data-stu-id="25d7f-114">A proforma invoice can also be created from the **Project Contract** details page, which creates the invoice for that specific project contract.</span></span> <span data-ttu-id="25d7f-115">Системата проверява кой от избраните договори по проекти има изоставане **Готови за фактуриране**, датирано преди днешната дата.</span><span class="sxs-lookup"><span data-stu-id="25d7f-115">The system verifies that the project contract has a **Ready to Invoice** backlog that is dated before today's date.</span></span> <span data-ttu-id="25d7f-116">От тези договори системата създава проекти на проформа фактури въз основа на броя клиенти по всеки ред на договора.</span><span class="sxs-lookup"><span data-stu-id="25d7f-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="25d7f-117">Когато е създадена една проформа фактура, страница **Фактура** се отваря.</span><span class="sxs-lookup"><span data-stu-id="25d7f-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="25d7f-118">Ако за този договор за проект са създадени множество фактури, тогава **Фактури** се отваря страница със списък, за да се покажат всички създадени фактури.</span><span class="sxs-lookup"><span data-stu-id="25d7f-118">If there are multiple invoices created for that project contract, then the **Invoices** list page opens to show all of the created invoices.</span></span>
