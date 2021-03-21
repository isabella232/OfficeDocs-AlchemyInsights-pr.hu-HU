---
title: Problémák akkor, amikor gépeket vezet be a Végponthoz készült Microsoft Defenderhez (MDE)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901569"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>Problémák akkor, amikor gépeket vezet be a Végponthoz készült Microsoft Defenderhez (MDE)

Problémákat észlelhet akkor, amikor gépeket próbál bevezetni az MDE szolgáltatásba. Ha hozzá tud férni a végfelhasználói géphez, kövesse ezeket a lépéseket:

1. A [MDE Klienselemző](https://aka.ms/betamdeanalyzer) diagnosztikai eszköz legújabb előzetes verziójának letöltése.
2. Kattintson jobb kattintással a **MDEClientAnalyzer.cmd** elemre, és válassza a „Futtatás rendszergazdaként“ lehetőséget.
3. Kövesse a javasolt utasításokat a **MDEClientAnalyzer.htm** elemben megadottak szerint.
4. Részletesebb naplókért tekintse át a létrehozott almappát:**MDEClientAnalyzerResult**.
5. Ha további útmutatásra van szüksége, lépjen kapcsolatba a [Végponthoz készült Microsoft Defender támogatással](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) és adja meg a létrehozott MDEClientAnalyzerResult.zip fájlt elemzésre.
