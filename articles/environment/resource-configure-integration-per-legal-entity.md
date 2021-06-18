---
title: Конфигуриране на интеграция на Project Operations на юридическо лице
description: Тази тема предоставя информация за настройка на интеграция от юридическо лице в Project Operations.
author: sigitac
ms.date: 10/21/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e5a12de275a9f886434da45fbbed5140e3913d83
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000063"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a><span data-ttu-id="dd531-103">Конфигуриране на интеграция на Project Operations на юридическо лице</span><span class="sxs-lookup"><span data-stu-id="dd531-103">Configure Project Operations integration per legal entity</span></span> 

<span data-ttu-id="dd531-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="dd531-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="dd531-105">Тази тема ще ви преведе през стъпките, необходими за конфигуриране на Dynamics 365 Project Operations на база юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="dd531-105">This topic walks you through the steps required to configure Dynamics 365 Project Operations per legal entity.</span></span>

## <a name="enable-feature-keys-in-dynamics-365-finance"></a><span data-ttu-id="dd531-106">Активиране на клавиши за функции Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="dd531-106">Enable feature keys in Dynamics 365 Finance</span></span>

<span data-ttu-id="dd531-107">Изпълнете следните стъпки, за да активирате необходимите функции.</span><span class="sxs-lookup"><span data-stu-id="dd531-107">Complete the following steps to enable required features.</span></span>

1. <span data-ttu-id="dd531-108">В Dynamics 365 Finance отидете на работното пространство **Управление на функции**.</span><span class="sxs-lookup"><span data-stu-id="dd531-108">In Dynamics 365 Finance, go to the **Feature Management** workspace.</span></span>
2. <span data-ttu-id="dd531-109">В **Списък с функции**, намерете и активирайте следните функции:</span><span class="sxs-lookup"><span data-stu-id="dd531-109">In **Feature list**, find and enable the following features:</span></span>
  
    - <span data-ttu-id="dd531-110">**Активирайте множество договорени линии за проект**</span><span class="sxs-lookup"><span data-stu-id="dd531-110">**Enable multiple contract lines for a project**</span></span>
    - <span data-ttu-id="dd531-111">**Активиране на Project Operations в Dynamics 365 Customer Engagement**</span><span class="sxs-lookup"><span data-stu-id="dd531-111">**Enable Project Operations on Dynamics 365 Customer Engagement**</span></span>

> [!NOTE]
> <span data-ttu-id="dd531-112">Ако не виждате изброени **Клавиши за функции** проверете дали вашата версия на финансите отговаря на изискването за минимална версия (версия на приложението 10.0.13 с приложени всички актуализации на качеството или по-нова версия).</span><span class="sxs-lookup"><span data-stu-id="dd531-112">If you don't see **Feature keys** listed, verify that your Finance version meets the minimum version requirement (application version 10.0.13 with all quality updates applied or higher).</span></span> <span data-ttu-id="dd531-113">Изберете **Провери за актуализации**, за да опресните списъка с функции.</span><span class="sxs-lookup"><span data-stu-id="dd531-113">Select **Check for updates** to refresh the feature list.</span></span>

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a><span data-ttu-id="dd531-114">Определете сценария за внедряване на Project Operations за юридическо лице</span><span class="sxs-lookup"><span data-stu-id="dd531-114">Define the Project Operations deployment scenario for a legal entity</span></span>

<span data-ttu-id="dd531-115">Можете да активирате Project Operations на Dynamics 365 Customer Engagement на ниво юридическо лице.</span><span class="sxs-lookup"><span data-stu-id="dd531-115">You can enable Project Operations on Dynamics 365 Customer Engagement on a legal entity level.</span></span> <span data-ttu-id="dd531-116">Можете да имате едно юридическо лице, използващо Project Operations на Dynamics 365 Customer Engagement за сценарии, базирани на ресурси / на склад.</span><span class="sxs-lookup"><span data-stu-id="dd531-116">You can have one legal entity using Project Operations on Dynamics 365 Customer Engagement for resource/non-stocked based scenarios.</span></span> <span data-ttu-id="dd531-117">В същата среда можете да имате друго юридическо лице, използващо Project Operations за складови / производствени сценарии.</span><span class="sxs-lookup"><span data-stu-id="dd531-117">In the same environment, you can have another legal entity using Project Operations for stocked/production order scenarios.</span></span>

1. <span data-ttu-id="dd531-118">В Dynamics 365 Finance отидете на **Управление на проекти и счетоводство** > **Настройка** > **Глобално управление на проекти и счетоводни параметри**.</span><span class="sxs-lookup"><span data-stu-id="dd531-118">In Dynamics 365 Finance, go to **Project management and accounting** > **Setup** > **Global project management and accounting parameters**.</span></span>
2. <span data-ttu-id="dd531-119">В списъка на наличните юридически лица изберете субекти, в които са включени множество договорни линии и Project Operations за функции на Dynamics 365 Customer Engagement ще бъдат активирани.</span><span class="sxs-lookup"><span data-stu-id="dd531-119">In the list of available legal entities, select entities where multiple contract lines and Project Operations on Dynamics 365 Customer Engagement features will be enabled.</span></span> <span data-ttu-id="dd531-120">Оставете неизбрани юридически лица, които ще използват проектни операции за сценарии за складирани / производствени поръчки.</span><span class="sxs-lookup"><span data-stu-id="dd531-120">Leave legal entities that will be using Project Operations for stocked/production order scenarios unselected.</span></span>

> [!NOTE]
> <span data-ttu-id="dd531-121">Юридическо лице може да бъде избрано само ако няма съществуващи проекти.</span><span class="sxs-lookup"><span data-stu-id="dd531-121">A legal entity can be selected only if it doesn't have any existing projects.</span></span>

## <a name="configure-project-management-and-accounting-parameters"></a><span data-ttu-id="dd531-122">Конфигуриране на управление на проект и параметри на счетоводство</span><span class="sxs-lookup"><span data-stu-id="dd531-122">Configure Project management and accounting parameters</span></span>

<span data-ttu-id="dd531-123">Всяко юридическо лице, използващо проектни операции на Dynamics 365 Customer Engagement се нуждае от набор от параметри по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="dd531-123">Each legal entity using Project Operations on Dynamics 365 Customer Engagement needs a set of default parameters.</span></span> <span data-ttu-id="dd531-124">Тези параметри са конфигурирани на раздел **Project Operations** на страница **Управление на проекти и счетоводни параметри**.</span><span class="sxs-lookup"><span data-stu-id="dd531-124">These parameters are configured on the **Project Operations** tab on the **Project management and accounting parameters** page.</span></span> <span data-ttu-id="dd531-125">Параметрите са:</span><span class="sxs-lookup"><span data-stu-id="dd531-125">The parameters are:</span></span>

  - <span data-ttu-id="dd531-126">**Тип фактуриране по подразбиране**: Project Operations използва фиксиран набор от стойности по подразбиране за фактуриране, които трябва да бъдат картографирани в свойствата на линията Finance.</span><span class="sxs-lookup"><span data-stu-id="dd531-126">**Billing type defaults**: Project Operations uses a fixed set of billing type defaults that must be mapped to line properties Finance.</span></span> <span data-ttu-id="dd531-127">Създайте запис за всеки вид фактуриране: **Неопределено**, **Платимо**, **Без такса**, **Безплатно** и **Не е налично**.</span><span class="sxs-lookup"><span data-stu-id="dd531-127">Create a record for each billing type: **Not specified**, **Chargeable**, **Non-chargeable**, **Complimentary**, and **Not available**.</span></span>
  - <span data-ttu-id="dd531-128">**По подразбиране за категорията на проекта**: Изберете категориите проекти по подразбиране, които да се използват за всеки тип транзакция.</span><span class="sxs-lookup"><span data-stu-id="dd531-128">**Project category defaults**: Select the default project categories to be used for each transaction type.</span></span> <span data-ttu-id="dd531-129">Тези настройки по подразбиране ще бъдат използвани в **Журнал за интеграция на Project Operations** и в прогнози, при които не е посочена категория транзакция за действителния проект.</span><span class="sxs-lookup"><span data-stu-id="dd531-129">These defaults will be used in the **Project Operations Integration journal** and in estimates where no transaction category is specified for the project actual.</span></span>
  - <span data-ttu-id="dd531-130">**Прогнози**: Изберете модела на прогнозата, който да се използва за прогнози за време и разходи.</span><span class="sxs-lookup"><span data-stu-id="dd531-130">**Forecasts**: Select the forecast model to be used for time and expense estimates.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]