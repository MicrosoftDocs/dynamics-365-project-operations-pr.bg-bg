---
title: Умения и модели на опитност
description: Тази тема предоставя информация за това как да използвате уменията и моделите на опитност.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/13/2019
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
ms.openlocfilehash: c7da8b2a7eda51b2aa7cf04e325a92f33d834efc
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147460"
---
# <a name="skills-and-proficiency-models"></a><span data-ttu-id="02560-103">Умения и модели на опитност</span><span class="sxs-lookup"><span data-stu-id="02560-103">Skills and proficiency models</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="02560-104">Уменията са характеристики на ресурсите, които се споделят между Dynamics 365 Project Service Automation и Dynamics 365 Field Service, ако е налице.</span><span class="sxs-lookup"><span data-stu-id="02560-104">Skills are resource characteristics that are shared between Dynamics 365 Project Service Automation and if present, Dynamics 365 Field Service.</span></span> 

<span data-ttu-id="02560-105">За да поддържате хранилището с умения в Project Service Automation, отидете в **Ресурси** \> **Умения на ресурси**.</span><span class="sxs-lookup"><span data-stu-id="02560-105">To maintain the repository of skills in Project Service Automation, go to **Resources** \> **Resource Skills**.</span></span> 

> ![Умения на ресурси](media/Resource-Management-image84.png)

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="02560-107">Използване на модели на опитност за оценка на ресурси</span><span class="sxs-lookup"><span data-stu-id="02560-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="02560-108">Уменията на ресурсите се оценяват чрез модели на опитност.</span><span class="sxs-lookup"><span data-stu-id="02560-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="02560-109">Индивидуалните оценки са в модел на опитност.</span><span class="sxs-lookup"><span data-stu-id="02560-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="02560-110">За да създадете модел на опитност, отидете в **Ресурси** \> **Модели на опитност** и след това изберете **Нов**.</span><span class="sxs-lookup"><span data-stu-id="02560-110">To create a proficiency model, go to **Resources** \> **Proficiency Models**, and then select **New**.</span></span>
2. <span data-ttu-id="02560-111">В новия модел на оценка укажете минималната стойност на оценка, максималната стойност на оценка и обекта, който се оценява.</span><span class="sxs-lookup"><span data-stu-id="02560-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="02560-112">В подмрежата **Стойности на оценки** можете да дефинирате различните стойности на оценки – от минималната до максималната.</span><span class="sxs-lookup"><span data-stu-id="02560-112">In the **Rating Values** subgrid, you can define the different rating values, from the minimum to the maximum.</span></span>

> ![Дефинирани минимални и максимални оценки](media/Resource-Management-image85.png)

<span data-ttu-id="02560-114">Тези стойности на оценки се показват във филтрите **Изисквания за ресурси**, **Табло на графика** и **Асистент за планиране**.</span><span class="sxs-lookup"><span data-stu-id="02560-114">These rating values are shown on the **Resource Requirements**, **Schedule Board**, and **Schedule Assistant** filters.</span></span>
