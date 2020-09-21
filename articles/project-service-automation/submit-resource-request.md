---
title: Подаване на заявка за ресурс
description: Тази тема предоставя информация за подаване на заявка за ресурс на проект.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/1/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
author: JohnPBurrows
ms.assetid: 9f4a6315-3905-4b15-8d06-e5dae30ccbb8
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 2b706ae25af5ba85647c98353b5950663fafc292
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "3749330"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="4b905-103">Подаване на заявка за ресурс</span><span class="sxs-lookup"><span data-stu-id="4b905-103">Submit a resource request</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="4b905-104">Можете да подадете генерирано изискване за ресурс като заявка за ресурс.</span><span class="sxs-lookup"><span data-stu-id="4b905-104">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="4b905-105">След това заявката се изпраща на мениджър на ресурси за изпълнение.</span><span class="sxs-lookup"><span data-stu-id="4b905-105">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="4b905-106">В Project Service Automation (PSA), на страницата **Проекти** щракнете върху раздела **Екип**, за да видите списък с наличните ресурси.</span><span class="sxs-lookup"><span data-stu-id="4b905-106">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab to view a list bookable resources.</span></span> 
2. <span data-ttu-id="4b905-107">Изберете общия ресурс, който има изискване за ресурс, от списъка и след това щракнете върху **Подаване на заявка**.</span><span class="sxs-lookup"><span data-stu-id="4b905-107">Select the generic resource that has a resource requirement from the list and then click **Submit Request**.</span></span>

![Подаване на заявка за ресурс](media/RM-how-to-18.png)

<span data-ttu-id="4b905-109">Състоянието на заявката на общия член на екипа ще се промени **Подадено**.</span><span class="sxs-lookup"><span data-stu-id="4b905-109">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="4b905-110">След като заявката бъде изпълнена от мениджъра на ресурси, общият ресурс ще бъде заменен с наименуван ресурс, ако мениджърът на ресурси изпълни заявката с резервацията на наименуван ресурс.</span><span class="sxs-lookup"><span data-stu-id="4b905-110">After the request is fulfilled by the resource manager, the generic resource will be replaced by a named resource if the resource manager fulfills the request with the booking of a named resource.</span></span> <span data-ttu-id="4b905-111">В противен случай общият ресурс ще остане в екипа и състоянието на заявката ще се промени на **Нуждае се от преглед**, ако мениджърът на ресурси е предложил наименуван ресурс.</span><span class="sxs-lookup"><span data-stu-id="4b905-111">Otherwise, the generic resource will remain on the team and the request status will change to **Needs Review**, if the resource manager has proposed a named resource.</span></span>
