---
title: Ценови листи на продукт
description: Тази тема предоставя информация за ценовите листи в ценообразуването по каталог, използвани за проектни оферти и договори.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: 3570aeb78804e9b267caa55a27e02d6c8df9a5c6
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898158"
---
# <a name="product-price-lists"></a>Ценови листи на продукт

_**Отнася се за:** Проектни операции за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

Обектите „Ценови листи“ и „Елемент в ценова листа“ поддържат ценообразуването на продуктовия каталог. В по-голямата си част тази функционалност се използва за редове, базирани на каталог, в оферти и договори по проекти.

За редове, базирани на проект, договорът представлява сделката, след като тя бъде спечелена. Тъй като процесът на договаряне обикновено предхожда спечелването, ценообразуването, което е приложено към офертата, винаги се копира както е в нова ценова листа и се прилага към договора. Тази нова ценова листа не може да бъде променена извън обхвата на договора. Това ограничение помага да се защити картата на ставките, която е договорена, от промени в цените, които възникват в главната ценова листа.

Продуктите трябва да бъдат настроени така, че да имат разходни и ценови листи по подразбиране в продуктовия каталог. Използвайте цената от листата, стандартните разходи и текущите разходи, за да конфигурирате разходите и цените в списъка по подразбиране. Цените в листата по подразбиране се използват в ред на оферта или ред на договор по проект само когато системата не може да намери ред на ценова листа за този продукт в ценовата листа на продукта за офертата или договора по проекта.

Себестойността в редовете на продуктовия каталог може да се променя между офертите. Тази възможност е важна, защото ако не проследявате точно разходите, не можете да определите оперативните печалби за ангажиментите по проекта. По подразбиране стандартният разход за продукта се използва като себестойност. Себестойността по подразбиране обаче може да се актуализира в реда на офертата, ако има различна себестойност за тази оферта.

## <a name="price-list-items"></a>Елементи в ценовата листа

Можете да добавяте продукти от продуктов каталог в различни ценови листи. Редовете на ценовата листа за продукти винаги се позовават на конкретна единица. Ценообразуването за продукт в ценова листа може да бъде конфигурирано като сума във валута. Или може да бъде конфигурирано като функция на цената от листата, текущата себестойност или стандартните разходи.

PSA поддържа различни опции за закръгляване, когато цените са конфигурирани като функция от цената от листата, стандартните разходи или текущите разходи. Освен да се възползвате от няколко метода на ценообразуване и опции за закръгляване, можете да свържете списъците с отстъпки с елементи от ценовата листа. 

Когато създавате нова персонализирана ценова листа за оферта чрез избиране на **Създаване на потребителско ценообразуване** на страницата **Оферта по проект**, се създава копие на ценовата листа и полето **Обект** в заглавката на новата ценова листа се задава на **Обект на продажби**. Името на новата ценова листа се допълва с името на офертата и времево клеймо. Можете също да използвате името на новата ценова листа и името на офертата в персонализирани работни потоци, за да задействате допълнителен преглед и одобрения за оферти, които използват персонализирано ценообразуване.

 
## <a name="default-product-price-list"></a>Ценова листа за продукти по подразбиране
Всеки запис на клиент има поле **Ценова листа по подразбиране**, където можете да укажете ценова листа, която отговаря на валутата на клиента. Стойността по подразбиране не се въвежда автоматично в това поле. Когато съществува споразумение за персонализирано ценообразуване с конкретен клиент, можете да използвате това поле, за да свържете ценова листа с този клиент.

Обектите „Възможност“, „Оферта“ и „Договор по проект“ използват следния ред, за да въведат ценови списъци на продукти по подразбиране. Същият ред се използва за ценови листи за проекти.

1.  Оферта
2.  Възможност
3.  Клиент
4.  Глобални настройки 

По подразбиране полето **Продукт** в реда на офертата изброява всички активни продукти в ценовата листа на продукти на офертата. Ако даден продукт е бил деактивиран или е проект на продукт, той не е в списъка, дори ако е в ценовата листа. 

Редове на продуктовия каталог се добавят като редове на фактура в първата фактура, която се създава за договор по проект. В чернова на фактура тези редове на фактурата могат да бъдат изтрити. В този случай редовете ще се повят в следваща фактура, докато не бъдат фактурирани или докато фактурата не бъде изпратена на клиента. Не можете да фактурирате частично количество на ред на фактура за продукт. Когато редовете за продукти от договора по проекта се фактурират, се създават действителни данни. Тези действителни данни обаче не са свързани със свързания обект на проект. С други думи, редовете на договор, базирани на продукти, са независими от базирана на проект употреба. Консумацията на материали по проекти не се проследява.
