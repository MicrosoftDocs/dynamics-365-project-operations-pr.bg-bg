---
title: Поръчки за продажба за проект
description: Тази статия описва различните методи, които можете да използвате за създаване на поръчки за покупка за проект. Методът, който използвате зависи от целта на поръчката за покупка и кога закупените артикули се консумират и таксуват по даден проект.
author: Yowelle
manager: AnnBe
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 83972
ms.assetid: 247e4d72-610b-4fa5-9873-601ed0f4b2d6
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: bd891aec5bcab66c5801a5d9ca8abbbf632d662d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071808"
---
# <a name="purchase-orders-for-a-project"></a>Поръчки за продажба за проект

[!include [banner](../includes/banner.md)]

Тази статия описва различните методи, които можете да използвате за създаване на поръчки за покупка за проект. Методът, който използвате зависи от целта на поръчката за покупка и кога закупените артикули се консумират и таксуват по даден проект.

### <a name="methods-for-creating-a-purchase-order"></a>Методи за създаване на поръчка за покупка

Можете да използвате един от следните методи за създаване на поръчка за покупка в Управление на проекти и счетоводство. Целта на поръчката за покупка определя кога поръчката за покупка се консумира и следователно кога артикулите се таксуват по даден проект.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Метод</th>
<th>Цел</th>
<th>Консумация на артикули</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Създаване на поръчка за покупка директно от проект.</td>
<td>Използвайте този метод за закупуване на артикули от външен доставчик за потребление по проект. Можете да създадете поръчка за покупка по два начина:
<ul>
<li>От самия проект. В този случай проектът вече е дефиниран за поръчката за покупка.</li>
<li>Чрез навигация до поръчката за закупуване на проект. Трябва да изберете както доставчика, така и проекта, за да създадете поръчка за покупка.</li>
</ul></td>
<td>Елементите се консумират, когато фактурата на доставчика се актуализира.</td>
</tr>
<tr class="even">
<td>Създаване на поръчка за покупка от поръчка за продажби.</td>
<td>Използвайте този метод, за да закупите артикули, когато създавате поръчка за продажба от проект.</td>
<td>Артикулите се консумират, когато поръчката за продажба е фактурирана на клиента.</td>
</tr>
<tr class="odd">
<td>Създайте поръчка за покупка от изискване за артикул.</td>
<td>Използвайте този метод, за да закупите артикули, когато създавате изискване за артикул от проект.</td>
<td>Артикулите се консумират, когато се актуализира бланката за опаковане на изискване за артикул.</td>
</tr>
</tbody>
</table>

> [!NOTE] 
> Когато актуализирате фактурата на доставчика или фиша за опаковане, ще бъдете подканени да актуализирате фиша за опаковане според изискването за артикула.

За повече информация вижте [Получавайте артикули по поръчка за покупка от изискването за артикул](tasks/receive-items-purchase-order-item-requirement.md).
