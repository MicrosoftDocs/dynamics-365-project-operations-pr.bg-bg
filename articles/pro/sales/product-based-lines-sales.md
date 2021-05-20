---
title: Базирани на продукт редове за възможност – олекотено
description: Тази тема предоставя информация за базирани на продукт елементи от ред на възможност в Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f7dfabd068e180c7122ede0f79aaebfe220250a1
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949531"
---
# <a name="product-based-opportunity-lines---lite"></a><span data-ttu-id="f33ee-103">Базирани на продукт редове за възможност – олекотено</span><span class="sxs-lookup"><span data-stu-id="f33ee-103">Product-based opportunity lines - lite</span></span>

<span data-ttu-id="f33ee-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="f33ee-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f33ee-105">Продуктово базирани редове за възможности са договорени покупки във възможността.</span><span class="sxs-lookup"><span data-stu-id="f33ee-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="f33ee-106">Тези отделни договорени покупки са в евентуалната фактура, която се предоставя на клиента.</span><span class="sxs-lookup"><span data-stu-id="f33ee-106">These distinct line items are on the eventual invoice that is provided to the customer.</span></span> <span data-ttu-id="f33ee-107">Фактурата не включва други допълнителни услуги.</span><span class="sxs-lookup"><span data-stu-id="f33ee-107">The invoice doesn't include any other additional services.</span></span> <span data-ttu-id="f33ee-108">Свързаните разходи и потребление не се проследяват по задачи на свързани проекти.</span><span class="sxs-lookup"><span data-stu-id="f33ee-108">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="f33ee-109">Продуктовите линии могат да бъдат артикули от каталога или продукти за записване.</span><span class="sxs-lookup"><span data-stu-id="f33ee-109">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="f33ee-110">Повечето от функционалностите на продуктовите линии на Opportunity следват функционалността, предоставена от приложението Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="f33ee-110">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="f33ee-111">За повече информация относно продуктовите линии за възможности, вижте [Добавете продукти към една възможност](/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="f33ee-111">For more information about product-based opportunity lines, see [Add products to an opportunity](/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="f33ee-112">**Бюджет на клиента** е концепция, която е специфична за базирани на проекти линии за възможности.</span><span class="sxs-lookup"><span data-stu-id="f33ee-112">**Customer budget** is a concept that is specific to project-based opportunity lines.</span></span> <span data-ttu-id="f33ee-113">Полето **Бюджет на клиента** проследява сумата, която клиентът е готов да плати за артикула.</span><span class="sxs-lookup"><span data-stu-id="f33ee-113">The **Customer budget** field tracks the amount the customer is willing to pay for the item.</span></span>

<span data-ttu-id="f33ee-114">Когато методът на приходите в обобщението на възможността е **Системно изчислена**, стойностите на бюджета на клиента по линиите за възможности са обобщени, за да се изчисли прогнозният приход.</span><span class="sxs-lookup"><span data-stu-id="f33ee-114">When the revenue method of the Opportunity summary is **System Calculated**, the customer budget values across the opportunity lines are summarized to calculate the estimated revenue.</span></span> 



[!INCLUDE[footer-include](../../includes/footer-banner.md)]