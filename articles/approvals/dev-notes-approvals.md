---
title: Бележки на разработчик за одобрения
description: Тази тема предоставя допълнителна информация за разработчици за работа с одобрения.
author: stsporen
ms.date: 11/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: a89ea669a262c145b9f391fddc19e79a425fabb5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996778"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="a1c93-103">Бележки на разработчик за одобрения</span><span class="sxs-lookup"><span data-stu-id="a1c93-103">Developer notes for Approvals</span></span>

<span data-ttu-id="a1c93-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="a1c93-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a1c93-105">Dynamics 365 Project Operations включва логика за проверка, която осигурява правилен преход на записа през етапите на одобрение.</span><span class="sxs-lookup"><span data-stu-id="a1c93-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="a1c93-106">Правилните преходи на записи осигуряват:</span><span class="sxs-lookup"><span data-stu-id="a1c93-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="a1c93-107">Всички поддържащи редове са създадени в свързани таблици, като журнали и действителни данни.</span><span class="sxs-lookup"><span data-stu-id="a1c93-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="a1c93-108">Одобряващият е маркиран като **Одобряващ на проект** в проекта, преди да продължите.</span><span class="sxs-lookup"><span data-stu-id="a1c93-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]