---
title: Навигиране в потребителския интерфейс
description: Тази тема предоставя информация за управление на проекти в Dynamics 365 Project operations.
author: ruhercul
manager: AnnBe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: ff624a13ec88ae64dba18715fbe9b94353b070e8
ms.sourcegitcommit: 396e0fea2f1598a5313cb0128eca4fe0bb5aade9
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961819"
---
# <a name="navigating-the-user-interface"></a>Навигиране в потребителския интерфейс

_**Отнася се за:** Project Operations за сценарии, базирани на ресурси / без складови наличности, внедряване на Lite - сделка с проформа фактуриране_

## <a name="overview"></a>Общ преглед

Основната форма на проекта е разделена на няколко раздела. Всеки раздел представлява различно ниво на детайлност в рамките на проекта.

- **Обобщение**: Осигурява описание на проекта и обобщава както планираното, така и действителното изпълнение на проекта.

    ![Раздел и полета Обобщение](media/navigation7.png)

- **Задачи**: Предоставя подробности относно структурата на разбивка на работата, представена от изглед на мрежа, изглед на дъска и гант.

    ![Раздел и полета за задачи](media/navigation8.png)

- **Екип**: Предоставя подробности относно участниците в проекта. Възложените усилия на всеки член на екипа също са обобщени в този изглед.

    ![Раздел и полета за екипи](media/navigation9.png)

- **Присвояване на ресурси**: Предоставя периодично представяне на усилията за всеки ресурс по даден проект.

    ![Раздел и полета за задания на ресурси](media/navigation10.png)

- **Изравняване на ресурсите**: Предоставя периодичен изглед на разликите между заданията на всеки именен ресурс и техните резервации.

    ![Раздел и полета за съгласуване на ресурси](media/navigation11.png)

- **Оценки**: Предоставя периодичен изглед на разходите и оценките на продажбите на даден проект.

    ![Раздел и полета за прогнозни данни](media/navigation12.png)

- **Проследяване**: Предоставя изглед, който показва напредъка на задачите в структурата на разбивка на работата за усилия, разходи и продажби.

    ![Раздел и полета за проследяване](media/navigation13.png)

- **Продажби**: Осигурява дълбоки връзки към оферти и договори, свързани с проекта.

- **Оценки на разходите**: Предоставя мрежа, която определя разходите по проекта въз основа на категориите организационни разходи.

    ![Раздел и полета за прогнози за разходи](media/navigation14.png)

## <a name="grid-controls"></a>Контроли на мрежата

Следва кратък преглед на типичните контроли, намерени в различните раздели за планиране на проекти.

### <a name="refresh"></a>Опресняване

**Обнови**: Извлича последните данни от сървъра, ако са настъпили промени след зареждането на мрежата.

![Бутон за опресняване](media/navigation7.png)

### <a name="group-by"></a>Групиране по

**Групиране по**: Актуализира групирането на редовете в мрежата, за да отрази или ресурси, роли или категории въз основа на нуждите на потребителя.

![Групиране по бутон](media/navigation6.png)

### <a name="previousnext"></a>Предишен/следващ

**Предишен**/**Следващ**: Актуализирайте видимите периоди от време във фазовите мрежи.

![Бутони Предишен и Следващ](media/navigation2.png)

### <a name="timescale"></a>Времева скала

**Времева скала**: Променете обобщението на фазовите данни между дни, седмици, месеци и години.

![Бутон за времева скала](media/navigation3.png)

### <a name="expand"></a>Разгъни

**Разгъване**: Предаване на видимата решетка на цял екран, осигурявайки повече възможност да видите допълнителни роли.

![Бутон за разгъване](media/navigation4.png)

### <a name="time-phase-by"></a>Време-фаза по

**Време-фаза по**: Актуализирайте групирането на редовете в мрежата, за да отразява приблизителните разходи за прогнозни продажби. Този контрол се отнася и за скрипта за оценка и мрежата за проследяване.

![Бутон Време-фаза по](media/navigation0.png)

### <a name="add-column"></a>Добавяне на колона

**Добавяне на колона**: Позволява на потребителя да дефинира видимите колони в мрежата. Само предварително подготвени колони могат да се добавят към решетките във формуляра **Планиран проект**.

![Бутон за добавяне на колона](media/navigation5.png)
