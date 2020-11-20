---
title: Настройване на размер на разход и продажби за продукти от каталог – олекотено
description: Тази тема предоставя информация за това как да настроите размер на разход и продажби за елементите в продуктов каталог.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 135b182af73bdab7a3520589431332ad059ec497
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176688"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products---lite"></a><span data-ttu-id="6fd19-103">Настройване на размер на разход и продажби за продукти от каталог – олекотено</span><span class="sxs-lookup"><span data-stu-id="6fd19-103">Set up cost and sales rates for catalog products - lite</span></span>

<span data-ttu-id="6fd19-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="6fd19-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="6fd19-105">Настройването на ценообразуване за артикулите на продуктовия каталог в Dynamics 365 Project Operations е същото като в Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="6fd19-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="6fd19-106">Тъй като продуктите не могат да бъдат оценени или използвани за проекти в Project Operations, не е необходимо да задавате цени на каталога на продуктите в ценовите листи на проекти за оферти и договори.</span><span class="sxs-lookup"><span data-stu-id="6fd19-106">Because products can't be estimated or used on projects in Project Operations, there is no need to set product catalog prices on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="6fd19-107">Цените на продуктовия каталог трябва да бъдат определени в **Цена на продукта** поле на оферта, договор или сметка.</span><span class="sxs-lookup"><span data-stu-id="6fd19-107">Product catalog prices should be set up in the **Product Price** field of a quote, contract, or account.</span></span> <span data-ttu-id="6fd19-108">Не задавайте цени на продуктовия каталог в ценовите листи на проекта за тези обекти.</span><span class="sxs-lookup"><span data-stu-id="6fd19-108">Don't set up product catalog prices in the project price lists for these entities.</span></span> <span data-ttu-id="6fd19-109">Ценовите списъци на проекти са изключителни за Project Operations.</span><span class="sxs-lookup"><span data-stu-id="6fd19-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="6fd19-110">Има специфична за приложението бизнес логика, която копира ценовите листи от оферта в договор.</span><span class="sxs-lookup"><span data-stu-id="6fd19-110">There is application-specific business logic that copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="6fd19-111">Резултатът е специфична за договор ценова листа.</span><span class="sxs-lookup"><span data-stu-id="6fd19-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="6fd19-112">Операцията за копиране може да забави процеса на спечелване на офертата, ако ценовата листа на проекта в офертата стане твърде голяма.</span><span class="sxs-lookup"><span data-stu-id="6fd19-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="6fd19-113">Ценовите листи на продуктите не се копират, за да се създадат персонализирани ценови листи по договори.</span><span class="sxs-lookup"><span data-stu-id="6fd19-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="6fd19-114">Това означава, че ценовите листи на продуктите не оказват влияние върху ефективността на процеса на печелене на оферти.</span><span class="sxs-lookup"><span data-stu-id="6fd19-114">This means that product price lists don't impact the performance of the quote win process.</span></span>
