---
title: Какво е новото или промененото в Project Service Automation, издание на актуализация 41, V3
description: Тази статия изброява функциите и корекциите, които са налични в Microsoft Dynamics 365 Project Service Automation актуализация издание 41, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 03/07/2022
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
ms.reviewer: johnmichalak
ms.openlocfilehash: 8625ae16e45da30614b3a3eec44193bee0c0b36f
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930535"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-41-v3"></a>Какво е новото или промененото в Project Service Automation, издание на актуализация 41, V3

[!include [banner](../includes/psa-now-project-operations.md)]

С удоволствие обявяваме най-новата актуализация за приложението Microsoft Dynamics 365 Project Service Automation. Тази версия включва някои важни подобрения в качеството, производителността и използваемостта. Съвместим е с Dynamics 365 9.x. За да актуализирате до тази версия, посетете страницата на центъра за администриране за решенията на Dynamics 365 Online и инсталирайте актуализацията. За повече информация вижте: [Инсталиране, актуализиране или премахване на предпочитано решение](/power-platform/admin/install-remove-preferred-solution).

Тази статия изброява функциите и корекциите, които са нови или променени за Project Service автоматизация актуализация издание 41, V3. Тази версия е с номер на компилация V3.10.62.162 и е общодостъпна за самостоятелно актуализиране от март 2022 г.

## <a name="update-release-41"></a>Издание на актуализация 41

### <a name="bug-fixes"></a>Корекции на грешки

Следните проблеми са коригирани.

**Управление на проекти**
- Когато се опитвате да създадете проект от шаблон, който се основава на проект, създаден от добавката на работния плот, следната грешка показва, "Проверка на полето "Планирана работа на присвояване на ресурси": Всяка крайна дата на време за присвояване на ресурси Slice не трябва да бъде по-ранна от началната му дата".

**Час и разход**
- Когато се опитвате да изтриете запис за време, следното съобщение за грешка показва, "Неочаквана грешка възниква от ISV код".

**Продажби**
- Когато създавате фактура за крайъгълен камък с фиксирана цена, **полетата Описание** и **външно описание** не се попълват. 
