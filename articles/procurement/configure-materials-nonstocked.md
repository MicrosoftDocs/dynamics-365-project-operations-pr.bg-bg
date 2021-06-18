---
title: Конфигурирайте не складирани материали и чакащи фактури на доставчици
description: Тази тема обяснява как да активирате не складирани материали и чакащи фактури на доставчици.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 24418f3aad8356bd209eef7487a47a3870bce10f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993898"
---
# <a name="configure-non-stocked-materials-and-pending-vendor-invoices"></a><span data-ttu-id="75865-103">Конфигурирайте не складирани материали и чакащи фактури на доставчици</span><span class="sxs-lookup"><span data-stu-id="75865-103">Configure non-stocked materials and pending vendor invoices</span></span>

<span data-ttu-id="75865-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="75865-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

## <a name="minimum-version-requirement"></a><span data-ttu-id="75865-105">Изискване за минимална версия</span><span class="sxs-lookup"><span data-stu-id="75865-105">Minimum version requirement</span></span>

<span data-ttu-id="75865-106">Използване на складови материали и чакащи фактури на доставчици за нескладирани/базирани на ресурси сценарии на Dynamics 365 Project Operations изисква следните версии:</span><span class="sxs-lookup"><span data-stu-id="75865-106">Using non-stocked materials and pending vendor invoices for Dynamics 365 Project Operations non-stocked/resource based scenarios requires the following versions:</span></span>

<span data-ttu-id="75865-107">Решения на Dynamics 365 Dataverse:</span><span class="sxs-lookup"><span data-stu-id="75865-107">Dynamics 365 Dataverse solutions:</span></span>

- <span data-ttu-id="75865-108">Project Operations – 4.9.0.221 или по-нова версия</span><span class="sxs-lookup"><span data-stu-id="75865-108">Project Operations – 4.9.0.221 or higher</span></span>
- <span data-ttu-id="75865-109">Решение за оркестрация на приложения с двойно писане - 2.2.2.23 или по-нова версия</span><span class="sxs-lookup"><span data-stu-id="75865-109">Dual-write application orchestration solution - 2.2.2.23 or higher</span></span>

<span data-ttu-id="75865-110">Dynamics 365 Finance:</span><span class="sxs-lookup"><span data-stu-id="75865-110">Dynamics 365 Finance:</span></span>
- <span data-ttu-id="75865-111">10.0.18 (10.0.793.52) или по-нова версия.</span><span class="sxs-lookup"><span data-stu-id="75865-111">10.0.18 (10.0.793.52) or higher.</span></span> <span data-ttu-id="75865-112">Уверете се, че вашата финансова среда е актуална и всички качествени актуализации се прилагат, за да отговарят на минималните изисквания за версия.</span><span class="sxs-lookup"><span data-stu-id="75865-112">Make sure that your Finance environment is current and all quality updates are applied to meet the minimum version requirements.</span></span>

## <a name="run-dual-write-maps-for-non-stocked-materials-and-vendor-invoice-integration"></a><span data-ttu-id="75865-113">Изпълнете карти с двойно писане за не складирани материали и интеграция на фактури на доставчик</span><span class="sxs-lookup"><span data-stu-id="75865-113">Run Dual-write maps for non-stocked materials and vendor invoice integration</span></span>

<span data-ttu-id="75865-114">Този раздел предоставя информация за конкретни карти, необходими за не складирани материали и фактури на доставчици.</span><span class="sxs-lookup"><span data-stu-id="75865-114">This section provides information about specific the maps required for non-stocked materials and vendor invoices.</span></span> <span data-ttu-id="75865-115">Уверете се, че необходимите карти, изброени в темата [Осигуряване на нова среда](../environment/resource-provision-new-environment.md#run-project-operations-dual-write-maps) се изпълняват във вашата среда.</span><span class="sxs-lookup"><span data-stu-id="75865-115">Verify that the prerequisite maps listed in the [Provision a new environment](../environment/resource-provision-new-environment.md#run-project-operations-dual-write-maps) topic are running on your environment.</span></span>

1. <span data-ttu-id="75865-116">Отидете на Lifecycle Services (LCS), отидете до вашия LCS проект и отидете на страницата **Подробности за среда**.</span><span class="sxs-lookup"><span data-stu-id="75865-116">Go to Lifecycle Services (LCS), navigate to your LCS project, and go to the **Environment details** page.</span></span>
2. <span data-ttu-id="75865-117">В секцията **Информация за среда на Common Data Service** изберете **Връзка към CDS за приложения**.</span><span class="sxs-lookup"><span data-stu-id="75865-117">In the **Common Data Service Environment Information** section, select **Link to CDS for Apps**.</span></span> <span data-ttu-id="75865-118">След като изберете връзката, ще бъдете пренасочени към списъка с обекти в съпоставянията.</span><span class="sxs-lookup"><span data-stu-id="75865-118">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="75865-119">Уверете се, че се изпълняват следните карти.</span><span class="sxs-lookup"><span data-stu-id="75865-119">Make sure the following maps are running.</span></span> <span data-ttu-id="75865-120">Ако не работят, стартирайте ги и не забравяйте да включите всички свързани карти на таблици.</span><span class="sxs-lookup"><span data-stu-id="75865-120">If they aren't running, start them and make sure to include all related table maps.</span></span>

    - <span data-ttu-id="75865-121">CDS издаде различни продукти (продукти)</span><span class="sxs-lookup"><span data-stu-id="75865-121">CDS released distinct products (products)</span></span>
    - <span data-ttu-id="75865-122">Доставчици v2 (msdyn_vendors)</span><span class="sxs-lookup"><span data-stu-id="75865-122">Vendors v2 (msdyn_vendors)</span></span>
    - <span data-ttu-id="75865-123">Таблица на Project Operations за материални оценки (msdyn_estimatelines)</span><span class="sxs-lookup"><span data-stu-id="75865-123">Project Operations table for material estimates (msdyn_estimatelines)</span></span>
    - <span data-ttu-id="75865-124">Обект за експортиране на фактура на доставчик на проект на Project Operations (msdyn_projectvendorinvoices)</span><span class="sxs-lookup"><span data-stu-id="75865-124">Project Operations integration project vendor invoice export entity (msdyn_projectvendorinvoices)</span></span>
    - <span data-ttu-id="75865-125">Обект за линейно експортиране на фактура на доставчик на проект на Project Operations (msdyn_projectvendorinvoicelines)</span><span class="sxs-lookup"><span data-stu-id="75865-125">Project Operations integration project vendor invoice line export entity (msdyn_projectvendorinvoicelines)</span></span>
    - <span data-ttu-id="75865-126">Действителни данни за интеграция на Project Operations (msdyn_actuals).</span><span class="sxs-lookup"><span data-stu-id="75865-126">Project Operations integration actuals (msdyn_actuals).</span></span> <span data-ttu-id="75865-127">Уверете се, че използвате версия на картата 1.0.0.14 или по-нова.</span><span class="sxs-lookup"><span data-stu-id="75865-127">Make sure you are running map version 1.0.0.14 or higher.</span></span> <span data-ttu-id="75865-128">Можете да видите активната версия на картата в колоната **Версия** на страницата **Двоен запис**.</span><span class="sxs-lookup"><span data-stu-id="75865-128">You can see the active version of the map in the **Version** column on the **Dual Write** page.</span></span> <span data-ttu-id="75865-129">Можете да активирате нова версия на картата, като изберете **Версия на табличната карта** и след това запазване на избраната версия.</span><span class="sxs-lookup"><span data-stu-id="75865-129">You can activate a new version of the map by selecting **Table map version** and then saving the selected version.</span></span>

<span data-ttu-id="75865-130">Ако използвате стандартни демонстрационни данни, може да се наложи да спрете и рестартирате следните карти на обекти с първоначална синхронизация:</span><span class="sxs-lookup"><span data-stu-id="75865-130">If you are using standard demo data, you might also need to stop and restart the following entity maps with initial sync:</span></span>
  - <span data-ttu-id="75865-131">Дни за плащане CDS V2 (msdyn_paymentdays)</span><span class="sxs-lookup"><span data-stu-id="75865-131">Payment days CDS V2 (msdyn_paymentdays)</span></span>
  - <span data-ttu-id="75865-132">График на плащанията (msdyn_paymentschedules)</span><span class="sxs-lookup"><span data-stu-id="75865-132">Payment schedule (msdyn_paymentschedules)</span></span>
  - <span data-ttu-id="75865-133">Условия за плащане (msdyn_paymentterms)</span><span class="sxs-lookup"><span data-stu-id="75865-133">Terms of payment (msdyn_paymentterms)</span></span>
  - <span data-ttu-id="75865-134">Групи доставчици (msdyn_vendorgroups)</span><span class="sxs-lookup"><span data-stu-id="75865-134">Vendor groups (msdyn_vendorgroups)</span></span>
  - <span data-ttu-id="75865-135">Мерни единици (uom)</span><span class="sxs-lookup"><span data-stu-id="75865-135">Units (uom)</span></span>

> [!NOTE]
> <span data-ttu-id="75865-136">Първоначалната синхронизация за групи доставчици и устройства може да не успее за няколко записа в съществуващия набор от демо данни.</span><span class="sxs-lookup"><span data-stu-id="75865-136">The initial sync for vendor groups and units might fail for a few records in the existing demo data set.</span></span> <span data-ttu-id="75865-137">Можете да игнорирате неуспехите, тъй като те няма да ви попречат да използвате демо данни с Project Operations.</span><span class="sxs-lookup"><span data-stu-id="75865-137">You can ignore the failures as they won't prevent you from using demo data with Project Operations.</span></span>

## <a name="configure-prerequisites-in-dataverse"></a><span data-ttu-id="75865-138">Конфигуриране на предпоставки в Dataverse</span><span class="sxs-lookup"><span data-stu-id="75865-138">Configure prerequisites in Dataverse</span></span>

### <a name="activate-workflow-to-create-accounts-based-on-vendor-entity"></a><span data-ttu-id="75865-139">Активирайте работния поток, за да създавате акаунти въз основа на обект на доставчик</span><span class="sxs-lookup"><span data-stu-id="75865-139">Activate workflow to create accounts based on vendor entity</span></span>

<span data-ttu-id="75865-140">Решението за двойна оркестрация на запис осигурява [интеграция за управление на доставчици](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-mapping.md).</span><span class="sxs-lookup"><span data-stu-id="75865-140">The Dual Write Orchestration solution provides [Vendors master integration](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-mapping.md).</span></span> <span data-ttu-id="75865-141">Като предпоставка за тази функция, данните за доставчика трябва да бъдат създадени в обекта **Акаунти**.</span><span class="sxs-lookup"><span data-stu-id="75865-141">As a prerequisite for this feature, vendor data must be created in the **Accounts** entity.</span></span> <span data-ttu-id="75865-142">Активирайте процес на работен процес на шаблон, за да създадете доставчици в таблицата **Акаунти**, както е описано в [Превключвайте между дизайни на доставчици](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-switch.md#use-the-extended-vendor-design-for-vendors-of-the-organization-type).</span><span class="sxs-lookup"><span data-stu-id="75865-142">Activate a template workflow process to create vendors in the **Accounts** table as described in [Switch between vendor designs](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-switch.md#use-the-extended-vendor-design-for-vendors-of-the-organization-type).</span></span>

### <a name="set-products-to-be-created-as-active"></a><span data-ttu-id="75865-143">Задайте продукти, които да бъдат създадени като активни</span><span class="sxs-lookup"><span data-stu-id="75865-143">Set products to be created as active</span></span>

<span data-ttu-id="75865-144">Не складираните материали трябва да бъдат конфигурирани като **Издадени продукти** във Finance.</span><span class="sxs-lookup"><span data-stu-id="75865-144">Non-stocked materials must be configured as **Released products** in Finance.</span></span> <span data-ttu-id="75865-145">Решението за двойна записваща оркестрация предлага предварително подготвен [Продуктов каталог с интеграция на издадени продукти в Dataverse](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/product-mapping.md).</span><span class="sxs-lookup"><span data-stu-id="75865-145">The Dual Write Orchestration solution provides an out-of-the-box [Released products integration to Dataverse Product catalog](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/product-mapping.md).</span></span> <span data-ttu-id="75865-146">По подразбиране продуктите от Finance се синхронизират с Dataverse в състояние на чернова.</span><span class="sxs-lookup"><span data-stu-id="75865-146">By default, products from Finance are synchronized to Dataverse in a draft state.</span></span> <span data-ttu-id="75865-147">За да синхронизирате продукта в активно състояние, така че да може да се използва директно в документи за използване на материали или в чакащи фактури на доставчици, отидете на **Система** > **Администрация** > **Администрация на системата** > **Системни настройки** и в раздел **Продажби**, задайте **Създавайте продукти в активно състояние** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="75865-147">To synchronize the product to an active state so that it can be directly used in material usage documents or pending vendor invoices, go to **System** > **Administration** > **System administration** > **System settings**, and on the **Sales** tab, set **Create products in active state** to **Yes**.</span></span>

## <a name="configure-prerequisites-in-finance"></a><span data-ttu-id="75865-148">Конфигуриране на предпоставки във Finance</span><span class="sxs-lookup"><span data-stu-id="75865-148">Configure prerequisites in Finance</span></span>

### <a name="enable-the-feature-key-for-pending-vendor-invoices"></a><span data-ttu-id="75865-149">Активирайте функционалния ключ за чакащи фактури на доставчици</span><span class="sxs-lookup"><span data-stu-id="75865-149">Enable the feature key for pending vendor invoices</span></span>

<span data-ttu-id="75865-150">Изпълнете следните стъпки, за да активирате функционалността за добавяне на подробности за проекта към чакащите линии на фактури на доставчик.</span><span class="sxs-lookup"><span data-stu-id="75865-150">Complete the following steps to enable functionality to add project details on pending vendor invoice lines.</span></span>

1. <span data-ttu-id="75865-151">Във Finance отидете на работно пространство **Управление на функции**.</span><span class="sxs-lookup"><span data-stu-id="75865-151">In Finance, go to the **Feature Management** workspace.</span></span>
2. <span data-ttu-id="75865-152">В списъка с функции намерете функция **Активирайте чакащите фактури на доставчици за Project Operations за сценарии, базирани на ресурси/нескладирани** и изберете **Активиране**.</span><span class="sxs-lookup"><span data-stu-id="75865-152">In the feature list, find **Enable pending vendor invoices on Project Operations for resource based/non-stocked scenarios** feature and select **Enable**.</span></span>

### <a name="define-category-groups-and-project-categories-for-items"></a><span data-ttu-id="75865-153">Определете групи категории и категории проекти за елементи</span><span class="sxs-lookup"><span data-stu-id="75865-153">Define category groups and project categories for items</span></span>

<span data-ttu-id="75865-154">Конфигурирайте поне една категория група за тип транзакция **елемент** и поне една категория проекти, използващи тази група.</span><span class="sxs-lookup"><span data-stu-id="75865-154">Configure at least one category group for the **Item** transaction type , and at least one project category using this group.</span></span> <span data-ttu-id="75865-155">За повече информация вижте [Конфигуриране на категории на проект](../project-accounting/configure-project-categories.md#category-groups).</span><span class="sxs-lookup"><span data-stu-id="75865-155">For more information, see [Configure project categories](../project-accounting/configure-project-categories.md#category-groups).</span></span>

<span data-ttu-id="75865-156">Прегледайте профилите на разходите и приходите на проекта и конфигурирайте настройката за осчетоводяване на книга за транзакции на артикули.</span><span class="sxs-lookup"><span data-stu-id="75865-156">Review the project cost and revenue profiles, and configure ledger posting setup for item transactions.</span></span> <span data-ttu-id="75865-157">За повече информация вижте [Конфигурирайте счетоводство за фактурирани проекти](../project-accounting/configure-accounting-billable-projects.md).</span><span class="sxs-lookup"><span data-stu-id="75865-157">For more information, see [Configure accounting for billable projects](../project-accounting/configure-accounting-billable-projects.md).</span></span>

### <a name="set-up-a-write-in-product"></a><span data-ttu-id="75865-158">Настройване на ръчно съставен елемент</span><span class="sxs-lookup"><span data-stu-id="75865-158">Set up a write-in product</span></span>

<span data-ttu-id="75865-159">В Project Operations можете да записвате приблизителни оценки и използване на материали за каталожни продукти, които са конфигурирани в пуснатия продуктов каталог и за продукти за вписване.</span><span class="sxs-lookup"><span data-stu-id="75865-159">In Project Operations, you can record material estimates and usage for catalog products that are configured in the released product catalog and for write-in products.</span></span> <span data-ttu-id="75865-160">Използването на продукти за записване изисква един освободен продукт, който е конфигуриран във Finance за тази цел.</span><span class="sxs-lookup"><span data-stu-id="75865-160">Using write-in products requires a single released product that's configured in Finance for this purpose.</span></span> <span data-ttu-id="75865-161">Изпълнете следните стъпки, за да конфигурирате продукт за запис.</span><span class="sxs-lookup"><span data-stu-id="75865-161">Complete the following steps to configure a write-in product.</span></span> <span data-ttu-id="75865-162">Повторете тези стъпки във всяко юридическо лице, което използва Project Operations за ресурсни / нескладови сценарии.</span><span class="sxs-lookup"><span data-stu-id="75865-162">Repeat these steps in each legal entity that is using Project Operations for resource/non-stocked scenarios.</span></span>

1. <span data-ttu-id="75865-163">В областта на финансите отидете на **Управление на информацията за продукта** > **Продукти** > **Издадени продукти** и изберете **Създаване**.</span><span class="sxs-lookup"><span data-stu-id="75865-163">In Finance, go to **Product Information Management** > **Products** > **Released products**, and select **New**.</span></span>
2. <span data-ttu-id="75865-164">В полето **Вид на продукта** изберете **Елемент** и в полето **Подтип на продукта** изберете **Продукт**.</span><span class="sxs-lookup"><span data-stu-id="75865-164">In the **Product type** field, select **Item** and in the **Product subtype** field, select **Product**.</span></span>
3. <span data-ttu-id="75865-165">Въведете номера на продукта (WRITEIN) и името на продукта (ръчно съставен елемент).</span><span class="sxs-lookup"><span data-stu-id="75865-165">Enter the product number (WRITEIN) and the product name (Write-in Product).</span></span>
4. <span data-ttu-id="75865-166">Изберете групата на моделите на артикули.</span><span class="sxs-lookup"><span data-stu-id="75865-166">Select  the item model group.</span></span> <span data-ttu-id="75865-167">Уверете се, че избраната от вас група модели артикули има полето **Политика на инвентар Складиран продукт**, зададено на **Невярно**.</span><span class="sxs-lookup"><span data-stu-id="75865-167">Make sure that the item model group you select has the **Inventory policy Stocked product** field set to **False**.</span></span>
5. <span data-ttu-id="75865-168">Изберете стойности в **Група артикули**, **Група с измерения за съхранение** и **Проследяваща група измерения** полета.</span><span class="sxs-lookup"><span data-stu-id="75865-168">Select values in the **Item group**, **Storage dimension group**, and **Tracking dimension group** fields.</span></span> <span data-ttu-id="75865-169">Използвайте само **Размери на съхранение** за **Сайт** и не задавайте никакви проследяващи размери.</span><span class="sxs-lookup"><span data-stu-id="75865-169">Use the **Storage dimension** for **Site** only, and do not set any tracking dimensions.</span></span>
6. <span data-ttu-id="75865-170">Изберете стойности в **Инвентарна единица**, **Покупна единица** и **Търговска единица** и след това запазете промените.</span><span class="sxs-lookup"><span data-stu-id="75865-170">Select values in the **Inventory unit**, **Purchase unit**, and **Sales unit** field, and then save your changes.</span></span>
7. <span data-ttu-id="75865-171">В раздела **План** задайте настройките по подразбиране за реда и на раздела **Складова наличност** задайте сайта и склада по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="75865-171">In the **Plan** tab, set the default order settings, and on the **Inventory** tab, set the default site and warehouse.</span></span>
8. <span data-ttu-id="75865-172">Отидете на **Управление на проекти и счетоводство** > **Настройвам** > **Управление на проекти и счетоводни параметри** и отворете **Project Operations в Dynamics 365 Dataverse**.</span><span class="sxs-lookup"><span data-stu-id="75865-172">Go to **Project management and accounting** > **Setup** > **Project management and accounting parameters** and open **Project Operations on Dynamics 365 Dataverse**.</span></span> 
9. <span data-ttu-id="75865-173">На раздела **Материали** в полето **ръчно съставен елемент** изберете продукта, който сте създали.</span><span class="sxs-lookup"><span data-stu-id="75865-173">On the **Materials** tab, in the **Write-in product** field, select the product you created.</span></span>
10. <span data-ttu-id="75865-174">В средата ви на Dataverse, в картата на сайта отворете обекта **Продукти** и намерете записания продукт за запис.</span><span class="sxs-lookup"><span data-stu-id="75865-174">In your Dataverse environment, in the site map, open the **Products** entity and find the write-in product record.</span></span> 
11. <span data-ttu-id="75865-175">Отворете данните за записа и задайте състоянието на продукта на **Изтеглено от употреба**.</span><span class="sxs-lookup"><span data-stu-id="75865-175">Open the record details and set product state to **Retired**.</span></span> <span data-ttu-id="75865-176">Това състояние на продукта предотвратява случайно използване на този запис директно в разчетите за материали и документи за употреба.</span><span class="sxs-lookup"><span data-stu-id="75865-176">This product state prevents anyone from accidentally using this record directly in material estimates and usage documents.</span></span>

### <a name="set-up-a-procurement-integration-account"></a><span data-ttu-id="75865-177">Създайте акаунт за интеграция на обществени поръчки</span><span class="sxs-lookup"><span data-stu-id="75865-177">Set up a procurement integration account</span></span>

<span data-ttu-id="75865-178">Сметката за интеграция на поръчки се използва като клирингов акаунт при публикуване на чакаща фактура на доставчик с редове, приписани на проект.</span><span class="sxs-lookup"><span data-stu-id="75865-178">The procurement integration account is used as a clearing account when posting a pending vendor invoice with lines attributed to a project.</span></span>

<span data-ttu-id="75865-179">Когато системата осчетоводи изчакваща фактура на доставчик, този акаунт се използва за сумата на разходите по проекта.</span><span class="sxs-lookup"><span data-stu-id="75865-179">When the system posts a pending vendor invoice, this account is used for the project cost amount.</span></span> <span data-ttu-id="75865-180">Данните за фактурите на доставчика се обработват в Dataverse, и се създава съответен действителен проект.</span><span class="sxs-lookup"><span data-stu-id="75865-180">The vendor invoice details are processed in Dataverse, and a corresponding project actual is created.</span></span> <span data-ttu-id="75865-181">Информацията от действителния проект се добавя към списанието Project Operations Integration.</span><span class="sxs-lookup"><span data-stu-id="75865-181">The information from the project actual is added to the Project Operations Integration journal.</span></span> <span data-ttu-id="75865-182">Когато публикувате дневника за интеграция, сумата се изчиства от сметката за интеграция на поръчки и се записва в разходите по проекта.</span><span class="sxs-lookup"><span data-stu-id="75865-182">When you post the integration journal, the amount is cleared from the procurement integration account and recorded to the project cost.</span></span>

1. <span data-ttu-id="75865-183">За да създадете акаунт за интеграция на осигуряване, отидете на **Управление на проекти и счетоводство** > **Настройка** > **Управление на проекти и счетоводни параметри** и отворете **Project Operations върху Dynamics 365 Dataverse**.</span><span class="sxs-lookup"><span data-stu-id="75865-183">To set up the procurement integration account, go to **Project management and accounting** > **Setup** > **Project management and accounting parameters**, and open **Project Operations on Dynamics 365 Dataverse**.</span></span> 
2. <span data-ttu-id="75865-184">Изберете раздел **Материали** и изберете стойност в полето **Сметка за интеграция на поръчки**.</span><span class="sxs-lookup"><span data-stu-id="75865-184">Select the **Materials** tab, and select a value in the **Procurement integration account** field.</span></span>

#### <a name="set-up-project-category-defaults-for-an-item"></a><span data-ttu-id="75865-185">Настройте по подразбиране категорията на проекта за даден елемент</span><span class="sxs-lookup"><span data-stu-id="75865-185">Set up project category defaults for an item</span></span>

1. <span data-ttu-id="75865-186">Във Finance отидете на **Управление на проекти и счетоводство** > **Настройка** > **Управление на проекти и счетоводни параметри** и отворете **Project Operations в Dynamics 365 Dataverse**.</span><span class="sxs-lookup"><span data-stu-id="75865-186">In Finance, go to **Project management and accounting** > **Setup** > **Project management and accounting parameters**, and open **Project Operations on Dynamics 365 Dataverse**.</span></span> 
2. <span data-ttu-id="75865-187">В раздела **Стойности по подразбиране за категорията на проекта** в полето **Артикул** изберете стойност.</span><span class="sxs-lookup"><span data-stu-id="75865-187">On the **Project category defaults** tab, in the **Item** field, select a value.</span></span> <span data-ttu-id="75865-188">Тази категория на проекта се използва за материални транзакции, ако категорията на проекта не е зададена в реалния запис на проекта.</span><span class="sxs-lookup"><span data-stu-id="75865-188">This project category is used for material transactions if the project category wasn't set on the project actuals record.</span></span>