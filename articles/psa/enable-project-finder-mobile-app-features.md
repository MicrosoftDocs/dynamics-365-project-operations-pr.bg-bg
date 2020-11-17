---
title: Разрешаване на функциите на приложението Project Finder Mobile
description: Как се разрешават функциите на приложението Project Finder Mobile за Project Service
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 749c5682dc2e639843a0a8a085fe8af65502d433
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071827"
---
# <a name="enable-project-finder-mobile-app-features-project-service"></a>Разрешаване на функциите на приложението Project Finder Mobile (Project Service)

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

Вашите ресурси могат да използват приложението Project Finder Mobile на телефона си с [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], за да се намерят нови проекти, по които да работят и да актуализират своите набори от умения.  
  
 Приложението е налично за телефони [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)], [!INCLUDE[tn_android](../includes/tn-android.md)] и [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)].  
  
 Трябва да зададете няколко опции в настройката на параметрите за вашата организационна единица, за да позволите на потребителите да разглеждат изискванията за ресурс на проекти и актуализират уменията си.  
  
> [!NOTE]
>  Приложението Project Finder Mobile работи само с [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)], а не с локални инсталации.  
  
1. Отидете на **Project Service > Параметри**.  
  
2. Щракнете върху настройката за параметри, която искате да използвате за разрешаване на функциите на приложението Project Finder Mobile.  
  
3. В зоната **Общи** задайте **Изисквания за ресурсите, видими за ресурсите** на **Да**.  
  
4. Задайте **Разрешаване на актуализация на уменията от ресурса** на **Да**.  
  
   ![ProjectService_ProjectFinderEnable](../psa/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")  
  
   Това е глобална настройка. Ръководителите на проекти могат да зададат дали даден проект ще се вижда на тази страница на **Екип на проекта** на проекта.  
  
   ![ProjectService_ProjectTeamVisible](../psa/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")  
  
## <a name="email-notifications"></a>Известявания по имейл  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] изпраща имейли по отношение на искания ресурс към следните получатели в следните часове:  
  
|Получател|Събитие|  
|---------------|-----------|  
|Мениджър на проект|-   Когато даден ресурс се запише за проект чрез приложението Project Finder Mobile.|  
|Ресурс|-   Когато работата по проект, за който ресурсът се е записал, вече е била изпълнена от друг ресурс.<br />-   Когато заявките им за одобрение на умение са били одобрени или отхвърлени.<br />-   Когато заявките им за записване за проект са били одобрени или отхвърлени.|  
  
## <a name="privacy-notice"></a>Съобщение за поверителност  
 [!INCLUDE[cc_privacy_crm_project_finder_mobile_app](../includes/cc-privacy-crm-project-finder-mobile-app.md)]  
  
### <a name="see-also"></a>Вижте също  
 [Задаване на ресурси](../psa/set-up-resources.md)