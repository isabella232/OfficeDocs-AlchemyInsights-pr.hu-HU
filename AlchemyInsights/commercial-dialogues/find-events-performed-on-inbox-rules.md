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
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882637"
---
# <a name="find-events-performed-on-inbox-rules"></a>A beérkezett üzenetekre vonatkozó szabályokon végrehajtott események megkeresése

A beérkezett üzenetekre vonatkozó szabályok létrehozásakor, létrehozásakor, illetve törlésekor a program rögzíti az eseményeket a naplóban. Ezeket a következőt kell áttekinteni:

1. Az alábbi műveletek közül választhat:
   - A Microsoft 365 Megfelelőségi központ a <https://compliance.microsoft.com> Megoldásvizsgálat  \> **hoz.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://compliance.microsoft.com/auditlogsearch> használja: .
   - A (Microsoft 365 Defender) portálon a <https://security.microsoft.com> Audit **(Naplózás) stb.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://security.microsoft.com/auditlogsearch> használja: .

    > [!NOTE]
    > Ha egy figyelmeztetést lát, amely szerint be kell kapcsolnia a naplózást, nyugodtan bekapcsolhatja most. Ha ez a funkció nincs bekapcsolva, a keresési eredmények nem tudnak adatokat bekeresni a korábbi dátumok adataiból.

2. A Naplózás **lap** Keresés **lapján** adja meg az alábbi beállításokat:
   - **Dátum- és időtartomány:** Válassza ki a dátum-/időtartományt a **Kezdő** és a **Záró** mezőben.
   - **Tevékenységek:** Válassza **a Beérkezett üzenetek** szabály létrehozása lehetőséget a Outlook Web App

3. Ha végzett, kattintson a Keresés **gombra.** A tevékenységek az új Naplókeresés **lapon jelennek** meg.

4. Jelöljön ki egy tevékenységet az eredmények között a részleteket tartalmazó úszó panel megnyitásához. A Parameters **(Paraméterek)** szakaszban láthatja a szabály nevét, a beállított feltételeket, valamint a szabály által végretért műveleteket.

További információért olvassa el a Keresés a naplóban a [gyakori támogatási problémák vizsgálatához.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
