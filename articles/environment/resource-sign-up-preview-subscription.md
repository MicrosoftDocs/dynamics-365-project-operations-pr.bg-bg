---
title: Регистрирайте се за абонаменти за предварителен преглед на Project Operations за сценарии за ресурси/неналичност
description: Тази статия предоставя информация за това как да се абонирате за и разполагане на Project Operations за сценарии на базата на resouce/non-stocked.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: fb196a50b4cb9e8533db52414e8536d77a30e425
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2022
ms.locfileid: "8920093"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a>Регистрирайте се за абонаменти за предварителен преглед на Project Operations за сценарии за ресурси/неналичност

_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_



В тази статия се обяснява как да се абонирате за пробната оферта и да разположите Project Operations среда за ресурси/не-заредени базирани сценарии.

## <a name="prerequisites"></a>Предварителни изисквания
- Потребителят, който използва визуализацията, трябва да има права на глобален администратор на Клиент на Azure. Можете да създадете наемател по време на първото осребряване на офертата. 
- Внедряването на среда на Finance изисква валиден абонамент за Azure, който ще бъде таксуван за среда. Можете да използвате съществуващия абонамент на вашите организации или да използвате [пробна версия на Azure](https://azure.microsoft.com/free/), за да започнете. CDS средата ще бъде предоставена безплатно за ограничен период от 30 дни.

> [!IMPORTANT]
> Само един човек, администраторът на наемател, в дадена организация трябва да изпълни тази задача. Ако не сте абонат на тази версия, изчакайте, докато организацията ви бъде регистрирана и не получите потребителските си идентификационни данни.
> 
> Пробните версии са еднократни за наемателя. Можете да стартирате пробна версия само веднъж. Препоръчваме ви да създадете нов клиент за целите на пробния период.


### <a name="dynamics-365-project-operations-ce---preview-trial"></a>Dynamics 365 Project Operations (CE) - Пробен преглед 

Преди да започнете, уверете се, че сте влезли в браузър с потребителския работен акаунт в наемателя, където искате визуализация на Project Operations.

1. Използвайте първия код на офертата, **Dynamics 365 Project Operations** тук [Пробна версия на Project Operations](https://aka.ms/try-po).
2. Потвърдете поръчката си.

  Ще видите, че офертата за потвърждение е осребрена успешно.

### <a name="dynamics-365-finance-preview-trial"></a>Dynamics 365 Finance пробна версия за визуализация

Отидете на [Пробен период за преглед на Dynamics 365 for Finance](https://aka.ms/trypoche) и повторете стъпките от предишния раздел с офертата, регистрирайте се в хоствана в облак среда.  

## <a name="assign-licenses"></a>Присвояване на лиценз

> [!IMPORTANT]
> Ще ви е необходим административен достъп до организацията на Портал на Microsoft 365 на вашата организация, за да изпълните следните стъпки.

1. Отидете в [Microsoft 365 администраторски център](https://portal.office.com/), за да присвоите лицензите на потребителите си.

2. На страницата **Активни потребители** изберете потребителите, на които искате да присвоите лиценз.

3. Проверете дали лиценз за **Dynamics 365 Project Operations** е избран и изберете **Записване на промените**.

> [!NOTE]
> Пробната оферта за Finance не трябва да се възлага на потребител.

## <a name="start-a-new-project-in-lcs"></a>Стартиране на нов проект в LCS

Създаване на нов LCS проект, както е описано в статията, [Стартирайте нов проект в LCS](create-lcs-project.md)

## <a name="add-an-azure-subscription-to-an-lcs-project"></a>Добавяне на абонамент за Azure към проект на LCS

За да завършите тази задача, изпълнете стъпките в статията, [Добавете абонамент за Azure към LCS проект](resource-add-azure-subscription-lcs-project.md).

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a>Разгърнете демонстрационната среда на Finance с Project Operations за сценарии с ресурси/неналичност

Следвайте насоките в статията, [Осигуряване на нова среда](resource-provision-new-environment.md) за завършване на разполагането. Използвайте [демо среда](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) тип разполагане за предварителен преглед. 

## <a name="install-cds-setup-and-configuration-data"></a>Инсталирайте данни за настройка и конфигурация на CDS

Инсталирайте данни за настройка и конфигурация на CDS, както е описано в статията, [Настройване и прилагане на Common Data Service](resource-apply-pro-setup-config-data.md) конфигурационни данни в.
Завършете тази стъпка само след като демо среда на Finance е внедрена и демо данните са готови.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
