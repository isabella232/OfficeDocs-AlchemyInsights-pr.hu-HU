---
title: A felhasználók összes tevékenységének kivizsgálása
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332345"
---
# <a name="investigate-all-the-users-activities"></a>A felhasználók összes tevékenységének kivizsgálása

Ehhez tegye a következőt:

1. Az alábbi műveletek közül választhat:
   - A Microsoft 365 Megfelelőségi központ a <https://compliance.microsoft.com> Megoldásvizsgálat  \> **ot.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://compliance.microsoft.com/auditlogsearch> használja: .
   - A (Microsoft 365 Defender) portálon a <https://security.microsoft.com> Audit **(Naplózás) stb.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://security.microsoft.com/auditlogsearch> használja: .

    **Megjegyzés:** Ha egy figyelmeztetést lát, amely szerint be kell kapcsolnia a funkciót, nyugodtan bekapcsolhatja most. Ha a funkció nincs bekapcsolva, a keresési eredmények nem tudnak adatokat lekért a korábbi dátumokhoz.

2. A Naplózás **lap** Keresés **lapján** adja meg az alábbi beállításokat:
   - **Dátum- és időtartomány:** Válassza ki a dátum-/időtartományt a **Kezdő** és a **Záró** mezőben.
   - **Tevékenységek:** Ha egy adott tevékenység érdekli, válassza ki azt a listából; ellenkező esetben az Összes **tevékenység** eredményének megjelenítése alapértelmezett érték az összes tevékenységet visszaadja.
   - **Felhasználók:** Fogadja el az üres alapértelmezett értéket, és adja meg az összes felhasználó találatát, vagy adjon meg egy vagy több felhasználót.

3. Ha végzett, kattintson a Keresés **gombra.** A tevékenységek az új Naplókeresés **lapon jelennek** meg. Itt látható az **IP-cím, a** **Felhasználó** és **a Tevékenység** neve.

4. Az eredmények letöltéséhez válassza **Az összes eredmény** letöltése \> **lehetőséget.**

5. Jelöljön ki egy tevékenységet az eredmények között a részleteket tartalmazó úszó panel megnyitásához.

További információért olvassa el a Keresés a naplóban a [gyakori támogatási problémák vizsgálatához.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
