---
title: Elveszett iOS-eszközök megkeresése az Intune-nal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439627"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Elveszett iOS-eszközök megkeresése az Intune-nal

Az elveszett mód engedélyezése iOS-eszközön lehetővé teszi a rendszergazda számára, hogy egy üzenet és a kapcsolattartó telefonszáma megjelenjen a zárolási képernyőn.

Az elveszett mód engedélyezése után a rendszergazda az Eszköz megkeresése művelettel azonosíthatja az eszköz fizikai helyét.

Az Eszköz megkeresése művelet az Intune-ban együttműködik az iOS-eszközökkel egy adott eszköz helyének megjelenítéséhez a térképen.

A művelet használatához az iOS-készüléknek a következőkben kell lennie:

- Felügyelt mód
- Elveszett mód

További információ: [Elveszett mód engedélyezése iOS/iPadOS eszközökön az Intune-nal,](https://docs.microsoft.com/intune/device-lost-mode) és [az elveszett vagy ellopott iOS/iPadOS-eszközök megkeresése az Intune-nal.](https://docs.microsoft.com/intune/device-locate)

**GYIK**

K: Távoli műveletet adtam ki a vállalati adatok eszközről való eltávolítására, és most függőállapotban ragadt.

Válasz: Ahhoz, hogy egy távoli művelet sikeresen befejeződjen, a megcélzott eszköznek online és kifogástalan állapotúnak kell lennie. A következő esetekben a távoli művelet 30 napig függőállapotban marad, vagy amíg az eszköz nem nyugtázza a parancsot:

- Ha az eszköz nem rendelkezik kapcsolattal
- Amikor az eszköz elveszíti felügyeleti állapotát az Intune-nal

Ha úgy gondolja, hogy egy eszköz már nem jelentkezik be, és nem tudja eltávolítani a vállalati adatokat, válassza a Törlés lehetőséget. A törlés eltávolítja az eszközrekordot, így az már nem jelenik meg az Intune eszközök listájában. Ha az eszköz ismét aktívvá válik, a felhasználónak újra regisztrálnia kell azt.

K: Miért nem érhetők el bizonyos távoli műveletek?

A: Nem minden platform támogatja az összes távoli eszközműveletet. A következő távoli műveletek platformspecifikusak, így csak a megjegyzett platformokhoz érhetők el.

- Az aktiválási zár megkerülése (csak iOS)
- Új kezdet (csak Windows)
- Elveszett mód (csak iOS esetén)
- Az eszköz megkeresése (csak iOS esetén)
- Újraindítás (csak Windows)

Az egyes műveletekről további információt az [Elérhető eszközműveletek (Available device actions) (Elérhető eszközműveletek) (Elérhető eszközműveletek) (Elérhető eszközműveletek) (Elérhető eszközműveletek) (Elérhető eszköz](https://docs.microsoft.com/intune/device-management#available-device-actions)