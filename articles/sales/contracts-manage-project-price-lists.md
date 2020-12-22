---
title: Управление на ценови листи на проект в договори по проекти
description: Тази тема предоставя информация за управление на ценови листи на проект в договори по проект.
author: rumant
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 030684576e1f53d27921907b07c9e5e0c5efe612
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4133280"
---
# <a name="manage-project-price-lists-on-project-contracts"></a>Управление на ценови листи на проект в договори по проекти

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

Договорите по проект в Dynamics 365 Project Operations са предназначени да поддържат няколко ценови листи с валидни дати на договор. В Project Operations има нов свързан обект, наречен **Ценови листи по проект**. Този обект има релация тип „едно към много” с договор по проект.

Ценовите листи на проекта се използват за определяне на цените на времевите и разходни транзакции по даден проект. Когато даден договор има една или повече ценови листи по проекти, тези ценови листи се използват за определяне на цени за прогнози за време и разходи и действителни данни за проекти, които са свързани с договора чрез аспектите на договора.

Когато в договор по проект няма ценови листи по проекта, ще видите предупредително съобщение, че няма ценови листи по проекта и прогнозите, действителната работа по проекта и разходите няма да са оценени. Няма да има цена за стойностите на продажбите.

## <a name="associate-or-unassociate-a-project-price-list-on-a-project-contract"></a>Свързване или премахване на връзката на ценова листа по проект в договор по проект

### <a name="create-or-associate-a-specific-price-list-for-estimating-project-based-work-and-expenses"></a>Създаване или свързване на конкретна ценова листа за оценка на работата и разходите, базирани на проект

1. В договора по проект изберете раздела **Ценови листи по проект**.
2. В подмрежата изберете **+ Добавяне на нова ценова листа по проект**.
3. На плъзгача **Бързо създаване** изберете ценова листа. 

  Падащият списък показва всички ценови листи с контекст, зададен като **Продажби**, където валутата в ценовата листа съответства на валутата в договора.
  
4. Въведете описание за свързването на ценовата листа по проекта, изберете **Записване** и след това затворете плъзгача **Бързо създаване**.

   Създава се асоциация на ценова листа по проект.
   
5. Повторете стъпки 1-4, за да свържете повече от една ценова листа по проект с договора по проект. Създайте няколко ценови листи по проект само ако имате различна дата на ефективност във всяка от свързаните ценови листи.

> [!NOTE]
> Project Operations не поддържа припокриване на дати на ефективност на ценовите листи по проект. Ако има няколко ценови листи по проект за трансакция с дадена дата, цената на тази трансакция ще бъде нула по подразбиране.

### <a name="remove-a-project-price-list-association"></a>Премахване на връзка на ценова листа по проект

- Изберете ценовата листа по проекта и след това изберете **Изтриване на ценова листа по проекта на договора** в подмрежата. 

  Ценовата листа се премахва от ценовите листи по проекта в договора. Самата ценова листа няма да се изтрие. Ще се изтрие само връзката към договора.

## <a name="set-up-automatic-defaulting-of-project-price-lists-on-a-contract"></a>Настройване на автоматично задаване по подразбиране на ценови листи по проект в договор

Ценовата листа на проекта може да се зададе като листа по подразбиране в договор по проект. Тази настройка може да помогне да се гарантира, че всички договори в организацията винаги ще започват със стандартна ценова листа за този ценови период.

### <a name="set-up-the-organizational-default-for-project-price-lists"></a>Настройване на стойности по подразбиране на организацията за ценови листи по проекти

1. Отидете на **Настройки** > **Общи**, след което изберете **Параметри**.
2. На страницата със списъка **Активни параметри** изберете и щракнете двукратно върху записа, за да го отворите. Докато щраквате двукратно, се уверете, че не щраквате върху стойност на полето, която е хипервръзка. 
3. На страницата **Активни параметри** изберете раздела **Ценова листа**. Подмрежа показва списък с ценови листи по подразбиране. Това е списък със стандартни ценови листи на разходи и продажби. Наличието на свързана ценова листа за **продажби** за всяка валута, в която продавате, гарантира, че ценовата листа за продажбите е по подразбиране и всеки договор, който създавате за клиентите, ще се изпълнява в тази валута.

### <a name="set-up-a-customer-specific-project-price-list"></a>Настройване на ценова листа по проект, специфична за клиента

Можете също така да настроите ценови листи, специфични за клиента, когато сте договорили главно споразумение за ценообразуване с клиентите.

1. Отидете в **Продажби** > **Клиенти**.
2. От списъка с активни акаунти изберете клиента, за когото има специална ценова листа.
3. Изберете клиентския запис, за да го отворите, след което изберете раздела **Ценови листи по проект**. Подмрежа показва списък с ценовите листи по проекта, специфични за този клиент. 
4. Създайте връзка към нова ценова листа тук, за да имате ценова листа по проекта, специфична за този клиент.

## <a name="custom-pricing-on-a-project-contract"></a>Персонализирано ценообразуване в договор по проект

След като имате организационни и специфични за клиента ценови листи по проекти по подразбиране, договорите по проекти ще се създават автоматично с тези връзки към ценови листи по проекти. Ценовите листи по проектите в договор по проект обаче винаги се копират с датата и името на договора, приложени към тях. След това мениджърите на клиенти и ръководителите на проекти могат да започнат да редактират цените в тези копия. Тези променени цени ще бъдат приложими само за този договор по проект.