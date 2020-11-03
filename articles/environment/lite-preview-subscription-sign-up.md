---
title: Регистриране за абонамент за преглед
description: Тази тема предоставя информация за това как да се абонирате и разгърнете внедряване на Project Operations lite - сделка за проформа фактуриране.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5342466f308ab62a9f73a85fbd838d7c33bb1f47
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071683"
---
# <a name="sign-up-for-a-preview-subscription-for-lite-deployment--deal-to-proforma-invoicing"></a>Регистрирайте се за предварителен абонамент за опростено внедряване - сключете проформа за фактуриране

Тази тема обяснява как да се абонирате за предложението на партньора за преглед и да внедрите Dynamics 365 Project Operations lite - сделка за проформа фактуриране.

> [!NOTE]
> Този процес ще се промени в предстоящите версии на Project Operations.

## <a name="prerequisites"></a>Предварителни изисквания

- Ще получите имейл с покана да участвате в визуализацията. Можете да поискате визуализация на [Уебсайт на Project Operations](https://dynamics.microsoft.com/en-us/project-operations/overview/).
- Потребителят, който използва визуализацията, трябва да има права на глобален администратор на Клиент на Azure.
- Прегледайте всички условия.

## <a name="subscribe"></a>Абониране

Когато получите одобрение за [заявка за предварителен преглед](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u), ще получите две оферти от Microsoft по имейл. Тези предложения ви позволяват да разгърнете визуализацията на Project Operations:

- Dynamics 365 Project Operations (CRM) – пробна версия за преглед
- Office 365 Project Operations - Пробна версия за преглед

> [!IMPORTANT]
> Само един човек, администраторът на наемател, в дадена организация трябва да изпълни тази задача. Ако не сте абонат на тази версия, изчакайте, докато организацията ви бъде регистрирана и не получите потребителските си идентификационни данни.

### <a name="dynamics-365-project-operations-crm---preview-trial"></a>Dynamics 365 Project Operations (CRM) – пробна версия за преглед 

Преди да започнете, уверете се, че сте влезли в браузър с потребителския работен акаунт в наемателя, където искате визуализация на Project Operations.

1. Осребрете първия код на офертата, **Dynamics 365 Project Operations (CRM) - Преглед на пробен период** като го поставите в URL адреса на браузъра.

![Осребряване на оферта](./media/16RedeemFirstOfferNew.png)

2. Потвърдете поръчката си.
![Потвърждаване на поръчката](./media/17ConfirmOrderNew.png)

Ще видите, че офертата за потвърждение е осребрена успешно.

![Потвърждение](./media/18OrderConfirmationNew.png)

### <a name="office-365-project-operations---preview-trial"></a>Office 365 Project Operations - Пробна версия за преглед

Повторете същите стъпки като при първия код на офертата. Не забравяйте да добавите втория код на офертата, като използвате същия потребителски акаунт, който е използван с първия код на офертата.

## <a name="assign-licenses"></a>Присвояване на лиценз

> [!IMPORTANT]
> Ще ви е необходим административен достъп до организацията на Портал на Microsoft 365 на вашата организация, за да изпълните следните стъпки.


1. Отидете на [Административен център на Microsoft 365](https://portal.office.com/), за да присвоите лицензите на вашите потребители.

![Начална страница на център за администрация](./media/14AdminPortal.png)

2. На страницата **Активни потребители** изберете потребителите, на които искате да присвоите лиценз.

![Присвояване на лицензи](./media/15AssignLicenses.png)

3. Проверете дали **Преглед на Dynamics 365 Project Operations (CRM)** и **Office 365 Project Operations - Преглед** лицензите са избрани. 
4. Изберете **Записване на промените**.

## <a name="create-a-new-cds-environment"></a>Създаване на нова среда на CDS

1. Осигурете нова среда за внедряване на CDS за Project Operations, като следвате инструкциите в темата, [Модел за внедряване на CDS](lite-deployment.md). Когато изберете типа среда, не забравяйте да използвате **Пробен период (базиран на абонамент)**.
![Нова среда](./media/19CreateEnvironment.png)

2. Изберете **Активирайте приложенията на Dynamics 365** настройка и оставете **Автоматично внедряване на тези приложения** празно.  
3. Изберете **Запиши** , за да създадете средата.

![Добавяне на база данни](./media/20CreateEnvironment1.png)

4. След като средата е създадена, инсталирайте **Microsoft Dynamics 365 Project Operations** решение. 

![Инсталиране на решение](./media/21InstallSolution.png)

## <a name="install-a-cds-configuration-and-setup-demo-data"></a>Инсталирайте конфигурация на CDS и настройте демонстрационни данни

Инсталирайте конфигурацията на CDS и настройте демонстрационни данни, като следвате инструкциите в темата, [Приложете демо настройка и данни за конфигурация](lite-apply-demo-setup-config-data.md).
