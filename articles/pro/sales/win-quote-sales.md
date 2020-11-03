---
title: Приключване на оферти
description: Тази тема предоставя информация за приключването на оферта в Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: cc3b2cdeb1ac46b7d927c1f96e94e9154d3eebf8
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071741"
---
# <a name="close-quotes"></a><span data-ttu-id="dd970-103">Приключване на оферти</span><span class="sxs-lookup"><span data-stu-id="dd970-103">Close quotes</span></span> 

<span data-ttu-id="dd970-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="dd970-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="dd970-105">Офертата на проекта може да бъде затворена като Спечелена или Изгубена.</span><span class="sxs-lookup"><span data-stu-id="dd970-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="dd970-106">Операциите Активиране и Ревизиране не се поддържат в Microsoft Dynamics 365 Project Operations, така че офертата в чернова може да бъде затворена.</span><span class="sxs-lookup"><span data-stu-id="dd970-106">The Activate and Revise operations on quotes is not supported in Microsoft Dynamics 365 Project Operations, so a draft quote can be closed.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="dd970-107">Затваряне на оферта като спечелена</span><span class="sxs-lookup"><span data-stu-id="dd970-107">Close a quote as Won</span></span>

<span data-ttu-id="dd970-108">Затварянето на оферта на проект като спечелена ще затвори офертата със състояние Затворено и описание на състоянието Спечелена.</span><span class="sxs-lookup"><span data-stu-id="dd970-108">Closing a project quote as Won will close the quote with the status set to Closed and the status reason set to Won.</span></span> <span data-ttu-id="dd970-109">Затварянето на оферта прави проекта само за четене и създава проект на договор за проект, който съдържа информацията за офертите.</span><span class="sxs-lookup"><span data-stu-id="dd970-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="dd970-110">Тъй като затворената оферта не може да бъде отворена отново, диалогов прозорец за потвърждение Съществува диалогов прозорец за потвърждение, преди промените да бъдат извършени, тъй като затворената оферта не може да бъде отворена отново и промените са необратими.</span><span class="sxs-lookup"><span data-stu-id="dd970-110">Because a closed quote can't be reopened, a confirmation dialog There is a confirmation dialog before the changes are done since a closed quote cannot be re-opened and the changes are irreversible.</span></span>

<span data-ttu-id="dd970-111">Ако офертата е прикрепена към възможност, всички други проектни оферти за възможността автоматично се затварят като Изгубени.</span><span class="sxs-lookup"><span data-stu-id="dd970-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="dd970-112">Финансово въздействие от затварянето на котировка като спечелена</span><span class="sxs-lookup"><span data-stu-id="dd970-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="dd970-113">Ако има фактически данни за времето, записано в даден проект, докато той все още е приложен към проектна оферта, се записват само разходите за времето или разходите.</span><span class="sxs-lookup"><span data-stu-id="dd970-113">If there have been any actuals for time recorded on a project while it is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="dd970-114">След като офертата бъде затворена като спечелена, приложението ще рефакторира разходите, като обърне по-старите фактически разходи и ще създаде нови действителни разходи.</span><span class="sxs-lookup"><span data-stu-id="dd970-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="dd970-115">Заявлението ще обработи тези фактически факти за разходите въз основа на метода за фактуриране на свързаната линия на договор за проект.</span><span class="sxs-lookup"><span data-stu-id="dd970-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="dd970-116">Ако фактическите факти за разходите се позовават на ред за времеви и материален договор, системата автоматично ще създаде съответни действителни факти за нефактурирани продажби, когато офертата е затворена и проектният договор е създаден.</span><span class="sxs-lookup"><span data-stu-id="dd970-116">If the cost actuals reference a time and material contract line, the system will automatically create corresponding unbilled sales actuals for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="dd970-117">Ако фактическите факти за разходите се позовават на договорна линия с фиксирана цена, приложението ще спре да обработва действителните факти за разходите въз основа на правилата за разделено фактуриране за клиентите по проекта.</span><span class="sxs-lookup"><span data-stu-id="dd970-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="dd970-118">Затваряне на оферта като загубена:</span><span class="sxs-lookup"><span data-stu-id="dd970-118">Closing a quote as lost:</span></span>

<span data-ttu-id="dd970-119">Затварянето на офертата на проекта като загубена, ще зададе статуса на Затворено и описание на състоянието на Загубена.</span><span class="sxs-lookup"><span data-stu-id="dd970-119">Closing a project quote as Lost will set the status to Closed and status reason to Lost.</span></span> <span data-ttu-id="dd970-120">Затварянето на офертата прави проектната оферта само за четене.</span><span class="sxs-lookup"><span data-stu-id="dd970-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="dd970-121">Тъй като затворена оферта не може да бъде отворена отново и преди да затворите оферта, диалоговият прозорец за потвърждение ще потвърди вашите промени.</span><span class="sxs-lookup"><span data-stu-id="dd970-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="dd970-122">Ако офертата на проекта, която е затворена като Lost, има проект, посочен в някой от неговите редове, този проект също е маркиран като Затворен и всички резервации на ресурси от този ден напред се анулират.</span><span class="sxs-lookup"><span data-stu-id="dd970-122">If the project quote that is closed as Lost has a project referenced on any of its lines, that project is also marked as Closed and any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="dd970-123">В Project Operations затварянето на оферта като спечелена или загубена няма да повлияе на това състояние на възможността, която ще остане отворена, докато не бъде ръчно затворена.</span><span class="sxs-lookup"><span data-stu-id="dd970-123">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>
