---
title: Проекти за прогнози за приходи с фиксирана цена
description: Тази тема предоставя информация за приходи с фиксирана цена в проекти.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7cf4d7853f7fedaeeeba99bc589f39989b924423
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278900"
---
# <a name="fixed-price-revenue-estimate-projects"></a><span data-ttu-id="bc010-103">Проекти за прогнози за приходи с фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="bc010-103">Fixed price revenue estimate projects</span></span> 

<span data-ttu-id="bc010-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="bc010-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="bc010-105">Когато създавате аспекти на договор по проект със следващите атрибути в Dynamics 365 Project Operations на Microsoft Dataverse, системата автоматично създава проект за оценка на приходи с фиксирана цена.</span><span class="sxs-lookup"><span data-stu-id="bc010-105">When you create a project contract line with the following attributes in Dynamics 365 Project Operations on Microsoft Dataverse, the system automatically creates a fixed price revenue estimate project.</span></span> <span data-ttu-id="bc010-106">Информацията в този проект се основава на следното:</span><span class="sxs-lookup"><span data-stu-id="bc010-106">The information in this project is based on the following:</span></span>

  - <span data-ttu-id="bc010-107">Метод за фактуриране с фиксирана цена.</span><span class="sxs-lookup"><span data-stu-id="bc010-107">A fixed price billing method.</span></span>
  - <span data-ttu-id="bc010-108">Свързан проект.</span><span class="sxs-lookup"><span data-stu-id="bc010-108">An associated project.</span></span>
  - <span data-ttu-id="bc010-109">Поне една контролна точка, определена в раздела **График на фактура** на страницата **Аспекти на договор по проект**.</span><span class="sxs-lookup"><span data-stu-id="bc010-109">At least one milestone defined on the **Invoice schedule** tab on the **Project contract line** page.</span></span>

## <a name="review-fixed-price-revenue-estimates-projects"></a><span data-ttu-id="bc010-110">Преглед на проекти за оценки на приходи с фиксирана цена</span><span class="sxs-lookup"><span data-stu-id="bc010-110">Review fixed price revenue estimates projects</span></span>
<span data-ttu-id="bc010-111">За да прегледате проектите за оценка на приходи с фиксирана цена, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="bc010-111">To review fixed price revenue estimates projects, complete the following steps:</span></span>

1. <span data-ttu-id="bc010-112">В средата на Dynamics 365 Finance отидете на **Управление на проекти и счетоводство** > **Проекти** > **Проекти за прогнози за приходи с фиксирана цена**.</span><span class="sxs-lookup"><span data-stu-id="bc010-112">In the Dynamics 365 Finance environment, go to **Projects management and accounting** > **Projects** > **Fixed price revenue estimate projects**.</span></span>
2. <span data-ttu-id="bc010-113">Изберете проекта, който искате да прегледате, и щракнете двукратно върху **ИД на оценка на проект**, за да отворите записа и да прегледате подробностите за проекта.</span><span class="sxs-lookup"><span data-stu-id="bc010-113">Select the project that you want to view and double-click the **Estimate project ID** to open the record and review the details of the project.</span></span>
3. <span data-ttu-id="bc010-114">Разгънете раздела **Проект**. Ще видите един проект в мрежата **Избрани проекти**.</span><span class="sxs-lookup"><span data-stu-id="bc010-114">Expand the **Project** tab. You will see one project in the **Selected projects** grid.</span></span> <span data-ttu-id="bc010-115">Системата го използва като проект по подразбиране, защото това е проектът, свързан с аспектите на договора по проект.</span><span class="sxs-lookup"><span data-stu-id="bc010-115">The system uses this as default project because it is the project associated to the project contract line.</span></span> 
4. <span data-ttu-id="bc010-116">За да промените връзката, изберете допълнителни проекти и ги добавете към мрежата **Избрани проекти**.</span><span class="sxs-lookup"><span data-stu-id="bc010-116">To change the association, select additional projects and add them to the **Selected projects** grid.</span></span> <span data-ttu-id="bc010-117">Ако в тази мрежа са избрани няколко проекта, процентът на завършеност на проекта и оценките на приходите се изчисляват заедно за всички избрани проекти.</span><span class="sxs-lookup"><span data-stu-id="bc010-117">If multiple projects are selected in this grid, the project percentage completion and revenue estimates are calculated together for of the all selected projects.</span></span>

  <span data-ttu-id="bc010-118">Разходите за проекта, профила на приходите, шаблона за разходите и кода на периода могат да се зададат ръчно.</span><span class="sxs-lookup"><span data-stu-id="bc010-118">Project cost, revenue profile, cost template, and the period code can be set manually.</span></span> <span data-ttu-id="bc010-119">Ако не са зададени ръчно, стойностите по подразбиране са първото изчисление на оценката на проекта, като се използват правилата, конфигурирани за профилите на разходите и приходите от проекта.</span><span class="sxs-lookup"><span data-stu-id="bc010-119">If they aren't set manually, the values default during the first estimate calculation for the project using the rules configured for project cost and revenue profiles.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]