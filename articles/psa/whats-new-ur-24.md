---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 24, V3
description: Тази тема изброява функциите и корекциите, които са налични в Project Service Automation V3, издание на актуализация 24, V3.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 10/02/2020
ms.topic: article
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
ms.openlocfilehash: 6c8348e65307f63a251f97bf1ea17578e7026da8
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071772"
---
# <a name="project-service-automation-update-release-24-v3"></a><span data-ttu-id="350a3-103">Project Service Automation, издание на актуализация 24, V3</span><span class="sxs-lookup"><span data-stu-id="350a3-103">Project Service Automation Update Release 24, V3</span></span>

<span data-ttu-id="350a3-104">С удоволствие съобщаваме за най-новата актуализация на приложението Project Service Automation за Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="350a3-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="350a3-105">Тази версия включва някои важни подобрения в качеството, производителността и използваемостта.</span><span class="sxs-lookup"><span data-stu-id="350a3-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="350a3-106">Това издание е съвместимо с Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="350a3-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="350a3-107">За да актуализирате до това издание, посетете центъра за администрация на Dynamics 365 Online на страницата с решения и инсталирайте актуализацията.</span><span class="sxs-lookup"><span data-stu-id="350a3-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="350a3-108">За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="350a3-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="350a3-109">Тази тема изброява функциите и корекциите, които са нови или променени за Project Service Automation V3, издание на актуализация 24.</span><span class="sxs-lookup"><span data-stu-id="350a3-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 24.</span></span> <span data-ttu-id="350a3-110">Тази версия е с номер на компилация V 3.10.42.43 и е общодостъпна за самостоятелно актуализиране от октомври 2020.</span><span class="sxs-lookup"><span data-stu-id="350a3-110">This version has a build number of V 3.10.42.43 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-24"></a><span data-ttu-id="350a3-111">Издание на актуализация 24</span><span class="sxs-lookup"><span data-stu-id="350a3-111">Update Release 24</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="350a3-112">Корекции на грешки</span><span class="sxs-lookup"><span data-stu-id="350a3-112">Bug fixes</span></span>

<span data-ttu-id="350a3-113">**Sales**</span><span class="sxs-lookup"><span data-stu-id="350a3-113">**Sales**</span></span>

<span data-ttu-id="350a3-114">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="350a3-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="350a3-115">Проблем при задаване на ценовата листа по подразбиране на продуктите.</span><span class="sxs-lookup"><span data-stu-id="350a3-115">Problem while setting default price list of products.</span></span>
- <span data-ttu-id="350a3-116">Изпълнението на печелене на оферта е бавно поради вградената ценова листа и копие на записи на ценови роли.</span><span class="sxs-lookup"><span data-stu-id="350a3-116">Performance of Quote win is slow due to the embedded price list and role price records copy.</span></span>
- <span data-ttu-id="350a3-117">**Договор за проект/център за продажби** > **Елемент на ред на продукт/Количество на ред за поръчка** автоматично се закръглява до най-близкото цяло число.</span><span class="sxs-lookup"><span data-stu-id="350a3-117">**Project Contract/Sales Hub** > **Product Line Item/Order Line Quantity** is automatically rounded to the nearest integer.</span></span>
- <span data-ttu-id="350a3-118">Издигнете до системни привилегии, когато четете ценоразписи.</span><span class="sxs-lookup"><span data-stu-id="350a3-118">Elevate to system privileges when reading price lists.</span></span>
- <span data-ttu-id="350a3-119">Копирайте полетата за адрес на клиента **address1_freighttermscode** и **address1_shippingmethodcode** за оферта/поръчка.</span><span class="sxs-lookup"><span data-stu-id="350a3-119">Copy customer address fields **address1_freighttermscode** and **address1_shippingmethodcode** to Quote/Order.</span></span> 


<span data-ttu-id="350a3-120">**Време и разход**</span><span class="sxs-lookup"><span data-stu-id="350a3-120">**Time and Expense**</span></span>

<span data-ttu-id="350a3-121">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="350a3-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="350a3-122">**Решетката за въвеждане на време** не поддържа поведение на времето **Само дата**.</span><span class="sxs-lookup"><span data-stu-id="350a3-122">The **Time Entry Grid** doesn't support **Date Only** time behavior.</span></span>
- <span data-ttu-id="350a3-123">**Въвеждане на час** не се опреснява автоматично.</span><span class="sxs-lookup"><span data-stu-id="350a3-123">**Time Entry** is not refreshing automatically.</span></span> <span data-ttu-id="350a3-124">Изисква се ръчно опресняване.</span><span class="sxs-lookup"><span data-stu-id="350a3-124">A manual refresh is required.</span></span>
- <span data-ttu-id="350a3-125">Не можете да импортирате записите за време от задание, когато има прекъсване (0 часа) в заданията на ресурс.</span><span class="sxs-lookup"><span data-stu-id="350a3-125">Unable to import the time entries from an assignment when there is a break (0 hours) in a resource's assignments.</span></span>
- <span data-ttu-id="350a3-126">Когато създавате запис на време, задайте начало на същото като **msdyn_date**.</span><span class="sxs-lookup"><span data-stu-id="350a3-126">When creating a time entry, set the start to the same as **msdyn_date**.</span></span>
- <span data-ttu-id="350a3-127">Повторно активирайте груповото редактиране за въвеждане на време.</span><span class="sxs-lookup"><span data-stu-id="350a3-127">Re-enable bulk edit for time entry.</span></span>

<span data-ttu-id="350a3-128">**Управление на ресурси**</span><span class="sxs-lookup"><span data-stu-id="350a3-128">**Resource Management**</span></span>

<span data-ttu-id="350a3-129">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="350a3-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="350a3-130">Опитът да актуализирате състоянието на междудневна резервация без изискване ще доведе до изключение null-ref.</span><span class="sxs-lookup"><span data-stu-id="350a3-130">Trying to update the status of an inter-day booking without a requirement will throw a null-ref exception.</span></span>
- <span data-ttu-id="350a3-131">Грешка при зареждането на **Изглед за съгласуване**.</span><span class="sxs-lookup"><span data-stu-id="350a3-131">Error loading the **Reconciliation View**.</span></span>


<span data-ttu-id="350a3-132">**Управление на проекти**</span><span class="sxs-lookup"><span data-stu-id="350a3-132">**Project Management**</span></span>

<span data-ttu-id="350a3-133">Следните проблеми са коригирани:</span><span class="sxs-lookup"><span data-stu-id="350a3-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="350a3-134">В **График на проекта** , при смяна от **Ръчно** на **Автоматично** автоматичното записване не завършва.</span><span class="sxs-lookup"><span data-stu-id="350a3-134">In the **Project Schedule** , when changing from **Manual** to **Auto** , auto save is not completing.</span></span>
- <span data-ttu-id="350a3-135">Разходите за разходи не трябва да се изчисляват към отклонение от **Решетка за проследяване на проекти**.</span><span class="sxs-lookup"><span data-stu-id="350a3-135">Expense costs should not calculate toward variance on the **Project Tracking Grid**.</span></span>
- <span data-ttu-id="350a3-136">Непоследователно поведение за колоните **Етикет за оценка** по време на зареждане спрямо промяна на типа **Време-фаза**.</span><span class="sxs-lookup"><span data-stu-id="350a3-136">Inconsistent behavior for **Estimates tag** columns during load versus changing the **Time-Phase** type.</span></span>
- <span data-ttu-id="350a3-137">Действителните разходи за даден проект може да не отразяват сумите от **Действителни данни**.</span><span class="sxs-lookup"><span data-stu-id="350a3-137">The actual cost on a project may not reflect the totals from **Actuals**.</span></span>
- <span data-ttu-id="350a3-138">**Очаквана крайна дата** на раздела **Обобщение** не съответства на **График на WBS**.</span><span class="sxs-lookup"><span data-stu-id="350a3-138">**Estimated Finish Date** on the **Summary** tab does not match the **WBS Schedule**.</span></span>
- <span data-ttu-id="350a3-139">**Актуализиране на действителните часове** в задържане не работи правилно.</span><span class="sxs-lookup"><span data-stu-id="350a3-139">**Update Actual Hours** on outdent does not work correctly.</span></span>
- <span data-ttu-id="350a3-140">Мениджър на проекти извън корена **BU** не може да създаде проект.</span><span class="sxs-lookup"><span data-stu-id="350a3-140">A Project manager outside of root **BU** can't create a project.</span></span>
- <span data-ttu-id="350a3-141">Промени в задача или категория на **Оценки на разходите** не се запазват.</span><span class="sxs-lookup"><span data-stu-id="350a3-141">Changes to task or category on **Expense Estimates** are not persisted.</span></span>
- <span data-ttu-id="350a3-142">**Копие на договор** копира графиците на фактурите и състоянието на изпълнение.</span><span class="sxs-lookup"><span data-stu-id="350a3-142">**Copy of contract** copies the invoice schedules and the run status.</span></span>
- <span data-ttu-id="350a3-143">Бутонът **Обновяване на актуалните данни** неправилно изчислява обобщени задачи.</span><span class="sxs-lookup"><span data-stu-id="350a3-143">**Refresh Actuals** button incorrectly calculates summary tasks.</span></span>
- <span data-ttu-id="350a3-144">Добавка за Microsoft Project: Коригирайте нулева грешка при справка, ако някой член на екипа има празно ресурсно звено.</span><span class="sxs-lookup"><span data-stu-id="350a3-144">Microsoft Project Add-in: Fix null reference error if any team member has an empty resourcing unit.</span></span>

