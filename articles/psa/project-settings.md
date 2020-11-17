---
title: Настройки на проекти
description: Тази тема предоставя информация за настройките за управление на проекти.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c9b8659f3b7ee81d2e21ef52743debd521fa9bb9
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071983"
---
# <a name="project-settings"></a>Настройки на проекти

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Използвайте следните настройки за достъп до функциите за планиране на проекти.

## <a name="work-template"></a>Работен шаблон

За да създадете график на проект, създайте шаблон на календар на проект, който определя броя на работни часове на ден и всички неработни дни. За да създадете шаблон за календар на проект, свържете работен шаблон с полето **Шаблон на календар** за проекта. Изпълнете следните стъпки, за да създадете работен шаблон.

1. В PSA, в левия навигационен екран, щракнете върху **Ресурси**. 
2. На страницата със списъка **Ресурси** отворете потребителски запис и след това изберете **Показване на работните часове**.

  > [!NOTE]
  > Уверете се, че сте разрешили изскачащи прозорци на страницата на браузъра. Това ви позволява да видите работните часове, зададени за ресурса.
  
3. В раздела **Месечен изглед** щракнете върху **Настройване**. Показва се списък с три опции: 

  - Нов седмичен график
  - Седмичен график за един ден
  - Почивка

> ![Настройване на опции](media/project-13.png)

4. Изберете **Нов седмичен график** и след това задайте опциите за този график на ресурс. Можете да зададете повтарящ се седмичен график, дневни часови параметри, неработни дни и др.
5. Задайте диапазон от дати, изберете **Запиши** и след това щракнете върху **Затваряне**. 
6. Върнете се на страницата със списъка **Ресурси** и изберете ресурса, за който задавате работните часове. 
7. Изберете **Задаване на календара като** , за да зададете работния шаблон. 
8. В диалоговия прозорец **Работен шаблон** въведете името за работния шаблон и след това изберете **Прилагане**. 

Сега можете да свържете работния шаблон с шаблон на календар на проект.

## <a name="resource-roles"></a>Роли на ресурси

Терминът *роля на ресурс* се отнася до набор от умения, компетенции и сертификати, които дадено лице трябва да притежава, за да изпълни определен набор от задачи по даден проект. PSA ви позволява да остойностявате и фактурирате времето на ресурс въз основа на ролята, с която е свързан ресурсът. Всяка организация трябва да настрои тези роли с помощта на лявата навигация в менюто на **Project Service**.

Всяка организация трябва да настрои тези роли в страницата **Активни категории ресурси**. За да отворите тази страница, в левия навигационен екран изберете **Роли на ресурси**.

## <a name="price-lists"></a>Ценови листи

Ценовите листи ви позволяват да задавате разходите и продажните цени за роли на ресурси, категории разходи, продукти и други елементи в дадена организация. Преди да настроите финансови прогнозни оценки за работата, която трябва да бъде извършена за проект, трябва да създадете поддържаща ценова листа за разходи и продажби. В секцията с параметри трябва също да настроите ценова листа за разходи и продажби по подразбиране, която се отнася за всички проекти, които са създадени в организацията. На страницата **Активни параметри на проекта** се уверете, че сте настроили ценова листа за разходи и продажби.