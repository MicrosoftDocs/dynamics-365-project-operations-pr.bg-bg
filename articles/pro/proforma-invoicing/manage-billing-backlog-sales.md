---
title: Управление на натрупването за фактуриране – олекотено
description: Тази тема предоставя информация за различните изгледи, които могат да се използват при управление на натрупването на фактуриране.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 0e3ca167fa53a6923727eff3e7c34c8706dc7455
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176957"
---
# <a name="manage-the-billing-backlog---lite"></a>Управление на натрупването за фактуриране – олекотено

_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_

Dynamics 365 Project Operations има специални изгледи, които помагат да се управлява натрупването за фактуриране. За да управлявате натрупването за фактуриране, изберете връзките в областта **Продажби** под **Фактуриране**. 

Налични са следните изгледи:

- Суми за капаро и аванси
- Налични суми за капаро и аванси
- Контролни точки на фиксирана цена
- Натрупване на фактуриране за продукт
- Натрупване на фактуриране на време и материал

## <a name="retainers-and-advances"></a>Суми за капаро и аванси

Изгледът **Суми за капаро и аванси** изброява всички суми за капаро и аванси във всички договори по проекти в системата. След фактуриране на капаро или аванс, сумата на авансовото плащане става достъпна за използване.

## <a name="available-retainers-and-advances"></a>Налични суми за капаро и аванси

Изгледът **Налични суми за капаро и аванси** изброява всички налични суми за капаро и аванси във всички договори по проекти в системата. След фактуриране на капаро или аванс, сумата на авансовото плащане става достъпна за използване и се добавя в списъка. След като сумата на капарото или аванса се използва изцяло, тя се премахва от списъка.

## <a name="fixed-price-milestones"></a>Контролни точки на фиксирана цена

Изгледът **Контролни точки за фиксирана цена** изброява всички контролни точки за фиксирана цена във всички аспекти на договор по проект в системата. Единични или няколко контролни точки могат да бъдат маркирани като **Готово за фактуриране** или **Не е готово за фактуриране** от този изглед. Маркирането на контролна точка като **Готово за фактуриране** я прави достъпна за включване в чернова на фактура.

Когато аспекти на договор за много клиенти имат метод за фактуриране с фиксирана цена, се създава контролна точка за всеки клиент в аспектите на договора. Може да се създаде контролна точка и след това да се раздели на отделни записи на специфични за клиента контролни точки. Това разделяне е вътрешно и е в съответствие с разделянето на процента на фактуриране, дефинирано за всеки клиент в аспектите на договора. В изгледа **Контролни точки за фиксирана цена** ще видите записите на отделните специфични за клиента контролни точки. Всеки от тези важни записи може да бъде маркиран като **Готови за фактуриране** отделно от този изглед. Когато едно или повече свързани разделяния на контролни точки се отбележи като **Готово за фактуриране**, състоянието на заглавката се актуализира на **В ход** от **Не е стартирано**. Когато се фактурират всички разделения на контролни точки, състоянието на контролните точки в заглавката се актуализира на **Завършено**.

В този изглед е показан етап на проект на фактура със състояние на фактуриране **Фактура на клиента е създадена**. Когато черновата на фактурата бъде потвърдена, състоянието на фактуриране в записа се актуализира до **Публикувана фактура на клиента**. Не актуализирайте тази стойност на състояние, като използвате персонализиран код. Project Operations не функционира правилно, когато тези стойности на състоянието се актуализират с персонализиран код.

## <a name="product-billing-backlog"></a>Натрупване на фактуриране за продукт

Изгледът **Натрупване на фактуриране за продукт** изброява всички базирани на продукт аспекти на договор във всички договори по проект в системата. Единични или няколко базирани на продукт аспекти на договор могат да бъдат маркирани като **Готово за фактуриране** или **Не е готово за фактуриране** от този изглед. Маркирането на базирани на продукт аспекти на договор като **Готово за фактуриране** ги прави достъпни за включване в чернова на фактура.

В този изглед са показани базирани на продукт аспекти на договор, които са в чернова на фактура, със състояние на фактуриране **Създадена фактура на клиент**. Когато проектофактурата бъде потвърдена, фактурата в този запис се актуализира до **Фактурата на клиента е публикувана**. Не актуализирайте тази стойност на състояние, като използвате персонализиран код. Project Operations не функционира правилно, когато тези стойности на състоянието се актуализират с персонализиран код.

## <a name="time-and-material-billing-backlog"></a>Натрупване на фактуриране на време и материал

Изгледът **Натрупване за фактуриране на време и материали** изброява всички действителни данни за нефактурирани продажби във всички договори по проекти в системата, които не са фактурирани. Единични или множество нефактурирани действителни данни за продажби етапи могат да бъдат маркирани като **Готови за фактуриране** или **Не е готов за фактуриране** от тази гледка. Маркиране на нефактурирани продажби в действителност като **Готови за фактуриране** дава възможност за поставяне в проект на фактура.

Действителните данни за нефактурирани продажби със състояние **Да не се надвишава** като **Неуспешно** не могат да се маркират като **Готово за фактуриране**. Ако действителните данни трябва да се маркират като **Готово за фактуриране**, нулирайте състоянието на другите действителни данни в аспектите на договора, които са разпределени. след което оценете отново състоянието **Да не се надвишава**.

Ако аспекти на договор за много клиенти имат метод за фактуриране на време и материали, когато времето и разходите са одобрени, се създават действителни данни за нефактурирани продажби за всеки клиент в аспектите на договора според разделянето на процента на фактуриране, определено за всеки от клиентите. В изгледа **Натрупване за фактуриране на време и материали** ще видите тези конкретни специфични за клиента действителни данни за продажби. Всеки от тези записи на действителни данни за нефактурирани продажби може да бъде маркиран като **Готови за фактуриране** отделно от този изглед.

Действителни данни за нефактурирани продажби, които са в чернова на фактура, се показват в този изглед със състояние на фактуриране **Създадена фактура на клиент**. Когато проектофактурата бъде потвърдена, фактурата в този запис се актуализира до **Фактурата на клиента е публикувана**. Не актуализирайте тази стойност на състояние чрез персонализиран код. Project Operations не функционира правилно, когато тези стойности на състоянието се актуализират с персонализиран код.