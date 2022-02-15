---
title: Управление на подизпълнение в Project Operations
description: Тази тема предоставя преглед на целия процес на управление на подизпълнение обикновено в базирани на проект организации.
author: rumant
ms.date: 08/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 993edfd064279a970d7c42d5fcefd794e949a931
ms.sourcegitcommit: 80aa1e8070f0cb4992ac408fc05bdffe47cee931
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "7323583"
---
# <a name="subcontract-management-in-project-operations"></a>Управление на подизпълнение в Project Operations

[!include [banner](../../includes/dataverse-preview.md)]

_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_

Тази тема предоставя преглед на целия процес на управление на подизпълнение в базирани на проект организации. Подизпълнението за услуги обикновено следва поток на бизнес процес, което е показано на следната диаграма.

![Поток на процеса на подизпълнение](../media/SubcontractingProcessFlow.png)

Следният списък предоставя описание стъпка по стъпка на процеса на подизпълнение.

1. Мениджърът на проекта създава подизпълнение с доставчик. По подразбиране ценовите листи, които са прикачени към записа на доставчика, се използват за подизпълнението. Акаунтът на доставчика имат релация от тип **Доставчик** или **Снабдител**.
2. Мениджърът на проекта може да посочи подробно всички покупки като елементи на ред за подизпълнение. Редовете за подизпълнение може да са за време, разходи или продукти. Класът на трансакцията на ред за подизпълнение, определя за какво е редът.
3. Мениджърът на акаунта на доставчика и мениджърът на проекта могат да повторят подизпълнението. Цените могат да се коригират в ценовите листи за покупка, които са прикачени към подизпълнението.
4. На този етап или по-късно в процеса, ако редът за подизпълнение е за време, мениджърът на акаунта на доставчика свързва контактите с всеки ред за подизпълнение. Тази асоциация предоставя информация на мениджъра на проекта, който работи по подизпълнението. Когато даден контакт на доставчик е свързан с ред за подизпълнение, системата автоматично създава наличен ресурс от контакта, ако наличният ресурс все още не съществува.
5. Методът на фактуриране на всеки ред за подизпълнение може да е **Фиксирана цена** или **Време и материал**. За редовете за подизпълнение с фиксирана цена се настройва график за фактури, базиран на контролни точки.
6.  След сключване на подизпълнението и преговорите приключват, той се потвърждава. Потвърдените подизпълнители не могат да бъдат редактирани, но ако настъпят промени, подизпълнителят може да бъде „отворен отново за редакции“, който определя състоянието от **Потвърдено** обратно към **Чернова** и преговорите могат да бъдат възобновени. 
7.  Когато създавате общ член на екип по проект, членът на екипа може да бъде свързан към линия на подизпълнител. Това показва необходимостта от персонал на общия член на екипа с капацитет на подизпълнители.
8.  Назованите членове на екипа могат или да бъдат създадени директно по проект, или да бъдат създадени, като ги резервирате с помощта на опита за планиране на ресурси. Ако посочен член на екип по проекта е работник по договор, възможно е това да бъде свързано с линия на подизпълнител. Това ще намали наличния капацитет по линия на подизпълнител.
9.  Ресурсите на подизпълнителя могат да регистрират време, разходи и използване на материали по проекти и задачи по проекта и след това да представят за одобрение. Подобно е и за служителите. Когато записва времето, работникът по договор може да избере конкретна подизпълнителска и подизпълнителна линия.
10. След одобрение, времето, одобрено от подизпълнители, ще записва действителната стойност на проекта въз основа на покупната цена на наетия работник или ролята, която те изпълняват по проекта.
11. Фактурите на доставчика и договорените покупки на фактури на доставчици могат да бъдат записани в системата за работата, извършена от ресурсите на доставчика или продуктите, доставени от доставчика. Редовете на фактури на доставчици трябва да са специфични за даден проект и за клас транзакция на време, разход, продукт/материал, етап или такса. По избор редовете на фактури на доставчици могат да се позовават на ред за подизпълнение.
12. Системата автоматично ще свърже всички фактически разходи, които съответстват на договора и проекта за подизпълнение, с фактурата на доставчика. Това ще улесни 3-странното съвпадение и процеса на проверка.
13. След това ръководителят на проекта може да прегледа автоматично съответстващите фактически данни на проекта, да премахне или добави други фактически данни за разходите по проекта и да завърши процеса на проверка.
14. Приключването на процеса на проверка на всички редове ще маркира фактурата на доставчика като **Готово за плащане**. На този етап фактурата и редовете на доставчика могат да бъдат прехвърлени в система за счетоводство или задължения за обработка на плащането към доставчика. Записаните преди това разходи по проекта ще бъдат отменени и действителните разходи от фактурата на доставчика ще бъдат записани в проекта.

## <a name="quantity-based-subcontract-lines-and-work-based-subcontract-lines"></a>Линии за подизпълнение въз основа на количества и линии за подизпълнение, базирани на работа

Редът за подизпълнение може да бъде базиран на количество, или на работа. 

Когато ред за подизпълнение е **базиран на количествено**, количеството, закупено на линията на подизпълнителя за време, разходи или материали, може да се използва за всеки проект.

Когато редът за подизпълнение е **базиран на работа**, линията на подизпълнителя се съпоставя с основна част от работата, представена от възел в плана на проекта. Стойността на договора за подизпълнение е сумата от всички компоненти, които са необходими за доставянето на тази работа. Те са моделирани като подробности за договора за подизпълнение и могат да бъдат съвкупност от време, разходи или материали. За линия за подизпълнение, базирана на работа, линията за подизпълнение също е посветена на един проект.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
