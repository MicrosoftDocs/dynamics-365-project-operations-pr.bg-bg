---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 17, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 17, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
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
ms.openlocfilehash: f9fb941a95b0610dc546b1c12a87aa7faef4d676
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/10/2021
ms.locfileid: "5143685"
---
# <a name="project-service-automation-update-release-17-v3"></a><span data-ttu-id="f6879-103">Project Service Automation, издание на актуализация 17, V3</span><span class="sxs-lookup"><span data-stu-id="f6879-103">Project Service Automation Update Release 17, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="f6879-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f6879-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="f6879-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="f6879-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="f6879-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="f6879-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="f6879-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения, за да инсталирате актуализацията.</span><span class="sxs-lookup"><span data-stu-id="f6879-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="f6879-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="f6879-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="f6879-109">Тази тема изброява функциите и корекциите, които са нови или променени за PSA V3, издание на актуализация 17.</span><span class="sxs-lookup"><span data-stu-id="f6879-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 17.</span></span> <span data-ttu-id="f6879-110">Тази версия е с номер на компилация V3.10.6.34 и е общодостъпна за самостоятелно актуализиране от март 2020 г.</span><span class="sxs-lookup"><span data-stu-id="f6879-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in March 2020.</span></span>


## <a name="update-release-17"></a><span data-ttu-id="f6879-111">Издание на актуализация 17</span><span class="sxs-lookup"><span data-stu-id="f6879-111">Update Release 17</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="f6879-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="f6879-112">Bug fixes</span></span>

<span data-ttu-id="f6879-113">**Общи**</span><span class="sxs-lookup"><span data-stu-id="f6879-113">**General**</span></span>

- <span data-ttu-id="f6879-114">Поправено: Актуализиране на Project Service Automation, за да се наложат лицензи за членове на екипа (Центърът за ресурси на проекта ще включва метаданни 3.x на план за обслужване на членове на екипа)</span><span class="sxs-lookup"><span data-stu-id="f6879-114">Fixed: Update Project Service Automation to enforce Team Member licenses (Project Resource Hub will include Team Member Service plan metadata 3.x)</span></span>
 
<span data-ttu-id="f6879-115">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="f6879-115">**Time and Expense**</span></span>

- <span data-ttu-id="f6879-116">Поправено: Не е възможно да се промени прогнозата за разходите от ненулева цена на нула (0).</span><span class="sxs-lookup"><span data-stu-id="f6879-116">Fixed: It is not possible to change an expense estimate from a non-zero price to zero (0).</span></span> <span data-ttu-id="f6879-117">Промяната се игнорира.</span><span class="sxs-lookup"><span data-stu-id="f6879-117">The change is ignored.</span></span>

<span data-ttu-id="f6879-118">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="f6879-118">**Project Management**</span></span>

- <span data-ttu-id="f6879-119">Поправено: Проверка за нулеви стойности е добавена в името на позицията на член на екипа.</span><span class="sxs-lookup"><span data-stu-id="f6879-119">Fixed: A check for null values has been added on a team member's position name.</span></span>
- <span data-ttu-id="f6879-120">Поправено: Полето **msdyn_userresourceid** на обекта **msdyn_resourceassignment** е оттеглено.</span><span class="sxs-lookup"><span data-stu-id="f6879-120">Fixed: **msdyn_userresourceid** field on the **msdyn_resourceassignment** entity has been deprecated.</span></span>
- <span data-ttu-id="f6879-121">Поправено: Надстройка от 2.x до 3.x сега обработва празни контури на усилието на присвоявания на задачите.</span><span class="sxs-lookup"><span data-stu-id="f6879-121">Fixed: Upgrade from 2.x to 3.x now handles empty effort contours on task assignments.</span></span>

<span data-ttu-id="f6879-122">**Sales**</span><span class="sxs-lookup"><span data-stu-id="f6879-122">**Sales**</span></span>

- <span data-ttu-id="f6879-123">Поправено: **Invoice.PreValidateInvoiceUpdate** вече обработва сценария за преназначаване на собствениците на записи правилно.</span><span class="sxs-lookup"><span data-stu-id="f6879-123">Fixed: **Invoice.PreValidateInvoiceUpdate** now handles the scenario of reassigning record owners properly.</span></span>
- <span data-ttu-id="f6879-124">Поправено: Когато класът на транзакциите е **Час**, **UnitGroup** не може да се редактира за всички обекти, включително, **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail** и **ContractLineDetails**.</span><span class="sxs-lookup"><span data-stu-id="f6879-124">Fixed: When the transaction class is **Time**, **UnitGroup** is non-editable for all entities including, **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail**, and **ContractLineDetails**.</span></span> <span data-ttu-id="f6879-125">Въпреки това **Единица** не може да се редактира само за **JournalLine** и **InvoiceLineDetails**.</span><span class="sxs-lookup"><span data-stu-id="f6879-125">However, **Unit** is non-editable only for **JournalLine** and **InvoiceLineDetails**.</span></span>


