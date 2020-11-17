---
title: Организационни единици
description: Тази тема предоставя информация за организационните единици в Dynamics 365 Project Service Automation.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/04/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 454d9a4c4d139f493adf4604f8ba40a0211f0eec
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071932"
---
# <a name="organizational-units"></a>Организационни единици 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Организационна единица в Dynamics 365 Project Service Automation е отделна група или подразделение във фирма за професионални услуги, която използва платими ресурси, които имат ставки за разход.

За фирмите за професионални услуги, които използват технически ресурси в различни сфери на дейност или бизнес линии, разходите за попълване на роля в една сфера на дейност или бизнес линия може да се различават от разходите за попълване на роля в друга сфера на дейност или бизнес линия. Концепцията на организационните единици помага в този сценарий чрез предоставяне на начин за групиране на набор от платими роли в отдел на фирма, която има отделна структура на разходите за тези роли.

## <a name="key-attributes-and-associations-of-organizational-units"></a>Основни атрибути и връзки на организационни единици

Организационна единица в PSA има конкретна валута и конкретни ценови листи на разходите.

Валутата на организационна единица е основната валута, която се използва за проследяване на разходите.

Един или повече ценови листи на разходите могат да бъдат прикачени към всяка организационна единица. PSA поставя следните ограничения върху ценовите листи, които могат да бъдат прикачени към организационна единица:

- Ценовите листи трябва да са във валутата на организационната единица
- Ценовите листи трябва да са от ценови листи на разходите

Освен това има атрибут за организационната единица в обекта „Ресурс“. Всеки ресурс може да бъде присвоен към една организационна единица.

## <a name="roles-of-organizational-units"></a>Роли на организационни единици

Организационната единица играе две роли в PSA:

- **Единица, сключваща договора** – организационната единица, представляваща групата или отдела на компанията, която е основно отговорна за спечелването на продажбата и управлението на доставката на работа и услуги на клиента. Единицата, сключваща договора, се идентифицира по полето **Единица, сключваща договора** в заглавната част на страниците **Възможност** **Оферта** , **Договор по проект** и **Проект**.
- **Ресурсна единица** – организационната единица, към която принадлежи или е присвоен ресурсът. Тази организационна единица може да предостави своите ресурси за някои роли по технически задания (SOW) и проекти, които са собственост на единицата, сключваща договора.

> ![Единици, сключващи договор, и ресурсни единици](media/advanced-1.png)

## <a name="organizational-unit-faqs"></a>ЧЗВ за организационните единици

По-долу са дадени някои от най-често задаваните въпроси относно организационните единици.

### <a name="how-is-the-organizational-unit-entity-in-psa-related-to-the-organization-entity-that-already-exists-in-dynamics-365"></a>Каква е връзката между обекта „Организационна единица“ в PSA и обекта „Организация“, която вече съществува в Dynamics 365?

Обектът „Организация“ в Microsoft Dynamics 365 представлява името на глобален екземпляр на Dynamics 365. Това име обикновено е името на глобалната фирма.

Обектът „Организационна единица“ представлява група или отдел в глобалната корпорация. Тази група или подразделение има набор от роли и ценова листа за тези роли, а тези роли и ценова листа се различават от ролите и ценовата листа на други групи или подразделения в корпорацията.

Когато е инсталиран PSA, се създава организационна единица по подразбиране въз основа на организацията. Всички съществуващи ресурси се присвояват към организационната единица по подразбиране. Ако нови потребители или ресурси на Active Directory се импортират в Dynamics 365, процесът на импортиране на потребители ги присвоява на организационната единица по подразбиране в PSA.
 
### <a name="how-does-the-organizational-unit-entity-differ-from-the-business-unit-entity"></a>По какво обектът „Организационна единица“ се различава от обекта „Бизнес единица“?

В Dynamics 365 обектът „Бизнес единица“ е концепция на защитата. Свързването на потребител с бизнес единица определя обектите и записите на обекти, до които потребителят има достъп. То също така определя разрешенията (създаване, четене, писане, изтриване, добавяне, добавяне към, присвояване или споделяне), които потребителят има за тези записи на обекти.

Обектът „Организационна единица“ представлява група или отдел на фирмата, който има различни ставки на разходите за служители, които са присвоени към него. Свързването на ресурс с организационна единица определя разхода на ресурса за ангажиране по проект.

Когато внедрявате Dynamics 365, оптимизирайте разрешаването на защитата за йерархията на бизнес единиците и присвояването на потребители към бизнес единиците. Присвоете всички потребители, които обикновено трябва да имат достъп до същия набор от записи в една и съща бизнес единица. Организационната единица не оказва въздействие върху разрешението на защитата или достъпа.

#### <a name="example-of-organizational-units-and-business-units"></a>Пример за организационни единици и бизнес единици

Contoso, Ltd. има процъфтяваща технологична дейност за Microsoft. Драган и Мира са C\# разработчици, но Мира е в Съединените щати, а Драган е в Индия. Повечето от ангажиментите по проекта изискват ресурси от Contoso Индия и Contoso САЩ, а Драган и Мира изискват еднакво ниво на достъп до проекти в тази сфера на дейност. Въпреки това цената на разработчиците от Contoso Индия се различава значително от цената на разработчиците от Contoso САЩ.

Ето оптимален начин за проектиране на този сценарий с помощта на Dynamics 365 и PSA.

1. Създайте технологичната дейност за Microsoft като бизнес единица и свържете Драган и Мира с нея. По този начин можете да помогнете да се гарантира, че и двамата служители имат едно и също ниво на достъп за сигурност до всички проекти в тази сфера на дейност. И двамата ще могат да проверяват напредъка и да отчитат времето, разходите и актуализациите на задачите. 
2. Създайте две организационни единици, за да се гарантира, че разходите за проекта се отразяват правилно. 
3. Свържете Мира с Contoso САЩ и Драган с Contoso Индия.
4. Присвоете подходящи ценови листи на разходи към двете организационни единици. По този начин вие помагате да се гарантира, че разходите, които са записани по проекта за Драган и Мира, отразяват точно разликата в разходите между Contoso САЩ и Contoso Индия.

### <a name="are-organizational-units-related-to-sales-territories-in-dynamics-365"></a>Организационните единици свързани ли са с продажбените региони в Dynamics 365?

Няма връзка или релация между продажбените региони и организационните единици. Продажбен регион обикновено е географска област, в която се извършват продажбите. Ценовата листа за продажби може да бъде свързана с всеки продажбен регион.

Организационна единица е вътрешна група или отдел във фирмата, проследяваща разходите за набор от роли, които продава на други отдели или на външни клиенти.

#### <a name="example-of-organizational-units-and-sales-territories"></a>Пример за организационни единици и продажбени региони

Contoso, Ltd. има два центъра за развитие: Contoso САЩ и Contoso Индия. Разходите за ресурси се различават значително между тези два центъра за развитие.

Contoso продава ИТ услугите си на много международни пазари, като Латинска Америка, Северна Америка, Азиатско-тихоокеанския регион, Западна Европа и Близкия изток. Ставките за фактуриране за едни и същи роли по проекта могат да варират значително между тези пазари.

Contoso САЩ и Contoso Индия трябва да бъдат настроени като организационни единици и всяка организационна единица трябва да има своя собствена ценова листа за разходи. Азиатско-тихоокеанският регион, Латинска Америка, Северна Америка, Западна Европа и Близкият изток трябва да бъдат настроени като продажбени региони и всеки продажбен регион трябва да има своя собствена ценова листа за продажби.

### <a name="why-is-there-a-restriction-on-the-association-of-price-lists-with-organizational-units"></a>Защо има ограничение на свързването на ценови листи с организационни единици? 

Ценообразуването на продажбите обикновено е уникално за географските райони или пазарите, където се продават услугите. Вътрешните отдели на дадена фирма обикновено нямат собствено ценообразуване на продажбите за един и същ тип услуги. Вътрешните отдели обаче имат различна себестойност на продадените стоки (СПС) в зависимост от уменията на хората, които наемат, и условията на труд в региона, в който оперират. Тъй като организационните единици са моделирани като вътрешни отдели на фирма, те могат да имат само ценови листи за разходи.

### <a name="why-cant-we-associate-sales-price-lists-to-organizational-units"></a>Защо не можем да свържем ценовите листи за продажби с организационни единици?

В PSA ценовите листи за продажби могат да се асоциират с клиенти и продажбени региони. Обектите за транзакции, като „Възможност“, „Оферта“, „Договор по проект“ и „Проект“, използват ценови листи за продажби, които са прикачени към акаунта на клиента или продажбения регион, за да определят ставките за фактуриране и потенциалните приходи от ангажимента по проекта.

Ценовите листи за разходи са свързани с организационни единици. Обектите за транзакции, като „Възможност“, „Оферта“, „Договор по проект“ и „Проект“, използват ценови листи за разходи, които са прикачени към единицата, подписваща договора, за определяне на разходите за ангажимент по проект.

### <a name="are-organizational-units-hierarchical-in-psa"></a>Организационните единици йерархични ли са в PSA?

Не. В текущото издание на PSA организационните единици не са йерархични. Това означава, че не можете да:

- конфигурирате модел за себестойности по подразбиране, които преминава нагоре в йерархия; 
- отчитате приходи или разходи, обобщени на различни нива на йерархията на организационната единица.

### <a name="were-a-big-multinational-firm-with-a-complex-multilevel-hierarchy-of-cost-centers-divisions-and-billing-offices-how-can-we-make-the-best-use-of-the-organizational-unit-concept-in-this-version-of-the-project-service-app"></a>Ние сме голяма мултинационална фирма със сложна, многостепенна йерархия от разходни центрове, отдели и офиси за фактуриране. Как можем да се възползваме най-добре от концепцията на организационните единици в тази версия на приложението Project Service?

Когато имате сложна йерархия от разходни центрове, отдели, офиси за фактуриране и т. н., настройте крайните възли на тази йерархия като отделни организационни единици.
Следващият пример показва типична йерархия:

**Contoso Индия**

  - Дейност по SAP 

    - Технически консултанти 
    - Функционални консултанти 
    
  - Технологична дейност за Microsoft 

    - Технически консултанти
    - Функционални консултанти 
    
**Contoso САЩ**

 - Дейност по SAP 

    - Технически консултанти 
    - Функционални консултанти 
    
 - Технологична дейност за Microsoft 

    - Технически консултанти 
    - Функционални консултанти 
 
Ако вашата йерархия е подобна, трябва да я настроите като плосък списък, както е показано тук:
- Contoso Индия – дейност по SAP – технически консултанти 
- Contoso Индия – дейност по SAP – функционални консултанти       
- Contoso Индия – технологична дейност за Microsoft – функционални консултанти 
- Contoso Индия – технологична дейност за Microsoft – функционални консултанти 
- Contoso САЩ – дейност по SAP – технически консултанти  
- Contoso САЩ – дейност по SAP – функционални консултанти  
- Contoso САЩ – технологична дейност за Microsoft – технически консултанти 
- Contoso САЩ – технологична дейност за Microsoft – функционални консултанти

### <a name="were-a-small-professional-services-company-that-operates-as-only-one-division-how-can-we-best-use-the-organizational-unit-concept-in-the-current-version-of-psa"></a>Ние сме малка фирма за професионални услуги, която има само един отдел. Как най-добре да използваме концепцията на организационните единици в текущата версия на PSA?

Ако вашата фирма работи като една единица, която има една ценова листа за разходи, не е нужно да настройвате никакви организационни единици. По време на инсталацията на PSA Dynamics 365 създава една организационна единица по подразбиране, която има същото име като организацията. По подразбиране всички потребители се присвояват към тази организационна единица. Винаги, когато системата изисква да бъде избрана организационна единица, тази организационна единица е избрана по подразбиране.

### <a name="when-a-project-is-created-from-a-quote-or-project-contract-line-the-default-contracting-unit-comes-from-the-quote-or-project-contract-if-a-project-is-created-before-sales-entities-such-as-quote-or-project-contract-what-is-the-default-contracting-unit"></a>Когато даден проект се създаде от ред на оферта или на договор по проект, единицата, която сключва договора, по подразбиране идва от офертата или договора по проект. Ако даден проект се създаде преди обекти за продажби, като оферта или договор по проект, коя е единицата по подразбиране, която сключва договора?

Когато даден проект се създава самостоятелно, единицата по подразбиране по проекта, която сключва договора, се основава на потребителя, който го създава. Този потребител е и мениджърът на проекта по подразбиране. Ако проектът се съпостави към обект на продажби, като например оферта или договор по проект, единицата на проекта, която подписва договора, се базира на обекта на продажби вместо това. В този случай прогнозните оценки за проекта могат да бъдат преизчислени, тъй като ценовата листа за разходи се използва за изчисляване на промените в прогнозните оценки на разходите, ако договарящата единица се промени. Ценовата листа за продажби се използва за изчисляване на прогнозните оценки за продажбите, които ще бъдат променени, така че да са синхронизирани с ценовата листа на проекта в офертата.

Полетата **Единица, която подписва договора** и **Валута** в проекта са заключени за редактиране, защото трябва да са синхронизирани със стойностите в обекта на продажби (оферта или договор по проект), към който е съпоставен проектът.