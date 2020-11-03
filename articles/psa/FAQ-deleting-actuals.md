---
title: Защо не мога да изтривам записи от обекта „Действителни данни”?
description: Тази тема предоставя информация защо не можете да изтривате записи от обекта „Действителните данни“.
author: JPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: f47e7ccd46642dc6129fbb3beac3c9490160d046
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071946"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="89ef6-103">Защо не мога да изтривам записи от обекта „Действителни данни”?</span><span class="sxs-lookup"><span data-stu-id="89ef6-103">Why can’t I delete records from the Actuals entity?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="89ef6-104">Project Service Automation (PSA) не ви позволява да изтривате действителни данни, защото те служат като източник на достоверни данни за транзакции, които имат финансови последици за системите надолу по веригата, като например счетоводната книга.</span><span class="sxs-lookup"><span data-stu-id="89ef6-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="89ef6-105">Ако действителните данни могат да бъдат изтрити, може да се постави под въпрос целостта на транзакциите за финансово отчитане.</span><span class="sxs-lookup"><span data-stu-id="89ef6-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="89ef6-106">За да установят одитна пътека, клиентите трябва да използват дневници за създаване на компенсиращи транзакции.</span><span class="sxs-lookup"><span data-stu-id="89ef6-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

