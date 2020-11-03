---
title: Обработване на разписка за разход
description: Тази тема предоставя информация за обработката на оптични разпознавания на символи (OCR) за разписки. Тази функция е предназначена да подобри потребителското изживяване при създаване на отчети за разходите в Microsoft Dynamics 365 Finance.
author: stsporen
manager: AnnBe
ms.date: 05/14/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.search.region: Global
ms.author: stsporen
ms.search.validFrom: 2019-11-20
ms.dyn365.ops.version: 10.0.8
ms.openlocfilehash: 31c08ea264e6caec3217f4b424275495f39123e3
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071978"
---
# <a name="expense-receipt-processing"></a><span data-ttu-id="47a69-104">Обработване на разписка за разход</span><span class="sxs-lookup"><span data-stu-id="47a69-104">Expense receipt processing</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="47a69-105">Въвеждането на разходи е подобрено чрез въвеждането на обработка за оптични разпознавания на символи (OCR) за разписки.</span><span class="sxs-lookup"><span data-stu-id="47a69-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="47a69-106">Тази функция е предназначена да подобри потребителското изживяване при създаване на отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="47a69-106">This feature is designed to improve the user experience when expense reports are created.</span></span>

## <a name="key-features"></a><span data-ttu-id="47a69-107">Ключови функции</span><span class="sxs-lookup"><span data-stu-id="47a69-107">Key features</span></span>

- <span data-ttu-id="47a69-108">Името на търговеца, датата и общата сума се извличат от касовите бележки.</span><span class="sxs-lookup"><span data-stu-id="47a69-108">The merchant name, date, and total amount are extracted from receipts.</span></span>
- <span data-ttu-id="47a69-109">Функцията опитва да съпостави необвързаните разписки с необвързаните разходни транзакции.</span><span class="sxs-lookup"><span data-stu-id="47a69-109">The feature tries to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="47a69-110">Потребителите могат да създават ръчно въведени разходни транзакции от касови бележки.</span><span class="sxs-lookup"><span data-stu-id="47a69-110">Users can create manually entered expense transactions from receipts.</span></span>

## <a name="usage-examples"></a><span data-ttu-id="47a69-111">Примери за използване</span><span class="sxs-lookup"><span data-stu-id="47a69-111">Usage examples</span></span>

<span data-ttu-id="47a69-112">За да прикачите автоматично разписки, които включват транзакции с кредитни карти, когато се създава отчет за разходите, изпълнете следното:</span><span class="sxs-lookup"><span data-stu-id="47a69-112">To automatically attach receipts that include credit card transactions when an expense report is created, do the following:</span></span>

  1. <span data-ttu-id="47a69-113">Отворете работна област **Управление на разходите**.</span><span class="sxs-lookup"><span data-stu-id="47a69-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="47a69-114">В раздела **Разписки** проверете дали съществуват необвързани разписки.</span><span class="sxs-lookup"><span data-stu-id="47a69-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="47a69-115">Можете също да качите разписки на раздела **Постъпления**.</span><span class="sxs-lookup"><span data-stu-id="47a69-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="47a69-116">В раздела **разходи** проверете дали съществуват необвързани разходи.</span><span class="sxs-lookup"><span data-stu-id="47a69-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="47a69-117">Обикновено администраторът на разходите импортира тези разходи от доставчика на кредитни карти.</span><span class="sxs-lookup"><span data-stu-id="47a69-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="47a69-118">Изберете **Нов отчет за разходите**.</span><span class="sxs-lookup"><span data-stu-id="47a69-118">Select **New expense report**.</span></span> <span data-ttu-id="47a69-119">Забележете, че можете да включите разходи и разписки и сега, когато създавате отчет за разходите.</span><span class="sxs-lookup"><span data-stu-id="47a69-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="47a69-120">Ако добавите както разходи, така и разписки, се задейства автоматично съвпадение на разписките с разходите.</span><span class="sxs-lookup"><span data-stu-id="47a69-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

<span data-ttu-id="47a69-121">За да създадете разход или да съпоставите на разход от разписка, направете следното:</span><span class="sxs-lookup"><span data-stu-id="47a69-121">To create an expense, or match an expense from a receipt, do the following:</span></span>

  1. <span data-ttu-id="47a69-122">В отчет за разходите, в раздела **Постъпления** , прикачете разписка, като изберете **Добавяне на разписки**.</span><span class="sxs-lookup"><span data-stu-id="47a69-122">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="47a69-123">Под каченото изображение на разписката забележете опциите **Създаване** и **Съпоставяне**.</span><span class="sxs-lookup"><span data-stu-id="47a69-123">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="47a69-124">Изберете **Създайте** за създаване на ръчно въведена транзакция за разходи и попълване на стойностите, които са извлечени от разписката.</span><span class="sxs-lookup"><span data-stu-id="47a69-124">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="47a69-125">Ако изберете **Съпоставяне** , системата се опитва да съобрази съществуващ разход с разписката.</span><span class="sxs-lookup"><span data-stu-id="47a69-125">If you select **Match** , the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="47a69-126">Инсталиране</span><span class="sxs-lookup"><span data-stu-id="47a69-126">Installation</span></span>

<span data-ttu-id="47a69-127">Тази функция работи в комбинация с **Преосмислени отчети за разходите** функция, която спомага за опростяване на разходите.</span><span class="sxs-lookup"><span data-stu-id="47a69-127">This feature works in combination with the **Expense reports re-imagined** feature to help simplify the expense experience.</span></span> <span data-ttu-id="47a69-128">Тази функция е достъпна само за среди от ниво 2+, които са ограничителен режим и производство.</span><span class="sxs-lookup"><span data-stu-id="47a69-128">This feature is only available for Tier 2+ environments, which are Sandbox and Production.</span></span>

<span data-ttu-id="47a69-129">За да използвате тези разширени възможности за разход, инсталирайте добавката Expense Management Service за Microsoft Dynamics 365 Finance и включете функциите във вашия екземпляр.</span><span class="sxs-lookup"><span data-stu-id="47a69-129">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="47a69-130">Можете да получите достъп до добавката от вашия проект през Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="47a69-130">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="47a69-131">Влезте в LCS и отворете желаната среда.</span><span class="sxs-lookup"><span data-stu-id="47a69-131">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="47a69-132">Отидете на **Пълни подробности**.</span><span class="sxs-lookup"><span data-stu-id="47a69-132">Go to **Full details**.</span></span>
3. <span data-ttu-id="47a69-133">Изберете **Поддръжка** , или превъртете надолу до FastTab **Добавки за среда**.</span><span class="sxs-lookup"><span data-stu-id="47a69-133">Select **Maintain** , or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="47a69-134">Изберете **Инсталирайте нова добавка**.</span><span class="sxs-lookup"><span data-stu-id="47a69-134">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="47a69-135">Изберете **Услуга за управление на разходи**.</span><span class="sxs-lookup"><span data-stu-id="47a69-135">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="47a69-136">Следвайте ръководството за инсталиране и се съгласете с правилата и условията.</span><span class="sxs-lookup"><span data-stu-id="47a69-136">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="47a69-137">Изберете **Инсталиране**.</span><span class="sxs-lookup"><span data-stu-id="47a69-137">Select **Install**.</span></span>

<span data-ttu-id="47a69-138">В работна област **Управление на функции** , включете следните функции:</span><span class="sxs-lookup"><span data-stu-id="47a69-138">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="47a69-139">Обновени отчетите за разходите</span><span class="sxs-lookup"><span data-stu-id="47a69-139">Expense reports re-imagined</span></span>
- <span data-ttu-id="47a69-140">Автоматично съвпадение и създаване на разходи от получаването</span><span class="sxs-lookup"><span data-stu-id="47a69-140">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="47a69-141">Когато включите тези функции, се извършват следните действия:</span><span class="sxs-lookup"><span data-stu-id="47a69-141">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="47a69-142">Съществуващата работна област **Управление на разходите** се заменя с новото работно пространство.</span><span class="sxs-lookup"><span data-stu-id="47a69-142">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="47a69-143">Добавен е нов елемент от менюто за видимост на полето за разходи.</span><span class="sxs-lookup"><span data-stu-id="47a69-143">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="47a69-144">Все още можете да отворите предишната страница **Доклади за разходите** , като отидете на **Управление на разходите > Моите разходи > Отчети за разходите**.</span><span class="sxs-lookup"><span data-stu-id="47a69-144">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="47a69-145">Работните процеси и всякакви одобрения все още ви отвеждат до съществуващата страница с отчети за разходите.</span><span class="sxs-lookup"><span data-stu-id="47a69-145">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="47a69-146">Касовите бележки ще бъдат обработени чрез Microsoft Azure Cognitive Services и метаданни ще бъдат извлечени и добавени.</span><span class="sxs-lookup"><span data-stu-id="47a69-146">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="47a69-147">Добавена е опция, която ви позволява да създадете отчет за разходите, който включва съвпадащи необвързани разписки.</span><span class="sxs-lookup"><span data-stu-id="47a69-147">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="47a69-148">Опция, която се добавя към отчетите за разходите, ви позволява да създадете разходна линия от разписка или да се опитате да съпоставите съществуваща разписка със съществуваща разходна линия.</span><span class="sxs-lookup"><span data-stu-id="47a69-148">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

<span data-ttu-id="47a69-149">За повече информация относно преосмислената функция на отчетите за разходи, вижте [Преосмислени са отчетите за разходите](ExpenseWorkspaceNew.md).</span><span class="sxs-lookup"><span data-stu-id="47a69-149">For more information about the Expense reports re-imagined feature, see [Expense reports reimagined](ExpenseWorkspaceNew.md).</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="47a69-150">Често задавани въпроси</span><span class="sxs-lookup"><span data-stu-id="47a69-150">Frequently asked questions</span></span>

<span data-ttu-id="47a69-151">**Използва ли Microsoft данните ми за своите модели?**</span><span class="sxs-lookup"><span data-stu-id="47a69-151">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="47a69-152">Не, Microsoft е изградила общ модел машинно обучение за услугата си за обработка на разписки.</span><span class="sxs-lookup"><span data-stu-id="47a69-152">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="47a69-153">Този модел не се основава на касовите бележки, които качвате.</span><span class="sxs-lookup"><span data-stu-id="47a69-153">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="47a69-154">**Къде е достъпна и обработена тази функция?**</span><span class="sxs-lookup"><span data-stu-id="47a69-154">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="47a69-155">В момента САЩ се поддържа.</span><span class="sxs-lookup"><span data-stu-id="47a69-155">Currently, the United States is supported.</span></span>

<span data-ttu-id="47a69-156">**Къде отиват моите разписки?**</span><span class="sxs-lookup"><span data-stu-id="47a69-156">**Where do my receipts go?**</span></span>

<span data-ttu-id="47a69-157">Finance ще се свърже с Cognitive Services, за да извлече данните на място.</span><span class="sxs-lookup"><span data-stu-id="47a69-157">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="47a69-158">Cognitive Services ще запазят копие от вашата разписка до 24 часа, докато настъпи обработката.</span><span class="sxs-lookup"><span data-stu-id="47a69-158">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="47a69-159">След приключване на обработката Cognitive Services ще премахне разписката.</span><span class="sxs-lookup"><span data-stu-id="47a69-159">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="47a69-160">Разписките все още се съхраняват във Finance.</span><span class="sxs-lookup"><span data-stu-id="47a69-160">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="47a69-161">За повече информация вижте [Активирайте разбирането на касовите бележки с новата възможност на Разпознавател на формуляри](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="47a69-161">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>
