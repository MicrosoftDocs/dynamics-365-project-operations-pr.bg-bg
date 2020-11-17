---
title: ЧЗВ за управление на ресурси
description: Тази тема дава отговори на често задавани въпроси за управлението на ресурси.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.openlocfilehash: 395aa57d73e5d4a0c9c827c79bf4e7ef229c3981
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4072031"
---
# <a name="resource-management-faq"></a>ЧЗВ за управление на ресурси

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

## <a name="what-is-the-difference-between-a-team-member-and-a-resource-requirement"></a>Каква е разликата между член на екипа и изискване за ресурс?

Член на екипа на проект може да бъде присвоен на задачи, резервиран или резервиран над капацитета и зададен като одобряващ. Изискване за ресурс може да съществува без член на екипа на проект, като чернова на бележка за търсене. 

## <a name="what-is-the-difference-between-proposed-and-soft-booked-hours"></a>Каква е разликата между предложените и непотвърдените часове?

Предложените часове и непотвърдените часове се различават по видимост. Предложените часове са видими само за мениджъри на ресурси и мениджъра на проекта, който е инициирал търсенето с помощта на заявка за ресурс. Непотвърдените часове са видими за всеки, който има достъп до таблото на графика.

## <a name="how-can-i-see-the-soft-booked-hours-for-resources-on-a-team"></a>Как мога да видя непотвърдените часове за ресурси в екип?

Непотвърдени резервации можете да направите, когато резервирате изискване за ресурс. Ресурси, които имат непотвърдена резервация в екип на проект, се показват като членове на екипа, които имат непотвърдени часове. Те се показват също и на таблото на графика.

## <a name="how-do-i-change-the-required-hours-and-the-start-and-end-dates-for-a-resource-generic-or-named-that-i-booked"></a>Как да променя необходимите часове, както и началната и крайната дата, за ресурс (общ или наименуван), които съм резервирал?

След като ресурсите са резервирани, изберете **Поддръжка на резервации** , за да направите всички необходими промени.

## <a name="what-resources-types-does-project-service-automation-support"></a>Какви типове ресурси поддържа Project Service Automation?

**Потребител** и **Контакт** са единствените типове ресурси, които се поддържат в Dynamics 365 Project Service Automation. Въпреки че можете да създавате други видове ресурси (например **Оборудване** и **Група** ), за тях не се поддържа случай на използване „от край до край“.

## <a name="what-is-the-difference-between-an-assignment-and-a-booking"></a>Каква е разликата между присвояване и резервация?

Присвояванията са присвояването на ресурси на задачи по проекта в графика на проекта. Ресурсите могат да бъдат реални или общи ресурси. Резервациите са потвърдено или непотвърдено разпределение на ресурси за даден проект. Потвърдените резервации консумират капацитет на ресурса. В идеалния случай за реални ресурси резервациите и присвояванията трябва да са съгласувани, защото не се различават. PSA обаче не прилага това съгласуване. Изгледът „Съгласуване“ показва на мениджъра на проекта местата, където резервациите на ресурса и присвояванията не са съгласувани.