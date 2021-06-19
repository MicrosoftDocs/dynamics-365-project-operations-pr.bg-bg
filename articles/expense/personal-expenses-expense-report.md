---
title: Работа с лични разходи в отчет за разходи
description: Тази тема предоставя информация за това как да работите с лични разходи, направени от служителите по време на пътуване с бизнес цел.
author: suvaidya
ms.date: 05/11/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: ae25eca08089d224f1e17e95eeb571054de8a5c0
ms.sourcegitcommit: fd6e9ff78392c7bac35591d9130c00d2750438ae
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/12/2021
ms.locfileid: "6025671"
---
# <a name="work-with-personal-expenses-on-an-expense-report"></a><span data-ttu-id="e00c0-103">Работа с лични разходи в отчет за разходи</span><span class="sxs-lookup"><span data-stu-id="e00c0-103">Work with personal expenses on an expense report</span></span>

<span data-ttu-id="e00c0-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="e00c0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e00c0-105">По време на бизнес пътуване служителят може да начисли лични разходи на корпоративната си кредитна карта.</span><span class="sxs-lookup"><span data-stu-id="e00c0-105">During business travel, an employee might charge personal expenses to their corporate credit card.</span></span> <span data-ttu-id="e00c0-106">Ако процесът не е дефиниран за обработка на лични разходи, процесът на одобрение на отчета за разходите може да бъде нарушен, когато служителят представи своя подробен отчет за разходите.</span><span class="sxs-lookup"><span data-stu-id="e00c0-106">If a process hasn't been defined for handling personal expenses, the expense report approval process might be disrupted when an employee submits their itemized expense report.</span></span>

<span data-ttu-id="e00c0-107">Има два метода, които можете да използвате, за да работите с личните разходи на служителя:</span><span class="sxs-lookup"><span data-stu-id="e00c0-107">There are two methods you can use to work with an employee's personal expenses:</span></span>

  - <span data-ttu-id="e00c0-108">**Платено от служител**: Вашата организация не плаща лични разходи, които се появяват в сметката за корпоративната кредитна карта.</span><span class="sxs-lookup"><span data-stu-id="e00c0-108">**Paid by employee**: Your organization doesn't pay personal expenses that appear on the bill for the corporate credit card.</span></span> <span data-ttu-id="e00c0-109">Вместо това служителят плаща директно на продавача на кредитната карта за разходите.</span><span class="sxs-lookup"><span data-stu-id="e00c0-109">Instead, the employee pays the credit card vendor directly for the expenses.</span></span> 
  - <span data-ttu-id="e00c0-110">**Платено от фирмата**: Вашата организация плаща цялата сметка за корпоративната кредитна карта и след това дебитира сметката на работника за личните разходи.</span><span class="sxs-lookup"><span data-stu-id="e00c0-110">**Paid by company**: Your organization pays the full bill for the corporate credit card, and then debits the worker's account for the personal expenses.</span></span>

<span data-ttu-id="e00c0-111">Можете да изберете метода, който вашата организация използва в **Параметри за управление на разходите** страница.</span><span class="sxs-lookup"><span data-stu-id="e00c0-111">You can select the method that your organization uses on the **Expense management parameters** page.</span></span>


## <a name="enable-split-expense-function-when-personal-amount-field-has-value-defined"></a><span data-ttu-id="e00c0-112">Активиране на функцията за разделяне на разходи, когато полето за лична сума има дефинирана стойност</span><span class="sxs-lookup"><span data-stu-id="e00c0-112">Enable split expense function when personal amount field has value defined</span></span>

<span data-ttu-id="e00c0-113">Функцията **Активиране на функцията за разделяне на разходи, когато полето за лична сума има дефинирана стойност** се отнася само за отчети за разходи, които са одобрени с помощта на работен поток на ниво ред.</span><span class="sxs-lookup"><span data-stu-id="e00c0-113">The feature, **Enable split expense function when personal amount field has value defined** only applies to expense reports that are approved using a line-level workflow.</span></span> <span data-ttu-id="e00c0-114">Отчетите се одобряват, като отидете на **Обработка на отчети за разходи** > **Отчети за разходи, присвоени към мен** > **Отваряне на отчет за разходи**.</span><span class="sxs-lookup"><span data-stu-id="e00c0-114">Reports are approved by going to **Process expense reports** > **Expense reports assigned to me** > **Open expense report**.</span></span> 

<span data-ttu-id="e00c0-115">За да активирате тази функция, отидете на **Работни пространства** > **Управление на функции**, изберете **Активиране на функцията за разделяне на разходи, когато полето за лична сума има дефинирана стойност** и след това изберете **Активиране сега**.</span><span class="sxs-lookup"><span data-stu-id="e00c0-115">To enable this feature, go to **Workspaces** > **Feature Management**, select **Enable split expense function when personal amount field has value defined**, and then select **Enable now**.</span></span> 

<span data-ttu-id="e00c0-116">Когато функцията е активирана, редовете за разход, които използват тази функционалност, генерират два реда при подаване на отчета.</span><span class="sxs-lookup"><span data-stu-id="e00c0-116">When the feature is enabled, expense lines that use this functionality generate two lines when the report is submitted.</span></span> <span data-ttu-id="e00c0-117">Генерират се два реда, така че одобряващият да може да одобри всеки ред поотделно.</span><span class="sxs-lookup"><span data-stu-id="e00c0-117">Two lines are generated so that the approver can approve each line separately.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
