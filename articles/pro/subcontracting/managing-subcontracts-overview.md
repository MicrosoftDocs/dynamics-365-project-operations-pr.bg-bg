---
title: Управление на подизпълнение в Project Operations
description: Тази тема предоставя преглед на целия процес на управление на подизпълнение в Microsoft Dynamics 365 Project Operations.
author: rumant
ms.date: 08/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 6ffceb0886fdc841ea01a099243cf4eeb43e5374a18414576f3639a3e50857fd
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/06/2021
ms.locfileid: "6994218"
---
# <a name="subcontract-management-in-project-operations"></a>Управление на подизпълнение в Project Operations

[!include [banner](../../includes/dataverse-preview.md)]

_**Прилага се за:** Леко внедряване – фактуриране на сделката към проформа_

Подизпълнението в Microsoft Dynamics 365 Project Operations поддържа следния поток на бизнес процес.

![Поток на процеса на подизпълнение](../media/SubcontractingProcessFlow.png)

Ето описание стъпка по стъпка на процеса на подизпълнение.

1. Мениджърът на проекта създава подизпълнение с доставчик. По подразбиране ценовите листи, които са прикачени към записа на доставчика, се използват за подизпълнението. Акаунтът на доставчика имат релация от тип **Доставчик** или **Снабдител**.
2. Мениджърът на проекта може да посочи подробно всички покупки като елементи на ред за подизпълнение. Редовете за подизпълнение може да са за време, разходи или продукти. Класът на трансакцията, който е избран на всеки ред за подизпълнение, определя за какво е редът.
3. Мениджърът на акаунта на доставчика и мениджърът на проекта могат да повторят подизпълнението. Цените могат да се коригират в ценовите листи за покупка, които са прикачени към подизпълнението.
4. На този етап или по-късно в процеса, ако редът за подизпълнение е за време, мениджърът на акаунта на доставчика свързва контактите с всеки ред за подизпълнение. Тази асоциация предоставя информация на мениджъра на проекта, който работи по подизпълнението. Когато даден контакт е свързан с ред за подизпълнение, системата автоматично създава наличен ресурс от контакта, ако наличният ресурс все още не съществува.
5. Методът на фактуриране на всеки ред за подизпълнение може да е **Фиксирана цена** или **Време и материал**. За редовете за подизпълнение с фиксирана цена може да настроите график за фактури, базиран на контролни точки.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]