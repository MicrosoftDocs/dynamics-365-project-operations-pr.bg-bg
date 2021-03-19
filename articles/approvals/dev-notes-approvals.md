---
title: Бележки на разработчик за одобрения
description: Тази тема предоставя допълнителна информация за разработчици за работа с одобрения.
author: stsporen
manager: Annbe
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: d58c776b0341c08b0292e1b459a7d7ebac550bcc
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290256"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="e997a-103">Бележки на разработчик за одобрения</span><span class="sxs-lookup"><span data-stu-id="e997a-103">Developer notes for Approvals</span></span>

<span data-ttu-id="e997a-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="e997a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e997a-105">Dynamics 365 Project Operations включва логика за проверка, която осигурява правилен преход на записа през етапите на одобрение.</span><span class="sxs-lookup"><span data-stu-id="e997a-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="e997a-106">Правилните преходи на записи осигуряват:</span><span class="sxs-lookup"><span data-stu-id="e997a-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="e997a-107">Всички поддържащи редове са създадени в свързани таблици, като журнали и действителни данни.</span><span class="sxs-lookup"><span data-stu-id="e997a-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="e997a-108">Одобряващият е маркиран като **Одобряващ на проект** в проекта, преди да продължите.</span><span class="sxs-lookup"><span data-stu-id="e997a-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]