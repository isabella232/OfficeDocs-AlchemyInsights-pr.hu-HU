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
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895181"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>A postaláda továbbítási beállításának kiderítésében és a

Ha a külső továbbítás be van állítva egy postaládában, a tevékenység naplózása a **Postaláda-halmaz** parancsmag részeként történik. Így találhatja meg a tevékenységet a naplóban:

1. Az alábbi műveletek közül választhat:
   - A Microsoft 365 Megfelelőségi központ a <https://compliance.microsoft.com> Megoldásvizsgálat  \> **hoz.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://compliance.microsoft.com/auditlogsearch> használja: .
   - A (Microsoft 365 Defender) portálon a <https://security.microsoft.com> Audit **(Naplózás) stb.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://security.microsoft.com/auditlogsearch> használja: .

   > [!NOTE]
   > Ha egy figyelmeztetést lát, amely szerint be kell kapcsolnia a naplózást, nyugodtan bekapcsolhatja most. Ha ez a funkció nincs bekapcsolva, a keresési eredmények nem tudnak adatokat bekeresni a korábbi dátumok adataiból.

2. A Naplózás **lapon** ellenőrizze,  hogy a Keresés lap van-e kiválasztva, majd adja meg az alábbi beállításokat:
   - Jelölje ki a dátum-/időtartományt a **Kezdő és** a **Záró** mezőben.
   - Ellenőrizze, **hogy a Tevékenységek mező** tartalmazza-e Az összes tevékenység **eredményének megjelenítése mezőt.**

3. Ha végzett, kattintson a Keresés **gombra.** A tevékenységek az új Naplókeresés **lapon jelennek** meg.

4. Az eredmények között kattintson a **Tevékenység** oszlopra az eredmények rendezéséhez, és keresse meg a Postaláda **beállítása** bejegyzéseket.

5. Jelöljön ki egy tevékenységet az eredmények között a részleteket tartalmazó úszó panel megnyitásához. Az egyes naplórekordok részleteiben kell megállapítania, hogy a tevékenység kapcsolódik-e az e-mail-továbbításhoz:
   - **ObjectId:** A módosított postaláda aliasértéke.
   - **Paraméterek:** _A ForwardingSmtpAddress_ a cél e-mail-címet jelzi.
   - **UserId:** Az **ObjectId** mező postaládájában e-mail-továbbítást konfiguráló felhasználó.

További információ: Annak megállapítása, hogy ki állíthatja be az e-mail-továbbítást [egy postaládában.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
