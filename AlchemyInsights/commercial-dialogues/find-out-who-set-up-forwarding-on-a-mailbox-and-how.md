---
title: A postaláda továbbítási beállításának kiderítésében és a
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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988204"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>A postaláda továbbítási beállításának kiderítésében és a

Ha a külső továbbítás be van állítva egy postaládában, a tevékenység naplózása a Set-Mailbox részeként történik. Így találhatja meg a tevékenységet a naplóban:

1. A biztonsági Office 365 [megfelelőségi & meg.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Válassza **a Keresés** >  **naplókeresés lehetőséget.**
    > [!NOTE]
    > Ha egy figyelmeztetést lát, amely szerint be kell kapcsolnia a naplózást, nyugodtan bekapcsolhatja most. Ha ez a funkció nincs bekapcsolva, a keresési eredmények nem tudnak adatokat bekeresni a korábbi dátumok adataiból.
1. Győződjön meg **arról,** hogy a Tevékenységek mezőben Az összes tevékenység **eredményének** megjelenítése beállítás van megjelölve (ez az alapértelmezett). Adja meg a dátumtartományt. Nem kell megadnia a felhasználónevet.
1. Válassza a **Keresés lehetőséget.** A tevékenységek az Eredmények alatt **jelennek meg.**
1. Válassza **az Eredmények szűrése** lehetőséget, majd írja be a **Set-mailbox (Postaláda beállítása)** mezőt **a Tevékenység** szűrőmezőbe. Ez a beállítási **postaládával kapcsolatos összes tevékenységet visszaadja.**
1. A részletek megtekintéséhez jelöljön ki egy tevékenységet, majd válassza a **További információ lehetőséget.** A **Paraméterek** alatt láthatja a postaládában beállított továbbítási e-mail-címet. A **UserID** azonosító azt a felhasználót jelenti, aki külső továbbítást beállított a postaládában.
További információért olvassa el a Keresés a naplóban Office 365 gyakori esetek [elhárításához témakört.](https://go.microsoft.com/fwlink/?linkid=2103944)