---
title: Какво е новото в актуализацията на Project Service Automation, издание 13, V3
description: Тази тема предоставя информация за новостите в актуализацията на Project Service Automation, издание 13, V3.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 3.x
ms.assetid: c6f6a5b6-b5bb-467c-b7c7-7fb962504c6d
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5f1b6b3879c94a77ab62082aad1e470a3ba66552
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749284"
---
# <a name="project-service-automation-v3-update-release-13"></a><span data-ttu-id="bd030-103">Project Service Automation V3, издание на актуализация 13</span><span class="sxs-lookup"><span data-stu-id="bd030-103">Project Service Automation V3, Update Release 13</span></span>
<span data-ttu-id="bd030-104">С удоволствие съобщаваме за най-новата актуализация за приложението Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="bd030-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="bd030-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="bd030-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="bd030-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="bd030-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="bd030-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online и отидете на страницата с решения, за да инсталирате актуализацията.</span><span class="sxs-lookup"><span data-stu-id="bd030-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="bd030-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="bd030-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="bd030-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 13.</span><span class="sxs-lookup"><span data-stu-id="bd030-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 13.</span></span> <span data-ttu-id="bd030-110">Тази версия е с номер на компилация V3.10.3.18 и е достъпна по следния график:</span><span class="sxs-lookup"><span data-stu-id="bd030-110">This version has a build number of V3.10.3.18 and is available on the following schedule:</span></span>

- <span data-ttu-id="bd030-111">**Общодостъпна (самостоятелно актуализиране):** ноември 2019 г.</span><span class="sxs-lookup"><span data-stu-id="bd030-111">**General availability (self-update):** November 2019</span></span>
- <span data-ttu-id="bd030-112">**Автоматична актуализация:** декември 2019 г.</span><span class="sxs-lookup"><span data-stu-id="bd030-112">**Auto-update:** December 2019</span></span>


## <a name="update-release-13"></a><span data-ttu-id="bd030-113">Издание на актуализация 13</span><span class="sxs-lookup"><span data-stu-id="bd030-113">Update Release 13</span></span> 

### <a name="bug-fixes"></a><span data-ttu-id="bd030-114">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="bd030-114">Bug fixes</span></span>

- <span data-ttu-id="bd030-115">Време и разход</span><span class="sxs-lookup"><span data-stu-id="bd030-115">Time and Expense</span></span>

     - <span data-ttu-id="bd030-116">Поправено: Функционалността за търсене на страницата **Одобрение на разходи** не работи при търсене по предназначение на разход.</span><span class="sxs-lookup"><span data-stu-id="bd030-116">Fixed: Search functionality on the **Expense approval** page does not work when searching by expense purpose.</span></span>

- <span data-ttu-id="bd030-117">Управление на ресурс</span><span class="sxs-lookup"><span data-stu-id="bd030-117">Resource Management</span></span>

     - <span data-ttu-id="bd030-118">Поправено: Числата в съгласуването са актуализирани, за да бъдат правилно обосновани.</span><span class="sxs-lookup"><span data-stu-id="bd030-118">Fixed: Numbers in the reconciliation have been updated to be right justified.</span></span>
     - <span data-ttu-id="bd030-119">Поправено: Наименуваните ресурси не могат да бъдат присвоени към задачи чрез раздела **График**.</span><span class="sxs-lookup"><span data-stu-id="bd030-119">Fixed: Named Resources can't be assigned to tasks through the **Schedule** tab.</span></span>

- <span data-ttu-id="bd030-120">Управление на проекти</span><span class="sxs-lookup"><span data-stu-id="bd030-120">Project Management</span></span>

     - <span data-ttu-id="bd030-121">Поправено: Изключението за нулева препратка при присвояване на член на екипа, когато в **TransactionType** липсва информация за настройка за **Единица** и **DefaultGroup**.</span><span class="sxs-lookup"><span data-stu-id="bd030-121">Fixed: Null reference exception when assigning team member when the **TransactionType** is missing setup information for **Unit** and **DefaultGroup**.</span></span>

- <span data-ttu-id="bd030-122">Sales</span><span class="sxs-lookup"><span data-stu-id="bd030-122">Sales</span></span>

     - <span data-ttu-id="bd030-123">Поправено: Дублиращите се записи на типове трансакции връщат грешка при създаване на записи на цени на роли.</span><span class="sxs-lookup"><span data-stu-id="bd030-123">Fixed: Duplicate transaction type records return an error when role price records are created.</span></span>
     - <span data-ttu-id="bd030-124">Поправено: Допълнителните бутони за **Нова възможност**, **Оферта**, **Ред за поръчка** и **Добавяне на продукт** се виждат в командите за възможности, оферти, продукти по поръчка и подмрежата на редове, базирани на проект.</span><span class="sxs-lookup"><span data-stu-id="bd030-124">Fixed: Extra buttons for **New Opportunity**, **Quote**, **Order Line**, and **Add Product** are visible in commands for Opportunities, Quotes, Order Products, and the project-based Lines sub-grid.</span></span>


