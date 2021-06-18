---
title: Интегриране на данни за настройка и конфигурация на Project Operations
description: Тази тема предоставя информация за настройване и конфигуриране на карти с двойно писане на Project Operations.
author: sigitac
manager: Annbe
ms.date: 4/23/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d5fe81dca30039f99d5d7b9bb459214e540db945
ms.sourcegitcommit: bc51629df94c164325cf2afee387d0e7cda66da7
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2021
ms.locfileid: "5938949"
---
# <a name="project-operations-setup-and-configuration-data-integration"></a><span data-ttu-id="0d068-103">Интегриране на данни за настройка и конфигурация на Project Operations</span><span class="sxs-lookup"><span data-stu-id="0d068-103">Project Operations setup and configuration data integration</span></span>

<span data-ttu-id="0d068-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="0d068-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="0d068-105">Тази тема предоставя информация за интеграция на двойни записи за Project Operations за обекти на настройка и конфигурация.</span><span class="sxs-lookup"><span data-stu-id="0d068-105">This topic provides information about Project Operations dual-write integration for setup and configuration entities.</span></span>

## <a name="project-contracts-contract-lines-and-projects"></a><span data-ttu-id="0d068-106">Договори по проект, аспекти на договор и проекти</span><span class="sxs-lookup"><span data-stu-id="0d068-106">Project contracts, contract lines, and projects</span></span>

<span data-ttu-id="0d068-107">Договори за проекти, аспекти на договор и проекти се създават през Dataverse и са синхронизирани с приложения на Finance and Operations за допълнително счетоводство.</span><span class="sxs-lookup"><span data-stu-id="0d068-107">Project contracts, contract lines, and projects are created in Dataverse and synchronized to Finance and Operations apps for additional accounting.</span></span> <span data-ttu-id="0d068-108">Записите в тези обекти могат да се създават и изтриват само в Dataverse.</span><span class="sxs-lookup"><span data-stu-id="0d068-108">The records in these entities can be created and deleted only in Dataverse.</span></span> <span data-ttu-id="0d068-109">Обаче счетоводни атрибути, като неизпълнение на данъчната група по продажби и финансови измерения, могат да бъдат добавени към тези записи в приложения на Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="0d068-109">However, accounting attributes such as sales tax group defaults and financial dimensions can be added to these records in the Finance and Operations apps.</span></span>

  ![Концепции за интеграция на договор по проект](./media/1ProjectContract.jpg)

<span data-ttu-id="0d068-111">Проследяват се потенциални клиенти, възможности и оферти в Dataverse и не синхронизирайте с приложения на Finance and Operations, тъй като няма счетоводство надолу по веригата, свързано с тази дейност.</span><span class="sxs-lookup"><span data-stu-id="0d068-111">Sales activity leads, opportunities, and quotes are tracked in Dataverse and don't synchronize to Finance and Operations apps because there is no downstream accounting associated with this activity.</span></span>

<span data-ttu-id="0d068-112">Функционалността на проектния договор в Dataverse създава запис на договор за проект в приложения на Finance and Operations, използващи **Заглавки на проектни договори (поръчки за продажба)** карта на таблица.</span><span class="sxs-lookup"><span data-stu-id="0d068-112">The project contract functionality in Dataverse creates a project contract record in Finance and Operations apps using the **Project contract headers (salesorders)** table map.</span></span> <span data-ttu-id="0d068-113">Запазване на договор за проект в Dataverse също така започва създаването на запис на обект на клиент по договор за проект.</span><span class="sxs-lookup"><span data-stu-id="0d068-113">Saving a project contract in Dataverse also starts the creation of a project contract customer entity record.</span></span> <span data-ttu-id="0d068-114">Този запис се синхронизира с приложения на Finance and Operations, използващи карта на таблица **Източник на финансиране на проекта (msdyn\_projectcontractssplitbillingrules)**.</span><span class="sxs-lookup"><span data-stu-id="0d068-114">This record is synchronized to Finance and Operations apps using the **Project funding source (msdyn\_projectcontractssplitbillingrules)** table map.</span></span> <span data-ttu-id="0d068-115">Тази карта също така синхронизира добавянията, актуализациите и изтриванията на клиентски договор.</span><span class="sxs-lookup"><span data-stu-id="0d068-115">This map also synchronizes project contract customer additions, updates, and deletions.</span></span> <span data-ttu-id="0d068-116">Разделените проценти на фактуриране между клиенти по договор се усвояват само в Dataverse и не е синхронизиран с приложения на Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="0d068-116">Split billing percentages between project contract customers are mastered only in Dataverse and not synchronized to Finance and Operations apps.</span></span>

<span data-ttu-id="0d068-117">След създаване на договор за проект през Dataverse, счетоводителят на проекта може да актуализира счетоводните атрибути за този договор за проект през приложения Finance and Operations, като отидете на **Управление на проекти и счетоводство** > **Договори за проекти** > **Настройвам** > **Показване на счетоводството по подразбиране**.</span><span class="sxs-lookup"><span data-stu-id="0d068-117">After a project contract is created in Dataverse, the project accountant can update the accounting attributes for this project contract in Finance and Operations apps by going to **Project management and accounting** > **Project contracts** > **Set up** > **Show default accounting**.</span></span> <span data-ttu-id="0d068-118">Счетоводителят може да прегледа оперативните атрибути на договор за проект, като например поисканата дата на доставка и сумата на договора, като избере идентификационния номер на договора за проект в приложения на Finance and Operations, което отваря свързания запис на договор за проект в Dataverse.</span><span class="sxs-lookup"><span data-stu-id="0d068-118">The accountant can review operational project contract attributes, such as requested delivery date and contract amount by selecting the project contract ID in Finance and Operations apps which opens the related project contract record in Dataverse.</span></span>

<span data-ttu-id="0d068-119">Обектът на проекта се синхронизира с приложения на Finance and Operations, използващи карта на таблица **Projects V2 (msdyn\_projects)**.</span><span class="sxs-lookup"><span data-stu-id="0d068-119">The project entity is synchronized to Finance and Operations apps using the **Projects V2 (msdyn\_projects)** table map.</span></span> <span data-ttu-id="0d068-120">Счетоводителят на проекта може:</span><span class="sxs-lookup"><span data-stu-id="0d068-120">The project accountant can:</span></span>

  - <span data-ttu-id="0d068-121">Преглед на проекти в приложения на Finance and Operations, като отидете на **Управление на проекти и счетоводство** > **Всички проекти**.</span><span class="sxs-lookup"><span data-stu-id="0d068-121">Review projects in Finance and Operations apps by going to **Project management and accounting** > **All projects**.</span></span> 
  - <span data-ttu-id="0d068-122">Актуализирайте счетоводните атрибути за проекта през приложения на Finance and Operations, като отидете на **Управление на проекти и счетоводство** > **Всички проекти** > **Настройвам** > **Показване на счетоводството по подразбиране**.</span><span class="sxs-lookup"><span data-stu-id="0d068-122">Update accounting attributes for the project in Finance and Operations apps by going to **Project management and accounting** > **All projects** > **Set up** > **Show default accounting**.</span></span>  
  - <span data-ttu-id="0d068-123">Прегледайте оперативните атрибути на проекта, като приблизителни начални и крайни дати, като изберете идентификатора на проекта в приложения на Finance and Operations, което отваря свързания запис на проекта в Dataverse.</span><span class="sxs-lookup"><span data-stu-id="0d068-123">Review operational project attributes, such as estimated start and end dates, by selecting the project ID in Finance and Operations apps which opens the related project record in Dataverse.</span></span>

<span data-ttu-id="0d068-124">Проектът е свързан с договор за проект чрез обект на **Проектна линия на договора**.</span><span class="sxs-lookup"><span data-stu-id="0d068-124">A project is associated with a project contract through the **Project contract line** entity.</span></span>

<span data-ttu-id="0d068-125">Аспекти на договор по проект в Dataverse създава правило за фактуриране на договор за проект в приложения на Finance and Operations, използващи карта на таблица **Заглавки на аспекти на договор (salesorderdetails)**.</span><span class="sxs-lookup"><span data-stu-id="0d068-125">Project contract lines in Dataverse creates a project contract billing rule in Finance and Operations apps using the **Project contract lines (salesorderdetails)** table map.</span></span> <span data-ttu-id="0d068-126">Методът за фактуриране дефинира типа правило за фактуриране на проектния договор в приложения на Finance and Operations:</span><span class="sxs-lookup"><span data-stu-id="0d068-126">The billing method defines the project contract billing rule type in Finance and Operations apps:</span></span>

  - <span data-ttu-id="0d068-127">Проектите на договорни линии с фактурен метод за време и материал създават фактуриращо правило за време и вид материал.</span><span class="sxs-lookup"><span data-stu-id="0d068-127">Project contract lines with a billing method of time and material create a billing rule of time and material type.</span></span>
  - <span data-ttu-id="0d068-128">Договорените линии по метода на таксуване с фиксирана цена създават ключово правило за таксуване.</span><span class="sxs-lookup"><span data-stu-id="0d068-128">Fixed price billing method contract lines create a milestone billing rule.</span></span>

<span data-ttu-id="0d068-129">Договорните редове за проекти могат да бъдат прегледани от счетоводителя на проекта чрез приложения на Finance and Operations, като отидете на **Управление на проекти и счетоводство** > **Договори за проекти** > **Настройвам** > **Показване на счетоводството по подразбиране** и преглед на подробностите за раздел **Договорни редове**. Счетоводителят може също така да зададе финансови размери по подразбиране за договорните линии по метода на таксуване с фиксирана цена в този раздел.</span><span class="sxs-lookup"><span data-stu-id="0d068-129">Project contract lines can be reviewed by the project accountant in Finance and Operations apps by going to **Project management and accounting** > **Project contracts** > **Set up** > **Show default accounting**, and reviewing the details on the **Contract lines** tab. The accountant can also set default financial dimensions for the fixed price billing method contract lines on this tab.</span></span>

## <a name="billing-milestones"></a><span data-ttu-id="0d068-130">Контролни точки за фактуриране</span><span class="sxs-lookup"><span data-stu-id="0d068-130">Billing milestones</span></span>

<span data-ttu-id="0d068-131">Линиите на договорни проекти, използващи метода за фактуриране с фиксирана цена, се фактурират чрез етапи на фактуриране.</span><span class="sxs-lookup"><span data-stu-id="0d068-131">Project contract lines using the fixed price billing method are invoiced through billing milestones.</span></span> <span data-ttu-id="0d068-132">Факторите за фактуриране се синхронизират с проектиране на транзакции по сметка в приложения на Finance and Operations с помощта на карта на таблица **Основни етапи на договора за интеграция на Project Operations (msdyn\_contractlinescheduleofvalues)**.</span><span class="sxs-lookup"><span data-stu-id="0d068-132">Billing milestones are synchronized to project on-account transactions in Finance and Operations apps by using the **Project Operations integration contract line milestones (msdyn\_contractlinescheduleofvalues)** table map.</span></span>

  ![Интеграция на контролни точки за фактуриране](./media/2Milestones.jpg)

<span data-ttu-id="0d068-134">Счетоводителят може да прегледа транзакциите по сметката и да коригира счетоводните атрибути за тези транзакции, като отиде на **Управление на проекти и счетоводство** > **Договори за проекти** > **Поддържайте** > **Транзакции по сметка** или **Управление на проекти и счетоводство** > **Всички проекти** > **Поддържайте** > **Транзакции по сметка**.</span><span class="sxs-lookup"><span data-stu-id="0d068-134">The accountant can review on-account transactions and adjust the accounting attributes for those transactions by going to **Project management and accounting** > **Project contracts** > **Maintain** > **On-account transactions** or **Project management and accounting** > **All projects** > **Maintain** > **On-account transactions**.</span></span>

<span data-ttu-id="0d068-135">Когато за първи път създадете фактор за фактуриране за даден ред на договор за проект, системата автоматично създава проект за оценка на приходите с фиксирана цена за проекта, свързан с този ред на договора.</span><span class="sxs-lookup"><span data-stu-id="0d068-135">When you first create a billing milestone for a given project contract line, the system automatically creates a fixed price revenue estimate project for the project associated with this contract line.</span></span> <span data-ttu-id="0d068-136">Проектите за оценка на приходите с фиксирана цена могат да бъдат прегледани, като отидете на **Управление на проекти и счетоводство** > **Проекти за оценка на приходите с фиксирана цена**.</span><span class="sxs-lookup"><span data-stu-id="0d068-136">Fixed-price revenue estimate projects can be reviewed by going to **Project management and accounting** > **Fixed-price revenue estimate projects**.</span></span>

### <a name="project-tasks"></a><span data-ttu-id="0d068-137">Задачи от проекти</span><span class="sxs-lookup"><span data-stu-id="0d068-137">Project tasks</span></span>

<span data-ttu-id="0d068-138">Задачите на проекта се синхронизират с приложения на Finance and Operations чрез **Задачи на проекта (msdyn\_projecttasks)** карта на таблицата само за справка.</span><span class="sxs-lookup"><span data-stu-id="0d068-138">Project tasks are synchronized to Finance and Operations apps through the **Project tasks (msdyn\_projecttasks)** table map for reference purposes only.</span></span> <span data-ttu-id="0d068-139">Операциите за създаване, актуализиране и изтриване не се поддържат чрез Finance and Operations приложения.</span><span class="sxs-lookup"><span data-stu-id="0d068-139">Creating, updating, and deleting operations isn't supported through Finance and Operations apps.</span></span>

  ![Интегриране на задача по проект](./media/3Tasks.jpg)

## <a name="project-resources"></a><span data-ttu-id="0d068-141">Ресурси на проект</span><span class="sxs-lookup"><span data-stu-id="0d068-141">Project resources</span></span>

<span data-ttu-id="0d068-142">Обектът **Роли на проектните ресурси** е синхронизиран с приложения на Finance and Operations, използващи карта на таблицата **Роли на проектните ресурси за всички компании (bookableresourcecategories)** само за справка.</span><span class="sxs-lookup"><span data-stu-id="0d068-142">The **Project resource roles** entity is synchronized to Finance and Operations apps using the **Project resource roles for all companies (bookableresourcecategories)** table map for reference purposes only.</span></span> <span data-ttu-id="0d068-143">Защото ресурсните роли в Dataverse не са специфични за компанията, системата автоматично създава съответни записи за ролите на специфични за компанията ресурси в Finance and Operations приложения автоматично за всички юридически лица, включени в обхвата на интеграция с двойно писане.</span><span class="sxs-lookup"><span data-stu-id="0d068-143">Because resource roles in Dataverse are not company-specific, the system automatically creates respective company-specific resource roles records in Finance and Operations apps automatically for all legal entities included into dual-write integration scope.</span></span>

![Интегриране на роли на ресурс](./media/5Resources.jpg)

<span data-ttu-id="0d068-145">Ресурсите на проекта в Project Operations се поддържат в Dataverse и не са синхронизирани с приложения на Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="0d068-145">Project resources in Project Operations are maintained in Dataverse and aren't synchronized to Finance and Operations apps.</span></span>

### <a name="transaction-categories"></a><span data-ttu-id="0d068-146">Категории трансакция</span><span class="sxs-lookup"><span data-stu-id="0d068-146">Transaction categories</span></span>

<span data-ttu-id="0d068-147">Категориите на транзакциите се поддържат в Dataverse и синхронизирани с приложения на Finance and Operations, използващи карта на таблицата **Категории на проектни транзакции (msdyn\_transactioncategories)**.</span><span class="sxs-lookup"><span data-stu-id="0d068-147">Transaction categories are maintained in Dataverse and synchronized to Finance and Operations apps using the **Project transaction categories (msdyn\_transactioncategories)** table map.</span></span> <span data-ttu-id="0d068-148">След като записът на категорията транзакции бъде синхронизиран, системата автоматично създава четири записа на споделена категория.</span><span class="sxs-lookup"><span data-stu-id="0d068-148">After the transaction category record is synchronized, the system automatically creates four shared category records.</span></span> <span data-ttu-id="0d068-149">Всеки запис съответства на тип транзакция в приложения на Finance and Operations и ги свързва към записа на категорията транзакции.</span><span class="sxs-lookup"><span data-stu-id="0d068-149">Each record corresponds to a transaction type in Finance and Operations apps and links them to the transaction category record.</span></span>

![Интеграция на категории транзакции](./media/4TransactionCategories.jpg)

<span data-ttu-id="0d068-151">Използването на категории транзакции за оценки и факти изисква от счетоводителя на проекта или системния администратор да създаде съответни категории проекти във всяко юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="0d068-151">Using transaction categories for estimates and actuals requires the project accountant or system administrator to create corresponding project categories in every legal entity.</span></span> <span data-ttu-id="0d068-152">За повече информация вижте [Конфигуриране на категории на проект](../project-accounting/configure-project-categories.md).</span><span class="sxs-lookup"><span data-stu-id="0d068-152">For more information, see [Configure project categories](../project-accounting/configure-project-categories.md).</span></span>