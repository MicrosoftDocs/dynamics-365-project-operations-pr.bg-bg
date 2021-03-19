---
title: Какво е новото или промененото в Project Service Automation, версия 3.x, вълна 1, 2020 г.
description: Тази тема предоставя информация за това какво е новото и промененото в Project Service Automation, версия 3, вълна 1, 2020 г.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 05/15/2020
ms.topic: article
author: stsporen
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: fef9cb62e989c693c8b3d00cb15441c284f66554
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280160"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a><span data-ttu-id="79bb9-103">Какво е новото или промененото в Project Service Automation, версия 3, вълна 1, 2020 г.</span><span class="sxs-lookup"><span data-stu-id="79bb9-103">What's new or changed in Project Service Automation version 3 wave 1 2020</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="79bb9-104">Темата подчертава основните съображения за надграждане при преминаване към най-новата версия на Project Service Automation (PSA), версия 3.x, вълна 1, 2020 г.</span><span class="sxs-lookup"><span data-stu-id="79bb9-104">The topic highlights key upgrade considerations when moving to the latest release of Project Service Automation (PSA) version 3.x wave 1 2020.</span></span>

## <a name="time-entry"></a><span data-ttu-id="79bb9-105">Запис за време</span><span class="sxs-lookup"><span data-stu-id="79bb9-105">Time entry</span></span>
<span data-ttu-id="79bb9-106">Функционалността за записи за време е разширена, за да предостави възможности за разширяване на записите за време в повече клиентски сценарии.</span><span class="sxs-lookup"><span data-stu-id="79bb9-106">The time entry experience has been extended to deliver capabilities for extending time entry into more customer scenarios.</span></span> <span data-ttu-id="79bb9-107">Това включва възможността за добавяне на типове записи, която сега стартира конкретно поведение въз основа на името на схемата на полето **Настройки на запис за време**, показано като **Източник на време**.</span><span class="sxs-lookup"><span data-stu-id="79bb9-107">This includes the capability to add entry types, which now drive specific behavior based on the field schema name **Time Entry Settings**, displayed as **Time Source**.</span></span> <span data-ttu-id="79bb9-108">Ново решение, наречено „Време, разход, определяне на състояние и одобрения“ (TESA), е добавено за поддържане на тази функционалност.</span><span class="sxs-lookup"><span data-stu-id="79bb9-108">A new solution, called Time, Expense, Statusing, and Approvals (TESA) has been added to support this functionality.</span></span>

### <a name="upgrade-consideration"></a><span data-ttu-id="79bb9-109">Съображение за надстройката</span><span class="sxs-lookup"><span data-stu-id="79bb9-109">Upgrade consideration</span></span>
<span data-ttu-id="79bb9-110">За поддържане на тази функционалност ролите в PSA са актуализирани, за да включват нови привилегии.</span><span class="sxs-lookup"><span data-stu-id="79bb9-110">To support this functionality, the roles within PSA have been updated to include new privileges.</span></span> <span data-ttu-id="79bb9-111">Тези привилегии предоставят достъп за четене на новия обект **Настройки на запис за време**.</span><span class="sxs-lookup"><span data-stu-id="79bb9-111">These privileges grant read access to the new entity, **Time Entry Settings**.</span></span>

<span data-ttu-id="79bb9-112">Потребителите, които се нуждаят от възможността да регистрират време, трябва да получат потребителската роля **Потребител на запис за време** в допълнение към съществуващите роли.</span><span class="sxs-lookup"><span data-stu-id="79bb9-112">Users who require the ability to log time should be granted the user role **Time Entry User** in addition to existing roles.</span></span> <span data-ttu-id="79bb9-113">Тази роля включва новата функционалност и гарантира, че записът за време ще продължи да работи.</span><span class="sxs-lookup"><span data-stu-id="79bb9-113">This role includes the new functionality and ensures that time entry will continue to work.</span></span>

<span data-ttu-id="79bb9-114">В допълнение, ако имате персонализирани модули на приложението, които включват всички формуляри за обекта на запис за време, ще трябва да премахнете **Формуляра за бързо създаване на запис за време TESA** от модула.</span><span class="sxs-lookup"><span data-stu-id="79bb9-114">Additionally, if you have any custom app modules that include all forms for the time entry entity, you will be required to remove the **TESA time Entry Quick Create Form** from the module.</span></span>

### <a name="currently-extended-time-entry-changes"></a><span data-ttu-id="79bb9-115">Промени на записите за време, разширени в момента</span><span class="sxs-lookup"><span data-stu-id="79bb9-115">Currently extended time entry changes</span></span>
<span data-ttu-id="79bb9-116">За да се сведе до минимум въздействието на текущите потребители на записи за време, тази промяна на ролята е единственото основно изискване, необходимо за продължаване на използването на записите за време.</span><span class="sxs-lookup"><span data-stu-id="79bb9-116">To minimize the impact to current users of time entry, this role change is the only core requirement necessary to continue utilizing time entry.</span></span> <span data-ttu-id="79bb9-117">Ако сте създали персонализирани изгледи или отделни записи за време, трябва да зададете полетата **Настройка на запис за време** на правилната стойност на PSA.</span><span class="sxs-lookup"><span data-stu-id="79bb9-117">If you have created custom views or separate time entry experiences, you must set the **Time Entry Setting** fields to the correct PSA value.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]