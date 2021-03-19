---
title: Подаване на заявка за ресурс
description: Можете да подадете генерирано изискване за ресурс като заявка за ресурс. След това заявката се изпраща на мениджър на ресурси за изпълнение.
author: ruhercul
manager: Annbe
ms.date: 10/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: bc97af1ec90e60417c502eb329a85004e769e05b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279125"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="cf84e-104">Подаване на заявка за ресурс</span><span class="sxs-lookup"><span data-stu-id="cf84e-104">Submit a resource request</span></span>

<span data-ttu-id="cf84e-105">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="cf84e-105">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cf84e-106">Можете да подадете генерирано изискване за ресурс като заявка за ресурс.</span><span class="sxs-lookup"><span data-stu-id="cf84e-106">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="cf84e-107">След това заявката се изпраща на мениджър на ресурси за изпълнение.</span><span class="sxs-lookup"><span data-stu-id="cf84e-107">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="cf84e-108">В Dynamics 365 Project Operations, на страницата **Проекти** изберете раздела **Екип**, за да видите списък с наличните ресурси.</span><span class="sxs-lookup"><span data-stu-id="cf84e-108">In Dynamics 365 Project Operations, on the **Projects** page, select the **Team** tab to view a list of bookable resources.</span></span> 
2. <span data-ttu-id="cf84e-109">Изберете общия ресурс, който има изискване за ресурс, от списъка и след това щракнете върху **Подаване на заявка**.</span><span class="sxs-lookup"><span data-stu-id="cf84e-109">Select the generic resource that has a resource requirement from the list, and then click **Submit Request**.</span></span>

<span data-ttu-id="cf84e-110">Състоянието на заявката на общия член на екипа ще се промени **Подадено**.</span><span class="sxs-lookup"><span data-stu-id="cf84e-110">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="cf84e-111">След като заявката бъде изпълнена, общият ресурс ще бъде заменен с наименуван ресурс, ако мениджърът на ресурси изпълни заявката , като направи резервация на наименуван ресурс.</span><span class="sxs-lookup"><span data-stu-id="cf84e-111">After the request is fulfilled, the generic resource is replaced by a named resource if the resource manager fulfills the request by booking a named resource.</span></span> <span data-ttu-id="cf84e-112">В противен, ако мениджърът на ресурс предложи наименуван ресурс генеричният ресурс остава в екипа и състоянието на заявката ще се промени на **Нуждае се от преглед**.</span><span class="sxs-lookup"><span data-stu-id="cf84e-112">Otherwise, if the resource manager proposes a named resource, the generic resource remains on the team and the request status will change to **Needs Review**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]