---
title: Прогнози за ресурс
description: Тази тема предоставя информация за това как се изчисляват прогнози в Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2ebde2b3c5bcfb5faa02ee476065ac34b1953432
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071740"
---
# <a name="resource-estimates"></a>Прогнози за ресурс

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

Оценките на ресурсите идват от усилията във времето, които са дефинирани в структурата на разбивка на работата, заедно с приложимите измерения на ценообразуването. Обикновено изчислението е **скорост/час за всяка роля x часа.** Постепенното усилие за всеки ресурс се съхранява в записа за присвояване на ресурс. Ценообразуването се съхранява в предварително дефинирана ценова листа. Преобразуването на мерни единици се прилага въз основа на приложимия ценоразпис.

![Прогнози за ресурс](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a>Цена и валута за разходи за разход по подразбиране

Разходните цени са по подразбиране от организационната единица.

## <a name="default-bill-rate-and-sales-currency"></a>Стойност на сметката и валута на продажбите по подразбиране

Продажните цени се прилагат веднъж за сделка. Йерархията по подразбиране на ценовата листа за продажба е следната:

1. Организация
2. Клиент
3. Оферта/договор