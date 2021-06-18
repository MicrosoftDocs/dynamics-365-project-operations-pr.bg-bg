---
title: Затваряне на оферта – олекотено
description: Тази тема предоставя информация за приключването на оферта в Project Operations.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 75345fed57dcbdb84f2a82587c7d0c152530c72b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994123"
---
# <a name="close-a-quote---lite"></a><span data-ttu-id="ddea5-103">Затваряне на оферта – олекотено</span><span class="sxs-lookup"><span data-stu-id="ddea5-103">Close a quote - lite</span></span>

<span data-ttu-id="ddea5-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="ddea5-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ddea5-105">Офертата на проекта може да бъде затворена като Спечелена или Изгубена.</span><span class="sxs-lookup"><span data-stu-id="ddea5-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="ddea5-106">Чернова на оферта може да бъде затворена, тъй като операциите за активиране и преразглеждане на оферти не се поддържат в Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="ddea5-106">A draft quote can be closed because the Activate and Revise operations on quotes isn't supported in Microsoft Dynamics 365 Project Operations.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="ddea5-107">Затваряне на оферта като спечелена</span><span class="sxs-lookup"><span data-stu-id="ddea5-107">Close a quote as Won</span></span>

<span data-ttu-id="ddea5-108">Когато затворите оферта за проект като „Спечелена”, състоянието е настроено на „Затворено” и описание на състоянието е „Спечелено”.</span><span class="sxs-lookup"><span data-stu-id="ddea5-108">When you close a project quote as Won, the status is set to Closed and the status reason is Won.</span></span> <span data-ttu-id="ddea5-109">Затварянето на оферта прави проекта само за четене и създава проект на договор за проект, който съдържа информацията за офертите.</span><span class="sxs-lookup"><span data-stu-id="ddea5-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="ddea5-110">Тъй като затворената оферта не може да бъде отворена отново, диалоговият прозорец за потвърждение ще потвърди вашите промени.</span><span class="sxs-lookup"><span data-stu-id="ddea5-110">Because a closed quote can't be reopened, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="ddea5-111">Ако офертата е прикрепена към възможност, всички други проектни оферти за възможността автоматично се затварят като Изгубени.</span><span class="sxs-lookup"><span data-stu-id="ddea5-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="ddea5-112">Финансово въздействие от затварянето на котировка като спечелена</span><span class="sxs-lookup"><span data-stu-id="ddea5-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="ddea5-113">Ако има действителни факти за времето на даден проект, докато все още е приложен към проектна оферта, се записват само разходите за времето или разходите.</span><span class="sxs-lookup"><span data-stu-id="ddea5-113">If there are any actuals for time on a project while is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="ddea5-114">След като офертата бъде затворена като спечелена, приложението ще рефакторира разходите, като обърне по-старите фактически разходи и ще създаде нови действителни разходи.</span><span class="sxs-lookup"><span data-stu-id="ddea5-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="ddea5-115">Заявлението ще обработи тези фактически факти за разходите въз основа на метода за фактуриране на свързаната линия на договор за проект.</span><span class="sxs-lookup"><span data-stu-id="ddea5-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="ddea5-116">Ако фактическите факти за разходите се позовават на ред за договор за време и материал, се създават съответни факти за нефактурирани продажби, когато офертата е затворена и проектният договор е създаден.</span><span class="sxs-lookup"><span data-stu-id="ddea5-116">If the cost actuals reference a time and material contract line, corresponding unbilled sales actuals are created for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="ddea5-117">Ако фактическите факти за разходите се позовават на договорна линия с фиксирана цена, приложението ще спре да преработва действителните разходи, които се основават на правилата за разделено фактуриране за клиентите по проекта.</span><span class="sxs-lookup"><span data-stu-id="ddea5-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals that are based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="ddea5-118">Затваряне на оферта като загубена:</span><span class="sxs-lookup"><span data-stu-id="ddea5-118">Closing a quote as lost:</span></span>

<span data-ttu-id="ddea5-119">Когато затворите оферта за проект като „Загубена”, състоянието е настроено на „Затворено” и описание на състоянието е „Загубено”.</span><span class="sxs-lookup"><span data-stu-id="ddea5-119">When you close a project quote as Lost, the status is set to Closed and status reason is Lost.</span></span> <span data-ttu-id="ddea5-120">Затварянето на офертата прави проектната оферта само за четене.</span><span class="sxs-lookup"><span data-stu-id="ddea5-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="ddea5-121">Тъй като затворена оферта не може да бъде отворена отново и преди да затворите оферта, диалоговият прозорец за потвърждение ще потвърди вашите промени.</span><span class="sxs-lookup"><span data-stu-id="ddea5-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="ddea5-122">Ако офертата на проекта, която е затворена като „Загубено”, препраща към проект по някой от неговите редове, този проект също е маркиран като „Затворено”.</span><span class="sxs-lookup"><span data-stu-id="ddea5-122">If the project quote that is closed as Lost references a project on any of its lines, that project is also marked as Closed.</span></span> <span data-ttu-id="ddea5-123">Всички резервации на ресурси от този ден нататък се анулират.</span><span class="sxs-lookup"><span data-stu-id="ddea5-123">Any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="ddea5-124">В Project Operations затварянето на оферта като спечелена или загубена няма да повлияе на това състояние на възможността, която ще остане отворена, докато не бъде ръчно затворена.</span><span class="sxs-lookup"><span data-stu-id="ddea5-124">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]