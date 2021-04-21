---
title: Какво е ново и променено в Project Operations от март 2021 г. за сценарии, базирани на наличност/производство
description: Тази тема предоставя информация за актуализациите на качеството, налични в изданието на Project Operations от март 2021 г. за складови/производствени сценарии.
author: andchoi
manager: tfehr
ms.date: 03/22/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: andchoi
ms.openlocfilehash: 804b5d1cc3392349fb6bcc81a91d69d0d9dc51da
ms.sourcegitcommit: 386921f44f1e9a8a828b140206d52945de07aee7
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/22/2021
ms.locfileid: "5701909"
---
# <a name="whats-new-or-changed-in-project-operations-march-2021-for-stockedproduction-based-scenarios"></a>Какво е ново и променено в Project Operations от март 2021 г. за сценарии, базирани на наличност/производство

_**Приложимо за:** Project Operations за сценарии, базирани на наличност/производство_

Тази тема се отнася за следните компоненти и версии на Dynamics 365 Project Operations:

- Управление на проекти и счетоводство в среда на Dynamics 365 Finance, версия 10.0.17

## <a name="features-included-in-this-release"></a>Функции, включени в тази версия
Следните функции са включени в това издание:

  - [Производителност на предложение за фактуриране по проект](../project-invoice-proposal-performance.md)
 
### <a name="quality-updates"></a>Актуализации на качеството

| Област с функции                        | Номер за справка | Актуализация на качеството                                                                                                                                                                                                                                                   |
|-------------------------------------|------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Управление на проекти и счетоводство | [420064](https://fix.lcs.dynamics.com/Issue/Details/?bugId=420064) | Отрицателните публикувани транзакции на проекти не се актуализират след преизчисляване на инвентара.                                                                                                                      |
| Управление на проекти и счетоводство | [438692](https://fix.lcs.dynamics.com/Issue/Details/?bugId=438692) | Изтриването на източник на финансиране трябва да е възможно, ако за източника на финансиране няма разпределена транзакция или фактура.                                                                                                           |
| Управление на проекти и счетоводство | [439470](https://fix.lcs.dynamics.com/Issue/Details/?bugId=439470) | Действителните прогнозни транзакции не показват транзакции на разходи и позиции от предходния период.                                                                                                       |
| Управление на проекти и счетоводство | [452710](https://fix.lcs.dynamics.com/Issue/Details/?bugId=452710) | Стойността на описанието на счетоводната книга е неправилна за опаковъчния фиш на изискванията на проектната позиция.                                                                                                              |
| Управление на проекти и счетоводство | [455602](https://fix.lcs.dynamics.com/Issue/Details/?bugId=455602) | Когато се публикуват списания за даден проект, финансовите измерения не се избират от служителя и елемента във ваучера.                                                                               |
| Управление на проекти и счетоводство | [472988](https://fix.lcs.dynamics.com/Issue/Details/?bugId=472988) | Когато нетната сума на реда се актуализира в общата фактура за проекта, сумата на продажбите се попълва с коригираната сума в осчетоводената транзакция.                                                                               |
| Управление на проекти и счетоводство | [477969](https://fix.lcs.dynamics.com/Issue/Details/?bugId=477969) | Фактурата не избира препратка към идентификатора на проекта при преглед на редовете на фактурите на доставчика на страницата **Плащане на фактурите на доставчика при плащане**.                                                                                                   |
| Управление на проекти и счетоводство | [478667](https://fix.lcs.dynamics.com/Issue/Details/?bugId=478667) | Сумата на договора е неправилна на страницата **По сметка** за проект с фиксирана цена с множество източници на финансиране.                                                                                                  |
| Управление на проекти и счетоводство | [481443](https://fix.lcs.dynamics.com/Issue/Details/?bugId=481443) | Натрупаните приходи по проект с фиксирана цена не се коригират дори след публикуване на елиминирането.                                                                                                                                |
| Управление на проекти и счетоводство | [483209](https://fix.lcs.dynamics.com/Issue/Details/?bugId=483209) | Статутът на акредитива не се актуализира, когато поръчка за продажба на проект се фактурира чрез предложение за фактура.                                                                                                  |
| Управление на проекти и счетоводство | [484274](https://fix.lcs.dynamics.com/Issue/Details/?bugId=484274) | Когато поръчката за покупка е фактурирана и фактурата съдържа категория на поръчка и артикул, клиентът ще получи грешна информация за акаунта.                                                                                              |
| Управление на проекти и счетоводство | [484817](https://fix.lcs.dynamics.com/Issue/Details/?bugId=484817) | Предложенията за фактури за проекти, които се генерират чрез повтарящи се пакетни задачи, имат дублирани транзакции с нулева сума.                                                                                                  |
| Управление на проекти и счетоводство | [486817](https://fix.lcs.dynamics.com/Issue/Details/?bugId=486817) | Премахнете проверката за ограничение на грешки, докато изпълнявате отчетите за печалби и загуби на проекта.                                                                                                                                  |
| Управление на проекти и счетоводство | [488076](https://fix.lcs.dynamics.com/Issue/Details/?bugId=488076) | Разходите, които се осчетоводяват чрез вътрешнофирмено презареждане, не показват запис на печалбата и загубата при използване на **Пощенски разходи** функционалност на **Код на проекта за време и материал**.                                                         |
| Управление на проекти и счетоводство | [488382](https://fix.lcs.dynamics.com/Issue/Details/?bugId=488382) | Филтърът **Състояние на фактурата** в публикувани транзакции на проекти за проекти с фиксирана цена не работи.                                                                                                   |
| Управление на проекти и счетоводство | [488783](https://fix.lcs.dynamics.com/Issue/Details/?bugId=488783) | Записите в разписанието се дублират поради дублирани записи на делегат.                                                                                                                                           |
| Управление на проекти и счетоводство | [491941](https://fix.lcs.dynamics.com/Issue/Details/?bugId=491941) | Елиминирането на обратната оценка не работи в **Периодични**.                                                                                                                                                 |
| Управление на проекти и счетоводство | [498010](https://fix.lcs.dynamics.com/Issue/Details/?bugId=498010) | Не мога да избера правилните данни от опцията **Коригиране на транзакциите** в модула **Управление на проекти и счетоводство**, когато се добави допълнителен диапазон. Филтърът **Допълнителни** се игнорира.                      |
| Управление на проекти и счетоводство | [508494](https://fix.lcs.dynamics.com/Issue/Details/?bugId=508494) | След като запишете работа, не можете да нулирате състоянието на производствената поръчка.                                                                                                              |
| Управление на проекти и счетоводство | [509716](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509716) | Елементи с автоматичен резерв и възможност за обещание (CTP), идващи от проект, не се резервират.                                                                                                                      |
| Управление на проекти и счетоводство | [509773](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509773) | Функцията **Счетоводна корекция** създава проблем с акаунти на счетоводната книга, които имат избрани **Не позволявайте ръчно въвеждане**.                                                                     |
| Управление на проекти и счетоводство | [510079](https://fix.lcs.dynamics.com/Issue/Details/?bugId=510079) | Не трябва да се показва стойност в полето **Натрупани приходи – стойност на продажбите** за отчети за проекти, когато оценката е елиминирана.                                                                                 |
| Управление на проекти и счетоводство | [510607](https://fix.lcs.dynamics.com/Issue/Details/?bugId=510607) | Разходите и продажните цени са неправилни при корекция на проект с ценообразуване по роли.                                                                                                                        |
| Управление на проекти и счетоводство | [10728](https://fix.lcs.dynamics.com/Issue/Details/?bugId=10728) | В Project Operations фактурата за корекция на фиксатор не работи след частична корекция на фиксатора.                                                                                                                   |
| Управление на проекти и счетоводство | [510743](https://fix.lcs.dynamics.com/Issue/Details/?bugId=510743) | Опцията **Премахване на връзката** трябва да бъде активирана само ако анулирате вътрешнофирмена поръчка за покупка.                                                                                                                                          |
| Управление на проекти и счетоводство | [514364](https://fix.lcs.dynamics.com/Issue/Details/?bugId=514364) | Публикуването на стойността на WIP продажбите при фактуриране на междуфирмен проект избира неочаквана сметка.                                                                                                                  |
| Управление на проекти и счетоводство | [514432](https://fix.lcs.dynamics.com/Issue/Details/?bugId=514432) | Таксата от правилото за фактуриране не се преизчислява, когато предложението за фактура съдържа редове, избрани за кредитни бележки.                                                                                            |
| Управление на проекти и счетоводство | [515820](https://fix.lcs.dynamics.com/Issue/Details/?bugId=515820) | Графикът на разходите на Federal Awards Inquiry показва сумите на получаването, когато предложение за фактура за проект не е стартирано за разходна транзакция.                                               |
| Управление на проекти и счетоводство | [516301](https://fix.lcs.dynamics.com/Issue/Details/?bugId=516301) | WIP-разходите са неправилни в изявлението на проекта за елемент на услуга, който има група на проект **Баланс**.                                                                                               |
| Управление на проекти и счетоводство | [516553](https://fix.lcs.dynamics.com/Issue/Details/?bugId=516553) | Не могат да се правят корекции на фактура със свободен текст, свързана с проект.                                                                                                                                                  |
| Управление на проекти и счетоводство | [517074](https://fix.lcs.dynamics.com/Issue/Details/?bugId=517074) | Когато коригирате транзакция по проект на продажна цена от нула, се създава нова коригирана транзакция със статус на фактура **Без такса**.                                                               |
| Управление на проекти и счетоводство | [517414](https://fix.lcs.dynamics.com/Issue/Details/?bugId=517414) | Има проблем при публикуване на корекция на проект, когато настройвате няколко реда едновременно.                                                                                                                               |
| Управление на проекти и счетоводство | [518001](https://fix.lcs.dynamics.com/Issue/Details/?bugId=518001) | Коригирането се осчетоводява с неправилна стойност на разходите, ако цената на себестойността на продукта и количеството на изискванията за артикули се променят след осчетоводяване на фиша за опаковане.                                                                   |
| Управление на проекти и счетоводство | [518092](https://fix.lcs.dynamics.com/Issue/Details/?bugId=518092) | Финансовите измерения на поръчката за директна доставка са неправилни и са заменени от финансови измерения на поръчката за продажба.                                                              |
| Управление на проекти и счетоводство | [518605](https://fix.lcs.dynamics.com/Issue/Details/?bugId=518605) | Редът на дневника за проект с отрицателно количество няма да актуализира прогнозата, когато количеството на прогнозата е нула.                                                                                        |
| Управление на проекти и счетоводство | [518657](https://fix.lcs.dynamics.com/Issue/Details/?bugId=518657) | Опит за импортиране на изисквания за артикули с помощта на Microsoft Excel води до грешка в датата на получаване.                                                                                                                                                    |
| Управление на проекти и счетоводство | [519200](https://fix.lcs.dynamics.com/Issue/Details/?bugId=519200) | Препратката към транзакцията на елемент на проект към транзакция на фактура на доставчик не се актуализира, когато фактурата е осчетоводена.                                                                                               |
| Управление на проекти и счетоводство | [519716](https://fix.lcs.dynamics.com/Issue/Details/?bugId=519716) | Когато публикувате предложение за фактура за проект, може да възникне следната грешка: „Транзакцията не балансира върху отчитащата валута при добавяне на приспадната авансова фактура“.                                                                    |
| Управление на проекти и счетоводство | [520268](https://fix.lcs.dynamics.com/Issue/Details/?bugId=520268) | Идентификаторът на проекта и името на проекта не се попълват в отчета **Задържане на плащането от доставчика**, ако използвате оформлението на проекта.                                                                                              |
| Управление на проекти и счетоводство | [520872](https://fix.lcs.dynamics.com/Issue/Details/?bugId=520872) | Когато проект се създава чрез обект на данни, приоритетът за сортиране на книгата е неправилен.                                                                                                                      |
| Управление на проекти и счетоводство | [521150](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521150) | Размерът на разходите е неправилен за осчетоводени транзакции на проекти, които се генерират въз основа на поръчка за покупка с повторно запазване на доставчика. Това води до генериране на неправилни стойности в отчети за проекти и контрол на разходите за проекти с фиксирана цена. |
| Управление на проекти и счетоводство | [521374](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521374) | Офертата за продажби на проект актуализира неправилно единичната цена, когато заглавката се актуализира.                                                                                                                    |
| Управление на проекти и счетоводство | [521807](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521807) | Когато работите с фиксатори в Project Operations, промяната на проекта по подразбиране по договора след фактуриране на предплащанията води до проблеми по-късно с входящи удръжки.                                                                        |
| Управление на проекти и счетоводство | [521857](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521857) | Актуализирането на датата на фактурата за фактурите на доставчика и продажните цени на проекти се промениха.                                                                                                                                  |
| Управление на проекти и счетоводство | [522897](https://fix.lcs.dynamics.com/Issue/Details/?bugId=520872) | Проблеми възникват, когато коригирате вътрешнофирмени транзакции, които имат различни обменни курсове.                                                                                                                |
| Управление на проекти и счетоводство | [522983](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522983) | Ангажираните разходи с изискване за артикул и поръчка за покупка са неправилни в процеса на фактуриране на поръчката за покупка с частично получаване на продукта и частично фактуриране.                                                |
| Управление на проекти и счетоводство | [523960](https://fix.lcs.dynamics.com/Issue/Details/?bugId=523960) | Неправилни стойности възникват, когато дадена оценка е обърната с обменния курс.                                                                                                                                             |
| Управление на проекти и счетоводство | [524242](https://fix.lcs.dynamics.com/Issue/Details/?bugId=524242) | Усилията в часове се изчистват автоматично в шаблона за структура на разбивка на работата на ниво задача.                                                                                                                         |
| Управление на проекти и счетоводство | [524911](https://fix.lcs.dynamics.com/Issue/Details/?bugId=524911) | Когато актуализирате състоянието на офертата на **Изгубена**, състоянието на всички стартирани оферти, които имат статус **Създадено** или **Изпратено**, също се актуализират до **Изгубена**.                 |
| Управление на проекти и счетоводство | [525182](https://fix.lcs.dynamics.com/Issue/Details/?bugId=525182) | Фактурата за продажби не се вижда в предложението за фактура, ако датата за доставка е в бъдеще.                                                                                                                  |
| Управление на проекти и счетоводство | [526180](https://fix.lcs.dynamics.com/Issue/Details/?bugId=526180) | Има промяна в бизнес логиката за обекта **Редове на дневника на проектни елементи**.                                                                                                                                          |
| Управление на проекти и счетоводство | [526522](https://fix.lcs.dynamics.com/Issue/Details/?bugId=526522) | Натрупаните приходи по вътрешнофирмена клиентска фактура не съответстват на работния лист и преоценката в чуждестранна валута.                                                                                 |
| Управление на проекти и счетоводство | [526650](https://fix.lcs.dynamics.com/Issue/Details/?bugId=526650) | Ангажираната цена се изчислява неправилно, след като напомнянето за доставка на реда за поръчка за проект е създадено от заявка за покупка на проект или от проект.                    |
| Управление на проекти и счетоводство | [526812](https://fix.lcs.dynamics.com/Issue/Details/?bugId=526812) | Когато коригирате проект, може да възникне следната грешка: „Не се актуализират финансови данни в инвентарната единица“.                                                                                                             |
| Управление на проекти и счетоводство | [527319](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527319) | В Project Operations премахването на проект от договор трябва да нулира проекта по подразбиране на договора, ако е необходимо.                                                                                       |
| Управление на проекти и счетоводство | [527945](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527945) | Продажната цена за разход в проект е грешна, когато се прилага данък за ползване.                                                                                                                                         |
| Управление на проекти и счетоводство | [528020](https://fix.lcs.dynamics.com/Issue/Details/?bugId=528020) | Грешното количество е осчетоводено в изискване за елемент на проект, когато редът за поръчка за проект се актуализира с допълнителни фактури.                                                                                                 |
| Управление на проекти и счетоводство | [528212](https://fix.lcs.dynamics.com/Issue/Details/?bugId=528212) | В Project Operations грешните разходни линии се показват в списъка **Добавяне на ред** във вътрешнофирмената фактура.                                                                                                |
| Управление на проекти и счетоводство | [529887](https://fix.lcs.dynamics.com/Issue/Details/?bugId=529887) | Полето **Сметка на доставчика** е празно на страницата **Транзакция, публикувана в проекта**, когато транзакциите се осчетоводяват с помощта на регистър на фактурите и одобрение на фактура.                                                                  |
| Управление на проекти и счетоводство | [530008](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530008) | Оригиналната дата на проекта не се отчита при корекция, която причинява грешка при **Използвайте датата на корекция като нова дата на проекта** е зададено на **Не**.                                                                     |
| Управление на проекти и счетоводство | [530241](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530241) | Продажната цена в общия дневник и дневник на разходите, свързани с проекта, се изчислява неправилно, когато валутата на сделката се различава от валутата на компанията.                                     |
| Управление на проекти и счетоводство | [530658](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530658) | Транзакциите за продажба не се показват във ваучери за частична фактура на поръчка за проект.                                                                                                                          |
| Управление на проекти и счетоводство | [530883](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530883) | Ролите на счетоводителя на проекта и ръководителя на проекта не могат да създават часови списания с настройка на групата за одобрение.                                                                                                         |
| Управление на проекти и счетоводство | [531974](https://fix.lcs.dynamics.com/Issue/Details/?bugId=531974) | Не може да се публикува отчет за разходи, който е импортиран с помощта Microsoft Excel.                                                                                                                                                              |
| Управление на проекти и счетоводство | [532106](https://fix.lcs.dynamics.com/Issue/Details/?bugId=532106) | Не може да създаде политика за разписание, защото полето **Съобщение** не е активно.                                                                                                                               |
| Управление на проекти и счетоводство | [532548](https://fix.lcs.dynamics.com/Issue/Details/?bugId=532548) | Има проблем, при който е разрешено обръщане на транзакции на доставчик в междуфирмени сценарии. Това се отнася както за фактури на доставчици, така и за отчети за разходите.                                                                                 |
| Управление на проекти и счетоводство | [532692](https://fix.lcs.dynamics.com/Issue/Details/?bugId=532692) | Разпределенията в одобрен работен лист не могат да бъдат нулирани.                                                                                                                                                     |
| Управление на проекти и счетоводство | [532843](https://fix.lcs.dynamics.com/Issue/Details/?bugId=532843) | Неправилни стойности възникват при обръщане на прогноза с обменния курс за часове за часове и статии.                                                                                                                  |
| Управление на проекти и счетоводство | [533426](https://fix.lcs.dynamics.com/Issue/Details/?bugId=533426) | Корекцията на проекта не актуализира правилно сумата на продажбите с непреки разходи.                                                                                                                              |
| Управление на проекти и счетоводство | [534597](https://fix.lcs.dynamics.com/Issue/Details/?bugId=534597) | Когато публикувате дневника за часовете, се появява следното съобщение за грешка: „Стойността на измерението не е посочена“.                                                                                                                                  |
| Управление на проекти и счетоводство | [535428](https://fix.lcs.dynamics.com/Issue/Details/?bugId=535428) | Проектният договор с различна валута не изчислява правилно счетоводната валута във ваучера.                                                                                              |
| Управление на проекти и счетоводство | [535652](https://fix.lcs.dynamics.com/Issue/Details/?bugId=535652) | Грешният WIP акаунт за продажби се използва за WIP осчетоводяване на вътрешнофирмен лист.                                                                                                                                     |
| Управление на проекти и счетоводство | [536536](https://fix.lcs.dynamics.com/Issue/Details/?bugId=536536) | Проектната оферта представлява грешно изчисляване на цените, когато се приложи отстъпка и складът се актуализира.                                                                                                       |
| Управление на проекти и счетоводство | [537905](https://fix.lcs.dynamics.com/Issue/Details/?bugId=537905) | Когато стартирате преизчисляване, след като корекция на разходите за артикули се използва в транзакция на проект, се появява следното съобщение за грешка: „Преизчислението е на пауза поради грешка“.                                                               |
| Управление на проекти и счетоводство | [540622](https://fix.lcs.dynamics.com/Issue/Details/?bugId=540622) | Не се създават записи в главната книга при коригиране на транзакции от фактурируеми към нефактурируеми при натрупване на приходи.                                                                                              |
| Управление на проекти и счетоводство | [540633](https://fix.lcs.dynamics.com/Issue/Details/?bugId=540633) | Когато функцията за запазване на фактура на доставчик на проект, **Активиране на изчислението на сумата на разходите** е включено, **ProjTrans** не се създава с плащане при плащане.                                             |
| Управление на проекти и счетоводство | [541421](https://fix.lcs.dynamics.com/Issue/Details/?bugId=541421) | Има множество проблеми със страницата **Създайте предложение за фактура**.                                                                                                                                                     |
| Управление на проекти и счетоводство | [543968](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543968) | В Project Operations страницата **Договор за покупка** не се вижда във Финансовите юридически лица, които са интегрирани с Project Operations.                                                                                             |
| Управление на проекти и счетоводство | [544132](https://fix.lcs.dynamics.com/Issue/Details/?bugId=544132) | Разширените списания не могат да се публикуват с отчетна дата в затворен период дори когато опцията **Автоматично задайте счетоводна дата към следващия отворен период** опцията е включена.                                                |
| Управление на проекти и счетоводство | [545878](https://fix.lcs.dynamics.com/Issue/Details/?bugId=545878) | Заради интеграционна грешка на Dataverse, не можете да конвертирате оферта в спечелена в Project Operations.                                                                                                                                       |
| Управление на проекти и счетоводство | [546604](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546604) | В Project Operations се появява съобщение за грешка, когато се опитвате да свържете ред на договор с идентификатор на проект поради проверката за припокриващи се линии на договора и типове транзакции.                                                |
| Управление на проекти и счетоводство | [547440](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547440) | **ProjCDSProjectContractEntity** може да зададе адреса на фактура на източника на финансиране от различен клиент.                                                                                                             |
| Управление на проекти и счетоводство | [547606](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547606) | Стандартното търсене на ресурса на страниците не е налично след актуализацията 10.0.15.                                                                                                                    |
| Управление на проекти и счетоводство | [547831](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547831) | Акаунтът на книгата и типът на осчетоводяване са неправилни във ваучера на главната книга, а типът на осчетоводяване е неправилен във ваучера за поръчка за покупка за елемент, който не е на склад, когато групата на проекти е зададена на **Баланс**.                                 |
| Управление на проекти и счетоводство | [550030](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550030) | Номерът на активността не се показва за чакаща фактура на доставчик, въпреки че **Блокиране на избора на родителска активност** е зададено на „Не“.                                                                    |
| Управление на проекти и счетоводство | [557376](https://fix.lcs.dynamics.com/Issue/Details/?bugId=557376) | В Project Operations не се избират измерения, когато създавате фактура за осчетоводяване за транзакция.                                                                                                                   |
| Управление на проекти и счетоводство | [442814](https://fix.lcs.dynamics.com/Issue/Details/?bugId=442814) | При управлението на проекти и счетоводството приоритетът на трансферната цена не е точно отразен за вътрешнофирмените разписания.                                                                            |
| Управление на проекти и счетоводство | [533530](https://fix.lcs.dynamics.com/Issue/Details/?bugId=533530) | Методът на наследената съставна структура на работата (WBS) **ProjWBSUpdateController::updateOutlineNumbersAndPublishInPreOrder** е оттеглен.                                                                                                   |

### <a name="regulatory-updates"></a>Нормативни актуализации
За информация относно нормативните актуализации за приложенията на Finance and Operations вижте [Нормативни актуализации](https://docs.microsoft.com/dynamics365/finance/localizations/regulatory-updates). Можете също да влезете в LCS и да прегледате планираните нормативни актуализации с помощта на инструмента за търсене на издания. Търсенето на издания ви позволява да търсите по държава, тип функция и издание.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]