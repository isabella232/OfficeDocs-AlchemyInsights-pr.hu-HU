---
title: Az IP-cím megkeresés a naplóban
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 258e92368b8a33e8ea807f0cb9af90132c86ed5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58303579"
---
# <a name="find-the-ip-address-in-audit-log"></a>Az IP-cím megkeresés a naplóban

A naplókban az IP-cím látható, amely egy felhasználó vagy rendszergazda által végrehajtott tevékenységnek felel meg. A program az ügyféladatokat is naplózza. Így azonosíthatja az IP-címet:

1. Az alábbi műveletek közül választhat:
   - A Microsoft 365 Megfelelőségi központ a <https://compliance.microsoft.com> Megoldásvizsgálat  \> **ot.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://compliance.microsoft.com/auditlogsearch> használja: .
   - A (Microsoft 365 Defender) portálon a <https://security.microsoft.com> Audit **(Naplózás) stb.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://security.microsoft.com/auditlogsearch> használja: .

    **Megjegyzés:** Ha egy figyelmeztetést lát, amely szerint be kell kapcsolnia a naplózást, nyugodtan bekapcsolhatja most. Ha ez a funkció nincs engedélyezve, a keresési eredmények nem tudnak adatokat lekért a korábbi dátumok adataiból.

2. A Naplózás **lapon** ellenőrizze,  hogy a Keresés lap van-e kiválasztva, majd adja meg az alábbi beállításokat:
   - **Dátum- és időtartomány:** Válassza ki a dátum-/időtartományt a **Kezdő** és a **Záró** mezőben.
   - **Tevékenységek:** Ha egy adott tevékenység érdekli, válassza ki azt a listából; ellenkező esetben az  összes tevékenység eredményének megjelenítése alapértelmezett érték az összes tevékenységet visszaadja. Felhívjuk a figyelmét arra, hogy egyes tevékenységek nem érhetők el a kijelöléshez; azonban ezeket a naplóelemeket fogja visszaadni a rendszer, ha az Összes tevékenység **eredményének** megjelenítése jelölőnégyzet be van jelölve.
   - **Felhasználók:** Fogadja el az üres alapértelmezett értéket, és adja meg az összes felhasználó találatát, vagy adjon meg egy vagy több felhasználót.

3. Ha végzett, kattintson a Keresés **gombra.** A tevékenységek az új Naplókeresés **lapon jelennek** meg.

4. A találatok között kattintson az Eredmények **szűrése elemre,** és írja be a **Set-Mailbox (Postaláda beállítása)** mezőt a tevékenységszűrő mezőbe.

5. Jelöljön ki egy naplórekordot az eredmények között a **Részletek úszó** panel megnyitásához.

További információt a Keresés a naplóban a gyakori támogatási problémák [vizsgálatához.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
