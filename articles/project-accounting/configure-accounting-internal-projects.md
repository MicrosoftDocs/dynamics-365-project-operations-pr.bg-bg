---
title: Конфигуриране на счетоводство за вътрешни проекти
description: Тази тема предоставя информация за това как да настроите практики за счетоводство за вътрешни проекти в Project Operations.
author: sigitac
ms.date: 10/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ad8b974ef75cb0a4e43af0aa254cec1bbcab154a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012843"
---
# <a name="configure-accounting-for-internal-projects"></a><span data-ttu-id="57a35-103">Конфигуриране на счетоводство за вътрешни проекти</span><span class="sxs-lookup"><span data-stu-id="57a35-103">Configure accounting for internal projects</span></span>

<span data-ttu-id="57a35-104">_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_</span><span class="sxs-lookup"><span data-stu-id="57a35-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="57a35-105">Вътрешните проекти позволяват на компаниите да проследяват разходите, свързани с дейности, които не се таксуват от клиента.</span><span class="sxs-lookup"><span data-stu-id="57a35-105">Internal projects allow companies track cost related to activities that aren't being billed to a customer.</span></span> <span data-ttu-id="57a35-106">Примери за вътрешни проекти включват:</span><span class="sxs-lookup"><span data-stu-id="57a35-106">Examples of internal projects include:</span></span>

- <span data-ttu-id="57a35-107">Разработване на продукт, като мобилно приложение, и проследяване на разходите, свързани с разработката.</span><span class="sxs-lookup"><span data-stu-id="57a35-107">Developing a product, such as a mobile app, and tracking the cost associated with the development.</span></span>
- <span data-ttu-id="57a35-108">Управление на времето и разходите за предварителна продажба.</span><span class="sxs-lookup"><span data-stu-id="57a35-108">Managing pre-sale time and expense.</span></span> <span data-ttu-id="57a35-109">Този предпродажен вътрешен проект може да бъде конвертиран по-късно в проект за плащане, ако се спечели оферта.</span><span class="sxs-lookup"><span data-stu-id="57a35-109">This pre-sale internal project can be converted later to a billable project if quote is won.</span></span>

<span data-ttu-id="57a35-110">Всеки проект, който не е свързан с договор в Dynamics 365 Project Operations се третира като вътрешен.</span><span class="sxs-lookup"><span data-stu-id="57a35-110">Any project not associated with a contract in Dynamics 365 Project Operations is treated as internal.</span></span> <span data-ttu-id="57a35-111">Профилите за разходи и приходи по проект не се използват за определяне на правилата за осчетоводяване за проекта.</span><span class="sxs-lookup"><span data-stu-id="57a35-111">Project cost and revenue profiles aren't used to determine accounting rules for the project.</span></span> <span data-ttu-id="57a35-112">Вътрешните разходи по проекта винаги се осчетоводяват, като се използват принципите на печалбата и загубата.</span><span class="sxs-lookup"><span data-stu-id="57a35-112">Internal project cost is always posted using profit and loss principles.</span></span> <span data-ttu-id="57a35-113">Счетоводните книги за осчетоводяване са дефинирани на страницата **Настройка на осчетоводяване на книга**.</span><span class="sxs-lookup"><span data-stu-id="57a35-113">Ledger accounts for postings are defined on the **Ledger posting setup** page.</span></span>

- <span data-ttu-id="57a35-114">Транзакциите във времето се осчетоводяват чрез дебитиране на **Разходи** сметка и кредитиране на акаунт **Разпределение на заплати**.</span><span class="sxs-lookup"><span data-stu-id="57a35-114">Time transactions are posted by debiting the **Cost** account and crediting the **Payroll allocation** account.</span></span>
- <span data-ttu-id="57a35-115">Транзакциите на разходи се осчетоводяват чрез дебитиране на **Разходи** сметка и кредитиране на **Сметка за компенсиране за разход**.</span><span class="sxs-lookup"><span data-stu-id="57a35-115">Expense transactions are posted by debiting the **Cost** account and crediting the **Offset account for expense**.</span></span>
- <span data-ttu-id="57a35-116">Транзакциите с артикули се осчетоводяват чрез дебитиране на сметката **Разходи** и кредитиране на сметката **Разходи - артикул**.</span><span class="sxs-lookup"><span data-stu-id="57a35-116">Item transactions are posted by debiting the **Cost** account and crediting the **Cost - Item** account.</span></span>

<span data-ttu-id="57a35-117">След като транзакциите бъдат осчетоводени в проекта, ако проектът е свързан с договор за проект, системата обръща всички натрупани транзакции и създава нови таксувани транзакции.</span><span class="sxs-lookup"><span data-stu-id="57a35-117">After transactions are posted to the project, if the project is associated with a project contract, the system reverses all accumulated transactions and creates new billable transactions.</span></span> <span data-ttu-id="57a35-118">Фактурираните транзакции следват счетоводните правила, определени в съответния профил на разходите и приходите на проекта.</span><span class="sxs-lookup"><span data-stu-id="57a35-118">The billable transactions follow the accounting rules defined in respective Project cost and revenue profile.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]
