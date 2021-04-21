---
title: Какво е новото от април 2021 г. – Project Operations за сценарии, базирани на ресурси/неналичност
description: Тази тема предоставя информация за актуализациите на качеството, налични в изданието на Project Operations от април 2021 г. за ресурс/неналичност сценарии.
author: sigitac
manager: tfehr
ms.date: 04/05/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 359d39898ed60c7253b122cb884465fbd9605e0c
ms.sourcegitcommit: 8ff9fe396db6dec581c21cd6bb9acc2691c815b0
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/07/2021
ms.locfileid: "5867980"
---
# <a name="whats-new-april-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>Какво е новото от април 2021 г. – Project Operations за сценарии, базирани на ресурси/неналичност

_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_

Тази тема се отнася за следните компоненти и версии на Dynamics 365 Project Operations:

- Project Operations в среда на Dataverse, версия 4.9.0.221
- Управление на проекти и счетоводство в среда на Dynamics 365 Finance, версия 10.0.17

## <a name="features-included-in-this-release"></a>Функции, включени в тази версия

Следните функции са включени в това издание:

- Нескладови материали за проекти. Основните възможности включват:
  - Оценка и ценообразуване на складовите материали по време на цикъла на продажбите на даден проект. За повече информация вижте [Настройване на размер на разход и продажби за продукти от каталог – олекотено](../pro/pricing-costing/set-up-cost-sales-rates-catalog-products.md).
  - Проследяване на използването на складови материали по време на изпълнението на проекта. За повече информация вижте [Записване на използването на материали по проекти и проектни задачи](../material/material-usage-log.md).
  - Фактуриране на използвани не складирани материални разходи. За повече информация вижте [Управление на натрупване на фактуриране](../proforma-invoicing/manage-billing-backlog.md).
- Тактуване на базата на задачи: Добавена е възможност за свързване на проектни задачи с редове на договора за проект, като по този начин ги подлага на същия метод на фактуриране, честота на фактурите и клиенти като тези по договора. Тази асоциация осигурява точно фактуриране, счетоводство, оценка на приходите и признание, за да работи в съответствие с тази настройка по проектни задачи.
- Нови API в Dynamics 365 Dataverse позволяват създаване, актуализиране и изтриване на операции с **Обекти за планиране**. За повече информация вижте [Използвайте API на графика, за да извършвате операции с обекти за планиране](../project-management/schedule-api-preview.md).

## <a name="quality-updates"></a>Актуализации на качеството

### <a name="project-operations-in-dynamics-365-dataverse"></a>Project Operations в Dynamics 365 Dataverse

| **Област с функции** | **Номер за справка** | **Актуализация на качеството** |
| --- | --- | --- |
| Фактуриране и ценообразуване | 2124532 | Бутонът **Коригиране на фактура** се показва на проформа фактура, когато сумата на фиксатора или приложената сума на фиксатора присъства в оригиналната фактура. Бутонът се показва само за среди с Finance версия 10.0.19 или по-нова. |
| Фактуриране и ценообразуване | 2224568 | Добавена логика за активиране на персонализации, които включват извикване на приставката за потвърждение на фактура. |
| Фактуриране и ценообразуване | 2101098 | Подобрена логика на полетата по подразбиране за проформа фактура: **Адрес за фактуриране**, **Име за фактуриране** и **Условия за плащане** сега по подразбиране от съответния клиентски запис на договор за проект. |
| Фактуриране и ценообразуване | 2021413 | Актуализирани са полетата **Реална цена** и **Продажби** на обекта **Задача** за включване на стойности на продажби от нефактурирани и фактурирани разходи за задачи. |
| Фактуриране и ценообразуване | 2182110 | При копиране на договор за проект идентификационният номер на договора се регенерира в договора за проект на дестинация, за да се гарантира, че е уникален. |
| Управление на възможности | 2186741 | Добавени са валидации, за да се гарантира, че полетата **Произход** и **Тип транзакция** не могат да бъдат актуализирани за подробности за съществуващите оферти. |
| Управление на възможности | 2191353 | Важни етапи не трябва да се създават по времева и съществена договорна линия. |
| Управление на възможности | 2216956 | Отстранени проблеми с **Актуализирайте цените**. |
| Планиране и проследяване | 2182979 | Подобрена е функцията за копиране на проект, за да се гарантира, че редовете за оценка на разходите се копират от оригиналния проект. |
| Планиране и проследяване | 2184144 | Подобрена е функцията за копиране на проект, за да се гарантира, че името на позиция на ресурс се копира от оригиналния проект. |
| Планиране и проследяване | 2184799 | Копиране на проект: Засилен контрол, за да се гарантира, че очакваната начална дата не може да бъде променена, докато копирането е в ход. |
| Планиране и проследяване | 2185134 | Копие на проекта: Очакваната начална дата на проекта за дестинация е зададена на днешната дата. |
| Планиране и проследяване | 2196373 | Копие на проекта: Уверете се, че записите на мениджъра на проекта и членовете на екипа не се дублират в екипа на проекта. |
| Планиране и проследяване | 2211833 | Копиране на проект: Присвояването на ресурси се копира от проектната задача-източник в целевия проект. |
| Планиране и проследяване | 2186541 | Поправени проблеми в мрежата **Оценки** при групиране по ресурси. |
| Планиране и проследяване | 2166906 | Категорията на транзакцията от задача трябва да бъде копирана в обекта **Възлагане на ресурси**. |
| Управление на ресурс | 2125362 | Отстранени са проблеми със създаването на общ член на екипа, използващ метод на разпределение, базиран на часове. |
| Време и разход | 2113603 | Коригиран проблем, свързан с персонализирането, с премахване на атрибути от страницата **Въвеждане на време**. Сега системата проверява дали атрибутът съществува на страницата, преди да осъществи достъп до тях чрез скрипт. |
| Време и разход | 2204377 | Копираните разписания трябва да се показват автоматично, когато изберете **Копиране на седмица** по време на въвеждане на време. |
| Време и разход | 2209059 | Полето **Състояние** може да се редактира за времеви записи на Dynamics 365 Field Service. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Управление на проекти и счетоводство в Dynamics 365 Finance

| **Област с функции** | **Номер за справка** | **Актуализация на качеството** |
| --- | --- | --- |
| Управление на проекти и счетоводство | [491941](https://fix.lcs.dynamics.com/Issue/Details/?bugId=491941) | Елиминирането на обратната оценка не работи в **Периодични**.  |
| Управление на проекти и счетоводство | [509773](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509773) | Функцията **Счетоводна корекция** създава проблем с акаунти на счетоводната книга, които имат избрани **Не позволявайте ръчно въвеждане**. |
| Управление на проекти и счетоводство | [510728](https://fix.lcs.dynamics.com/Issue/Details/?bugId=5109728) | Добавена е бизнес логика за обработка на фактури за корекция, включително сума за фиксиране или приложена сума за фиксиране. |
| Управление на проекти и счетоводство | [514364](https://fix.lcs.dynamics.com/Issue/Details/?bugId=514364) | Публикуването на стойността на WIP продажбите при фактуриране на междуфирмен проект избира неочаквана сметка. |
| Управление на проекти и счетоводство | [521807](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521807) | Когато работите с фиксатори в Project Operations, промяната на проекта по подразбиране по договора след фактуриране на предплащанията води до проблеми с входящи удръжки. |
| Управление на проекти и счетоводство | [527319](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527319) | В Project Operations премахването на проект от договор трябва да нулира проекта по подразбиране на договора, ако е необходимо. |
| Управление на проекти и счетоводство | [528212](https://fix.lcs.dynamics.com/Issue/Details/?bugId=528212) | В Project Operations грешните разходни линии се показват в списъка **Добавяне на ред** във вътрешнофирмената фактура. |
| Управление на проекти и счетоводство | [543968](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543968) | В Project Operations страницата **Договор за покупка** не се вижда във Финансовите юридически лица, които са интегрирани с Project Operations. |
| Управление на проекти и счетоводство | [545878](https://fix.lcs.dynamics.com/Issue/Details/?bugId=545878) | Заради интеграционна грешка на Dataverse, не можете да конвертирате оферта в спечелена в Project Operations. |
| Управление на проекти и счетоводство | [547440](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547440) | **ProjCDSProjectContractEntity** може да зададе адреса на фактура на източника на финансиране от различен клиент.  |
| Управление на проекти и счетоводство | [557376](https://fix.lcs.dynamics.com/Issue/Details/?bugId=557376) | В Project Operations не се избират измерения, когато създавате фактура за осчетоводяване за транзакция. |
| Пътуване и разход | [441256](https://fix.lcs.dynamics.com/Issue/Details/?bugId=441256) | Авансовото салдо в брой не се актуализира за отчет за разходите, ако е одобрено и осчетоводено ред по ред. |
| Пътуване и разход | [482041](https://fix.lcs.dynamics.com/Issue/Details/?bugId=482041) | Данъците за подробни отчети за вътрешнофирмени разходи не се изчисляват правилно. |
| Пътуване и разход | [483469](https://fix.lcs.dynamics.com/Issue/Details/?bugId=483469) | Допълнителни полета, свързани с проекти, се показват на преиздадената страница **Отчети за вътрешнофирмени разходи**. |
| Пътуване и разход | [486592](https://fix.lcs.dynamics.com/Issue/Details/?bugId=486592) | Появява се неправилно съобщение за грешка в заглавните разписки на отчети за разходите. |
| Пътуване и разход | [487971](https://fix.lcs.dynamics.com/Issue/Details/?bugId=487971) | Отчет за разходите е осчетоводен неправилно в междуфирмен сценарий, ако данъкът върху продажбите е осчетоводен в юридическото лице на местоназначението. |
| Пътуване и разход | [505696](https://fix.lcs.dynamics.com/Issue/Details/?bugId=505696) | Датите за подаване на отчети не се отпечатват в одобрени отчети за разходите. |
| Пътуване и разход | [508726](https://fix.lcs.dynamics.com/Issue/Details/?bugId=508726) | Полетата **Дата на одобрение** и **Дата на отхвърляне** не се попълват след одобряване на разход. |
| Пътуване и разход | [509913](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509913) | Изискване за пътуване, създадено за един работник, може да се използва за отчета за разходите на друг работник. |
| Пътуване и разход | [518186](https://fix.lcs.dynamics.com/Issue/Details/?bugId=518186) | Категориите на разходите се заключват при добавяне на нов ред за разходи. |
| Пътуване и разход | [520914](https://fix.lcs.dynamics.com/Issue/Details/?bugId=520914) | Посочването на вече разделени редове на отчета за разходите води до непълно осчетоводяване на ваучера „Сметки за плащане\Главна книга“ и прекъсва Account Explorer Source Explorer, защото **TRVEXPTRANS.SOURCEDOCUMENTLINE** се дублира. |
| Пътуване и разход | [521943](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521943) | Политиката за заявки за пътуване не работи според очакванията. |
| Пътуване и разход | [522567](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522567) | Името на сметката на доставчика не се показва при публикувани транзакции на проекти за отчети за разходи. |
| Пътуване и разход | [525106](https://fix.lcs.dynamics.com/Issue/Details/?bugId=525106) | В Project Operations не можете да одобрите време със задача за междуфирмен проект. |
| Пътуване и разход | [526336](https://fix.lcs.dynamics.com/Issue/Details/?bugId=526336) | Категорията за връщане на авансови плащания не актуализира салдата на авансовите плащания при публикуване. |
| Пътуване и разход | [527218](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527218) | Продажната цена се изчислява неправилно в отчети за разходите, които са създадени в чуждестранна валута с помощта на транзакции с вносни кредитни карти и са свързани с проект. |
| Пътуване и разход | [542927](https://fix.lcs.dynamics.com/Issue/Details/?bugId=542927) | Върнат е обратно обектът на данни **TrvRequisitionLine** и свързаният уникален индекс. |
| Пътуване и разход | [543239](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543239) | Добавена е апаратура към генерирането на **SOURCEDOCUMENTLINE**. |
| Пътуване и разход | [544323](https://fix.lcs.dynamics.com/Issue/Details/?bugId=544323) | Неправилният журнал на вторична книга се показва в междуфирмен сценарий, ако данъкът върху продажбите е осчетоводен в юридическото лице на местоназначението. |
| Пътуване и разход | [546877](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546877) | В Project Operations прогнозните разходи не се изтриват от Finance, когато се изтриват от Dataverse. |
| Пътуване и разход | [550575](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550575) | Когато категорията на разходите е непроектна категория, финансовите измерения, избрани на страницата **Разход** не се копират в отчета за разходите. |