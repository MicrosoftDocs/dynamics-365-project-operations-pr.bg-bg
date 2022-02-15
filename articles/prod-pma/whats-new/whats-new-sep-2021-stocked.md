---
title: Какво е ново или променено в Project Operations, септември 2021 г. за сценарии, базирани на запаси/производство
description: Тази тема предоставя информация за актуализациите на качеството, които са налични в изданието от септември 2021 г. на Project Operations за заредени/производствени базирани сценарии.
author: andchoi
ms.date: 11/11/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: andchoi
ms.openlocfilehash: 7016d702719b2d432ec929aaca8d609ebf6e996b
ms.sourcegitcommit: abdd6cb3461ebb12fd2ca7ea78439c29aecd0a94
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/16/2021
ms.locfileid: "7815818"
---
# <a name="whats-new-or-changed-in-project-operations-september-2021-for-stockedproduction-based-scenarios"></a>Какво е ново или променено в Project Operations, септември 2021 г. за сценарии, базирани на запаси/производство

_**Приложимо за:** Project Operations за сценарии, базирани на наличност/производство_

Тази тема се отнася за следните компоненти и версии на Microsoft Dynamics 365 Project Operations:

- Управление на проекти и счетоводство в Dynamics 365 Finance среда версия 10.0.21
 
## <a name="quality-updates"></a>Актуализации на качеството

| Област с функции | Номер за справка | Актуализация на качеството |
|---|---|---|
| Управление на проекти и счетоводство | [412077](https://fix.lcs.dynamics.com/Issue/Details/?bugId=412077) | Ако ролята на мениджър "Покупка" получи достъп до едно юридическо лице, тя получава достъп и до всички проекти във всички юридически лица. |
| Управление на проекти и счетоводство | [537214](https://fix.lcs.dynamics.com/Issue/Details/?bugId=537214) | Проблем със закръгляването на данък добавена стойност (ДДС) възниква, докато кредитна бележка е уредена срещу оригинална фактура за проект. |
| Управление на проекти и счетоводство | [538002](https://fix.lcs.dynamics.com/Issue/Details/?bugId=538002) | Използвайте алтернативен проектен бюджет за проверка на бюджета. |
| Управление на проекти и счетоводство | [546265](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546265) | Ценовата **група "Продажна цена час"** не се изчислява в структурата на разбивката на работата за котировките на проекта. |
| Управление на проекти и счетоводство | [555604](https://fix.lcs.dynamics.com/Issue/Details/?bugId=555604) | Оценка елиминиране е неуспешно, когато е разрешена функцията разрешаване на проект договор валута за оценка **изчисление** функция. |
| Управление на проекти и счетоводство | [563523](https://fix.lcs.dynamics.com/Issue/Details/?bugId=563523) | Факторизацията на данък продажби по количество се добавя към сумата на продажната цена, когато данък използване се използва в данъчната група продажби на дневника за разходи на Проекта. |
| Управление на проекти и счетоводство | [564701](https://fix.lcs.dynamics.com/Issue/Details/?bugId=564701) | Условен данък не се изчислява правилно за последното плащане при задържане на доставчика и предварително плащане се прилагат към фактури за поръчка за покупка. |
| Управление на проекти и счетоводство | [565642](https://fix.lcs.dynamics.com/Issue/Details/?bugId=565642) | Проследяване на корекция не работи за Начало баланс дневници. |
| Управление на проекти и счетоводство | [568814](https://fix.lcs.dynamics.com/Issue/Details/?bugId=568814) | **Разпределението на бюджетните ревизии по проекти по периоди** се разделя на всички бюджетни периоди. Когато разпределението е подадено, записът не е изчистен. |
| Управление на проекти и счетоводство | [569250](https://fix.lcs.dynamics.com/Issue/Details/?bugId=569250) | Работа в процес (НП) осчетоводявания в счетоводството имат неправилна сума. |
| Управление на проекти и счетоводство | [570731](https://fix.lcs.dynamics.com/Issue/Details/?bugId=570371) | Одобрението на дневника "Час на проекта" не работи. |
| Управление на проекти и счетоводство | [571391](https://fix.lcs.dynamics.com/Issue/Details/?bugId=571391) | Продажната цена за корекция на проекта не се актуализира с непреки разходи, когато лимитът за финансиране е немаркиран. |
| Управление на проекти и счетоводство | [575831](https://fix.lcs.dynamics.com/Issue/Details/?bugId=575831) | Изискване за артикул не може да бъде създадено, когато заглавният блок на таблицата "Продажби" е фактуриран и бек-поръчката за покупка за съществуващи редове е финализирана. |
| Управление на проекти и счетоводство | [578036](https://fix.lcs.dynamics.com/Issue/Details/?bugId=578036) | Сумата на задържане за правило за фактуриране, което има момент за различен проект, не е осчетоводена в съответния ИД на проект, който е избран за най-близкия момент. Вместо това се публикува с първия проект. |
| Управление на проекти и счетоводство | [578327](https://fix.lcs.dynamics.com/Issue/Details/?bugId=578327) | Когато изберете **Финансово ниво на аналитичност, зададено на предложение за** фактура, възниква следната грешка: "Не може да се хвърли обект от тип 'Dynamics.AX. Application.FormIntControl", за да въведете 'Dynamics.AX. Application.FormStringКонтрол"." |
| Управление на проекти и счетоводство | [581167](https://fix.lcs.dynamics.com/Issue/Details/?bugId=581167) | Отчетът за фактура за **проект** пропуска редове. |
| Управление на проекти и счетоводство | [581489](https://fix.lcs.dynamics.com/Issue/Details/?bugId=581489) | Възниква грешка, когато изчислявате контролата на разходите за инвестиционен проект. |
| Управление на проекти и счетоводство | [590357](https://fix.lcs.dynamics.com/Issue/Details/?bugId=590357) | **ProjTable::InitFromCustTable - canDeletePostalAddress** метод причинява проблем с производителността. |
| Управление на проекти и счетоводство | [592493](https://fix.lcs.dynamics.com/Issue/Details/?bugId=592493) | Съобщението за грешка трябва да бъде по-ясно от "Неочаквана грешка". |
| Управление на проекти и счетоводство | [598810](https://fix.lcs.dynamics.com/Issue/Details/?bugId=598810) | Проект фактура осчетоводяване пакетно задание процеси и осчетоводява фактура предложение дори ако редовете от фактура не са генерирани. |
| Управление на проекти и счетоводство | [574282](https://fix.lcs.dynamics.com/Issue/Details/?bugId=574282) | Възниква проблем със закръгляването, когато ключът за конфигуриране на лиценза на публичния сектор е изключен. Неправилен разход или продажна цена се генерира в часовете на времевия лист за договори, които имат няколко основателни източници. |
| Управление на проекти и счетоводство | [577598](https://fix.lcs.dynamics.com/Issue/Details/?bugId=577598) | Продажбената цена на проекта на фактурирана поръчка за покупка на проект неправилно се изчислява, когато моделът на продажбената цена е **Съотношение принос**. |
| Управление на проекти и счетоводство | [580784](https://fix.lcs.dynamics.com/Issue/Details/?bugId=580784) | Системата не разглежда активните дни между това кога изчислява ефективната ставка на труд за служител. |
| Управление на проекти и счетоводство | [584054](https://fix.lcs.dynamics.com/Issue/Details/?bugId=584054) | Грешка при осчетоводяване възниква в междуфирмения времеви лист поради следната грешка при проверка: "Никой търговски партньор не е конфигуриран за юридическо лице." |
| Управление на проекти и счетоводство | [586303](https://fix.lcs.dynamics.com/Issue/Details/?bugId=586303) | Описанието от поръчка за покупка, която има категория разходи, не се извлича в списъка с осчетоводени транзакции по проекта. |
| Управление на проекти и счетоводство | [590349](https://fix.lcs.dynamics.com/Issue/Details/?bugId=590349) | Има неправилно преобразуване в дневници за артикули, които са осчетоводени към проект. |
| Управление на проекти и счетоводство | [557294](https://fix.lcs.dynamics.com/Issue/Details/?bugId=557294) | Можете да потвърдите поръчка за покупка, дори ако лимитът за финансиране е надвишен. |
| Управление на проекти и счетоводство | [574162](https://fix.lcs.dynamics.com/Issue/Details/?bugId=574162) | Корекция/отказ фактура раздел на свободен **текст** фактура изчезва, когато е избран ИД на проект. |
| Управление на проекти и счетоводство | [575425](https://fix.lcs.dynamics.com/Issue/Details/?bugId=575425) | Има проблеми с производителността, когато проект фактура предложение е осчетоводен от проект поръчка, която включва зареден елемент. |
| Управление на проекти и счетоводство | [575939](https://fix.lcs.dynamics.com/Issue/Details/?bugId=575939) | Фактурите за покупка на проекти не могат да бъдат публикувани, защото възниква следната грешка: "Функция AccDistProcessorProjectExtension.createForProjectRevenueLine е неправилно извикан." |
| Управление на проекти и счетоводство | [578970](https://fix.lcs.dynamics.com/Issue/Details/?bugId=578970) | Актуализация до създаването на проект оценка пакетни задания за подпомагане на изпълнението на няколко подзадачи. |
| Управление на проекти и счетоводство | [584519](https://fix.lcs.dynamics.com/Issue/Details/?bugId=584519) | Състоянието на даден времеви лист не може да бъде актуализирано в **Чернова,** когато работният поток е заседнал в **отменено** състояние. |
| Управление на проекти и счетоводство | [584757](https://fix.lcs.dynamics.com/Issue/Details/?bugId=584757) | Сумите за задържане не се изчисляват в предложението за фактура за кредитна бележка, ако съществуват няколко реда. |
| Управление на проекти и счетоводство | [586034](https://fix.lcs.dynamics.com/Issue/Details/?bugId=586034) | Когато се опитате да промените сумата на генерирана фактура от поръчка за покупка, възниква следната грешка: "Транзакциите на ваучер не баланс като за XX/XX/XXXX. (счетоводна валута: 0,00 - отчетна валута: 0,01)." |
| Управление на проекти и счетоводство | [588714](https://fix.lcs.dynamics.com/Issue/Details/?bugId=588714) | Има проблем с производителността, когато проект фактура предложение е публикуван в пакетен режим, поради присъединяването с **GeneralJournalAccountEntry**. |
| Управление на проекти и счетоводство | [588851](https://fix.lcs.dynamics.com/Issue/Details/?bugId=588851) | Има проблеми с производителността, когато е осчетоводен времеви лист. |
| Управление на проекти и счетоводство | [590535](https://fix.lcs.dynamics.com/Issue/Details/?bugId=590535) | Прогнозата за разходите йерархия на структурата на разбивка на работата не е правилно подравнени след разширяване на всички задачи или след ръчно разширяване на една задача. |
| Управление на проекти и счетоводство | [593663](https://fix.lcs.dynamics.com/Issue/Details/?bugId=593663) | Шаблонът за проектна оферта Excel не може да бъде добавен към **менюто Отвори в** Excel. |
| Управление на проекти и счетоводство | [596669](https://fix.lcs.dynamics.com/Issue/Details/?bugId=596669) | Освободеният от данъци номер за правен обект не е включен във фактурата за печатен проект. |
| Управление на проекти и счетоводство | [597563](https://fix.lcs.dynamics.com/Issue/Details/?bugId=597563) | Не се актуализират финансови данни в грешката на складовата единица, когато даден проект се коригира във връзка с кредитни редове. |
| Управление на проекти и счетоводство | [598109](https://fix.lcs.dynamics.com/Issue/Details/?bugId=598109) | След като приложите KB 461935, не можете да публикувате прогнози, ако преминете към непрекъснати числени последователности. |
| Управление на проекти и счетоводство | [598688](https://fix.lcs.dynamics.com/Issue/Details/?bugId=598688) | **TimeEntryDataManager кара мобилното приложение за времеви лист на** Project за Android да спре да отговаря. |
| Управление на проекти и счетоводство | [602677](https://fix.lcs.dynamics.com/Issue/Details/?bugId=602677) | Обратната на НП стойност от осчетоводяване на фактура се различава от първоначално осчетоводената стойност на НП от записа за време. |
| Управление на проекти и счетоводство | [602728](https://fix.lcs.dynamics.com/Issue/Details/?bugId=602728) | В приложни случаи на контейнер транзакциите на ваучер не баланс, когато фактурирани приходи за проект е осчетоводен. |
| Управление на проекти и счетоводство | [603320](https://fix.lcs.dynamics.com/Issue/Details/?bugId=603320) | Когато е разрешена функцията за подобряване на производителността на планиране на ресурси на **Project**, десетичните стойности неправилно се закръгляват за наличност на ресурси и капацитет. |
| Управление на проекти и счетоводство | [607324](https://fix.lcs.dynamics.com/Issue/Details/?bugId=607324) | Когато е разрешена функцията Създаване на проект с **помощта на няколко пакетни задачи** функция, създаване на оценки в папка, която има няколко подзадачи работи само за текущия период. |
| Пътуване и разход | [551911](https://fix.lcs.dynamics.com/Issue/Details/?bugId=551911) | Правилата за пътно запитване се игнорират, а работният поток е одобрен без грешки. |
| Пътуване и разход | [563752](https://fix.lcs.dynamics.com/Issue/Details/?bugId=563752) | <p>Приложението "Мобилни разходи" не записва следната информация в разходния ред:</p><ul><li>Идентификационният номер на проекта</li><li>Дали разходът е таксуван</li><li>Номерът на дейността</li></ul> |
| Пътуване и разход | [569458](https://fix.lcs.dynamics.com/Issue/Details/?bugId=569458) | Полето **Прикачени разписки е** зададено на **"Да", дори ако към реда на** разходите не е прикачена разписка. |
| Пътуване и разход | [571334](https://fix.lcs.dynamics.com/Issue/Details/?bugId=571334) | Възниква грешка, когато промените категорията на разходите на **Лична**. |
| Пътуване и разход | [572783](https://fix.lcs.dynamics.com/Issue/Details/?bugId=572783) | Не можете да прикачите разписка и да редактирате родителския разход, след като транзакция с кредитна карта бъде разделена на личен разход. |
| Пътуване и разход | [574252](https://fix.lcs.dynamics.com/Issue/Details/?bugId=574252) | Правилата за разходите за междуфирмени транзакции, които имат ИД на проект, не работят правилно. |
| Пътуване и разход | [574489](https://fix.lcs.dynamics.com/Issue/Details/?bugId=574489) | Информацията за осчетоводената дата липсва за осчетоводените отчети за разходите. |
| Пътуване и разход | [574504](https://fix.lcs.dynamics.com/Issue/Details/?bugId=574504) | Има проблеми с начина на плащане в мобилното приложение Разход. |
| Пътуване и разход | [584799](https://fix.lcs.dynamics.com/Issue/Details/?bugId=584799) | Запитване за пътуване, което е създадено за един работник, може да се използва за отчета за разходите на друг работник преди датата на представителя. |
| Пътуване и разход | [586023](https://fix.lcs.dynamics.com/Issue/Details/?bugId=586023) | Когато създавате разход, промените в стойностите на финансовите нива на аналитичност не се актуализират правилно на ниво на счетоводна дистрибуция в **работната област за управление на** разходите. |
| Пътуване и разход | [586081](https://fix.lcs.dynamics.com/Issue/Details/?bugId=586081) | Състоянието на одобрението на главния разходен ред не се синхронизира със състоянието на одобрение на itemized line workflow. |
| Пътуване и разход | [590544](https://fix.lcs.dynamics.com/Issue/Details/?bugId=590544) | Възниква грешка, ако публикувате отчет за разходите и възстановяване на данъци е разрешено. |
| Пътуване и разход | [564851](https://fix.lcs.dynamics.com/Issue/Details/?bugId=564851) | Делегат не може да изтрие документи за разходи за уволнен служител. |
| Пътуване и разход | [587306](https://fix.lcs.dynamics.com/Issue/Details/?bugId=587306) | Изтриването на разходна линия отнема повече време от очакваното и влияе върху производителността. |
| Пътуване и разход | [600455](https://fix.lcs.dynamics.com/Issue/Details/?bugId=600455) | **TrvExpTrans** причинява осиротели **TaxНекомитет** запис, защото само **SourceDocumentLine** се изтрива. |
| Пътуване и разход | [609918](https://fix.lcs.dynamics.com/Issue/Details/?bugId=609918) | **ReleaseUpdateDB72_Expense.updateTrvExpTransProjTransId()** не почита **trvExpTrans.ReferenceDataAreaId** за създаване на новата последователност от числа. |

## <a name="regulatory-updates"></a>Нормативни актуализации

За информация относно регулаторни актуализации за приложения "Финанси и операции" вижте [Регулаторни актуализации](/dynamics365/finance/localizations/regulatory-updates). Можете също да влезете в Microsoft Dynamics Lifecycle Services (LCS) и да използвате инструмента за търсене на проблем, за да прегледате планираните регулаторни актуализации. Търсенето на проблеми ви позволява да търсите по държава или регион, тип функция и освобождаване.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]