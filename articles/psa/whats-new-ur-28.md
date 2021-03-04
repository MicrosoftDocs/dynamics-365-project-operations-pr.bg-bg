---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 28, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 28, V3.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/26/2021
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
ms.openlocfilehash: 2c50d6bdc033836e1259a2fd12b78015280d8093
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150610"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a><span data-ttu-id="81b51-103">Какво е новото или промененото в Project Service Automation, издание на актуализация 28, V3</span><span class="sxs-lookup"><span data-stu-id="81b51-103">What's new or changed in Project Service Automation Update Release 28, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="81b51-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="81b51-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="81b51-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="81b51-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="81b51-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="81b51-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="81b51-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="81b51-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="81b51-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="81b51-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="81b51-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 28. Тази версия е с номер на компилация V3.10.46.32 и е общодостъпна чрез самостоятелна актуализация от януари 2021.</span><span class="sxs-lookup"><span data-stu-id="81b51-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 28 This version has a build number of V3.10.46.32 and is generally available through a self-update in January 2021.</span></span>

## <a name="update-release-28"></a><span data-ttu-id="81b51-110">Издание на актуализация 28</span><span class="sxs-lookup"><span data-stu-id="81b51-110">Update Release 28</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="81b51-111">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="81b51-111">Bug fixes</span></span>

<span data-ttu-id="81b51-112">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="81b51-112">**Time and Expense**</span></span>

<span data-ttu-id="81b51-113">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="81b51-113">The following issues have been fixed:</span></span>

- <span data-ttu-id="81b51-114">Потребителите могат да използват **Групово редактиране** за актуализиране на записите за време, които са одобрени и изпратени.</span><span class="sxs-lookup"><span data-stu-id="81b51-114">Users can use **Bulk Edit** to update time entries that have been approved and submitted.</span></span>

<span data-ttu-id="81b51-115">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="81b51-115">**Project Management**</span></span>

<span data-ttu-id="81b51-116">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="81b51-116">The following issues have been fixed:</span></span>

- <span data-ttu-id="81b51-117">В случаите, когато GUID на задачата се интерпретира като число, задачите не могат да бъдат отворени за редактиране с помощта на **Редактиране на задача** в лентата на страницата **съставна структура на работата**.</span><span class="sxs-lookup"><span data-stu-id="81b51-117">In cases where the task GUID is interpreted as a number, tasks can't be opened for edit using **Edit Task** in the ribbon on the **Work Breakdown Structure** page.</span></span>

<span data-ttu-id="81b51-118">**Sales**</span><span class="sxs-lookup"><span data-stu-id="81b51-118">**Sales**</span></span>

<span data-ttu-id="81b51-119">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="81b51-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="81b51-120">Изключване на нулева препратка се генерира, когато добавката **GetEstimatesForProject** бъде извикана.</span><span class="sxs-lookup"><span data-stu-id="81b51-120">A null reference exception is generated when the **GetEstimatesForProject** plug-in is invoked.</span></span>
- <span data-ttu-id="81b51-121">**Маркирайте готовност за фактуриране** в решетката на етапа само частично актуализира атрибутите, с изключение на атрибута **InvoiceStatus**, който се актуализира.</span><span class="sxs-lookup"><span data-stu-id="81b51-121">**Mark ready to invoice** on the milestone grid only partially updates attributes, except for the **InvoiceStatus** attribute, which is updated.</span></span>

