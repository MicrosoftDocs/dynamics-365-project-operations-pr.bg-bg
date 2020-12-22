---
title: Управление на множество клиенти в договори по проект
description: Тази тема предоставя информация за начина на управление на множество клиенти в договор по проект.
author: rumant
manager: Annbe
ms.date: 11/18/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5554cb062710c3587d81b1a29771a7af84d2d05f
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/25/2020
ms.locfileid: "4643144"
---
# <a name="manage-multiple-customers-on-project-contracts"></a>Управление на множество клиенти в договори по проект

Тази тема предоставя информация за начина на управление на множество клиенти в договор по проект. Можете да използвате договор по проект, когато е необходимо договорно споразумение за множество клиенти за финансиране на сделка. На страницата **Договор по проект** разделът **Обобщение** включва информация за основния клиент за дадена сделка. Други клиенти, които участват в сделката, могат да бъдат добавени към раздела **Клиенти**.

Всички клиенти на договора в раздела **Клиенти** на договора по проекта се задават по подразбиране като клиенти в аспектите на договора във всички нови базирани на проект аспекти на договор, създадени за договора по проекта. Всички съществуващи базирани на проект аспекти на договор не наследяват нови записи на клиенти на договор, които са създадени в по-късен момент.

Можете да добавяте, актуализирате или изтривате клиенти на договор или аспекти на договор по всяко време преди спечелването на договора. Трябва да се настрои клиент на договор по проект като клиент в притежаващата фирма или юридическо лице на страницата **Клиенти**. Юридическите лица се задават в модула **Управление на проекти и счетоводство** на Dynamics 365 Project Operations и са налични като фирми в модулите **Продажби по проект** и **Доставка** на Project Operations.

## <a name="primary-customers"></a>Основни клиенти

Потенциалният клиент в раздела **Обобщение** на договора по проект е основният клиент на договора. Не може да актуализирате основния клиент от списъка с клиенти на договор. Ако се опитате да изтриете основния клиент от списъка с клиенти в договора, ще получите грешка, че основният клиентски запис в договор не може да се изтрива. Вместо това променете клиента в полето **Потенциален клиент** в раздела **Обобщение** на договора по проект. Когато актуализирате това поле, новоизбраният клиент се добавя като нов клиент на договор с флаг **Основен**, зададен на **Да**. Предишният основен клиент все още е клиент по договора, но вече не е основен клиент.

## <a name="create-update-or-delete-a-contract-customer-record"></a>Създаване, актуализиране или изтриване на запис на клиент по договор

Можете да създавате, актуализирате или изтривате клиент на договор от раздела **Клиенти на договор** на страницата **Договор**. Следните полета са включени в записа на клиента на договор на договор по проект.

| **Поле** | **Местонахождение** | **Описание** | 
| --- | --- | --- | 
| Клиент | Редактируема мрежа в раздела **Клиенти на договор** и основната страница и страницата за бързо създаване за клиент на договор. | Изброява всички активни акаунти. Това поле се заключва след създаването на записа. За да актуализирате записа, трябва да го изтриете и да го създадете отново. Ако сте записали действителни данни или ако записът на клиента по договора е „Основен клиент”, не можете да изтриете записа. Когато се създават аспекти на договор, клиентите на договор се копират като клиенти на аспектите на договора. |
| Процент на разделяне на фактуриране | Редактируема мрежа в раздела **Клиенти на договор** и основната страница и страницата за бързо създаване за клиент на договор. | Представлява процентът на всяка нефактурирана трансакция за продажба, която е приписана на клиента на договор. Когато се създават нови аспекти на договор по проект, процентът на разделяне на фактурирането се копира в новосъздадените аспекти на договор и в клиентите на аспектите на договор по проект. |
| Име на контакт за фактуриране | Редактируема мрежа в раздела **Клиенти на договор** и основната страница и страницата за бързо създаване за клиент на договор. | Това текстово поле трябва да се използва за идентифициране на лицето за връзка във фактурата за клиента. Стойността по подразбиране идва от свързания запис на клиент. Името на контакта се копира във **Фактуриране на име на договор** на фактурата, която се генерира за клиента. |
| Име за фактуриране | Редактируема мрежа в раздела **Клиенти на договор** и основната страница и страницата за бързо създаване за клиент на договор. | Използвайте това текстово поле за идентифициране на лицето за връзка във фактурата за клиента. Стойността по подразбиране идва от свързания запис на клиент. Името е копирано в полето **Фактуриране на име на договор** на фактурата, която се генерира за клиента. |
| Условия за плащане | Редактируемата мрежа в раздела **Клиенти на договор** и основната страница и страницата за бързо създаване за клиент на договор. | Стойността по подразбиране идва от свързания запис на клиент. Термините се копират във **Фактуриране на име на договор** на фактурата, която се генерира за клиента. |
| Притежаваща фирма | Редактируема мрежа в раздела **Клиенти на договор по проект** и основната страница и страницата за бързо създаване за клиент на договор по проект. | Юридическото лице, в което е зададен клиентът в модула **Управление на проекти и счетоводство**. Това поле е само за четене и е зададено на притежаващата фирма на договора по проект.</br>Списъкът с клиенти, които да добавите в полето **Акаунт** вече е филтрирано към списъка от компанията собственик в модула **Управление на проекти и счетоводство** от Project Operations. Притежаващата фирма е същата като юридическото лице в модула **Управление на проекти и счетоводство** от Project Operations. Всички разходи и приходи, натрупани от проекта, се отчитат в главната книга на притежаващата фирма. |
| Е закръгляне | Редактируема мрежа в раздела **Клиенти на договор** и основната страница и страницата за бързо създаване за клиент на договор. | Показва дали клиентът е клиент за закръгляване по подразбиране за сделката. В договор по проект може да има само един клиент за закръгляване. Когато разделянето на разходите и нефактурираните продажби на количества водят до разлика в закръгляването, тази разлика се прилага към действителните данни, които се нанасят за клиента. |
| Ограничение, което да не се надвишава | Редактируема мрежа в раздела **Клиенти на договор** и основната страница и страницата за бързо създаване за клиент на договор. | Показва дали има договорено ограничение или горен лимит на общата сума, която ще се фактурира на клиента за ангажимента. Ограничението, което да не се надвишава, настроено на ниво клиент по договор, се оценява в действителните данни за нефактурирани продажби, които посочват клиента по договора. |

## <a name="edit-billing-split-percentages"></a>Редактиране на проценти на разделяне на фактурирането

Може да редактирате процентите на разделяне на фактурирането, като редактирате в мрежата. Когато процентите на разделяне на фактурирането не възлизат на 100 процента, възниква грешка. След като редактирате процента на разделяне на фактурирането, обновете страницата **Договор по проект**, за да премахнете грешката.

Можете също да изберете **Равномерно разпределяне** в подмрежата на клиентите на договора по проект. Разделянето на фактурирането се разпределя равномерно на клиентите на договора по проект. Ако има някакъв коефициент на закръгляване, факторът ще се добави към клиента за закръгляване. Един от клиентите по договор винаги има флаг **Закръгляване**, зададен на **Да**. Този клиент е клиентът за закръгляване. Обикновено клиентът за закръгляване е и основният клиент на договора, но това не е задължително.