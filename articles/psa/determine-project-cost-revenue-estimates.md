---
title: Определяне на прогнози за разходите и приходите по проект
description: Как се определят прогнози за разходите и приходите по проект в Project Service
author: ruhercul
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
ms.openlocfilehash: 1652b39b6c8a703bf198a990eb9047eff9dc9f4c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071828"
---
# <a name="determine-project-cost-and-revenue-estimates"></a>Определяне на прогнози за разходите и приходите по проект 

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

Прогнозите за проект предоставят финансов поглед за прогнозната и планираната работа в съставната структура на работата по проекта. Изгледът на прогнозите ви информира за въздействието на разходите и приходите на планираната работа. Изгледът на прогнозите предоставя инструмент за преглед на информация с редица предварително дефинирани величини, за да ви информира най-добре за финансовото въздействие на проекта.  
  
## <a name="cost-and-sales-value-of-the-project"></a>Цена и стойност на продажбите на проекта  
Ценовите листи на [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] определят разходите и ставките за фактуриране за ролите, които използва проектът. Въз основа на ролите, свързани със задачите в съставната структура на работата по проекта, можете да определите въздействието на разходите и приходите от съответната работа.  
  
## <a name="cost-price-defaulting"></a>Извличане на себестойност  
Всеки проект принадлежи към организация (посочена в **Притежаваща единица** в проекта). Ценовата листа, свързана с притежаващата организационна единица, определя себестойността на единицата. [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] определя себестойността за ролите чрез търсене на комбинацията от роля, единица и организационна единица в ценовата листа за разходи, за да се получи правилната себестойност за валидната дата за редовете за прогнози.  
  
Ако комбинацията от роля, единица и организационна единица не води до себестойността от ценовата листа на притежаващата единица, единицата се пренебрегва в полза на комбинацията от роля и организационна единица. Ако има себестойности, цената се преобразува към единица, която сте избрали в реда за прогнозата.  
  
Ако комбинацията на роля и организационна единица не води до себестойност, организационната единица се пренебрегва в полза на комбинацията от роля и единица, а цената се извлича след прилагане на всяко преобразуване, ако е необходимо.  
  
 Ако няма цена за ролята, тогава себестойността възлиза на 0,00 в реда за прогнозата.  
  
 Всички суми за разходи в редовете за прогнозни цени по проекта са във валутата на притежаващата организационна единица.  
  
## <a name="sales-price-defaulting"></a>Извличане на продажна цена  
Ценовата листа за продажби е базиран на обекта на продажба, към който е прикачен проектът. Ценовата листа за продажби, свързана с офертата или договора, определя единичната продажна цена. Ако офертата или договорът имат ценова листа по избор, тя ще бъде ценовата листа за продажби по подразбиране за прогнозите за проекта. Ако няма никаква асоциация с обектите на продажбите, ценовата листа за продажби по подразбиране, конфигурирана в настройките на параметрите, ще бъде ценовата листа за продажби по подразбиране за проекта. Всеки ред за прогнозна оценка има свързана организационна единица за ресурс, за да укаже организационна единица, от която ресурсите ще бъдат резервирани за извършване на работата. Продажната цена на свързаните роли се определя чрез чрез търсене на комбинацията от роля, единица и организационна единица на ресурса в ценовата листа за продажби, за да се получи правилната цена за продажби за валидната дата за редовете за прогнози.  
  
Ако комбинацията на ролята, единицата и организационна единица на ресурса не доведе до продажна цена от ценовата листа на продажбите, системата ще пренебрегне единицата и ще търси комбинацията от единица и организационна единица на ресурса. Ако се намери продажна цена, тя ще се преобразува към единицата, която сте избрали в реда за прогнозата за продажбите.  
  
Ако системата не открие цена за ролята, тогава продажната цена трябва да възлиза на 0,00 в реда за прогнозата.  
  
Изгледът на прогнозите има изглед на мрежа, който показва равна мрежа от редове за прогнози с единична и обща цена за разходите и продажбите.  
  
## <a name="time-phased-view-of-project-estimates"></a>Изглед с времеви фази на прогнозите за проекта  
В изгледа на времеви фази за прогнозите на проекта данните за прогнозите от изгледа на мрежа се анализират по подразбиране по роля и показват разпределение на прогнозните данни по времевата линия на избраната времева рамка.  
  
## <a name="effort-estimate-allocation-based-on-task-mode"></a>Прогнозно разпределение на усилията въз основа на режима на задачи  
В изгледа на времеви фази общите прогнозни усилия за задачата се разпределят чрез възлагане на определен брой часове на усилия за единица време от избраната времева рамка. В project service режимът на задачите определя как се разпределят усилията по продължителността на задачата. Двата вида разпределение са равномерно разпределение и разпределение на базата на работни часове  
  
## <a name="work-hours-based-allocation"></a>Разпределение на базата на работни часове  
Автоматично планиране на режима на задачите за дадена задача обуславя, че за броя прогнозни ресурси за задачата те се очаква да бъдат използвани за пълното работно време на ден.Работете в движение Това се прилага и при разпределяне на усилията чрез разделяне по продължителността на задачите изгледа с времеви фази. Например една времева рамка „Ден“ за задача, за която се очаква да бъде завършена от един ресурс, усилието, разпределено на ден, няма да надвиши работно време на ден, определено в календара на проекта. Следователно разпределението на усилията винаги гарантира, че ресурсите са очаква да бъдат използвани през целия ден.  
  
## <a name="even-distribution"></a>Равномерно разпределение  
Режимът на задачите с ръчно планиране не спазва работното време, календара на проекта или броя ресурси, определени за задачата. Графикът за задача се основава на въвеждането от потребителя. За такива задачи разпределението на усилията за единица време от избраната времева рамка няма никакви ограничаващи фактори. Общите усилия за задачата са еднакво разделени и разпределени за всяка единица време за избраната времева рамка.  
  
По този начин режимът на задачите, дефиниран в задачата, определя разпространението или разпределението на усилията за единица време период в прогнози с времеви фази.  
  
## <a name="grouping-and-time-phasing-options"></a>Опции за групиране и времеви фази  
Този изглед ви помага да разберете разпределението на усилията, разходите и прогнозните продажби на ден, седмица, месец или година. Опцията „Групиране по“ позволява анализирането на данните от прогнозите с две други величини: категория и ресурс. В изгледа на мрежа и в изгледа на времеви фази можете да изберете полетата, които да се показват. Общи суми за всеки от времевите блокове се показват в долната част, като указват общите прогнозна усилия, разходи и продажби за ден, седмица, месец или година.  
  
Извличането на цените за разходи и продажби зависи от датата – когато ставките за ролите се променят, това ще е по-видимо в изгледа на времеви фази при преглеждане на прогнозни данни, анализирани според „Ресурс“ и с времева фаза седмица.  
  
## <a name="expense-estimates"></a>Прогнози за разноски  
Всички разноски, които ще бъдат направени в проекта, които не са пряко свързани с труда, който ще се положи, могат да бъдат записани в прогнозите за проекта изгледа на мрежа. С помощта на опцията **Добавяне на прогнозни разноски** в изгледа на мрежата можете да постигнете това. Прогнозните разноски могат да бъдат записани за конкретна задача или за целия проект; можете да изберете категории на разноските в тези редове и да изберете ориентировъчна дата за това кога се очаква да се направят разноските. Ако свързаните ценови листи за разходи и продажби имат цени по подразбиране или проценти на надценки, дефинирани за категориите разноски, това ще бъде съответно изведено в реда на прогнозата.  
  
### <a name="see-also"></a>Вижте също  
 [Ръководство за мениджъри на проекти](../psa/project-manager-guide.md)