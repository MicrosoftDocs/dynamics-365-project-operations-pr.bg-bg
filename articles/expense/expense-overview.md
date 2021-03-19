---
title: Общ преглед на разход
description: Тази тема предоставя информация за функционалността Разход в Project Operations.
author: stsporen
manager: AnnBe
ms.date: 10/06/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: c4e2f441e1c4b1bcba5bca292b8075b4334a004d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276560"
---
# <a name="expense-home-page"></a><span data-ttu-id="7bf30-103">Начална страница за разходи</span><span class="sxs-lookup"><span data-stu-id="7bf30-103">Expense home page</span></span>

<span data-ttu-id="7bf30-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="7bf30-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="7bf30-105">Dynamics 365 Project Operations поддържа способността за обработка на разходи.</span><span class="sxs-lookup"><span data-stu-id="7bf30-105">Dynamics 365 Project Operations supports the ability to process expenses.</span></span> <span data-ttu-id="7bf30-106">Обработката на разходите се извършва със или без проекти чрез използване на персонализиран работен поток от политики, категории транзакции и одобрения.</span><span class="sxs-lookup"><span data-stu-id="7bf30-106">Expense processing occurs with or without projects by using a customizable workflow of policies, transaction categories, and approvals.</span></span>

<span data-ttu-id="7bf30-107">В Project Operations има два поддържани модела за внедряване на разходи:</span><span class="sxs-lookup"><span data-stu-id="7bf30-107">In Project Operations, there are two supported deployment models for Expense:</span></span> 

- <span data-ttu-id="7bf30-108">**Пълно**: На разположение е пълно разгръщане **Project Operations за сценарии, базирани на ресурси / без наличност** или **Project Operations за сценарии, базирани на производствени поръчки**.</span><span class="sxs-lookup"><span data-stu-id="7bf30-108">**Full**: Full deployment is available for **Project Operations for resource/non-stocked based scenarios** or **Project Operations for production order-based scenarios**.</span></span>
- <span data-ttu-id="7bf30-109">**Основно**: Основното разполагане е достъпно за **Project Operations за сценарии, базирани на ресурси / без наличност** и **Олекотено внедряване - сделка за проформа фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="7bf30-109">**Basic**: Basic deployment is available for **Project Operations for resource/non-stocked based scenarios** and **Lite deployment – deal to proforma invoicing**.</span></span>

## <a name="full"></a><span data-ttu-id="7bf30-110">Пълен</span><span class="sxs-lookup"><span data-stu-id="7bf30-110">Full</span></span> 
<span data-ttu-id="7bf30-111">Разгръщането на Full Expense осигурява пълно прилагане на политиките, което включва възможността за създаване на политики, като например:</span><span class="sxs-lookup"><span data-stu-id="7bf30-111">Full Expense deployment provides a complete policy enforcement that includes the ability to create policies, such as:</span></span>

  - <span data-ttu-id="7bf30-112">Ограничения на категория на разход</span><span class="sxs-lookup"><span data-stu-id="7bf30-112">Expense category limits</span></span>
  - <span data-ttu-id="7bf30-113">Пътуване</span><span class="sxs-lookup"><span data-stu-id="7bf30-113">Travel</span></span>
  - <span data-ttu-id="7bf30-114">Дневни</span><span class="sxs-lookup"><span data-stu-id="7bf30-114">Per diem</span></span>
  - <span data-ttu-id="7bf30-115">Импортирания на кредитната карта</span><span class="sxs-lookup"><span data-stu-id="7bf30-115">Credit card imports</span></span>
  - <span data-ttu-id="7bf30-116">Получаване на оптично разпознаване на символи</span><span class="sxs-lookup"><span data-stu-id="7bf30-116">Receipt optical character recognition</span></span>

## <a name="basic"></a><span data-ttu-id="7bf30-117">Основен</span><span class="sxs-lookup"><span data-stu-id="7bf30-117">Basic</span></span> 
<span data-ttu-id="7bf30-118">Сценарият за внедряване на Основен разход ви позволява да записвате само основни разходи спрямо проект.</span><span class="sxs-lookup"><span data-stu-id="7bf30-118">Basic Expense deployment scenario only allows you to record basic expenses against a project.</span></span> 

<span data-ttu-id="7bf30-119">За повече информация вижте [Вписване на разходи (олекотен)](basic-expense.md)</span><span class="sxs-lookup"><span data-stu-id="7bf30-119">For more information, see [Expense entry (lite)](basic-expense.md)</span></span>

## <a name="determine-your-expense-deployment"></a><span data-ttu-id="7bf30-120">Определяне типа на внедряването на разход</span><span class="sxs-lookup"><span data-stu-id="7bf30-120">Determine your Expense deployment</span></span>
<span data-ttu-id="7bf30-121">За да определите дали изпълнявате внедряването на управление на основните разходи, проверете дали URL адресът на адреса завършва с **.crm.dynamics.com**.</span><span class="sxs-lookup"><span data-stu-id="7bf30-121">To determine if you're running the Basic Expense management deployment, verify that the address URL ends with **.crm.dynamics.com**.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]