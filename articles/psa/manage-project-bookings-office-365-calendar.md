---
title: Управление на проекти и резервации във вашия календар на Office 365
description: Как да управлявате проекти и резервации във вашия календар на Office 365
author: ruhercul
manager: kfend
ms.service: project-operations
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
- D365PS
- ProjectOperations
ms.openlocfilehash: 31ff541f5b817c29b162c38c282df8cfd866e375
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129035"
---
# <a name="manage-projects-and-bookings-in-your-calendar-project-service"></a>Управление на проекти и резервации във вашия календар (Project Service)

> [!Note]
> ОТХВЪРЛЕНА: Тази функция е отхвърлена и вече не е налична.

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] 

Преглед на лични ангажименти, резервации за работа по проекти и присвоявания на работна поръчка за Field Service с помощта на календара на [!INCLUDE[pn_office_365](../includes/pn-office-365.md)].  
  
 С всичко това на едно място е лесно да организирате своя ден. Всички ваши срещи, ангажименти, резервации и задачи са налични в календара на [!INCLUDE[pn_office_365](../includes/pn-office-365.md)].  
  
 Ако използвате [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], можете да въведете и личните си ангажименти в изгледа за въвеждане на време в Project Service. Това позволява на мениджърите по проекти и ресурси да разберат дали сте налични за проекти. Също така ви спестява време, защото не е нужно да въвеждате информацията за вашите лични ангажименти два пъти. Просто можете да импортирате своите лични ангажименти от календара си в изгледа за въвеждане на време в Project Service.  
  
 Вашият календар ще синхронизира проекта и резервациите за работна поръчка от днес за следващите четири седмици. Тази настройка не може да се променя.  
  
 Синхронизирането се поддържа само еднопосочно, от PSA към календара ви на [!INCLUDE[pn_office_365](../includes/pn-office-365.md)]. Можете да синхронизирате в обратен ред. 
  
 За да научите как да използвате вашия календар на [!INCLUDE[pn_office_365](../includes/pn-office-365.md)], вижте [Календар в Outlook в уеб за бизнес](https://support.office.com/article/Calendar-in-Outlook-on-the-web-for-business-5219c457-d1fe-4c2f-9032-1a816b88e936)  
  
## <a name="setup"></a>Инсталация  
 Преди да можете да видите и управлявате вашите резервации в календара на [!INCLUDE[pn_office_365](../includes/pn-office-365.md)], трябва да настроите няколко неща.  
  
- Необходимо е да имате идентификационни данни на глобален администратор или системен администратор на [!INCLUDE[pn_office_365](../includes/pn-office-365.md)].  
  
- Администраторите ще трябва да конфигурират профила на имейл сървъра, а всеки потребител ще трябва да конфигурира пощенската си кутия. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Настройване на обработка на имейл чрез синхронизиране от страна на сървъра](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks)  
  
## <a name="turn-on-synchronization-for-your-organization-admin-task"></a>Включване на синхронизация за организацията (задача за администратор)  
  
1.  От главното меню щракнете върху **Настройки** > **Администрация**.  
  
2.  Щракнете върху **Системни настройки**.  
  
3.  Щракнете върху раздела **Синхронизация**.  
  
4.  Под **Изберете дали да разрешите синхронизирането на резервиране на ресурси с**, изберете **Синхронизиране на резервация на ресурси с Outlook**.  
  
## <a name="turn-on-synchronization-for-your-user-profile-user-task"></a>Включване на синхронизацията за вашия потребителски профил (задача за потребител)  
  
1.  Щракнете върху бутона **Настройки** в горния десен ъгъл на екрана.  
  
2.  Щракнете върху **Опции**.  
  
3.  Щракнете върху раздела **Синхронизация**.  
  
4.  Под **Синхронизация на резервиране на ресурс с Outlook**, изберете **Синхронизиране на резервиране на ресурс с Outlook**.  
  
## <a name="import-your-personal-appointments-user-task"></a>Импортиране на личните ви ангажименти (задача за потребител)  
 Можете да импортирате своите лични ангажименти от календара си в изгледа за въвеждане на време в Project Service Automation.  
  
1. Отворете календара на [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] и щракнете върху **Импортиране на данни**.  
  
2. На екрана с филтрите, изберете **Ангажименти от Exchange** и след това щракнете върху **Приложи**.  
  
3. Системата ще извлече ангажиментите в изглед за въвеждане на време като предложени записи от текущата седмица. За да добавите записи за още една седмица, щракнете върху **Назад** или **Напред**.  
  
4. Изберете ангажимента, който искате да добавите към изгледа за въвеждане на време на Project Service Automation.  
  
5. На изскачащия прозорец **Въвеждане на време** изберете подходящите опции за преобразуване на ангажимента в изглед за въвеждане на време на Project Service Automation.  
  
6. Щракнете върху **Запиши**.  
  
### <a name="see-also"></a>Вижте също  
 [Ръководство за време, разходи и сътрудничество](../psa/time-expense-collaboration-guide.md)
