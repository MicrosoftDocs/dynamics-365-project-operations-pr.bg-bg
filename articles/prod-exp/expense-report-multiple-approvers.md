---
title: Множество одобряващи за отчет за разходите
description: Тази тема предоставя информация за отчетите за разходите, които изискват одобрение от множество хора.
author: saraschi2
manager: AnnBe
ms.date: 02/23/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvExpensesReportList
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: ce24b156a268f9f5aada35f9314d2d9c6607200b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071976"
---
# <a name="multiple-approvers-on-an-expense-report"></a>Множество одобряващи за отчет за разходите

[!include [banner](../includes/banner.md)]

В зависимост от политиките за одобрение на разходите на вашата организация може да се наложи повече от едно лице да одобри отчет за разходите, подаден от служител. Когато настройвате процеса на работния поток за одобрение на отчета за разходите, можете да добавите елементи на работния поток, които включват задачи или стъпки за един или повече одобряващи отчета за разходите. Например може да изискате всички отчети за разходите да бъдат одобрени първо от мениджъра на служителя, който е представил отчета, и след това от координатора на задълженията по сметките.

Ако решите да изисквате множество одобряващи отчети за разходите, можете да добавите елементи на работния поток по всеки от следните начини:

- Добавете един елемент за одобрение, който има една стъпка. Например, стъпката може да изисква отчет за разходите да бъде присвоен на група потребители и да бъде одобрен от 50 процента от членовете на групата потребители.
- Добавете един елемент за одобрение, който има няколко стъпки. Например елементът за одобрение може да има следните стъпки:

    1. Управителят на служителя, подал отчета за разходите, го одобрява.
    2. Служителят по задълженията проверява разписките и елементите на отчета за разходите.
    3. Собственикът на бюджета одобрява отчета за разходите.

- Добавете множество елементи за одобрение, всеки от които има една стъпка. Например можете да добавите отделен елемент за одобрение за всяка от следните стъпки:

    1. Мениджърът на служителя одобрява отчета за разходите.
    2. Собственикът на бюджета одобрява отчета за разходите.