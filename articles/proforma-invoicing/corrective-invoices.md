---
title: Коригирани фактури
description: Тази тема предоставя информация за коригираните фактури.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 1ebfec053a59bbadd261d4333f6737cf16292e81
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122375"
---
# <a name="corrected-invoices"></a><span data-ttu-id="02681-103">Коригирани фактури</span><span class="sxs-lookup"><span data-stu-id="02681-103">Corrected invoices</span></span>

<span data-ttu-id="02681-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="02681-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="02681-105">Потвърдени фактури могат да бъдат редактирани.</span><span class="sxs-lookup"><span data-stu-id="02681-105">Confirmed invoices can be edited.</span></span> <span data-ttu-id="02681-106">Когато редактирате потвърдена фактура, се създава чернова на коригираната фактура.</span><span class="sxs-lookup"><span data-stu-id="02681-106">When you edit a confirmed invoice, a draft of the corrected invoice is created.</span></span> <span data-ttu-id="02681-107">Тъй като се предполага, че искате да сторнирате всички транзакции и количества от първоначалната фактура, коригираната фактура включва всички транзакции от оригиналната фактура и всички количества в нея са нула (0).</span><span class="sxs-lookup"><span data-stu-id="02681-107">Because the assumption is that you want to reverse all the transactions and quantities from the original invoice, the corrected invoice includes all the transactions from the original invoice, and all the quantities on it are zero (0).</span></span>

<span data-ttu-id="02681-108">Когато транзакциите не изискват корекция, можете да ги премахнете от черновата на коригираща фактура.</span><span class="sxs-lookup"><span data-stu-id="02681-108">When transactions don't require correction, you can remove them from the draft corrective invoice.</span></span> <span data-ttu-id="02681-109">Ако сторнирате или върнете само частично количество, можете да редактирате полето Количество в подробностите за реда.</span><span class="sxs-lookup"><span data-stu-id="02681-109">To reverse or return only a partial quantity, you can edit the Quantity field on the line detail.</span></span> <span data-ttu-id="02681-110">Ако отворите подробностите за реда на фактурата, можете да видите количеството в първоначалната фактура.</span><span class="sxs-lookup"><span data-stu-id="02681-110">If you open the invoice line detail, you can see the original invoice quantity.</span></span> <span data-ttu-id="02681-111">След това можете да редактирате количеството в текущата фактура, така че да е по-малко или повече от количеството в първоначалната фактура.</span><span class="sxs-lookup"><span data-stu-id="02681-111">You can then edit the current invoice quantity so that it's less than or more than the original invoice quantity.</span></span>

<span data-ttu-id="02681-112">Когато потвърдите коригираща фактура, първоначално фактурираните действителни продажби се сторнират и се създават нови фактурирани действителни продажби.</span><span class="sxs-lookup"><span data-stu-id="02681-112">When you confirm a corrective invoice, the original billed sales actual is reversed, and a new billed sales actual is created.</span></span> <span data-ttu-id="02681-113">Ако количеството е било намалено, разликата ще доведе до създаването също и на нова нефактурирана действителна продажба.</span><span class="sxs-lookup"><span data-stu-id="02681-113">If the quantity was reduced, the difference will cause a new unbilled sales actual to be created too.</span></span> <span data-ttu-id="02681-114">Например, ако първоначалната фактурирана продажба са били за осем часа, а подробностите на реда на коригираната фактура имат намалено количество от шест часа, редът на първоначално фактурираната продажба се сторнира и създава две нови действителни данни:</span><span class="sxs-lookup"><span data-stu-id="02681-114">For example, if the original billed sale was for eight hours, and the corrected invoice line detail has a reduced quantity of six hours, the original billed sales line is revered and two new actuals are created:</span></span>

- <span data-ttu-id="02681-115">фактурирана действителна продажба за шест часа.</span><span class="sxs-lookup"><span data-stu-id="02681-115">A billed sales actual for six hours.</span></span>
- <span data-ttu-id="02681-116">нефактурирана действителна продажба за оставащите два часа.</span><span class="sxs-lookup"><span data-stu-id="02681-116">An unbilled sales actual for the remaining two hours.</span></span> <span data-ttu-id="02681-117">Тази транзакция може или да бъде фактурирана по-късно, или отбелязана като неплатима, в зависимост от договорките с клиента.</span><span class="sxs-lookup"><span data-stu-id="02681-117">This transaction can either be billed later or marked as non-chargeable, depending on the negotiations with the customer.</span></span>
