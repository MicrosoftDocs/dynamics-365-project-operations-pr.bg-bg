---
title: Актуализиране на оценка при завършване
description: Тази тема предоставя информация за актуализиране на прогнозата за усилията върху даден проект.
author: ruhercul
manager: AnnBe
ms.date: 09/20/2020
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
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 42824cc4cfc2b934f69d319944fe7ee43183955c
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897753"
---
# <a name="update-estimate-at-completion"></a><span data-ttu-id="f8b9f-103">Актуализиране на оценка при завършване</span><span class="sxs-lookup"><span data-stu-id="f8b9f-103">Update estimate at completion</span></span>

<span data-ttu-id="f8b9f-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="f8b9f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f8b9f-105">Обичайно за ръководител на проект е да преразглежда на първоначалните прогнозни оценки за задача.</span><span class="sxs-lookup"><span data-stu-id="f8b9f-105">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="f8b9f-106">Повторните прогнози на проекта са разбирането на прогнозните оценки на ръководителя на проекта, като се има предвид текущото състояние на проекта.</span><span class="sxs-lookup"><span data-stu-id="f8b9f-106">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="f8b9f-107">Ние обаче не препоръчваме на мениджърите на проекти да променят базовите числа, защото базовата линия на проекта представлява установеният източник на достоверни данни за графика на проекта и прогнозните разходи и всички заинтересовани лица по проекта са я приели.</span><span class="sxs-lookup"><span data-stu-id="f8b9f-107">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="f8b9f-108">Има два начина, по които ръководител на проект може да прогнозира повторно усилия по задачи:</span><span class="sxs-lookup"><span data-stu-id="f8b9f-108">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="f8b9f-109">Заместете прогнозата по подразбиране, за да попълните (ОДЗ) по подразбиране с нова прогнозна оценка на действителните оставащите усилия по задачата.</span><span class="sxs-lookup"><span data-stu-id="f8b9f-109">Override the default estimate to complete (ETC) with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="f8b9f-110">Заместване на процента на напредъка по подразбиране с нова прогнозна оценка на действителния напредък по задачата.</span><span class="sxs-lookup"><span data-stu-id="f8b9f-110">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="f8b9f-111">Всеки от тези подходи води до преизчисляване на ОДЗ, оценка при завършване (ОПЗ) и процента на напредък по задачата и прогнозираната разлика в усилията по дадена задача.</span><span class="sxs-lookup"><span data-stu-id="f8b9f-111">Each of these approaches cause a recalculation of the task's ETC, estimate at complete (EAC), and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="f8b9f-112">ОДЗ, ОПЗ и процентът на напредъка по обобщаващи задачи се преизчисляват и създават нова прогноза за разлика в усилията.</span><span class="sxs-lookup"><span data-stu-id="f8b9f-112">The EAC, ETC, and progress percentage on the summary tasks are recalculated, and produce a new projection of effort variance.</span></span>
