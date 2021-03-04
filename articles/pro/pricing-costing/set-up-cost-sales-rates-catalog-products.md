---
title: Настройване на размер на разход и продажби за продукти от каталог – олекотено
description: Тази тема предоставя информация за това как да настроите размер на разход и продажби за елементите в продуктов каталог.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5e851193df8151821e112e01a9f33df5afee7df7
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764536"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products---lite"></a><span data-ttu-id="2932d-103">Настройване на размер на разход и продажби за продукти от каталог – олекотено</span><span class="sxs-lookup"><span data-stu-id="2932d-103">Set up cost and sales rates for catalog products - lite</span></span>

<span data-ttu-id="2932d-104">_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_</span><span class="sxs-lookup"><span data-stu-id="2932d-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="2932d-105">Настройване на ценообразуване за артикулите от продуктовия каталог в Dynamics 365 Project Operations е същото като в Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="2932d-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="2932d-106">При Project Operations продуктите не могат да бъдат оценени или използвани по проекти, така че не е необходимо цените на продуктовите каталози да се задават в ценовите листи на проекти за оферти и договори.</span><span class="sxs-lookup"><span data-stu-id="2932d-106">In Project Operations, products can't be estimated or used on projects, so product catalog prices don't need to be set on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="2932d-107">Използвайте полето **Цена на продукта** за оферта, договор или акаунт за задаване на цени на продуктовия каталог.</span><span class="sxs-lookup"><span data-stu-id="2932d-107">Use the **Product Price** field of a quote, contract, or account to set up product catalog prices.</span></span> <span data-ttu-id="2932d-108">Не настройвайте цените на продуктовия каталог в ценовите листи на проекта.</span><span class="sxs-lookup"><span data-stu-id="2932d-108">Don't set up product catalog prices in the project price lists.</span></span> <span data-ttu-id="2932d-109">Ценовите списъци на проекти са изключителни за Project Operations.</span><span class="sxs-lookup"><span data-stu-id="2932d-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="2932d-110">Бизнес логиката, специфична за приложението, копира ценовите листи от оферта в договор.</span><span class="sxs-lookup"><span data-stu-id="2932d-110">Application-specific business logic copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="2932d-111">Резултатът е специфична за договор ценова листа.</span><span class="sxs-lookup"><span data-stu-id="2932d-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="2932d-112">Операцията за копиране може да забави процеса на спечелване на офертата, ако ценовата листа на проекта в офертата стане твърде голяма.</span><span class="sxs-lookup"><span data-stu-id="2932d-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="2932d-113">Ценовите листи на продуктите не се копират, за да се създадат персонализирани ценови листи по договори.</span><span class="sxs-lookup"><span data-stu-id="2932d-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="2932d-114">Тъй като няма копиране, изпълнението на процеса на котиране не се влияе.</span><span class="sxs-lookup"><span data-stu-id="2932d-114">Because there's no copying involved, the performance of the quote process isn't affected.</span></span>
