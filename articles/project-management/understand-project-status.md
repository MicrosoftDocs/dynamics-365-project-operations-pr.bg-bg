---
title: Разбиране на състоянието на проекта
description: Тази тема предоставя информация за състоянието, присвоено към проекти в Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: bc5bc174518e46b32cf88ea7231bb2df10fde292
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127280"
---
# <a name="understand-project-status"></a><span data-ttu-id="09557-103">Разбиране на състоянието на проекта</span><span class="sxs-lookup"><span data-stu-id="09557-103">Understand project status</span></span>

<span data-ttu-id="09557-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="09557-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="09557-105">Секцията **Състояние** на страницата **Обект на проект** предоставя резюме на състоянието на проекта въз основа на разходите и усилията.</span><span class="sxs-lookup"><span data-stu-id="09557-105">The **Status** section on the **Project Entity** page provides a summary of a project's health based upon cost and effort.</span></span>


## <a name="status-summary-fields"></a><span data-ttu-id="09557-106">Полета за обобщение на състоянието</span><span class="sxs-lookup"><span data-stu-id="09557-106">Status summary fields</span></span>

- <span data-ttu-id="09557-107">Полето **Цялостно състояние на проекта** е редактируемо поле, което показва цялостното състояние на проекта.</span><span class="sxs-lookup"><span data-stu-id="09557-107">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="09557-108">Това поле използва цветово кодиране, като зелено, жълто и червено, за да покаже нарастващ риск.</span><span class="sxs-lookup"><span data-stu-id="09557-108">This field uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> 
- <span data-ttu-id="09557-109">Полето **Коментари** позволява на мениджъра на проекти да въведете конкретни коментари за състоянието.</span><span class="sxs-lookup"><span data-stu-id="09557-109">The **Comments** field lets the project manager enter specific comments about the status.</span></span> 
- <span data-ttu-id="09557-110">Полето **Състоянието е актуализирано на** не може да се редактира.</span><span class="sxs-lookup"><span data-stu-id="09557-110">The **Status updated on** field isn't editable.</span></span> <span data-ttu-id="09557-111">Стойността в това поле е времева марка, която показва кога последно е актуализирано състоянието.</span><span class="sxs-lookup"><span data-stu-id="09557-111">The value in this field is a timestamp that indicates when the status was last updated.</span></span>
- <span data-ttu-id="09557-112">Полетата **Ефективност на графика** и **Ефективност на разходите** се задават от мрежата за проследяване.</span><span class="sxs-lookup"><span data-stu-id="09557-112">The **Schedule performance** and **Cost performance** fields are set from the tracking grid.</span></span> <span data-ttu-id="09557-113">Когато графикът и разликата в разходите за основния възел в изгледа **Проследяване на усилията** са положителни, тези полета се актуализират на **Изпреварване**.</span><span class="sxs-lookup"><span data-stu-id="09557-113">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, these fields are updated to **Ahead**.</span></span> <span data-ttu-id="09557-114">Когато графикът и разликата в разходите за основния възел са отрицателни, тези полета се задават на **Изостанали**.</span><span class="sxs-lookup"><span data-stu-id="09557-114">When the schedule and cost variance for the root node are negative, these fields are set to **Behind**.</span></span>
