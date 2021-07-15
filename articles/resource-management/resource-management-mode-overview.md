---
title: Общ преглед на режими на управление на ресурси
description: Тази тема предоставя информация за функционалността за управление на ресурс в Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.custom: intro-internal
ms.openlocfilehash: 41265534661e51565bf31105ef69cec9b3b181c3
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/07/2021
ms.locfileid: "6367878"
---
# <a name="resource-management-modes-overview"></a>Общ преглед на режими на управление на ресурси

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_


Dynamics 365 Project Operations поддържа два режима, за да можете да изпълните цялостния процес на резервация. Режимът на управление се определя като параметър на проекта и може да бъде модифициран, ако вашият бизнес се нуждае от промяна.    

## <a name="central-mode"></a>Централен режим
За организации, които централизират разпределението на ресурси за проекти, централният режим осигурява начин да се гарантира, че мениджърите на проекти могат да определят изискванията за ресурси на ниво проект. Изпълнението на изискванията за ресурси се делегира на мениджър на ресурси. Мениджърите на проекти могат да приемат или отхвърлят ресурси, предложени от Мениджъра на ресурси.

![Централен режим](./media/resource-management-central.png)

За да управлявате ресурси с централния режим, вижте:

- [Присвояване на общи налични ресурси на задача и генериране на изисквания за ресурси](/dynamics365/project-service/assign-generic-bookable-resource)
- [Резервиране на наименувани ресурси от изисквания за ресурси](/dynamics365/project-service/book-named-resource)
- [Подаване на заявка за ресурс](/dynamics365/project-service/submit-resource-request)
- [Изпълнете заявка за ресурс](/dynamics365/project-service/resource-management-fulfill-requests)
- [Приемане или отхвърляне на предложен ресурс по проект от заявка за ресурс](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a>Хибриден режим
За организации, които изискват гъвкавост при разпределението на ресурсите, хибридният режим дава възможност както на ръководителите на проекти, така и на мениджърите на ресурси да резервират ресурси.

![Хибриден режим](./media/resource-management-hybrid.png)

В допълнение към процеса на поддържан централен режим, вижте следните теми за управление на всички други поддържани потоци на резервации в хибриден режим:

Резервиране на ресурс директно към проект:
- [Резервиране на наименувани налични ресурси в екип по проект и присвояване на задачи](/dynamics365/project-service/assign-named-bookable-resource)

Резервиране на ресурс от изискване за ресурси:
- [Присвояване на общи налични ресурси на задача и генериране на изисквания за ресурси](/dynamics365/project-service/assign-generic-bookable-resource)
- [Резервиране на наименувани ресурси от изисквания за ресурси](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]