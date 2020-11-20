---
title: Потвърждение на договор по проект
description: Тази тема предоставя информация за това как да потвърдите договор в Project Operations.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 24da0887c0266d51bddcbbf8efd6f2644b6d0f4f
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128270"
---
# <a name="confirm-a-project-contract"></a><span data-ttu-id="c4722-103">Потвърждение на договор по проект</span><span class="sxs-lookup"><span data-stu-id="c4722-103">Confirm a project contract</span></span>

<span data-ttu-id="c4722-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="c4722-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c4722-105">Договор за проект в Dynamics 365 Project Operations може да бъде активен с причина **Потвърдено**, или затворени с причина **Изгубени**.</span><span class="sxs-lookup"><span data-stu-id="c4722-105">A project contract in Dynamics 365 Project Operations can be active with a reason of **Confirmed**, or closed with a reason of **Lost**.</span></span> <span data-ttu-id="c4722-106">Когато потвърдите договор за проект, състоянието се актуализира от **Чернова** на **Активен** и описание на състоянието е **Потвърдено**.</span><span class="sxs-lookup"><span data-stu-id="c4722-106">When you confirm a project contract, the status updates from **Draft** to **Active** and the status reason is **Confirmed**.</span></span> <span data-ttu-id="c4722-107">Активен или затворен договор не може да бъде редактиран или отворен.</span><span class="sxs-lookup"><span data-stu-id="c4722-107">An active or closed contract can't be edited or reopened.</span></span> 

### <a name="financial-impact-of-confirming-a-project-contract"></a><span data-ttu-id="c4722-108">Финансово въздействие от потвърждаване на договор за проект</span><span class="sxs-lookup"><span data-stu-id="c4722-108">Financial impact of confirming a project contract</span></span>

<span data-ttu-id="c4722-109">След потвърждаването на договор по проект приложението ще преизчисли разходите, като обърне по-старите фактически разходи и ще създаде нови действителни разходи.</span><span class="sxs-lookup"><span data-stu-id="c4722-109">After a project contract is confirmed, the application recalculates the costs by reversing the older cost actuals and creating new cost actuals.</span></span> <span data-ttu-id="c4722-110">Новите действителни данни за разходи след това се обработват въз основа на метода на фактуриране на свързаната линия на договор за проект.</span><span class="sxs-lookup"><span data-stu-id="c4722-110">The new cost actuals are then processed based on the billing method of the associated project contract line.</span></span> <span data-ttu-id="c4722-111">Ако действителните разходи се позовават на ред за договор за време и материали, приложението автоматично пресъздава съответните актуализирани факти за продажби.</span><span class="sxs-lookup"><span data-stu-id="c4722-111">If the cost actuals reference a Time and Material contract line, the application automatically re-creates corresponding unbilled sales actuals.</span></span> <span data-ttu-id="c4722-112">Ако действителните разходи се позовават на договорна линия с фиксирана цена, приложението спира да обработва действителните факти.</span><span class="sxs-lookup"><span data-stu-id="c4722-112">If the cost actuals reference a Fixed Price contract line, the application stops reprocessing the cost actuals.</span></span>

<span data-ttu-id="c4722-113">Лимитите, които не трябва да надвишават, настройката за таксуване и ценообразуването и цената на актуалните данни се оценяват и след това актуализират като част от процеса на потвърждаване.</span><span class="sxs-lookup"><span data-stu-id="c4722-113">Not-to-exceed limits, chargeability setup, and pricing and costing on the actuals is evaluated and then updated as part of the confirmations process.</span></span>

## <a name="close-a-project-contract-as-lost"></a><span data-ttu-id="c4722-114">Приключване на договор по проект като загубен</span><span class="sxs-lookup"><span data-stu-id="c4722-114">Close a project contract as lost</span></span>

<span data-ttu-id="c4722-115">Когато затворите договор за проект като загубен, състоянието на договора се актуализира на **Затворено** и описание на състоянието е **Изгубено**.</span><span class="sxs-lookup"><span data-stu-id="c4722-115">When you close a project contract as lost, the contract status is updated to **Closed** and the status reason is **Lost**.</span></span> <span data-ttu-id="c4722-116">Проектният договор става само за четене.</span><span class="sxs-lookup"><span data-stu-id="c4722-116">The project contract becomes read-only.</span></span> <span data-ttu-id="c4722-117">Предоставя се диалогов прозорец за потвърждение, преди промените да приключат, тъй като не можете да отворите отново затворен договор за проект.</span><span class="sxs-lookup"><span data-stu-id="c4722-117">A confirmation dialog is provided before the changes are complete because you can't reopen a closed project contract.</span></span>

<span data-ttu-id="c4722-118">Ако проектният договор, който е затворен като изгубен, препраща проект към неговите линии, този проект също се маркира като затворен.</span><span class="sxs-lookup"><span data-stu-id="c4722-118">If the project contract that is closed as lost references a project on its lines, that project is also marked as closed.</span></span> <span data-ttu-id="c4722-119">Всички резервации на ресурси от този ден нататък се анулират.</span><span class="sxs-lookup"><span data-stu-id="c4722-119">Any resource bookings from that day forward are canceled.</span></span> <span data-ttu-id="c4722-120">Всички нефактурирани факти по продажбите по договора за проект, които не са вече във фактура, ще бъдат отменени.</span><span class="sxs-lookup"><span data-stu-id="c4722-120">Any unbilled sales actuals on the project contract that aren't already on an invoice, will be reversed.</span></span>

> [!NOTE]
> <span data-ttu-id="c4722-121">В Dynamics 365 Project Operations затварянето на договор за проект като загубен няма да повлияе на състоянието на свързаната възможност.</span><span class="sxs-lookup"><span data-stu-id="c4722-121">In Dynamics 365 Project Operations, closing a project contract as lost will not impact that status of the associated opportunity.</span></span> <span data-ttu-id="c4722-122">Възможността ще остане отворена и трябва да бъде ръчно затворена.</span><span class="sxs-lookup"><span data-stu-id="c4722-122">The opportunity will remain open and must be manually closed.</span></span>
