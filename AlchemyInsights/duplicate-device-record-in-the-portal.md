---
title: Duplikált eszközrekord a portálon
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789864"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplikált eszközrekord a portálon

Előfordulhat, hogy a portálon 2 rekord található egy eszközhöz, ha az eszköz nem jelenti megfelelően az együttes felügyeleti állapotát a Konfigurációkezelő webhelynek. Egy eszköz együttes felügyeleti állapotának ellenőrzéséhez tekintse át az eszközhöz tartozó **Együttes felügyelet** oszlopot a Konfigurációkezelő konzolon. Ha az oszlop nem látható, akkor a megjelenítéséhez a jobb gombbal bármelyik oszlopfejlécre kattintva kiválaszthatja a listáról.

Az Együttes felügyelet mezőben **Igen** értéknek kell szerepelnie. Ha az érték **Nem**, nyissa meg a Konfigurációkezelő ügyfélalkalmazást az ügyféleszközön, és ellenőrizze az Általános lapon látható **Együttes felügyelet** tulajdonságot.

- Ha a tulajdonság értéke **Engedélyezve**, ez az ügyfél és a felügyeleti pont közötti kommunikációval kapcsolatos problémákra utal. Tekintse át a **CcmMessaging.log** fájlt az eszközön a lehetséges kapcsolódási hibák kivizsgálásához.

- Ha az érték **Letiltva**, és az eszköz regisztrálva van az Intune szolgáltatásban, akkor győződjön meg arról, hogy az eszköz megkapta az együttes felügyeleti házirendet; ehhez tekintse át a **CoManagementHandler.log** fájlt az eszközön.
