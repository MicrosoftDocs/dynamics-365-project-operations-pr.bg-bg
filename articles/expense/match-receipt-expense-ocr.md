---
title: Съпоставяне на разписката с разходите с помощта на OCR
description: Тази тема предоставя информация за обработката на оптични разпознавания на символи (OCR) за разписки.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 02c1bafbe907a657689b610ae792f88085320903
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896988"
---
# <a name="match-a-receipt-to-an-expense-using-ocr"></a><span data-ttu-id="f3d18-103">Съпоставяне на разписката с разходите с помощта на OCR</span><span class="sxs-lookup"><span data-stu-id="f3d18-103">Match a receipt to an expense using OCR</span></span>

<span data-ttu-id="f3d18-104">_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="f3d18-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f3d18-105">Въвеждането на разходи е подобрено чрез въвеждането на обработка за оптични разпознавания на символи (OCR) за разписки.</span><span class="sxs-lookup"><span data-stu-id="f3d18-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="f3d18-106">Тази функционалност е предназначена да подобри потребителското изживяване при създаване на отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="f3d18-106">This functionality is designed to improve the user experience when creating expense reports.</span></span>

## <a name="key-features"></a><span data-ttu-id="f3d18-107">Ключови функции</span><span class="sxs-lookup"><span data-stu-id="f3d18-107">Key features</span></span>

- <span data-ttu-id="f3d18-108">Системата извлича името на търговеца, датата и общата сума от касовите бележки.</span><span class="sxs-lookup"><span data-stu-id="f3d18-108">The system extracts the merchant name, date, and total amount from receipts.</span></span>
- <span data-ttu-id="f3d18-109">Системата ще се опита да съпостави необвързаните разписки с необвързаните разходни транзакции.</span><span class="sxs-lookup"><span data-stu-id="f3d18-109">The system will try to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="f3d18-110">Можете да създавате ръчно въведени разходни транзакции от касови бележки.</span><span class="sxs-lookup"><span data-stu-id="f3d18-110">You can create manually entered expense transactions from receipts.</span></span>

## <a name="attach-receipts-to-an-expense-report"></a><span data-ttu-id="f3d18-111">Прикачете разписки към отчет за разходите</span><span class="sxs-lookup"><span data-stu-id="f3d18-111">Attach receipts to an expense report</span></span>

<span data-ttu-id="f3d18-112">За да прикачите автоматично разписки, които включват транзакции с кредитни карти, когато се създава отчет за разходите, изпълнете следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="f3d18-112">To automatically attach receipts that include credit card transactions when an expense report is created, complete the following steps.</span></span>

  1. <span data-ttu-id="f3d18-113">Отворете работна област **Управление на разходите**.</span><span class="sxs-lookup"><span data-stu-id="f3d18-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="f3d18-114">В раздела **Разписки** проверете дали съществуват необвързани разписки.</span><span class="sxs-lookup"><span data-stu-id="f3d18-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="f3d18-115">Можете също да качите разписки на раздела **Постъпления**.</span><span class="sxs-lookup"><span data-stu-id="f3d18-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="f3d18-116">В раздела **разходи** проверете дали съществуват необвързани разходи.</span><span class="sxs-lookup"><span data-stu-id="f3d18-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="f3d18-117">Обикновено администраторът на разходите импортира тези разходи от доставчика на кредитни карти.</span><span class="sxs-lookup"><span data-stu-id="f3d18-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="f3d18-118">Изберете **Нов отчет за разходите**.</span><span class="sxs-lookup"><span data-stu-id="f3d18-118">Select **New expense report**.</span></span> <span data-ttu-id="f3d18-119">Забележете, че можете да включите разходи и разписки и сега, когато създавате отчет за разходите.</span><span class="sxs-lookup"><span data-stu-id="f3d18-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="f3d18-120">Ако добавите както разходи, така и разписки, се задейства автоматично съвпадение на разписките с разходите.</span><span class="sxs-lookup"><span data-stu-id="f3d18-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

## <a name="create-or-match-receipts-to-an-expense-report"></a><span data-ttu-id="f3d18-121">Създаване или съпоставяне на разписки към отчет за разходите</span><span class="sxs-lookup"><span data-stu-id="f3d18-121">Create or match receipts to an expense report</span></span>
<span data-ttu-id="f3d18-122">За да създадете разход или да съпоставите на разход от разписка, изпълнете следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="f3d18-122">To create an expense, or match an expense from a receipt, complete the following steps.</span></span>

  1. <span data-ttu-id="f3d18-123">В отчет за разходите, в раздела **Постъпления**, прикачете разписка, като изберете **Добавяне на разписки**.</span><span class="sxs-lookup"><span data-stu-id="f3d18-123">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="f3d18-124">Под каченото изображение на разписката забележете опциите **Създаване** и **Съпоставяне**.</span><span class="sxs-lookup"><span data-stu-id="f3d18-124">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="f3d18-125">Изберете **Създайте** за създаване на ръчно въведена транзакция за разходи и попълване на стойностите, които са извлечени от разписката.</span><span class="sxs-lookup"><span data-stu-id="f3d18-125">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="f3d18-126">Ако изберете **Съпоставяне**, системата се опитва да съобрази съществуващ разход с разписката.</span><span class="sxs-lookup"><span data-stu-id="f3d18-126">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="f3d18-127">Инсталиране</span><span class="sxs-lookup"><span data-stu-id="f3d18-127">Installation</span></span>

<span data-ttu-id="f3d18-128">За да използвате тези разширени възможности за разход, инсталирайте добавката Expense Management Service за Microsoft Dynamics 365 Finance и включете функциите във вашия екземпляр.</span><span class="sxs-lookup"><span data-stu-id="f3d18-128">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="f3d18-129">Можете да получите достъп до добавката от вашия проект през Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="f3d18-129">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="f3d18-130">Влезте в LCS и отворете желаната среда.</span><span class="sxs-lookup"><span data-stu-id="f3d18-130">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="f3d18-131">Отидете на **Пълни подробности**.</span><span class="sxs-lookup"><span data-stu-id="f3d18-131">Go to **Full details**.</span></span>
3. <span data-ttu-id="f3d18-132">Изберете **Поддръжка**, или превъртете надолу до FastTab **Добавки за среда**.</span><span class="sxs-lookup"><span data-stu-id="f3d18-132">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="f3d18-133">Изберете **Инсталирайте нова добавка**.</span><span class="sxs-lookup"><span data-stu-id="f3d18-133">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="f3d18-134">Изберете **Услуга за управление на разходи**.</span><span class="sxs-lookup"><span data-stu-id="f3d18-134">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="f3d18-135">Следвайте ръководството за инсталиране и се съгласете с правилата и условията.</span><span class="sxs-lookup"><span data-stu-id="f3d18-135">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="f3d18-136">Изберете **Инсталиране**.</span><span class="sxs-lookup"><span data-stu-id="f3d18-136">Select **Install**.</span></span>

<span data-ttu-id="f3d18-137">В работна област **Управление на функции**, включете следните функции:</span><span class="sxs-lookup"><span data-stu-id="f3d18-137">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="f3d18-138">Обновени отчетите за разходите</span><span class="sxs-lookup"><span data-stu-id="f3d18-138">Expense reports re-imagined</span></span>
- <span data-ttu-id="f3d18-139">Автоматично съвпадение и създаване на разходи от получаването</span><span class="sxs-lookup"><span data-stu-id="f3d18-139">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="f3d18-140">Когато включите тези функции, се извършват следните действия:</span><span class="sxs-lookup"><span data-stu-id="f3d18-140">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="f3d18-141">Съществуващата работна област **Управление на разходите** се заменя с новото работно пространство.</span><span class="sxs-lookup"><span data-stu-id="f3d18-141">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="f3d18-142">Добавен е нов елемент от менюто за видимост на полето за разходи.</span><span class="sxs-lookup"><span data-stu-id="f3d18-142">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="f3d18-143">Все още можете да отворите предишната страница **Доклади за разходите**, като отидете на **Управление на разходите > Моите разходи > Отчети за разходите**.</span><span class="sxs-lookup"><span data-stu-id="f3d18-143">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="f3d18-144">Работните процеси и всякакви одобрения все още ви отвеждат до съществуващата страница с отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="f3d18-144">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="f3d18-145">Касовите бележки ще бъдат обработени чрез Microsoft Azure Cognitive Services и метаданни ще бъдат извлечени и добавени.</span><span class="sxs-lookup"><span data-stu-id="f3d18-145">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="f3d18-146">Добавена е опция, която ви позволява да създадете отчет за разходите, който включва съвпадащи необвързани разписки.</span><span class="sxs-lookup"><span data-stu-id="f3d18-146">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="f3d18-147">Опция, която се добавя към отчетите за разходите, ви позволява да създадете разходна линия от разписка или да се опитате да съпоставите съществуваща разписка със съществуваща разходна линия.</span><span class="sxs-lookup"><span data-stu-id="f3d18-147">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="f3d18-148">Често задавани въпроси</span><span class="sxs-lookup"><span data-stu-id="f3d18-148">Frequently asked questions</span></span>

<span data-ttu-id="f3d18-149">**Използва ли Microsoft данните ми за своите модели?**</span><span class="sxs-lookup"><span data-stu-id="f3d18-149">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="f3d18-150">Не, Microsoft е изградила общ модел машинно обучение за услугата си за обработка на разписки.</span><span class="sxs-lookup"><span data-stu-id="f3d18-150">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="f3d18-151">Този модел не се основава на касовите бележки, които качвате.</span><span class="sxs-lookup"><span data-stu-id="f3d18-151">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="f3d18-152">**Къде е достъпна и обработена тази функция?**</span><span class="sxs-lookup"><span data-stu-id="f3d18-152">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="f3d18-153">В момента САЩ се поддържа.</span><span class="sxs-lookup"><span data-stu-id="f3d18-153">Currently, the United States is supported.</span></span>

<span data-ttu-id="f3d18-154">**Къде отиват моите разписки?**</span><span class="sxs-lookup"><span data-stu-id="f3d18-154">**Where do my receipts go?**</span></span>

<span data-ttu-id="f3d18-155">Finance ще се свърже с Cognitive Services, за да извлече данните на място.</span><span class="sxs-lookup"><span data-stu-id="f3d18-155">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="f3d18-156">Cognitive Services ще запазят копие от вашата разписка до 24 часа, докато настъпи обработката.</span><span class="sxs-lookup"><span data-stu-id="f3d18-156">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="f3d18-157">След приключване на обработката Cognitive Services ще премахне разписката.</span><span class="sxs-lookup"><span data-stu-id="f3d18-157">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="f3d18-158">Разписките все още се съхраняват във Finance.</span><span class="sxs-lookup"><span data-stu-id="f3d18-158">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="f3d18-159">За повече информация вижте [Активирайте разбирането на касовите бележки с новата възможност на Разпознавател на формуляри](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="f3d18-159">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>
