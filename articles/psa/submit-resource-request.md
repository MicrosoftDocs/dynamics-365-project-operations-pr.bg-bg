---
title: Подаване на заявка за ресурс
description: Тази тема предоставя информация за подаване на заявка за ресурс на проект.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/1/2018
ms.topic: article
author: JohnPBurrows
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: bcea3d640d7e9ee2b071c55bff9ade3268edb319
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071913"
---
# <a name="submitting-a-resource-request"></a>Подаване на заявка за ресурс

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Можете да подадете генерирано изискване за ресурс като заявка за ресурс. След това заявката се изпраща на мениджър на ресурси за изпълнение.

1. В Project Service Automation (PSA), на страницата **Проекти** щракнете върху раздела **Екип** , за да видите списък с наличните ресурси. 
2. Изберете общия ресурс, който има изискване за ресурс, от списъка и след това щракнете върху **Подаване на заявка**.

![Подаване на заявка за ресурс](media/RM-how-to-18.png)

Състоянието на заявката на общия член на екипа ще се промени **Подадено**.

След като заявката бъде изпълнена от мениджъра на ресурси, общият ресурс ще бъде заменен с наименуван ресурс, ако мениджърът на ресурси изпълни заявката с резервацията на наименуван ресурс. В противен случай общият ресурс ще остане в екипа и състоянието на заявката ще се промени на **Нуждае се от преглед** , ако мениджърът на ресурси е предложил наименуван ресурс.
