---
title: Деинсталиране на Dynamics 365 Project Operations
description: Тази статия предоставя информация за това как да деинсталирате Dynamics 365 Project Operations.
author: stsporen
ms.date: 11/09/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 33a505594d6db47b4f8a0c8a630a0836f424e7d5
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2022
ms.locfileid: "8911951"
---
# <a name="uninstall-dynamics-365-project-operations"></a>Деинсталиране на Dynamics 365 Project Operations 

_**Прилага се за:** Project Operations за сценарии, базирани на ресурси/неналичност_

За да деинсталирате Dynamics 365 Project Operations, трябва да ви бъде назначена ролята на администратор.

1. Отидете в **Настройки** > **Решения**.

    ![Страница с настройки.](./media/uninstall-proj-ops-solutions.png)
  
2. Премахнете решенията в точния ред, в който са изброени в следващата таблица. 

    | Стъпка | Решение   име                                    | Забележка                                                                                         |
    |------|----------------------------------------------------|----------------------------------------------------------------------------------------------|
    | 1 | msdyn_ProjectServiceUpgrade_managed.cab            | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 2 | ProjectOperations_Anchor                           | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 3 | Dynamics365ProjectOperationsDualWriteEntityMaps    | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 4 | Dynamics365ProjectOperationsDualWrite              | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 5 | ProjectService                                     | Няма допълнителни бележки.                                                                         |
    | 6 | ProjectServiceCore_Patch                           | Няма допълнителни бележки.                                                                         |
    | 7 | ProjectServiceCore                                 | Няма допълнителни бележки.                                                                         |
    | 8 | ProjectServiceDeprecatedComponents                 | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 9 | FieldServiceCommon                                 | Изисква се за двунаписване с Dynamics 365 Finance или Dynamics 365 Supply Chain Management.   |
    | 10 | msdyn_AssetCommon                                  | Изисква се за двунаписване с Dynamics 365 Finance или Dynamics 365 Supply Chain Management.   |
    | 11 | msdyn_TESA_Anchor                                  | Задължително за Dynamics 365 Field Service.                                                     |
    | 12 | msdyn_TESA_Patch                                   | Задължително за Dynamics 365 Field Service.                                                     |
    | 13 | msdyn_TESA                                         | Задължително за Dynamics 365 Field Service.                                                     |
    | 14 | ResourceSchedulingControls                         | Задължително за Dynamics 365 Field Service.                                                     |
    | 15 | MicrosoftDynamicsScheduling3_CumulativePatch       | Задължително за Dynamics 365 Field Service.                                                     |
    | 16 | MicrosoftDynamicsScheduling_Patch_xx               | Задължително за Dynamics 365 Field Service.                                                     |
    | 17 | MicrosoftDynamicsScheduling                        | Задължително за Dynamics 365 Field Service.                                                     |
    | 18 | Dynamics365FinanceAndOperationsAnchor              | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 19 | Dynamics365Notes                                   | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 20 | Dynamics365FinanceAndOperationsDualWriteEntityMaps | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 21 | DualWriteCore                                      | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 22 | Dynamics365AssetManagementApp                      | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 23 | Dynamics365AssetManagement                         | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 24 | Dynamics365SupplyChainExtended                     | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 25 | Dynamics365FinanceExtended                         | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 26 | HCMCommon                                          | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 27 | Dynamics365FinanceAndOperationsCommon              | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 28 | Купон                                              | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 29 | Dynamics365Company                                 | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 30 | CurrencyExchangeRates                              | Ако не бъде намерено, пропуснете това решение.                                                            |
    | 31 | AssetCommon                                        | Ако не бъде намерено, пропуснете това решение.                                                            |
