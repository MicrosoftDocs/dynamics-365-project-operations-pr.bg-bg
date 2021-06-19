---
title: Подаване на заявка за ресурс
description: Можете да подадете генерирано изискване за ресурс като заявка за ресурс. След това заявката се изпраща на мениджър на ресурси за изпълнение.
author: ruhercul
ms.date: 10/04/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 6ac0044a27d1e506c9c62c477014017fd0ca06cb
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014013"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="95420-104">Подаване на заявка за ресурс</span><span class="sxs-lookup"><span data-stu-id="95420-104">Submit a resource request</span></span>

<span data-ttu-id="95420-105">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="95420-105">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="95420-106">Можете да подадете генерирано изискване за ресурс като заявка за ресурс.</span><span class="sxs-lookup"><span data-stu-id="95420-106">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="95420-107">След това заявката се изпраща на мениджър на ресурси за изпълнение.</span><span class="sxs-lookup"><span data-stu-id="95420-107">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="95420-108">В Dynamics 365 Project Operations, на страницата **Проекти** изберете раздела **Екип**, за да видите списък с наличните ресурси.</span><span class="sxs-lookup"><span data-stu-id="95420-108">In Dynamics 365 Project Operations, on the **Projects** page, select the **Team** tab to view a list of bookable resources.</span></span> 
2. <span data-ttu-id="95420-109">Изберете общия ресурс, който има изискване за ресурс, от списъка и след това щракнете върху **Подаване на заявка**.</span><span class="sxs-lookup"><span data-stu-id="95420-109">Select the generic resource that has a resource requirement from the list, and then click **Submit Request**.</span></span>

<span data-ttu-id="95420-110">Състоянието на заявката на общия член на екипа ще се промени **Подадено**.</span><span class="sxs-lookup"><span data-stu-id="95420-110">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="95420-111">След като заявката бъде изпълнена, общият ресурс ще бъде заменен с наименуван ресурс, ако мениджърът на ресурси изпълни заявката , като направи резервация на наименуван ресурс.</span><span class="sxs-lookup"><span data-stu-id="95420-111">After the request is fulfilled, the generic resource is replaced by a named resource if the resource manager fulfills the request by booking a named resource.</span></span> <span data-ttu-id="95420-112">В противен, ако мениджърът на ресурс предложи наименуван ресурс генеричният ресурс остава в екипа и състоянието на заявката ще се промени на **Нуждае се от преглед**.</span><span class="sxs-lookup"><span data-stu-id="95420-112">Otherwise, if the resource manager proposes a named resource, the generic resource remains on the team and the request status will change to **Needs Review**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]