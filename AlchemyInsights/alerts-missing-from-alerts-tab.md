---
title: A Riasztások lapról hiányzó értesítések
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454683"
---
# <a name="alerts-missing-from-alerts-tab"></a>A Riasztások lapról hiányzó értesítések

A **Riasztások** lap az appirányítási portálon a bérlői webhely beállításán és aktiválásán alapuló házirendek alapján működik. Az Alkalmazásirányítás funkcióban is aktiválni kell a nem azonnal aktiválódó házirendeket, hogy jelzéseket küldve a riasztások **lapra** továbbítva legyen. 

Győződjön meg arról, hogy a riasztás létre lett hozva:

1. Az alkalmazásirányítási [szabályzatok](https://compliance.microsoft.com/m365appprotection?viewid=policies) között győződjön meg arról, hogy legalább egy aktív vagy naplózási házirendet hozott létre.

1. Jelölje ki a házirendet, majd válassza a **Szerkesztés lehetőséget** az úszó panelen. 

1. Ellenőrizze a házirend konfigurációját, és győződjön meg arról, hogy több mint 24 órája kezdeményezett házirendesemény miatt riasztást kellett volna generálni.

Az Alkalmazásirányítás riasztásokkal kapcsolatos további információkért lásd: Az app veszélyforrások észlelésének és megoldásának első [lépéseke.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)