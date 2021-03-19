---
title: Създаване на ръчна проформа фактура – олекотено
description: Тази тема предоставя информация за създаване на ръчна проформа фактура в Project Operations.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 104c2f3f7f0ca0682158d0f7fa0f50a4967e6dd0
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274175"
---
# <a name="create-a-manual-proforma-invoice---lite"></a><span data-ttu-id="cc015-103">Създаване на ръчна проформа фактура – олекотено</span><span class="sxs-lookup"><span data-stu-id="cc015-103">Create a manual proforma invoice - lite</span></span>

<span data-ttu-id="cc015-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="cc015-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cc015-105">В Dynamics 365 Project Operations проформа фактурите могат да се създават ръчно, ако е необходимо.</span><span class="sxs-lookup"><span data-stu-id="cc015-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="cc015-106">Можете ръчно да създадете проформа фактура от **Договори за проекти** страница от списъка или от **Договор за проект** страница с подробности.</span><span class="sxs-lookup"><span data-stu-id="cc015-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="cc015-107">Страница със списък на договори по проекта</span><span class="sxs-lookup"><span data-stu-id="cc015-107">Project Contracts list page</span></span>

<span data-ttu-id="cc015-108">От страница със списък **Договори за проекти**, изберете един или повече договори за проекти и създайте фактури за всички избрани записи.</span><span class="sxs-lookup"><span data-stu-id="cc015-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="cc015-109">Системата проверява кой от избраните договори за проекти има **Готови за фактуриране** изоставане, датирано преди днешната дата.</span><span class="sxs-lookup"><span data-stu-id="cc015-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog dated before today's date.</span></span> <span data-ttu-id="cc015-110">От тези договори системата създава проекти на проформа фактури.</span><span class="sxs-lookup"><span data-stu-id="cc015-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="cc015-111">Ако проектният договор има множество клиенти, може да има една фактура, създадена на клиент, и няколко фактури за договор за проект.</span><span class="sxs-lookup"><span data-stu-id="cc015-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="cc015-112">Всички създадени фактури по проекта са достъпни в **Фактура** страница в секцията **Таксуване** на област **Продажби**.</span><span class="sxs-lookup"><span data-stu-id="cc015-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="cc015-113">Страница с подробности за договор по проект</span><span class="sxs-lookup"><span data-stu-id="cc015-113">Project Contract details page</span></span>

<span data-ttu-id="cc015-114">Проформа фактура също може да бъде създадена от страницата с подробности **Договор за проект**.</span><span class="sxs-lookup"><span data-stu-id="cc015-114">A proforma invoice can also be created from the **Project Contract** details page.</span></span> <span data-ttu-id="cc015-115">Системата проверява дали договорът на проекта има **Готово за фактуриране** изоставане, датирано преди днешната дата.</span><span class="sxs-lookup"><span data-stu-id="cc015-115">The system verifies the project contract has a **Ready to Invoice** backlog dated before today's date.</span></span> <span data-ttu-id="cc015-116">От тези договори системата създава проекти на проформа фактури въз основа на броя клиенти по всеки ред на договора.</span><span class="sxs-lookup"><span data-stu-id="cc015-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="cc015-117">Когато е създадена една проформа фактура, страница **Фактура** се отваря.</span><span class="sxs-lookup"><span data-stu-id="cc015-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="cc015-118">Ако за този договор за проект са създадени множество фактури, **Фактури** се отваря страница със списък, за да се покажат всички създадени фактури.</span><span class="sxs-lookup"><span data-stu-id="cc015-118">If multiple invoices are created for that project contract, the **Invoices** list page opens to show all of the created invoices.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]