---
title: Защо не мога да изтривам записи от обекта „Действителни данни”?
description: Тази тема предоставя информация защо не можете да изтривате записи от обекта „Действителните данни“.
author: JPBurrows
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
ms.topic: article
ms.prod: Project Service
ms.technology: Applies to all versions of Project Service
ms.assetid: ff504c34-7337-474f-89e8-d8afdd1e0a98
ms.author: Jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5817940933c161dccac0fe549fabacbe57e7077a
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749238"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="37d73-103">Защо не мога да изтривам записи от обекта „Действителни данни”?</span><span class="sxs-lookup"><span data-stu-id="37d73-103">Why can’t I delete records from the Actuals entity?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="37d73-104">Project Service Automation (PSA) не ви позволява да изтривате действителни данни, защото те служат като източник на достоверни данни за транзакции, които имат финансови последици за системите надолу по веригата, като например счетоводната книга.</span><span class="sxs-lookup"><span data-stu-id="37d73-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="37d73-105">Ако действителните данни могат да бъдат изтрити, може да се постави под въпрос целостта на транзакциите за финансово отчитане.</span><span class="sxs-lookup"><span data-stu-id="37d73-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="37d73-106">За да установят одитна пътека, клиентите трябва да използват дневници за създаване на компенсиращи транзакции.</span><span class="sxs-lookup"><span data-stu-id="37d73-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

