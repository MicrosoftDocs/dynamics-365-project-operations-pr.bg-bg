---
title: Коригирани фактури
description: Тази тема предоставя информация за коригираните фактури.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: e14da1c07d5b697de6caf1b9041c30581ecff102
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898068"
---
# <a name="corrected-invoices"></a><span data-ttu-id="01191-103">Коригирани фактури</span><span class="sxs-lookup"><span data-stu-id="01191-103">Corrected invoices</span></span>

<span data-ttu-id="01191-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="01191-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="01191-105">Потвърдени фактури могат да бъдат редактирани.</span><span class="sxs-lookup"><span data-stu-id="01191-105">Confirmed invoices can be edited.</span></span> <span data-ttu-id="01191-106">Когато редактирате потвърдена фактура, се създава чернова на коригираната фактура.</span><span class="sxs-lookup"><span data-stu-id="01191-106">When you edit a confirmed invoice, a draft of the corrected invoice is created.</span></span> <span data-ttu-id="01191-107">Тъй като се предполага, че искате да сторнирате всички транзакции и количества от първоначалната фактура, коригираната фактура включва всички транзакции от оригиналната фактура и всички количества в нея са нула (0).</span><span class="sxs-lookup"><span data-stu-id="01191-107">Because the assumption is that you want to reverse all the transactions and quantities from the original invoice, the corrected invoice includes all the transactions from the original invoice, and all the quantities on it are zero (0).</span></span>

<span data-ttu-id="01191-108">Когато транзакциите не изискват корекция, можете да ги премахнете от черновата на коригираща фактура.</span><span class="sxs-lookup"><span data-stu-id="01191-108">When transactions don't require correction, you can remove them from the draft corrective invoice.</span></span> <span data-ttu-id="01191-109">Ако сторнирате или върнете само частично количество, можете да редактирате полето Количество в подробностите за реда.</span><span class="sxs-lookup"><span data-stu-id="01191-109">To reverse or return only a partial quantity, you can edit the Quantity field on the line detail.</span></span> <span data-ttu-id="01191-110">Ако отворите подробностите за реда на фактурата, можете да видите количеството в първоначалната фактура.</span><span class="sxs-lookup"><span data-stu-id="01191-110">If you open the invoice line detail, you can see the original invoice quantity.</span></span> <span data-ttu-id="01191-111">След това можете да редактирате количеството в текущата фактура, така че да е по-малко или повече от количеството в първоначалната фактура.</span><span class="sxs-lookup"><span data-stu-id="01191-111">You can then edit the current invoice quantity so that it's less than or more than the original invoice quantity.</span></span>

<span data-ttu-id="01191-112">Когато потвърдите коригираща фактура, първоначално фактурираните действителни продажби се сторнират и се създават нови фактурирани действителни продажби.</span><span class="sxs-lookup"><span data-stu-id="01191-112">When you confirm a corrective invoice, the original billed sales actual is reversed, and a new billed sales actual is created.</span></span> <span data-ttu-id="01191-113">Ако количеството е било намалено, разликата ще доведе до създаването също и на нова нефактурирана действителна продажба.</span><span class="sxs-lookup"><span data-stu-id="01191-113">If the quantity was reduced, the difference will cause a new unbilled sales actual to be created too.</span></span> <span data-ttu-id="01191-114">Например, ако първоначалната фактурирана продажба са били за осем часа, а подробностите на реда на коригираната фактура имат намалено количество от шест часа, редът на първоначално фактурираната продажба се сторнира и създава две нови действителни данни:</span><span class="sxs-lookup"><span data-stu-id="01191-114">For example, if the original billed sale was for eight hours, and the corrected invoice line detail has a reduced quantity of six hours, the original billed sales line is revered and two new actuals are created:</span></span>

- <span data-ttu-id="01191-115">фактурирана действителна продажба за шест часа.</span><span class="sxs-lookup"><span data-stu-id="01191-115">A billed sales actual for six hours.</span></span>
- <span data-ttu-id="01191-116">нефактурирана действителна продажба за оставащите два часа.</span><span class="sxs-lookup"><span data-stu-id="01191-116">An unbilled sales actual for the remaining two hours.</span></span> <span data-ttu-id="01191-117">Тази транзакция може или да бъде фактурирана по-късно, или отбелязана като неплатима, в зависимост от договорките с клиента.</span><span class="sxs-lookup"><span data-stu-id="01191-117">This transaction can either be billed later or marked as non-chargeable, depending on the negotiations with the customer.</span></span>
