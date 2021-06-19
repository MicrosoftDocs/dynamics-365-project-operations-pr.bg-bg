---
title: Настройване на интеграция на кредитни карти
description: Тази тема обяснява как да работите с транзакции с кредитни карти, свързани с разходи.
author: suvaidya
ms.date: 04/02/2021
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 3555e894e206c2aafb30b0df1e52efadd69b0713
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001790"
---
# <a name="set-up-credit-card-integration"></a><span data-ttu-id="d5df7-103">Настройване на интеграция на кредитни карти</span><span class="sxs-lookup"><span data-stu-id="d5df7-103">Set up credit card integration</span></span>

<span data-ttu-id="d5df7-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="d5df7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d5df7-105">Свързаните с разходи транзакции с кредитни карти могат да бъдат настроени така, че да бъдат автоматично импортирани по повтарящ се график.</span><span class="sxs-lookup"><span data-stu-id="d5df7-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="d5df7-106">Алтернативно, транзакциите могат да бъдат импортирани ръчно, както са необходими.</span><span class="sxs-lookup"><span data-stu-id="d5df7-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="d5df7-107">Транзакциите с кредитни карти се импортират чрез субекта за данни за транзакции с кредитни карти.</span><span class="sxs-lookup"><span data-stu-id="d5df7-107">The credit card transactions are imported through the credit card transactions data entity.</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="d5df7-108">Внос на транзакции с кредитни карти</span><span class="sxs-lookup"><span data-stu-id="d5df7-108">Import credit card transactions</span></span>

<span data-ttu-id="d5df7-109">За да импортирате транзакции с кредитни карти, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="d5df7-109">To import credit card transactions, follow these steps:</span></span>

1. <span data-ttu-id="d5df7-110">На страницата **Транзакции с кредитни карти** изберете **Импортни транзакции**.</span><span class="sxs-lookup"><span data-stu-id="d5df7-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="d5df7-111">Ако отваряте управлението на данни за първи път, системата трябва да актуализира списъка с обекти на данни, преди да можете да продължите.</span><span class="sxs-lookup"><span data-stu-id="d5df7-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="d5df7-112">В полето **Име**, въведете уникално описание за заданието за импортиране.</span><span class="sxs-lookup"><span data-stu-id="d5df7-112">In the **Name** field, enter a unique description for the import job.</span></span>
3. <span data-ttu-id="d5df7-113">В полето **Формат на изходните данни** изберете формата на файла, който съдържа транзакциите с кредитни карти за импортиране.</span><span class="sxs-lookup"><span data-stu-id="d5df7-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="d5df7-114">Изберете **Качване** и след това намерете и изберете файла за импортиране.</span><span class="sxs-lookup"><span data-stu-id="d5df7-114">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="d5df7-115">След като файлът бъде качен, потвърдете картографирането на файла с транзакциите на кредитната карта и колоните на обекта с данни за транзакции с кредитни карти, като изберете връзката **Вижте карта** на плочката.</span><span class="sxs-lookup"><span data-stu-id="d5df7-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="d5df7-116">Ако има грешки в картографирането или ако трябва да промените картографирането, направете промените в картографирането или от раздела **Визуализация на картографиране** или раздела **Подробности за картографиране**.</span><span class="sxs-lookup"><span data-stu-id="d5df7-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="d5df7-117">За да автоматизирате транзакциите с кредитни карти, изберете **Създайте повтаряща се работа с данни**.</span><span class="sxs-lookup"><span data-stu-id="d5df7-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="d5df7-118">След това можете да зададете повторение, което определя колко често да се импортират транзакции с кредитни карти.</span><span class="sxs-lookup"><span data-stu-id="d5df7-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="d5df7-119">Когато сте готови, изберете **ОК**.</span><span class="sxs-lookup"><span data-stu-id="d5df7-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="d5df7-120">За да импортирате избрания файл сега, изберете **Импортиране**.</span><span class="sxs-lookup"><span data-stu-id="d5df7-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="d5df7-121">Ако по време на импортирането възникнат грешки, можете да прегледате дневника за изпълнение или промените, за да видите грешките, които трябва да поправите, за да осигурите успешен импорт.</span><span class="sxs-lookup"><span data-stu-id="d5df7-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help ensure a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="d5df7-122">Ако трябва да импортирате повече от един файлов формат, трябва да създадете отделни задания за импортиране за всеки тип формат.</span><span class="sxs-lookup"><span data-stu-id="d5df7-122">If you need to import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="d5df7-123">Преразпределете транзакциите с кредитни карти за прекратени служители</span><span class="sxs-lookup"><span data-stu-id="d5df7-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="d5df7-124">След прекратяване на записа на служител акаунтът на домейн услуги на Active Directory (AD DS) на служителя е деактивиран.</span><span class="sxs-lookup"><span data-stu-id="d5df7-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="d5df7-125">Възможно е обаче да има активни транзакции с кредитни карти, които все пак трябва да бъдат разходни и възстановени.</span><span class="sxs-lookup"><span data-stu-id="d5df7-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="d5df7-126">На страницата **Транзакции с кредитни карти**, можете да преназначите служителя за всяка транзакция с кредитна карта, при която свързаният служител е прекратен.</span><span class="sxs-lookup"><span data-stu-id="d5df7-126">On the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="d5df7-127">Изберете една или повече транзакции с кредитни карти и след това изберете **Преназначете транзакции**.</span><span class="sxs-lookup"><span data-stu-id="d5df7-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="d5df7-128">След това можете да изберете друг служител, на когото да възложите транзакциите с кредитни карти.</span><span class="sxs-lookup"><span data-stu-id="d5df7-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="d5df7-129">След като транзакциите с кредитни карти бъдат преназначени, те могат да бъдат избрани за отчет на разходите и да бъдат платени чрез обичайния процес за възстановяване на разходите.</span><span class="sxs-lookup"><span data-stu-id="d5df7-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>

## <a name="delete-credit-card-transactions"></a><span data-ttu-id="d5df7-130">Изтриване на транзакции с кредитни карти</span><span class="sxs-lookup"><span data-stu-id="d5df7-130">Delete credit card transactions</span></span> 

<span data-ttu-id="d5df7-131">Понякога след импортиране на транзакции с кредитни карти може да се наложи да се изтрият определени транзакции.</span><span class="sxs-lookup"><span data-stu-id="d5df7-131">Sometimes, after credit card transactions are imported, certain transactions may need to be deleted.</span></span> <span data-ttu-id="d5df7-132">Това може да се дължи на това, че транзакциите са дублирани или защото данните може да не са точни.</span><span class="sxs-lookup"><span data-stu-id="d5df7-132">This could be because the transactions are duplicates or because the data might isn't accurate.</span></span> <span data-ttu-id="d5df7-133">Администраторите могат да използват **„Изтриване на транзакции с кредитни карти“** функция за избор и изтриване на транзакции с кредитни карти, които са **не е приложен** към отчет за разходите.</span><span class="sxs-lookup"><span data-stu-id="d5df7-133">Admins can use the **"Delete credit card transactions"** feature to select and delete credit card transactions that are **not attached** to an expense report.</span></span> 

1. <span data-ttu-id="d5df7-134">Отидете на **Периодични задачи** > **Изтриване на транзакции с кредитни карти**.</span><span class="sxs-lookup"><span data-stu-id="d5df7-134">Go to **Periodic tasks** > **Delete credit card transactions**.</span></span>
2. <span data-ttu-id="d5df7-135">Изберете **Филтър** и предоставят информация за идентифициране на записите, които да бъдат включени.</span><span class="sxs-lookup"><span data-stu-id="d5df7-135">Select **Filter** and provide information to identify the records to include.</span></span>
3. <span data-ttu-id="d5df7-136">Изберете **ОК**, за да изтриете записите.</span><span class="sxs-lookup"><span data-stu-id="d5df7-136">Select **OK** to delete the records.</span></span> 

[!INCLUDE[footer-include](../includes/footer-banner.md)]
