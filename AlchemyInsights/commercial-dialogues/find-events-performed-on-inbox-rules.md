---
title: A beérkezett üzenetekre vonatkozó szabályokon végrehajtott események megkeresése
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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313501"
---
# <a name="find-events-performed-on-inbox-rules"></a>A beérkezett üzenetekre vonatkozó szabályokon végrehajtott események megkeresése

A beérkezett üzenetekre vonatkozó szabályok létrehozásakor, létrehozásakor, illetve törlésekor a program rögzíti az eseményeket a naplóban. Ezeket a következőt kell áttekinteni:

1. Az alábbi műveletek közül választhat:
   - A Microsoft 365 Megfelelőségi központ a <https://compliance.microsoft.com> Megoldásvizsgálat  \> **ot.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://compliance.microsoft.com/auditlogsearch> használja: .
   - A (Microsoft 365 Defender) portálon a <https://security.microsoft.com> Audit **(Naplózás) stb.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://security.microsoft.com/auditlogsearch> használja: .

    **Megjegyzés:** Ha egy figyelmeztetést lát, amely szerint be kell kapcsolnia a naplózást, nyugodtan bekapcsolhatja most. Ha ez a funkció nincs bekapcsolva, a keresési eredmények nem tudnak adatokat bekeresni a korábbi dátumok adataiból.
1. Jelölje ki a Tevékenységek mezőt, keresse meg Exchange postaláda-tevékenységeket, majd New-InboxRule Levelezési szabály létrehozása a Outlook Web App. Amikor végzett, kattintson az ablaktáblán kívülre a Tevékenységek ablaktábla kis méretűvé állításhoz.
1. Adja meg a dátumtartományt, majd a Felhasználók mezőben válassza ki a vizsgálni kívánt felhasználó felhasználónevét. Egyszerre több felhasználót is kijelölhet.
1. Válassza a Keresés lehetőséget. A tevékenységek az Eredmények alatt jelennek meg.
1. A részletek megtekintéséhez jelöljön ki egy tevékenységet, majd válassza a További információ lehetőséget. A Parameters (Paraméterek) szakaszban láthatja a szabály nevét, a beállított feltételeket, valamint a szabály által végretért műveleteket.

2. A Naplózás **lap** Keresés **lapján** adja meg az alábbi beállításokat:
   - **Dátum- és időtartomány:** Válassza ki a dátum-/időtartományt a **Kezdő** és a **Záró** mezőben.
   - **Tevékenységek:** Válassza **az Új-Beérkezett üzenetekRule Beérkezett** üzenetek szabály létrehozása lehetőséget a Outlook Web App

3. Ha végzett, kattintson a Keresés **gombra.** A tevékenységek az új Naplókeresés **lapon jelennek** meg.

4. Jelöljön ki egy tevékenységet az eredmények között a részleteket tartalmazó úszó panel megnyitásához. A Parameters **(Paraméterek)** szakaszban láthatja a szabály nevét, a beállított feltételeket, valamint a szabály által végretért műveleteket.

További információért olvassa el a Keresés a naplóban a [gyakori támogatási problémák vizsgálatához.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
