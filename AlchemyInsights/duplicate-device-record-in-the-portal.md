---
title: Duplikált eszközrekord a portálon
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004156"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplikált eszközrekord a portálon

Előfordulhat, hogy a portálon 2 rekord található egy eszközhöz, ha az eszköz nem jelenti megfelelően az együttes felügyeleti állapotát a Konfigurációkezelő webhelynek. Egy eszköz együttes felügyeleti állapotának ellenőrzéséhez tekintse át az eszközhöz tartozó **Együttes felügyelet** oszlopot a Konfigurációkezelő konzolon. Ha az oszlop nem látható, akkor a megjelenítéséhez a jobb gombbal bármelyik oszlopfejlécre kattintva kiválaszthatja a listáról.

Az Együttes felügyelet mezőben **Igen** értéknek kell szerepelnie. Ha az érték **Nem**, nyissa meg a Konfigurációkezelő ügyfélalkalmazást az ügyféleszközön, és ellenőrizze az Általános lapon látható **Együttes felügyelet** tulajdonságot.

- Ha a tulajdonság értéke **Engedélyezve**, ez az ügyfél és a felügyeleti pont közötti kommunikációval kapcsolatos problémákra utal. Tekintse át a **CcmMessaging.log** fájlt az eszközön a lehetséges kapcsolódási hibák kivizsgálásához.

- Ha az érték **Letiltva**, és az eszköz regisztrálva van az Intune szolgáltatásban, akkor győződjön meg arról, hogy az eszköz megkapta az együttes felügyeleti házirendet; ehhez tekintse át a **CoManagementHandler.log** fájlt az eszközön.
