---
title: Актуализиране на оценка при завършване
description: Тази тема предоставя информация за актуализиране на прогнозата за усилията върху даден проект.
author: ruhercul
manager: AnnBe
ms.date: 09/20/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: 0e63bdb815a6f758c57d055c8c03d92e04700445
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286415"
---
# <a name="update-estimate-at-completion"></a><span data-ttu-id="b2207-103">Актуализиране на оценка при завършване</span><span class="sxs-lookup"><span data-stu-id="b2207-103">Update estimate at completion</span></span>

<span data-ttu-id="b2207-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="b2207-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b2207-105">Обичайно за ръководител на проект е да преразглежда на първоначалните прогнозни оценки за задача.</span><span class="sxs-lookup"><span data-stu-id="b2207-105">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="b2207-106">Повторните прогнози на проекта са разбирането на прогнозните оценки на ръководителя на проекта, като се има предвид текущото състояние на проекта.</span><span class="sxs-lookup"><span data-stu-id="b2207-106">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="b2207-107">Ние обаче не препоръчваме на мениджърите на проекти да променят базовите числа, защото базовата линия на проекта представлява установеният източник на достоверни данни за графика на проекта и прогнозните разходи и всички заинтересовани лица по проекта са я приели.</span><span class="sxs-lookup"><span data-stu-id="b2207-107">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="b2207-108">Има два начина, по които ръководител на проект може да прогнозира повторно усилия по задачи:</span><span class="sxs-lookup"><span data-stu-id="b2207-108">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="b2207-109">Заместете прогнозата по подразбиране, за да попълните (ОДЗ) по подразбиране с нова прогнозна оценка на действителните оставащите усилия по задачата.</span><span class="sxs-lookup"><span data-stu-id="b2207-109">Override the default estimate to complete (ETC) with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="b2207-110">Заместване на процента на напредъка по подразбиране с нова прогнозна оценка на действителния напредък по задачата.</span><span class="sxs-lookup"><span data-stu-id="b2207-110">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="b2207-111">Всеки от тези подходи води до преизчисляване на ОДЗ, оценка при завършване (ОПЗ) и процента на напредък по задачата и прогнозираната разлика в усилията по дадена задача.</span><span class="sxs-lookup"><span data-stu-id="b2207-111">Each of these approaches cause a recalculation of the task's ETC, estimate at complete (EAC), and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="b2207-112">ОДЗ, ОПЗ и процентът на напредъка по обобщаващи задачи се преизчисляват и създават нова прогноза за разлика в усилията.</span><span class="sxs-lookup"><span data-stu-id="b2207-112">The EAC, ETC, and progress percentage on the summary tasks are recalculated, and produce a new projection of effort variance.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]