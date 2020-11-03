---
title: Базирани на възможност аспекти на договор
description: Тази тема предоставя информация за базирани на продукт елементи от ред на възможност в Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 17ffcf8dc94d42102115281d281d6b553cf1fa17
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071746"
---
# <a name="product-based-opportunity-lines"></a><span data-ttu-id="1e16f-103">Базирани на възможност аспекти на договор</span><span class="sxs-lookup"><span data-stu-id="1e16f-103">Product-based opportunity lines</span></span>

<span data-ttu-id="1e16f-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="1e16f-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1e16f-105">Продуктово базирани редове за възможности са договорени покупки във възможността.</span><span class="sxs-lookup"><span data-stu-id="1e16f-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="1e16f-106">Тези редове се доставят на клиента като отделни позиции в евентуалната фактура без други услуги с добавена стойност.</span><span class="sxs-lookup"><span data-stu-id="1e16f-106">These lines are delivered to the customer as distinct line items on the eventual invoice without any other value-added services.</span></span> <span data-ttu-id="1e16f-107">Свързаните разходи и потребление не се проследяват по задачи на свързани проекти.</span><span class="sxs-lookup"><span data-stu-id="1e16f-107">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="1e16f-108">Продуктовите линии могат да бъдат артикули от каталога или продукти за записване.</span><span class="sxs-lookup"><span data-stu-id="1e16f-108">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="1e16f-109">Повечето от функционалностите на продуктовите линии на Opportunity следват функционалността, предоставена от приложението Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="1e16f-109">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="1e16f-110">За повече информация относно продуктовите линии за възможности, вижте [Добавете продукти към една възможност](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="1e16f-110">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="1e16f-111">Една концепция за продуктово базирани възможности, която е специфична за възможностите, базирани на проекти, е **Бюджет на клиента**.</span><span class="sxs-lookup"><span data-stu-id="1e16f-111">One concept about product-based opportunity lines that is specific to project-based opportunities is **Customer Budget**.</span></span> <span data-ttu-id="1e16f-112">Използвайте това поле, за да проследите сумата, която клиентът е готов да плати за договорената покупка.</span><span class="sxs-lookup"><span data-stu-id="1e16f-112">Use this field to track the amount the customer is willing to pay for the line item.</span></span>

<span data-ttu-id="1e16f-113">Ако методът на приходите в обобщението на възможността е зададен на **Изчислено от системата** , стойностите на клиентския бюджет по линии, базирани на продукти и проекти, са обобщени, за да се изчисли прогнозният приход.</span><span class="sxs-lookup"><span data-stu-id="1e16f-113">If the revenue method of the Opportunity summary is set to **System Calculated** , the customer budget values across product- and project-based lines are summarized to calculate the estimated revenue.</span></span>
