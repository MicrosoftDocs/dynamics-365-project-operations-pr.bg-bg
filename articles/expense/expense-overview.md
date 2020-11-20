---
title: Общ преглед на разход
description: Тази тема предоставя информация за функционалността Разход в Project Operations.
author: stsporen
manager: AnnBe
ms.date: 10/06/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 6c5ef2a45e8141bda38baf3eaf0a403d6db95e48
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122809"
---
# <a name="expense-home-page"></a><span data-ttu-id="b62fc-103">Начална страница за разходи</span><span class="sxs-lookup"><span data-stu-id="b62fc-103">Expense home page</span></span>

<span data-ttu-id="b62fc-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="b62fc-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="b62fc-105">Dynamics 365 Project Operations поддържа възможността за обработка на разходи.</span><span class="sxs-lookup"><span data-stu-id="b62fc-105">Dynamics 365 Project Operations supports the ability to process expenses.</span></span> <span data-ttu-id="b62fc-106">Обработката на разходите се извършва със или без проекти чрез използване на персонализиран работен поток от политики, категории транзакции и одобрения.</span><span class="sxs-lookup"><span data-stu-id="b62fc-106">Expense processing occurs with or without projects by using a customizable workflow of policies, transaction categories, and approvals.</span></span>

<span data-ttu-id="b62fc-107">В Project Operations има два поддържани модела за внедряване на разходи:</span><span class="sxs-lookup"><span data-stu-id="b62fc-107">In Project Operations, there are two supported deployment models for Expense:</span></span> 

- <span data-ttu-id="b62fc-108">**Пълно**: На разположение е пълно разгръщане **Project Operations за сценарии, базирани на ресурси / без наличност** или **Project Operations за сценарии, базирани на производствени поръчки**.</span><span class="sxs-lookup"><span data-stu-id="b62fc-108">**Full**: Full deployment is available for **Project Operations for resource/non-stocked based scenarios** or **Project Operations for production order based scenarios**.</span></span>
- <span data-ttu-id="b62fc-109">**Основно**: Основното разполагане е достъпно за **Project Operations за сценарии, базирани на ресурси / без наличност** и **Олекотено внедряване - сделка за проформа фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="b62fc-109">**Basic**: Basic deployment is available for **Project Operations for resource/non-stocked based scenarios** and **Lite deployment – deal to proforma invoicing**.</span></span>

## <a name="full"></a><span data-ttu-id="b62fc-110">Пълен</span><span class="sxs-lookup"><span data-stu-id="b62fc-110">Full</span></span> 
<span data-ttu-id="b62fc-111">Разгръщането на Пълен разход осигурява пълно прилагане на политиката, което включва възможността за създаване на политики, като например:</span><span class="sxs-lookup"><span data-stu-id="b62fc-111">Full Expense deployment provides a complete policy enforcement which includes the ability to create policies, such as:</span></span>

  - <span data-ttu-id="b62fc-112">Ограничения на категория на разход</span><span class="sxs-lookup"><span data-stu-id="b62fc-112">Expense category limits</span></span>
  - <span data-ttu-id="b62fc-113">Пътуване</span><span class="sxs-lookup"><span data-stu-id="b62fc-113">Travel</span></span>
  - <span data-ttu-id="b62fc-114">Дневни</span><span class="sxs-lookup"><span data-stu-id="b62fc-114">Per diem</span></span>
  - <span data-ttu-id="b62fc-115">Импортирания на кредитната карта</span><span class="sxs-lookup"><span data-stu-id="b62fc-115">Credit card imports</span></span>
  - <span data-ttu-id="b62fc-116">Получаване на оптично разпознаване на символи</span><span class="sxs-lookup"><span data-stu-id="b62fc-116">Receipt optical character recognition</span></span>

## <a name="basic"></a><span data-ttu-id="b62fc-117">Основен</span><span class="sxs-lookup"><span data-stu-id="b62fc-117">Basic</span></span> 
<span data-ttu-id="b62fc-118">Сценарият за внедряване на Основен разход ви позволява да записвате само основни разходи спрямо проект.</span><span class="sxs-lookup"><span data-stu-id="b62fc-118">Basic Expense deployment scenario only allows you to record basic expenses against a project.</span></span> 

<span data-ttu-id="b62fc-119">За повече информация вижте [Вписване на разходи (олекотен)](basic-expense.md)</span><span class="sxs-lookup"><span data-stu-id="b62fc-119">For more information, see [Expense entry (lite)](basic-expense.md)</span></span>

## <a name="determine-your-expense-deployment"></a><span data-ttu-id="b62fc-120">Определяне типа на внедряването на разход</span><span class="sxs-lookup"><span data-stu-id="b62fc-120">Determine your Expense deployment</span></span>
<span data-ttu-id="b62fc-121">За да определите дали изпълнявате внедряването на управление на основните разходи, проверете дали URL адресът на адреса завършва с **.crm.dynamics.com**.</span><span class="sxs-lookup"><span data-stu-id="b62fc-121">To determine if you're running the Basic Expense management deployment, verify that the address URL ends with **.crm.dynamics.com**.</span></span> 
