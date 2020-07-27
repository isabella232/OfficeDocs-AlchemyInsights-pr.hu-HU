---
title: Az aktiválási zár megkerülése felügyelt iOS-eszközökön az Intune-nal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423732"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Az aktiválási zár megkerülése felügyelt iOS-eszközökön az Intune-nal

Az iOS-eszközök aktiválási zárjának megkerülésének lehetősége megkönnyíti a helyreállítást abból a forgatókönyvből, amikor a felhasználó engedélyezi az aktiválási zárat egy vállalati eszközön, majd elhagyja a vállalatot.

Az aktiválási zár megkerüléséhez szükséges előfeltételek a következők:

- Az eszköz az, hogy a "felügyelt".
- Az aktiválási zárolás sikeresen engedélyezve van az Intune iOS-eszközkorlátozási házirendjével.

Ezenkívül az aktiválási zár megkerülésekénél a következőket kell tennie:

- Fizikailag birtokolják a letörölt eszközt.
- Másolja a kódot, mielőtt kiadja a törlést.

**Megjegyzés:** A törlési kód nem érzékeny a kis- és nagybetűkre, ezért a "-" karakterek nem szükségesek.

További információt az [Aktiválási zár megkerülése felügyelt iOS-eszközökön az Intune-nal.](https://docs.microsoft.com/intune/device-activation-lock-bypass)

**GYIK**

K: **Távoli műveletet adtam ki a vállalati adatok eszközről való eltávolítására, és most függőállapotban ragadt.**

Válasz: Ahhoz, hogy egy távoli művelet sikeresen befejeződjen, a megcélzott eszköznek online és kifogástalan állapotúnak kell lennie. A következő esetekben a távoli művelet 30 napig függőállapotban marad, vagy amíg az eszköz nem nyugtázza a parancsot, amikor az eszköz:

- Nem rendelkezik kapcsolattal.
- Az Intune-nal elveszíti felügyeleti állapotát.

Ha úgy gondolja, hogy egy eszköz már nem jelentkezik be, és nem távolítja el a vállalati adatokat, válassza a Törlés lehetőséget. A törlés eltávolítja az eszközrekordot, így az már nem jelenik meg az Intune eszközök listájában. Ahhoz, hogy az eszköz újra aktívvá váljon, a felhasználónak újra regisztrálnia kell az eszközt.

K: **Miért nem érhetők el bizonyos távoli műveletek?**

A: Nem minden platform támogatja az összes távoli eszközműveletet. A következő távoli műveletek platformspecifikusak.

- Az aktiválási zár megkerülése (csak iOS)
- Új kezdet (csak Windows)
- Elveszett mód (csak iOS esetén)
- Az eszköz megkeresése (csak iOS esetén)
- Újraindítás (csak Windows)

Az egyes műveletekről további információt az [Elérhető eszközműveletek (Available device actions) (Elérhető eszközműveletek) (Elérhető eszközműveletek) (Elérhető eszközműveletek) (Elérhető eszközműveletek) (Elérhető eszköz](https://docs.microsoft.com/intune/device-management#available-device-actions)