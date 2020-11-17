---
title: Инсталация на примерни данни
description: Тази тема предоставя информация за инсталиране на примерни данни в Project Service Automation.
ms.custom: dyn365-projectservice
ms.date: 11/08/2018
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.suite: ''
applies_to: Dynamics 365 Project Service Automation
author: ruhercul
ms.author: ruhercul
search.audienceType: IT Pro, Developer
search.app: ''
ms.openlocfilehash: 46dbd8d125396baa97537ea5d11c47864558c113
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071885"
---
# <a name="sample-data-installation-for-the-project-service-application"></a>Инсталиране на примерни данни за приложението Project Service

За да ви помогне да създадете своя собствена демонстрационна среда, Microsoft предоставя достъпни за изтегляне пакети с данни, които демонстрират възможностите на вашите приложения. Съществуват два типа примерни пакети с данни:
- справка/данни за настройка
- демонстрационни данни (справка/настройка и транзакционни данни, като работни поръчки и проекти)

Примерните пакети с данни за **справка** са достъпни за изтегляне в три различни пакета, така че можете да инсталирате данни само за Project Service или само за Field Service или можете да инсталирате примерни данни за двете приложения едновременно.

Примерните пакети са данни за настройка/справка са:

- [**V902PSMasterData** – Само за Project Service, версия 3.x](https://go.microsoft.com/fwlink/?linkid=2026540&clcid=0x409)

- [**V902FSMasterData** – Само за Field Service, версия 8.x](https://go.microsoft.com/fwlink/?linkid=2026536&clcid=0x409)

- [**V902FPSMasterData** – Field Service 8.x и Project Service 3.x](https://go.microsoft.com/fwlink/?linkid=2026041&clcid=0x409)

Най-новият пакет с **демонстрационни** данни е:

 - [**FPSDemoData** – Field Service 8.x и Project Service 3.x](https://aka.ms/fpsdemodatapackage)

   Инструкциите за инсталация се различават малко при създаването и конфигурирането на секция от потребителите, но останалото е същото като в предишната [**публикация в блог**](https://aka.ms/fpsdemodatablog). Този пакет включва ограничен набор от демонстрационни данни и инсталирането му отнема приблизително 3 часа.

Тези пакети с примерни данни са достъпни само на английски.

> [!IMPORTANT]
> **Няма възможност за деинсталиране на примерните данни.** Трябва да инсталирате тези пакети само на системи за демонстрация, оценяване, обучение или тест. Обърнете внимание също, инсталирането на индивидуален пакет и след това инсталирането на друг индивидуален пакет не се поддържа. (С други думи не можете да инсталирате **FSMasterData** и след това **PSMasterData** или обратно.) Ако считате, че ще имате нужда от примерни данни и за двете приложения в някакъв момент в бъдещето, трябва да инсталирате пакета **v902FPSMasterData**.

Когато инсталирате някой от пакетите с примерни данни, процесът на инсталация изпълнява следните действия:

- Създава или задава параметри по подразбиране за използване на Project Service, Field Service или и двете приложения (ако е приложимо).

- Импортира примерни данни за приложенията, като налични ресурси, специфични за приложение роли, продажби и ценови листи за разходи, организационни единици, записи за обработка на продажби и други обекти, за да демонстрира ключови възможности.  

С пакета с **демонстрационни данни** получавате горните и допълнителни данни за транзакция, като работни поръчки и проекти.

Чудите се какви възможности можете да демонстрирате чрез примерните данни? Вижте фиктивния сценарий за Fabrikam Robotics в [Технически забележки](#technical-notes).

Ако имате въпроси относно инсталирането на тези пакети с примерни данни, [ни изпратите имейл на адрес fpsdemodata@microsoft.com.](mailto:fpsdemodata@microsoft.com).

## <a name="requirements"></a>Изисквания

Протоколът за инсталация приема следното за целевия ви екземпляр (организация):

- Основният език е английски и основната валута е щатски долар (USD, $).

- Организацията няма все още данни на Project Service и Field Service или има само основни данни по подразбиране, които се предоставят с всяка нова организация.

- Правилната версия на бизнес приложението вече е инсталирана:
       
    - **For FPSDemoData или v902FPSMasterData:** Организацията има инсталирани Field Service, версия 8.x и Project Service, версия 3.x.

    - **For v902PSMasterData:** Организацията има инсталирано приложението Project Service, версия 3.x.

    - **For v902FSMasterData:** Организацията има инсталирано приложението Field Service, версия 8.x.

> [!NOTE]
> Ако трябва да инсталирате примерни данни върху съществуващи пробни или демонстрационни среди на Project Service и Field Service, които вече имат данни (не се препоръчва), ще трябва да преустановите предварителните проверки за защита, които се изпълняват от програмата за инсталация. За повече информация вижте техническите забележки по-долу.

## <a name="prepare-for-installation"></a>Подготовка за инсталация

Ще трябва да изпълните програмата за инсталация със скорошна версия на Windows (за предпочитане е Windows 10).

Трябва да планирате компютърът да остане свързан към мрежа и инсталацията да се изпълнява до **1 час** за **данни за настройка/справка**. (Обикновено инсталацията отнема около 30 минути за **FPSMasterData** , което включва примерни данни за двете приложения.) За **FPSDemoData** инсталацията ще отнеме около **3 часа**.

Функцията за скрийнсейвър на компютъра трябва да е изключена. В противен случай идентификационните данни за сесията за инсталацията може да бъдат загубени, когато скрийнсейвърът се включи (освен ако не държите сесията активна през цялото време).

> [!div class="mx-imgBorder"]
> ![Екранна снимка на настройките на скрийнсейвър при изключен скрийнсейвър](media/sample-data-1.png)

## <a name="download-and-unpack"></a>Изтегляне и разопаковане

Програмата за инсталиране на примерни данни на Project Service и Field Service се разпространява като самоизвличащ се изпълним файл. Имената на файловете може да се различават в зависимост от пакета с примерни данни, но иначе стъпките са еднакви без значение кой пакет инсталирате.

След като изтеглите пакета, изпълнете .exe файла и след това приемете условията, за да разопаковате компресирания zip файл. Трябва да извлечете съдържанието от този файл в папка на компютъра.

В зависимост от операционната система и настройките за защита трябва да изпълните следните стъпки след разопаковане на zip файла:

1. Намерете и щракнете с десния бутон върху файла **FPSDemoData.dll** в папката **v902FPSMasterData** / **PackageDeployer_FPSDemoData**.

2. Изберете **Деблокиране**.

3. Изберете **Прилагане**.

4. Изберете **OK**.


## <a name="create-or-configure-users"></a>Създаване или конфигуриране на потребители

Пакетът **FPSDemoData** изисква шестима потребители, докато пакетът **FPSMasterData** изисква един потребител. Вижте правилния за вашия пакет с примерни данни.

## <a name="create-or-configure-users---setupreference-data-packages"></a>Създаване или конфигуриране на потребители – пакети с данни за настройка/справка

Пакетът **FPSMasterData** е предназначен за инсталиране с един потребител на име Спенсър Лоу с настройките, описани тук. За да инсталирате пакета правилно, трябва да създадете (или преименувате временно) потребители във вашата среда, за да отговарят на пристигащата конфигурация на примерни данни.

За да създадете или конфигурирате потребители, отидете на **Настройки** > **Защита** > **Потребители** и направете следното:

1. Задайте UserFullname="Spencer Low" с потребителско име "spencerl" ( **малки букви** ) за ролите на мениджър на проект и оперативен мениджър.

2. Изберете потребителя **Спенсър Лоу** ,, след което изберете **Управление на роли**. Намерете и изберете ролята **Системен администратор** и след това изберете **OK** , за да предоставите пълни администраторски права на Спенсър Лоу. Тази стъпка е необходима, за да се гарантира, че примерните записи са създадени с правилната собственост на потребител и съответно попълват изгледите правилно.

3. От изтегления пакет трябва да актуализирате файла за съпоставяне на данни с имейл адресите на потребителския контекст по подразбиране. За да направите това, отворете **PkgFolder** и след това намерете и отворете файла **ImportUserMapFile.xml** в Notepad (или Visual Studio или друг XML редактор). Задайте полето **DefaultUserToMapTo=** на имейл адреса на потребителя Спенсър Лоу.

4. Ако не използвате Спенсър Лоу с потребителско име **spencerl** , трябва да актуализирате допълнителен файл. Отворете файла **DemoDataPreImportConfig.xml** и след това намерете етикета **userstocreateandconfigure**. Актуализирайте етикета **\<login\>** с потребителското име на вашия потребител Спенсър Лоу. За допълнителни подробности вижте [Технически забележки](#technical-notes).

## <a name="create-or-configure-users---demo-data-package"></a>Създаване или конфигуриране на потребители – пакет с демонстрационни данни

Пакетът с демонстрационни данни изисква шестима потребители. За да се инсталира пакетът правилно, направете следното:

 1. Създаване или преименувате временно съществуващите потребители, за да съответстват на конфигурацията на входящите примерни данни, като отидете на **Настройки** > **Защита** > **Потребители**.
 
    Тези роли са необходими само за базирани на лица демонстрации.  
    - Пълно потребителско име = „David So“ като техник на Field Service   
    - Пълно потребителско име = „Jamie Reding“ като диспечер на Customer Service и Field Service   
    - Пълно потребителско име = „Molly Clark“ като мениджър на клиенти   
    - Пълно потребителско име = „Spencer Low“ като мениджър проекти и оперативен мениджър  
    - Пълно потребителско име = „Veronica Quek“ като член на екипа   
    - Пълно потребителско име = „William Contoso“
  
2. За целите на импортиране на демонстрационни данни присвоете шестимата потребители над ролята на администратор, така че примерните записи да се импортират правилно. 

3. Отворете **PkgFolder** и след това намерете и отворете **ImportUserMapFile.xml**. Актуализирайте полетата **Ново=** на имейл адресите на съответните потребители в системата ви.

   > [!div class="mx-imgBorder"]
   > ![Екранна снимка на UserMapFile](media/sample-data-7.png)

4. Ако вашият потребител с пълно име „Spencer Low“ има различен от **„spencerl“** ИД, трябва да актуализирате допълнителен файл. Отворете **DemoDataPreImportConfig.xml** и намерете етикета **userstocreateandconfigure**. Актуализирайте етикета **\<login\>** с loginId (чувствителен на малки и главни букви). 

5. Календарът на първия потребител (в етикета **userstocreateandconfigure** ) се използва за попълване на работните часове за всички налични ресурси при импортиране на демонстрационни данни. Навигирайте до **Настройки** > **Защита** > **Потребители** , намерете своя потребител „Spencer Low“ и отворете опцията „Работни часове“. Редактирайте съществуващите работни часове, като изберете опцията **Целият периодичен седмичен график от начало до край**. Уверете се, че **Работните часове са зададени на 8:00 – 17:00 (9 часа), понеделник до петък и с часова зона, зададена на тихоокеанско време (САЩ и Канада)**. Това е необходимо, за да се гарантира, че таблата на проекта и графика се показват, както се очаква.

**Препоръка:** Помислете за създаване на резервно копие на вашата организация сега, в случай че трябва да се върнете към началната си точка, ако нещо се обърка по време на инсталирането на примерни данни. За повече информация вижте [Архивиране и възстановяване на екземпляри](https://docs.microsoft.com/dynamics365/customer-engagement/admin/backup-restore-instances).

## <a name="run-the-package-deployer"></a>Стартиране на Package Deployer

1. Намерете и изпълнете **PackageDeployer.exe** в папката **v902FPSMasterData** ИЛИ **PackageDeployer_FPSDemoData**.

2. Приемете правилата и условията.

3. На следващия прозорец:

   а. Изберете тип внедряване **Office 365**.

   б. Използвайте потребителя и паролата на системния администратор, конфигурирани в „Създаване или конфигуриране на потребители“ („Спенсър Лоу“ с потребителско име „spencerl“).

   в. Уверете се, че сте избрали **Показване на списък с достъпни организации**.

      > [!div class="mx-imgBorder"]
      > ![Екранна снимка на прозореца Package Deployer с избран „Показване на списък на налични организации“](media/sample-data-2.png)

4. Изберете организацията, където искате да инсталирате примерните данни.

5. Изберете **Напред** , докато видите диалоговия прозорец **Настройка на демонстрационни данни**.

   > [!div class="mx-imgBorder"]
   > ![Екранна снимка на прозореца за състояние на програмата за инсталиране на демонстрационни данни](media/sample-data-3.png)

6. Преди да продължите, обърнете внимание, че инсталирането на примерни данни може да отнеме до един час (обикновено ~ 10 минути). Трябва да се уверете, че компютърът остава работещ и свързан към мрежата по време на инсталационния процес и че вашата сесия остава активна.   

7. Когато сте готови, щракнете върху **Напред** , за да започнете процеса на инсталиране на примерни данни. След зареждането на примерните данни, щракнете върху **Готово**.

## <a name="verify-the-sample-data-installation"></a>Проверка на инсталацията на примерни данни

За всеки случай проверете дали броят записи и типове обекти, изброени във фиктивния сценарий за Fabrikam Robotics, изглеждат, както се очаква.

След пълното зареждане на примерни данни влезте като потребителя Спенсър Лоу и потвърдете следното:

- Ако приложението Project Service е инсталирано, отидете на **Project Service** > **Настройки** > **Ценови листи**. Потвърдете, че ставките за фактуриране и разходи съществуват с подходящата валута за всяка държава/регион в набора от данни.

- Ако приложението Project Service е инсталирано, отидете на **Universal Resource Scheduling** > **Настройки** > **Организационни единици**. Проверете дали ценовата листа за разходи с правилната валута е била свързана с всяка организационна единица (включително записите за град). Ако нещо липсва, намерете и свържете правилната ценова листа за разходи.

- Ако приложението Field Service е инсталирано, отидете на **Project Service** > **Настройки** > **Ценови листи**. Проверете дали ставките за фактуриране и разходи съществуват. Отидете на **Field Service** > **Настройки** > **Ценови листи** и проверете дали ставките за фактуриране и разходи съществуват с правилната валута за всяка държава/регион в набора от данни.

  > [!div class="mx-imgBorder"]
  > ![Екранна снимка на активни ценови листи](media/sample-data-4.png)

  > [!div class="mx-imgBorder"]
  > ![Екранна снимка на активни организационни единици](media/sample-data-5.png)

## <a name="technical-notes"></a>Технически забележки

Вижте по-долу за повече технически подробности относно инсталирането на тези данни.

### <a name="installing-sample-data-on-top-of-existing-data-not-recommended"></a>Инсталиране на примерни данни върху съществуващи данни (не се препоръчва)

Ако трябва да инсталирате примерни данни върху съществуващи пробни или демонстрационни среди на Field Service и Project Service, които вече имат данни, ще трябва да преустановите предварителните проверки за защита, които се изпълняват от програмата за инсталация.

За да направите това, отидете в папката **PkgFolder** , за да намерите и отворите файла **DemoDataPreImportConfig.xml** с Notepad (или друг XML редактор).

Намерете следната стойност и след това променете настройката от „true” на „false”:

```alias
<TerminateOnPreCheckFailure>true</TerminateOnPreCheckFailure>
```

Тази промяна води до това програмата за инсталиране да заобиколи някои важни проверки за защита, включително:

- Проверка, че няма повече от един активен запис **Организационна единица** и преименуването му на **Fabrikam US**.

- Проверка, ,че няма повече от един активен запис **Работен шаблон**.

- Проверка, че няма повече от един активен запис **Параметър на проект** и преименуването на този запис на **Параметри**.

### <a name="configuration-components"></a>Компоненти на конфигурация

Има редица други компоненти на конфигурация в този файл за конфигурация преди импортиране. За технически потребители някои от тях включват:

- **\<RequiredSolutions\>** указва инсталации на предпоставени решения и техните номера на версиите.

- **\<InstallSampleData\>** контролира дали стандартните примерни данни за приложенията са инсталирани.

    - false – пропуска инсталация на тези вграден данни (които могат да бъдат премахнати)

    - true – инсталира вградените данни едновременно с инсталирането на примерни данни за FS и PSA

- **\<PreImportDataCollection\>** указва карти на данни на фиксиран файл и свързаните записи да бъдат импортирани преди инсталирането на основните примерни данни.

- **\<EntitiesToEnableScheduling\>** указва кои обекти да бъдат разрешени за резервация в Microsoft Dynamics Scheduling (известно също като Universal Resource Scheduling).

- **\<UsersToCreateAndConfigure\>** указва налични ресурси, които ще бъдат създадени (ако вече не съществуват), преди да се изпълни импортирането на примерни данни. Обърнете внимание, че наличният ресурс на примерни данни на изходната система съответства на записите на наличен ресурс на целевата система в FullName и входа за всеки ресурс. По тази причина НЕ е възможно да промените имената в този предконфигурационен файл, освен ако не импортирате примерните данни първо в целевата система, като използвате тези имена, след което преименувате наличните ресурси на желания ви набор от имена със записите на активирания потребител, след което експортирате данните отново за импортиране в системата ви на последна дестинация (като съответно актуализирате старите и новите записи на **ImportUserMapFile.xml** ).

- **\<PluginsToDisable\>** указва много дискретни добавки за елемент на ред, които трябва да бъдат забранени по време на импортирането на примерни данни и след това отново разрешени.

### <a name="fabrikam-robotics-fictitious-scenario"></a>Фиктивен сценарий за Fabrikam Robotics

Пакетите с примерни данни за справка за Project Service и Field Service инсталират **решението Fabrikam Manufacturing Master Data (v3.0.0.0)** заедно с приблизително 4000 записа и приблизително 40 различни обекта. Отделните пакети с данни за Field Service или Project Service съдържат поднабор от примерни данни на **v902FPSMasterData** за това приложение. Пакетът с **Демонстрационни данни** инсталира **решението Fabrikam Manufacturing Demo Data (v3.0.0.7)** с приблизително 22 000 записа между 148 обекта.

Фиктивната фирма Fabrikam Robotics е производител на роботи за линия за сглобяване на електронни устройства и е позната с качеството на продуктите си, иновация и солидно обслужване на клиенти, включително планиране на инсталации, прилагане и услуги за текуща поддръжка. Главният офис на Fabrikam е в Съединените щати (Fabrikam US) и има базирани на проект операции по обслужване във Франция, Индия, Обединеното кралство и Швейцария.

Операциите по обслужване на място са центрирани в Съединените щати, като в най-голямата си част са в областта на Сиатъл. Фирмата е фокусирана върху използването на свързаността на интернет на нещата (IoT) за проследяване на производителността на клиентски актив и доставка на все по-проактивни услуги на място.

По-долу е представен общ преглед на високо ниво на примерните данни:

- Общи елементи на примерни данни (включени за двете приложения)

    - 1 потребител

    - 71 акаунта

    - 137 контакта

    - Различни типове транзакции и категории

    - 50 продукта с 1 ценова листа на продукт

    - 14 ценови листи/листи за разходи

    - 31 характеристики (умения на реусрс) в 2 модела на ранг с 3 нива (стойности на ранг)

- Project Service

    - 8 организационни единици

    - 6 специфични за роля нива на използване

    - Повече от 2800 спецификации тип роля-цена

- Field Service

    - 4 територии

    - 5 типа работни поръчки

    - 22 клиентски активи

    - 9 типове инциденти с диапазон на характеристиките на свързаните ресурси (9), услуги (13) и задачи за услуга (13)
   
Пакетът с **Демонстрационни данни** инсталира около 179 работни поръчки, 12 проекта и свързаните данни за транзакция. 

### <a name="change-the-work-hours-for-sample-resources"></a>Промяна на работните часове за примерни ресурси

По подразбиране всички налични ресурси имат календар с 24 работни часа.

Ако имате нужда да промените работните часове за примерни налични ресурси, отидете на **Universal Resource Scheduling** > **Планиране** > **Ресурси**.

Изберете потребител (например Спенсър Лоу) и променете работните часове на Спенсър на часовете, които искате да приложите към няколко потребителя. Отидете на **Universal Resource Scheduling** > **Настройки** > **Шаблони за работни часове** и редактирайте записа **Работен шаблон по подразбиране**. В полето **Ресурс на шаблон** изберете потребител с работни часове, които искате да приложите за други ресурси. Отидете на **Universal Resource Scheduling** > **Планиране** > **Ресурси** > **Активни налични ресурси**. Изберете ресурсите, които искате да промените и след това изберете **Задаване на календар**. В падащия списък **Работен шаблон** изберете шаблона **Работни часове по подразбиране** или друг шаблон с правилния ресурс за шаблон. Когато отидете на таблото за планиране, би трябвало да видите, че ресурсът вече има актуализирани работни часове.

> [!div class="mx-imgBorder"]
> ![Екранна снимка на активните налични ресурси](media/sample-data-6.png)