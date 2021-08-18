---
title: A törölt események naplóinak olvasása
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324735"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>A törölt események naplóinak olvasása

Ehhez tegye a következőt:

1. Az alábbi műveletek közül választhat:
   - A Microsoft 365 Megfelelőségi központ a <https://compliance.microsoft.com> Megoldásvizsgálat  \> **ot.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://compliance.microsoft.com/auditlogsearch> használja: .
   - A (Microsoft 365 Defender) portálon a <https://security.microsoft.com> Audit **(Naplózás) stb.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://security.microsoft.com/auditlogsearch> használja: .

    **Megjegyzés:** Ha egy figyelmeztetést lát, amely szerint be kell kapcsolnia a funkciót, nyugodtan bekapcsolhatja most. Ha a funkció nincs bekapcsolva, a keresési eredmények nem tudnak adatokat lekért a korábbi dátumokhoz.

2. A Naplózás **lap** Keresés **lapján** adja meg az alábbi beállításokat:
   - **Dátum- és időtartomány:** Válassza ki a dátum-/időtartományt a **Kezdő** és a **Záró** mezőben.
   - **Tevékenységek:** Adja meg **Exchange postaláda-tevékenységeket,** majd válassza ki az alábbi értékeket:
     - **Törölt üzenetek a Törölt elemek mappából**
     - **Üzenetek átkerültek a Törölt elemek mappába**

       Amikor végzett, kattintson az ablaktáblán kívülre a Tevékenységek ablaktábla kis **méretűvé állításhoz.**

   - **Felhasználók:** Fogadja el az üres alapértelmezett értéket, és adja meg az összes felhasználó találatát, vagy adjon meg egy vagy több felhasználót.

3. Ha végzett, kattintson a Keresés **gombra.** A tevékenységek az új Naplókeresés **lapon jelennek** meg.

4. Jelöljön ki egy tevékenységet az eredmények között a részleteket tartalmazó úszó panel megnyitásához. A Törölt elemek mezőben további információk jelennek meg a törölt elemről, például a tárgysorról és az elem törlés utáni **helyéről.**

   **Megjegyzés:** A napló funkcióval nem lehet visszaállítani a törölt elemeket. A törölt elemek visszaállításáról a [Törölt](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)e-mailek helyreállítása a Webes Outlook.

További információt a Keresés a naplóban a gyakori támogatási problémák [vizsgálatához.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
