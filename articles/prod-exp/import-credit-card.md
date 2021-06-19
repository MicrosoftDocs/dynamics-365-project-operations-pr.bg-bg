---
title: Импортиране и поддържане на трансакции с кредитна карта
description: Тази тема обяснява как да импортирате и поддържате транзакции с кредитни карти, свързани с разходи. Тези транзакции могат да бъдат настроени така, че да бъдат автоматично импортирани по повтарящ се график, или могат да бъдат импортирани ръчно, както се изисква.
author: KimANelson
ms.date: 01/12/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: TrvPbsMainDataLines
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 274023
ms.assetid: 3605eda1-a7ed-4675-8031-5279c5a8f5e4
ms.search.region: Global
ms.author: suvaidya
ms.dyn365.ops.version: Version 1611
ms.search.validFrom: 2016-11-30
ms.openlocfilehash: edeab157aa2fa6cf518ad086b4c1f22c5b45fa04
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005148"
---
# <a name="import-and-maintain-credit-card-transactions"></a><span data-ttu-id="f058b-104">Импортиране и поддържане на трансакции с кредитна карта</span><span class="sxs-lookup"><span data-stu-id="f058b-104">Import and maintain credit card transactions</span></span>

<span data-ttu-id="f058b-105">Свързаните с разходи транзакции с кредитни карти могат да бъдат настроени така, че да бъдат автоматично импортирани по повтарящ се график.</span><span class="sxs-lookup"><span data-stu-id="f058b-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="f058b-106">Алтернативно, транзакциите могат да бъдат импортирани ръчно, както са необходими.</span><span class="sxs-lookup"><span data-stu-id="f058b-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="f058b-107">Транзакциите с кредитни карти се импортират чрез субекта за данни за транзакции с кредитни карти.</span><span class="sxs-lookup"><span data-stu-id="f058b-107">The credit card transactions are imported through the Credit card transactions data entity.</span></span>

<span data-ttu-id="f058b-108">За повече информация относно обектите на данни вижте [Обекти на данни](/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities).</span><span class="sxs-lookup"><span data-stu-id="f058b-108">For more information about data entities, see [Data entities](/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities).</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="f058b-109">Внос на транзакции с кредитни карти</span><span class="sxs-lookup"><span data-stu-id="f058b-109">Import credit card transactions</span></span>

1. <span data-ttu-id="f058b-110">На страницата **Транзакции с кредитни карти** изберете **Импортни транзакции**.</span><span class="sxs-lookup"><span data-stu-id="f058b-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="f058b-111">Ако отваряте управлението на данни за първи път, системата трябва да актуализира списъка с обекти на данни, преди да можете да продължите.</span><span class="sxs-lookup"><span data-stu-id="f058b-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="f058b-112">В полето **Име** въведете уникално описание на заданието за импортиране.</span><span class="sxs-lookup"><span data-stu-id="f058b-112">In the **Name** field, enter a unique description of the import job.</span></span>
3. <span data-ttu-id="f058b-113">В полето **Формат на изходните данни** изберете формата на файла, който съдържа транзакциите с кредитни карти за импортиране.</span><span class="sxs-lookup"><span data-stu-id="f058b-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="f058b-114">Изберете **Качване** и след това намерете и изберете файла за импортиране.</span><span class="sxs-lookup"><span data-stu-id="f058b-114">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="f058b-115">След като файлът бъде качен, потвърдете картографирането на файла с транзакциите на кредитната карта и колоните на обекта с данни за транзакции с кредитни карти, като изберете връзката **Вижте карта** на плочката.</span><span class="sxs-lookup"><span data-stu-id="f058b-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the Credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="f058b-116">Ако има грешки в картографирането или ако трябва да промените картографирането, направете промените в картографирането или от раздела **Визуализация на картографиране** или раздела **Подробности за картографиране**.</span><span class="sxs-lookup"><span data-stu-id="f058b-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="f058b-117">За да автоматизирате транзакциите с кредитни карти, изберете **Създайте повтаряща се работа с данни**.</span><span class="sxs-lookup"><span data-stu-id="f058b-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="f058b-118">След това можете да зададете повторение, което определя колко често да се импортират транзакции с кредитни карти.</span><span class="sxs-lookup"><span data-stu-id="f058b-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="f058b-119">Когато сте готови, изберете **ОК**.</span><span class="sxs-lookup"><span data-stu-id="f058b-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="f058b-120">За да импортирате избрания файл сега, изберете **Импортиране**.</span><span class="sxs-lookup"><span data-stu-id="f058b-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="f058b-121">Ако по време на импортирането възникнат грешки, можете да прегледате дневника за изпълнение или данните за подреждане, за да видите грешките, които трябва да коригирате, за да гарантирате успешен импорт.</span><span class="sxs-lookup"><span data-stu-id="f058b-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help guarantee a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="f058b-122">Ако трябва да импортирате повече от един файлов формат, трябва да създадете отделни задания за импортиране за всеки тип формат.</span><span class="sxs-lookup"><span data-stu-id="f058b-122">If you must import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="f058b-123">Преразпределете транзакциите с кредитни карти за прекратени служители</span><span class="sxs-lookup"><span data-stu-id="f058b-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="f058b-124">След прекратяване на записа на служител акаунтът на домейн услуги на Active Directory (AD DS) на служителя е деактивиран.</span><span class="sxs-lookup"><span data-stu-id="f058b-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="f058b-125">Възможно е обаче да има активни транзакции с кредитни карти, които все пак трябва да бъдат разходни и възстановени.</span><span class="sxs-lookup"><span data-stu-id="f058b-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="f058b-126">От страницата **Транзакции с кредитни карти** можете да преназначите служителя за всяка транзакция с кредитна карта, при която свързаният служител е прекратен.</span><span class="sxs-lookup"><span data-stu-id="f058b-126">From the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="f058b-127">Изберете една или повече транзакции с кредитни карти и след това изберете **Преназначете транзакции**.</span><span class="sxs-lookup"><span data-stu-id="f058b-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="f058b-128">След това можете да изберете друг служител, на когото да възложите транзакциите с кредитни карти.</span><span class="sxs-lookup"><span data-stu-id="f058b-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="f058b-129">След като транзакциите с кредитни карти бъдат преназначени, те могат да бъдат избрани за отчет на разходите и да бъдат платени чрез обичайния процес за възстановяване на разходите.</span><span class="sxs-lookup"><span data-stu-id="f058b-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]