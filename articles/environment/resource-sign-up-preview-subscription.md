---
title: Регистрирайте се за абонаменти за предварителен преглед на Project Operations за сценарии за ресурси/неналичност
description: Тази тема предоставя информация за това как да се абонирате и да внедрите Project Operations за сценарии, базирани на ресурс/неналичност.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4d35a8bf9e8a841b45808b26ae2587c5b7d99d72
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948752"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a>Регистрирайте се за абонаменти за предварителен преглед на Project Operations за сценарии за ресурси/неналичност

_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_

Тази тема обяснява как да се абонирате за предварителен преглед/оферта за партньор и да внедрите среда на Project Operations за сценарии, базирани на ресурси/неналичност.

## <a name="prerequisites"></a>Предварителни изисквания

- Ще получите имейл с покана да участвате в визуализацията. Можете да поискате визуализация на [Уебсайт на Project Operations](https://dynamics.microsoft.com/en-us/project-operations/overview/).
- Потребителят, който използва визуализацията, трябва да има права на глобален администратор на Клиент на Azure.
- Внедряването на среда на Finance изисква валиден абонамент за Azure, който ще бъде таксуван за среда. Можете да използвате съществуващия абонамент на вашите организации или да използвате [пробна версия на Azure](https://azure.microsoft.com/en-us/free/), за да започнете. CDS средата ще бъде предоставена безплатно за ограничен период от 30 дни.

## <a name="subscribe"></a>Абониране

Когато вашата [заявка за предварителен преглед](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) бъде одобрена, ще получите две оферти от Microsoft по имейл. Тези предложения ви позволяват да разгърнете визуализацията на Project Operations:

- Dynamics 365 Project Operations – пробна версия за преглед
- Пробна версия за преглед на Dynamics 365 for Finance and Operations.

> [!IMPORTANT]
> Само един човек, администраторът на наемател, в дадена организация трябва да изпълни тази задача. Ако не сте абонат на тази версия, изчакайте, докато организацията ви бъде регистрирана и не получите потребителските си идентификационни данни.

### <a name="dynamics-365-project-operations--preview-trial"></a>Dynamics 365 Project Operations – пробна версия за преглед

1. Осребрете първата оферта, **Пробна версия на Dynamics 365 Project Operations** с URL адреса, предоставен в имейла за добре дошли.

![Първа оферта](./media/1FirstOffer.png)

2. Уверете се, че сте влезли като потребител, който принадлежи към организацията, която ще се абонира за услугата.
3. Продължете с осребряването на офертата. 
4. Изберете **Да, добавете го към моя акаунт**.

![Осребряване на оферта](./media/2RedeemFirstOffer.png)

![Потвърдете офертата](./media/3ConfirmFirstOffer.png)

![Офертата е осребрена](./media/4OfferSuccessfulyRedeemed.png)

### <a name="dynamics-365-finance-preview-trial"></a>Пробна версия за преглед на Dynamics 365 Finance

Повторете същите стъпки с втората оферта от имейла за добре дошли.

## <a name="assign-licenses"></a>Присвояване на лицензи

> [!IMPORTANT]
> Ще ви е необходим административен достъп до организацията на Портал на Office 365 на вашата организация, за да изпълните следните стъпки.

1. Отидете на [Административен център на Microsoft 365](https://portal.office.com/), за да присвоите лицензите на вашите потребители.

![Административен портал на Office](./media/5OfficeAdminPortal.png)

2. На страницата **Активни потребители** изберете потребителите, на които искате да присвоите лиценз.

![Присвояване на лицензи](./media/6AssignLicenses.png)

3. Проверете дали е избран лицензът Project Operations и изберете **Запазите промените**. 

> [!NOTE]
> Пробната оферта за Finance не трябва да се възлага на потребител.

## <a name="start-a-new-project-in-lcs"></a>Стартиране на нов проект в LCS

Създайте нов LCS проект, както е описано в темата [Стартирайте нов проект в LCS](create-lcs-project.md)

## <a name="add-an-azure-subscription-to-an-lcs-project"></a>Добавяне на абонамент за Azure към проект на LCS

За да изпълните тази задача, следвайте стъпките в темата [Добавете абонамент за Azure към LCS проект](resource-add-azure-subscription-lcs-project.md).

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a>Разгърнете демонстрационната среда на Finance с Project Operations за сценарии с ресурси/неналичност

Следвайте указанията в темата [Осигурете нова среда](resource-provision-new-environment.md) за завършване на разполагането. Използвайте [демо среда](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) тип разполагане за предварителен преглед.

## <a name="install-cds-setup-and-configuration-data"></a>Инсталирайте данни за настройка и конфигурация на CDS

Инсталирайте CDS данни за настройка и конфигурация, както е описано в темата [Настройте и приложете конфигурационни данни в Common Data Service](resource-apply-pro-setup-config-data.md).

