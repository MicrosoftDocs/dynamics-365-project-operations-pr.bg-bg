---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 13, V3
description: Тази тема предоставя информация за новостите в актуализацията на Project Service Automation, издание 13, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: a4ebc2e6ca3f6be0a05a7240d762d7a8cf92d81b
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949441"
---
# <a name="project-service-automation-update-release-13-v3"></a><span data-ttu-id="e38d2-103">Project Service Automation, издание на актуализация 13, V3</span><span class="sxs-lookup"><span data-stu-id="e38d2-103">Project Service Automation Update Release 13, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="e38d2-104">С удоволствие съобщаваме за най-новата актуализация за приложението Dynamics 365 Project Service Automation (PSA).</span><span class="sxs-lookup"><span data-stu-id="e38d2-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="e38d2-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="e38d2-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="e38d2-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="e38d2-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="e38d2-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online и отидете на страницата с решения, за да инсталирате актуализацията.</span><span class="sxs-lookup"><span data-stu-id="e38d2-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="e38d2-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="e38d2-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="e38d2-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 13.</span><span class="sxs-lookup"><span data-stu-id="e38d2-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 13.</span></span> <span data-ttu-id="e38d2-110">Тази версия е с номер на компилация V3.10.3.18 и е достъпна по следния график:</span><span class="sxs-lookup"><span data-stu-id="e38d2-110">This version has a build number of V3.10.3.18 and is available on the following schedule:</span></span>

- <span data-ttu-id="e38d2-111">**Общодостъпна (самостоятелно актуализиране):** ноември 2019 г.</span><span class="sxs-lookup"><span data-stu-id="e38d2-111">**General availability (self-update):** November 2019</span></span>
- <span data-ttu-id="e38d2-112">**Автоматична актуализация:** декември 2019 г.</span><span class="sxs-lookup"><span data-stu-id="e38d2-112">**Auto-update:** December 2019</span></span>


## <a name="update-release-13"></a><span data-ttu-id="e38d2-113">Издание на актуализация 13</span><span class="sxs-lookup"><span data-stu-id="e38d2-113">Update Release 13</span></span> 

### <a name="bug-fixes"></a><span data-ttu-id="e38d2-114">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="e38d2-114">Bug fixes</span></span>

- <span data-ttu-id="e38d2-115">Време и разход</span><span class="sxs-lookup"><span data-stu-id="e38d2-115">Time and Expense</span></span>

     - <span data-ttu-id="e38d2-116">Поправено: Функционалността за търсене на страницата **Одобрение на разходи** не работи при търсене по предназначение на разход.</span><span class="sxs-lookup"><span data-stu-id="e38d2-116">Fixed: Search functionality on the **Expense approval** page does not work when searching by expense purpose.</span></span>

- <span data-ttu-id="e38d2-117">Управление на ресурс</span><span class="sxs-lookup"><span data-stu-id="e38d2-117">Resource Management</span></span>

     - <span data-ttu-id="e38d2-118">Поправено: Числата в съгласуването са актуализирани, за да бъдат правилно обосновани.</span><span class="sxs-lookup"><span data-stu-id="e38d2-118">Fixed: Numbers in the reconciliation have been updated to be right justified.</span></span>
     - <span data-ttu-id="e38d2-119">Поправено: Наименуваните ресурси не могат да бъдат присвоени към задачи чрез раздела **График**.</span><span class="sxs-lookup"><span data-stu-id="e38d2-119">Fixed: Named Resources can't be assigned to tasks through the **Schedule** tab.</span></span>

- <span data-ttu-id="e38d2-120">Управление на проекти</span><span class="sxs-lookup"><span data-stu-id="e38d2-120">Project Management</span></span>

     - <span data-ttu-id="e38d2-121">Поправено: Изключението за нулева препратка при присвояване на член на екипа, когато в **TransactionType** липсва информация за настройка за **Единица** и **DefaultGroup**.</span><span class="sxs-lookup"><span data-stu-id="e38d2-121">Fixed: Null reference exception when assigning team member when the **TransactionType** is missing setup information for **Unit** and **DefaultGroup**.</span></span>

- <span data-ttu-id="e38d2-122">Sales</span><span class="sxs-lookup"><span data-stu-id="e38d2-122">Sales</span></span>

     - <span data-ttu-id="e38d2-123">Поправено: Дублиращите се записи на типове трансакции връщат грешка при създаване на записи на цени на роли.</span><span class="sxs-lookup"><span data-stu-id="e38d2-123">Fixed: Duplicate transaction type records return an error when role price records are created.</span></span>
     - <span data-ttu-id="e38d2-124">Коригирано: Допълнителните бутони за **Нова възможност**, **Оферта**, **Ред на поръчка** и **Добавяне на продукт** са видими в команди за възможности, оферти, поръчка на продукти и подмрежа с редове, базирани на проект.</span><span class="sxs-lookup"><span data-stu-id="e38d2-124">Fixed: Extra buttons for **New Opportunity**, **Quote**, **Order Line**, and **Add Product** are visible in commands for Opportunities, Quotes, Order Products, and the project-based Lines subgrid.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]