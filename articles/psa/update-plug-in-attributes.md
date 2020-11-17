---
title: Актуализиране на атрибути на добавка за включване на нови ценови измерения
description: Тази тема предоставя информация за актуализирането на атрибутите на добавката за ценови измерения.
author: Rumant
manager: kfend
ms.custom: ''
ms.date: 11/19/2018
ms.topic: article
ms.service: dynamics-365-customerservice
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: f215555dd7b29444e00499c0e731624e51057250
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071903"
---
# <a name="update-plug-in-attributes-to-include-new-pricing-dimensions"></a>Актуализиране на атрибути на добавка за включване на нови ценови измерения

> [!NOTE]
> Ако не използвате функциите за офериране и договаряне на Project Service Automation (PSA), можете да пропуснете тази тема.

Тази тема предполага, че сте изпълнили процедурите в темите [Създавате на персонализирани полета и обекти](create-custom-fields-entities.md), [Добавяне на персонализирани полета към настройка на цени и обекти за транзакции](field-references.md) и [Настройване на персонализирани полета като ценови измерения](set-up-pricing-dimensions.md). Ако не сте изпълнили тези процедури, върнете се и ги изпълнете, след което се върнете към тази тема.

Когато се създават подробности за ред на оферта в страницата **Ред на оферта** за ред за оферта по проект, системата създава два реда за прогнозна оценка във фонов режим – един ред за страната на разходите на прогнозата и един за страната на продажбите. Същото важи и за редовете на договор по проект.

Когато правите промяна в количеството или поле от страната на разходите, тази промяна се попълва от страната на продажбите. Това е възможно поради следните добавки, които трябва да бъдат регистрирани отново след промяна на ценови измерения.

- PreOperationContractLineDetailUpdate – актуализира **msdyn_orderlinetransaction**.
- PreOperationQuoteLineDetailUpdate – актуализира **msdyn_quotelinetransaction**.

Следващите стъпки ви превеждат през процеса на регистриране на добавките.

1. Отворете **PluginRegistrationTool** и се свържете към вашия онлайн екземпляр.
2. Щракнете върху **Търсене** и потърсете добавката за актуализация.

 ![Екранна снимка на дървото за търсене](media/PRT-1.png)

3. След като намерите добавката, изберете я и след това щракнете върху **Избор в главния формуляр**.

4. Изберете стъпката на добавката за актуализиране, щракнете с десния бутон, след което изберете **Актуализиране**.

 ![Екранна снимка на добавката за актуализиране](media/PRT-2.png)
 
5. В прозореца за актуализация щракнете върху многоточието ( **...** ) в атрибутите за филтриране.

 ![Екранна снимка на актуализацията на информацията за конфигуриране на съществуваща стъпка](media/PRT-3.png)
 
6. Поставете отметки в квадратчетата на атрибутите за ценообразуване.

 ![Екранна снимка, показваща поставянето на отметки за ценовите атрибути](media/PRT-4.png)

7. Щракнете върху **OK** , за да затворите страницата, след което изберете **Актуализиране на стъпката**.

 ![Екранна снимка, показваща бутона „Актуализиране на стъпката“](media/PRT-5.png)
 
8. Повторете този процес за втората добавка **PreOperationQuoteLineDetail - актуализира msdyn_quotelinetransaction**.

9. Затворете инструмента за регистрация на добавки.
