---
title: Актуализиране на проект
description: Тази тема предоставя информация за актуализирането на проекти в Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: c07542444b970430d8143a60aad6970305769b22
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993358"
---
# <a name="update-a-project"></a><span data-ttu-id="7312b-103">Актуализиране на проект</span><span class="sxs-lookup"><span data-stu-id="7312b-103">Update a project</span></span>

<span data-ttu-id="7312b-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="7312b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7312b-105">По-долу е дадено обобщение на полетата, които могат да бъдат актуализирани за даден проект, след като е създаден, и всички приложими последици от актуализациите.</span><span class="sxs-lookup"><span data-stu-id="7312b-105">Below is a summary of the fields that can be updated on a project after it has been created and any applicable implications of the updates.</span></span>

## <a name="project-detail-fields"></a><span data-ttu-id="7312b-106">Полета с подробности за проекта</span><span class="sxs-lookup"><span data-stu-id="7312b-106">Project detail fields</span></span>

- <span data-ttu-id="7312b-107">**Име**: Заглавието на проекта.</span><span class="sxs-lookup"><span data-stu-id="7312b-107">**Name**: The title of the project.</span></span>
- <span data-ttu-id="7312b-108">**Описание**: Общ преглед на проекта.</span><span class="sxs-lookup"><span data-stu-id="7312b-108">**Description**: An overview of the project.</span></span>
- <span data-ttu-id="7312b-109">**Клиент**: Компанията, на която ще бъде доставен проектът.</span><span class="sxs-lookup"><span data-stu-id="7312b-109">**Customer**: The company the project will be delivered to.</span></span>
- <span data-ttu-id="7312b-110">**Шаблон за календар**: Работното време на проекта.</span><span class="sxs-lookup"><span data-stu-id="7312b-110">**Calendar template**: The working hours of the project.</span></span> <span data-ttu-id="7312b-111">Когато полето се промени, целият график се преизчислява.</span><span class="sxs-lookup"><span data-stu-id="7312b-111">When the field is changed, the entire schedule is recalculated.</span></span>
- <span data-ttu-id="7312b-112">**Валута**: Валутата за проекта.</span><span class="sxs-lookup"><span data-stu-id="7312b-112">**Currency**: The currency for the project.</span></span> <span data-ttu-id="7312b-113">Това поле по подразбиране се базира на валутата, определена в договарящата единица.</span><span class="sxs-lookup"><span data-stu-id="7312b-113">This field defaults based on the currency defined in the contracting unit.</span></span> <span data-ttu-id="7312b-114">Когато договорната единица се актуализира, полето също се актуализира.</span><span class="sxs-lookup"><span data-stu-id="7312b-114">When the contracting unit is updated, the field is also updated.</span></span>
- <span data-ttu-id="7312b-115">**Единица, сключваща договора**: Организационната единица, представляваща групата или отдела на компанията, която е основно отговорна за спечелването на продажбата и управлението на доставката на работа и услуги на клиента.</span><span class="sxs-lookup"><span data-stu-id="7312b-115">**Contracting Unit**: The organizational unit that represents the company group or division that is primarily responsible for winning the sale and managing the delivery of work and services to the customer.</span></span> 
- <span data-ttu-id="7312b-116">**Ръководител проект**: Членът на проектния екип, който има правомощието да преглежда и одобрява записването на време и разходите.</span><span class="sxs-lookup"><span data-stu-id="7312b-116">**Project Manager**: The project team member who has the authority to review and approve time entries and expenses.</span></span>

## <a name="estimate-fields"></a><span data-ttu-id="7312b-117">Полета за оценка</span><span class="sxs-lookup"><span data-stu-id="7312b-117">Estimate fields</span></span>

- <span data-ttu-id="7312b-118">**Очаквана начална дата**: Датата, на която проектът ще започне.</span><span class="sxs-lookup"><span data-stu-id="7312b-118">**Estimated Start Date**: The date that the project will begin.</span></span> <span data-ttu-id="7312b-119">Когато това поле се актуализира, всички задачи в проекта ще се движат пропорционално на началната нова начална дата.</span><span class="sxs-lookup"><span data-stu-id="7312b-119">When this field is updated, any tasks on the project will move proportionately with the start new start date.</span></span>
- <span data-ttu-id="7312b-120">**Крайна дата**: Датата, на която проектът е планиран да приключи.</span><span class="sxs-lookup"><span data-stu-id="7312b-120">**Finish Date**: The date that the project is scheduled to end.</span></span>
- <span data-ttu-id="7312b-121">**Усилие**: Очакваните усилия на проекта.</span><span class="sxs-lookup"><span data-stu-id="7312b-121">**Effort**: The estimated effort of the project.</span></span> <span data-ttu-id="7312b-122">Когато задачите се добавят към проекта, това поле вече не може да се редактира.</span><span class="sxs-lookup"><span data-stu-id="7312b-122">When tasks are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="7312b-123">**Очаквани разходи за труд**: Очакваните разходи за труд на проекта.</span><span class="sxs-lookup"><span data-stu-id="7312b-123">**Estimated Labor Cost**: The estimated labor cost of the project.</span></span> <span data-ttu-id="7312b-124">Когато разходите за труд се добавят към проекта, това поле вече не може да се редактира.</span><span class="sxs-lookup"><span data-stu-id="7312b-124">When labor costs are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="7312b-125">**Очаквани разходи**: Очакваните разходи по проекта.</span><span class="sxs-lookup"><span data-stu-id="7312b-125">**Estimated Expenses**: The estimated expenses of the project.</span></span> <span data-ttu-id="7312b-126">Когато разходите се добавят към проекта, това поле вече не може да се редактира.</span><span class="sxs-lookup"><span data-stu-id="7312b-126">When expenses are added to the project, this field is no longer editable.</span></span>

## <a name="project-actual-fields"></a><span data-ttu-id="7312b-127">Проектирайте действителни полета</span><span class="sxs-lookup"><span data-stu-id="7312b-127">Project actual fields</span></span>
- <span data-ttu-id="7312b-128">**Действително начало**: Датата на стартиране на проекта.</span><span class="sxs-lookup"><span data-stu-id="7312b-128">**Actual Start**: The date that the project started.</span></span>
- <span data-ttu-id="7312b-129">**Действително завършване**: Да се актуализира, когато даден проект е завършен.</span><span class="sxs-lookup"><span data-stu-id="7312b-129">**Actual Finish**: To be updated when a project has been completed.</span></span>

## <a name="project-status-fields"></a><span data-ttu-id="7312b-130">Полета за състояние на проект</span><span class="sxs-lookup"><span data-stu-id="7312b-130">Project status fields</span></span>

- <span data-ttu-id="7312b-131">**Общо състояние на проекта**: Цялостното състояние на проекта, осигурено от ръководителя на проекта.</span><span class="sxs-lookup"><span data-stu-id="7312b-131">**Overall Project Status**: The overall project health provided by the Project manager.</span></span>
- <span data-ttu-id="7312b-132">**Коментари**: Разказ относно текущото състояние на проекта, предоставен от ръководителя на проекта.</span><span class="sxs-lookup"><span data-stu-id="7312b-132">**Comments**: A narrative regarding the current health of the project provided by the Project manager.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]