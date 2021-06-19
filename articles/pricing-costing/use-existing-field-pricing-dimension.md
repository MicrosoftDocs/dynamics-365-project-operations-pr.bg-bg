---
title: Полета на Project Operations като измерения на ценообразуване
description: Тази тема предоставя информация с помощта на полета като измерения на ценообразуването в Dynamics 365 Project Operations.
author: rumant
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: a29460b2a9dc9a9755e7e28a6cd9712c6b06e8c6
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004473"
---
# <a name="project-operations-fields-as-pricing-dimensions"></a><span data-ttu-id="8044d-103">Полета на Project Operations като измерения на ценообразуване</span><span class="sxs-lookup"><span data-stu-id="8044d-103">Project Operations fields as pricing dimensions</span></span>

<span data-ttu-id="8044d-104">_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_</span><span class="sxs-lookup"><span data-stu-id="8044d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8044d-105">Обектът **Действителни данни** има много полета, които могат да се използват като ценови измерения за ценообразуване въз основа на ресурси.</span><span class="sxs-lookup"><span data-stu-id="8044d-105">The **Actuals** entity has many fields that can be used as pricing dimensions for resource-based pricing.</span></span> <span data-ttu-id="8044d-106">Например едно общо поле е **Наличен ресурс**.</span><span class="sxs-lookup"><span data-stu-id="8044d-106">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="8044d-107">По-малките компании, които имат под 20 – 30 платими ресурси, може да установят, че да имаш ставки за фактуриране и разходи, специфични за всеки ресурс, е по-опростен подход.</span><span class="sxs-lookup"><span data-stu-id="8044d-107">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="8044d-108">С нарастването на фактурираната работна сила обаче нивата на отделни ресурси могат да станат нереалистични за поддържане.</span><span class="sxs-lookup"><span data-stu-id="8044d-108">However, as the billable workforce grows, resource-secific rates could become unrealistic to maintain.</span></span> <span data-ttu-id="8044d-109">Разходите за ресурси и сметките започват да варират, когато ресурсите се повишават, придобиват повече опит или придобиват различен набор от умения.</span><span class="sxs-lookup"><span data-stu-id="8044d-109">Resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different set of skills.</span></span> 

<span data-ttu-id="8044d-110">Друг пример е този на категорията на транзакцията.</span><span class="sxs-lookup"><span data-stu-id="8044d-110">Another example is that of transaction category.</span></span> <span data-ttu-id="8044d-111">Клиентите и изпълнителите са използвали категорията на транзакцията, за да класифицират работата и да използват полето за цена и разход на базата на категорията работа.</span><span class="sxs-lookup"><span data-stu-id="8044d-111">Customers and Implementers have used the transaction category to classify work and use the field to price and cost based on the category of work.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]