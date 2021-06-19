---
title: Заснемане на разписка с помощта на OCR
description: Тази тема предоставя информация за обработката на оптични разпознавания на символи (OCR) за разписки.
author: suvaidya
ms.date: 09/23/2020
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
ms.openlocfilehash: 3c7fa8a805acbf7c75edd49c4c49aa159493f525
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001998"
---
# <a name="capture-a-receipt-using-ocr"></a><span data-ttu-id="927fc-103">Заснемане на разписка с помощта на OCR</span><span class="sxs-lookup"><span data-stu-id="927fc-103">Capture a receipt using OCR</span></span>

<span data-ttu-id="927fc-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="927fc-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="927fc-105">Въвеждането на разходи е подобрено чрез въвеждането на обработка за оптични разпознавания на символи (OCR) за разписки.</span><span class="sxs-lookup"><span data-stu-id="927fc-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="927fc-106">Тази функционалност е предназначена да подобри потребителското изживяване при създаване на отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="927fc-106">This functionality is designed to improve the user experience when creating expense reports.</span></span>

## <a name="key-features"></a><span data-ttu-id="927fc-107">Ключови функции</span><span class="sxs-lookup"><span data-stu-id="927fc-107">Key features</span></span>

- <span data-ttu-id="927fc-108">Системата извлича името на търговеца, датата и общата сума от касовите бележки.</span><span class="sxs-lookup"><span data-stu-id="927fc-108">The system extracts the merchant name, date, and total amount from receipts.</span></span>
- <span data-ttu-id="927fc-109">Системата ще се опита да съпостави необвързаните разписки с необвързаните разходни транзакции.</span><span class="sxs-lookup"><span data-stu-id="927fc-109">The system will try to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="927fc-110">Можете да създавате ръчно въведени разходни транзакции от касови бележки.</span><span class="sxs-lookup"><span data-stu-id="927fc-110">You can create manually entered expense transactions from receipts.</span></span>

## <a name="attach-receipts-to-an-expense-report"></a><span data-ttu-id="927fc-111">Прикачете разписки към отчет за разходите</span><span class="sxs-lookup"><span data-stu-id="927fc-111">Attach receipts to an expense report</span></span>

<span data-ttu-id="927fc-112">За да прикачите автоматично разписки, които включват транзакции с кредитни карти, когато се създава отчет за разходите, изпълнете следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="927fc-112">To automatically attach receipts that include credit card transactions when an expense report is created, complete the following steps.</span></span>

  1. <span data-ttu-id="927fc-113">Отворете работна област **Управление на разходите**.</span><span class="sxs-lookup"><span data-stu-id="927fc-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="927fc-114">В раздела **Разписки** проверете дали съществуват необвързани разписки.</span><span class="sxs-lookup"><span data-stu-id="927fc-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="927fc-115">Можете също да качите разписки на раздела **Постъпления**.</span><span class="sxs-lookup"><span data-stu-id="927fc-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="927fc-116">В раздела **разходи** проверете дали съществуват необвързани разходи.</span><span class="sxs-lookup"><span data-stu-id="927fc-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="927fc-117">Обикновено администраторът на разходите импортира тези разходи от доставчика на кредитни карти.</span><span class="sxs-lookup"><span data-stu-id="927fc-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="927fc-118">Изберете **Нов отчет за разходите**.</span><span class="sxs-lookup"><span data-stu-id="927fc-118">Select **New expense report**.</span></span> <span data-ttu-id="927fc-119">Забележете, че можете да включите разходи и разписки и сега, когато създавате отчет за разходите.</span><span class="sxs-lookup"><span data-stu-id="927fc-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="927fc-120">Ако добавите както разходи, така и разписки, се задейства автоматично съвпадение на разписките с разходите.</span><span class="sxs-lookup"><span data-stu-id="927fc-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

## <a name="create-or-match-receipts-to-an-expense-report"></a><span data-ttu-id="927fc-121">Създаване или съпоставяне на разписки към отчет за разходите</span><span class="sxs-lookup"><span data-stu-id="927fc-121">Create or match receipts to an expense report</span></span>
<span data-ttu-id="927fc-122">За да създадете разход или да съпоставите на разход от разписка, изпълнете следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="927fc-122">To create an expense, or match an expense from a receipt, complete the following steps.</span></span>

  1. <span data-ttu-id="927fc-123">В отчет за разходите, в раздела **Постъпления**, прикачете разписка, като изберете **Добавяне на разписки**.</span><span class="sxs-lookup"><span data-stu-id="927fc-123">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="927fc-124">Под каченото изображение на разписката забележете опциите **Създаване** и **Съпоставяне**.</span><span class="sxs-lookup"><span data-stu-id="927fc-124">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="927fc-125">Изберете **Създайте** за създаване на ръчно въведена транзакция за разходи и попълване на стойностите, които са извлечени от разписката.</span><span class="sxs-lookup"><span data-stu-id="927fc-125">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="927fc-126">Ако изберете **Съпоставяне**, системата се опитва да съобрази съществуващ разход с разписката.</span><span class="sxs-lookup"><span data-stu-id="927fc-126">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="927fc-127">Инсталиране</span><span class="sxs-lookup"><span data-stu-id="927fc-127">Installation</span></span>

<span data-ttu-id="927fc-128">За да използвате тези разширени възможности за разход, инсталирайте добавката Expense Management Service за Microsoft Dynamics 365 Finance и включете функциите във вашия екземпляр.</span><span class="sxs-lookup"><span data-stu-id="927fc-128">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="927fc-129">Можете да получите достъп до добавката от вашия проект през Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="927fc-129">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="927fc-130">Влезте в LCS и отворете желаната среда.</span><span class="sxs-lookup"><span data-stu-id="927fc-130">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="927fc-131">Отидете на **Пълни подробности**.</span><span class="sxs-lookup"><span data-stu-id="927fc-131">Go to **Full details**.</span></span>
3. <span data-ttu-id="927fc-132">Изберете **Поддръжка**, или превъртете надолу до FastTab **Добавки за среда**.</span><span class="sxs-lookup"><span data-stu-id="927fc-132">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="927fc-133">Изберете **Инсталирайте нова добавка**.</span><span class="sxs-lookup"><span data-stu-id="927fc-133">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="927fc-134">Изберете **Услуга за управление на разходи**.</span><span class="sxs-lookup"><span data-stu-id="927fc-134">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="927fc-135">Следвайте ръководството за инсталиране и се съгласете с правилата и условията.</span><span class="sxs-lookup"><span data-stu-id="927fc-135">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="927fc-136">Изберете **Инсталиране**.</span><span class="sxs-lookup"><span data-stu-id="927fc-136">Select **Install**.</span></span>

<span data-ttu-id="927fc-137">В работна област **Управление на функции**, включете следните функции:</span><span class="sxs-lookup"><span data-stu-id="927fc-137">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="927fc-138">Обновени отчетите за разходите</span><span class="sxs-lookup"><span data-stu-id="927fc-138">Expense reports re-imagined</span></span>
- <span data-ttu-id="927fc-139">Автоматично съвпадение и създаване на разходи от получаването</span><span class="sxs-lookup"><span data-stu-id="927fc-139">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="927fc-140">Когато включите тези функции, се извършват следните действия:</span><span class="sxs-lookup"><span data-stu-id="927fc-140">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="927fc-141">Съществуващата работна област **Управление на разходите** се заменя с новото работно пространство.</span><span class="sxs-lookup"><span data-stu-id="927fc-141">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="927fc-142">Добавен е нов елемент от менюто за видимост на полето за разходи.</span><span class="sxs-lookup"><span data-stu-id="927fc-142">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="927fc-143">Все още можете да отворите предишната страница **Доклади за разходите**, като отидете на **Управление на разходите > Моите разходи > Отчети за разходите**.</span><span class="sxs-lookup"><span data-stu-id="927fc-143">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="927fc-144">Работните процеси и всякакви одобрения все още ви отвеждат до съществуващата страница с отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="927fc-144">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="927fc-145">Касовите бележки ще бъдат обработени чрез Microsoft Azure Cognitive Services и метаданни ще бъдат извлечени и добавени.</span><span class="sxs-lookup"><span data-stu-id="927fc-145">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="927fc-146">Добавена е опция, която ви позволява да създадете отчет за разходите, който включва съвпадащи необвързани разписки.</span><span class="sxs-lookup"><span data-stu-id="927fc-146">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="927fc-147">Опция, която се добавя към отчетите за разходите, ви позволява да създадете разходна линия от разписка или да се опитате да съпоставите съществуваща разписка със съществуваща разходна линия.</span><span class="sxs-lookup"><span data-stu-id="927fc-147">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="927fc-148">Често задавани въпроси</span><span class="sxs-lookup"><span data-stu-id="927fc-148">Frequently asked questions</span></span>

<span data-ttu-id="927fc-149">**Използва ли Microsoft данните ми за своите модели?**</span><span class="sxs-lookup"><span data-stu-id="927fc-149">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="927fc-150">Не, Microsoft е изградила общ модел машинно обучение за услугата си за обработка на разписки.</span><span class="sxs-lookup"><span data-stu-id="927fc-150">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="927fc-151">Този модел не се основава на касовите бележки, които качвате.</span><span class="sxs-lookup"><span data-stu-id="927fc-151">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="927fc-152">**Къде е достъпна и обработена тази функция?**</span><span class="sxs-lookup"><span data-stu-id="927fc-152">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="927fc-153">В момента САЩ се поддържа.</span><span class="sxs-lookup"><span data-stu-id="927fc-153">Currently, the United States is supported.</span></span>

<span data-ttu-id="927fc-154">**Къде отиват моите разписки?**</span><span class="sxs-lookup"><span data-stu-id="927fc-154">**Where do my receipts go?**</span></span>

<span data-ttu-id="927fc-155">Finance ще се свърже с Cognitive Services, за да извлече данните на място.</span><span class="sxs-lookup"><span data-stu-id="927fc-155">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="927fc-156">Cognitive Services ще запазят копие от вашата разписка до 24 часа, докато настъпи обработката.</span><span class="sxs-lookup"><span data-stu-id="927fc-156">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="927fc-157">След приключване на обработката Cognitive Services ще премахне разписката.</span><span class="sxs-lookup"><span data-stu-id="927fc-157">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="927fc-158">Разписките все още се съхраняват във Finance.</span><span class="sxs-lookup"><span data-stu-id="927fc-158">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="927fc-159">За повече информация вижте [Активирайте разбирането на касовите бележки с новата възможност на Разпознавател на формуляри](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="927fc-159">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
