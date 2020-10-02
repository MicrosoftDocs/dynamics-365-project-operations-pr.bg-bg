---
title: Определяне на умения и опитност
description: Тази тема предоставя информация за това как да настройвате моделите на опитност за оценяване на ресурси.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 9376e0b268a3ab682716da604ceecfa1e878da68
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897618"
---
# <a name="define-skills-and-proficiencies"></a><span data-ttu-id="23d04-103">Определяне на умения и опитност</span><span class="sxs-lookup"><span data-stu-id="23d04-103">Define skills and proficiencies</span></span>

<span data-ttu-id="23d04-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="23d04-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="23d04-105">Уменията са характеристики на ресурсите, които се споделят между Dynamics 365 Project Operations и Dynamics 365 Field Service, ако е налице.</span><span class="sxs-lookup"><span data-stu-id="23d04-105">Skills are resource characteristics that are shared between Dynamics 365 Project Operations and if present, Dynamics 365 Field Service.</span></span> 

- <span data-ttu-id="23d04-106">За да поддържате хранилището с умения в Project Operations, отидете в **Ресурси** \> **Умения на ресурси**.</span><span class="sxs-lookup"><span data-stu-id="23d04-106">To maintain the repository of skills in Project Operations, go to **Resources** \> **Resource Skills**.</span></span> 

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="23d04-107">Използване на модели на опитност за оценка на ресурси</span><span class="sxs-lookup"><span data-stu-id="23d04-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="23d04-108">Уменията на ресурсите се оценяват чрез модели на опитност.</span><span class="sxs-lookup"><span data-stu-id="23d04-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="23d04-109">Индивидуалните оценки са в модел на опитност.</span><span class="sxs-lookup"><span data-stu-id="23d04-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="23d04-110">За да създадете модел на опитност, отидете в **Ресурси** \> **Модели на опитност** и след това изберете **Нов**.</span><span class="sxs-lookup"><span data-stu-id="23d04-110">To create a proficiency model, go to **Resources** \> **Proficiency Models**, and then select **New**.</span></span>
2. <span data-ttu-id="23d04-111">В новия модел на оценка укажете минималната стойност на оценка, максималната стойност на оценка и обекта, който се оценява.</span><span class="sxs-lookup"><span data-stu-id="23d04-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="23d04-112">В подмрежата **Стойности на оценки** можете да дефинирате различните стойности на оценки – от минималната до максималната.</span><span class="sxs-lookup"><span data-stu-id="23d04-112">In the **Rating Values** sub-grid, you can define the different rating values, from the minimum to the maximum.</span></span>


<span data-ttu-id="23d04-113">Тези стойности на оценки се показват във филтрите **Изисквания за ресурси**, **Табло на графика** и **Асистент за планиране**.</span><span class="sxs-lookup"><span data-stu-id="23d04-113">These rating values are shown on the **Resource Requirements**, **Schedule Board**, and **Schedule Assistant** filters.</span></span>
