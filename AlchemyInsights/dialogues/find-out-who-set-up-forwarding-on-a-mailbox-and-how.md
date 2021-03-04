---
title: Tudja meg, hogy ki állíthatja be az továbbítást a postaládában, és hogyan
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429615"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Tudja meg, hogy ki állíthatja be az továbbítást a postaládában, és hogyan

Ha a külső továbbítás be van állítva egy postaládában, a tevékenység a Set-Mailbox részeként lesz naplózásra. Így találhatja meg a tevékenységet a naplóban:

1. Menjen az [Office 365 Biztonsági & megfelelőségi központba.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Válassza **a Keresés** >  **naplókeresés lehetőséget.**
    > [!NOTE]
    > Ha egy figyelmeztetést lát, amely szerint be kell kapcsolnia a naplózást, akkor most kapcsolja be. Ha ez a funkció nincs bekapcsolva, a keresési eredmények nem fogják tudni lekeresni az előző dátumok adatait.
1. Győződjön meg arról, **hogy a Tevékenységek** mezőben az összes tevékenység eredményének megjelenítése (az alapértelmezett beállítás) van megjelölve.  Adja meg a dátumtartományt. Nem kell megadnia a felhasználónevet.
1. Válassza a **Keresés lehetőséget.** A tevékenységek az Eredmények **alatt jelennek meg.**
1. Válassza **az Eredmények szűrése** lehetőséget, majd írja be a **Set-mailbox** mezőt a **Tevékenységszűrő** mezőbe. Ez az összes **Set-Mailbox-tevékenységet visszaadja.**
1. A részletek megtekintéséhez jelöljön ki egy tevékenységet, majd válassza a **További információ lehetőséget.** A **Paraméterek alatt** láthatja a postaládában beállított továbbítási e-mail-címet. A **UserID** az a felhasználó, aki külső továbbítást beállított a postaládában.
További információért olvassa el a Keresés az [Office 365 naplójában](https://go.microsoft.com/fwlink/?linkid=2103944)a gyakori esetek elhárításához.