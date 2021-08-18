---
title: Külső e-mail-továbbítás azonosítása a naplók postaládáiban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2af731bc9a1e28e2db7c6662041b930e1b05be4c3bf8340784d9ab87101c44af
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899886"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Annak azonosítása, hogy a külső e-mail-továbbítás mikor van beállítva a postaládákban

Amikor egy Microsoft 365 konfigurálja a külső **e-mail-továbbítást** egy postaládán, a tevékenység a Postaláda-halmaz parancsmag részeként lesz naplóállítva. A tevékenységet naplókereséssel is láthatja. Ezt a hogyan lehet megtenni.

1. Tegye a következők valamelyikét:
   - A Microsoft 365 Megfelelőségi központ a <https://compliance.microsoft.com> Megoldásvizsgálat  \> **ot.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://compliance.microsoft.com/auditlogsearch> használja: .
   - A (Microsoft 365 Defender) portálon a <https://security.microsoft.com> Audit **(Naplózás) hoz kell indulni.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://sip.security.microsoft.com/auditlogsearch> használja: .

2. A Naplózás **lapon** ellenőrizze,  hogy a Keresés lap van-e kiválasztva, majd adja meg az alábbi beállításokat:
   - Jelölje ki a dátum-/időtartományt a **Kezdő és** a **Záró** mezőben.
   - Ellenőrizze, **hogy a Tevékenységek mező** tartalmazza-e Az összes tevékenység **eredményének megjelenítése mezőt.**

3. Ha végzett, kattintson a Keresés **gombra.** A tevékenységek az új Naplókeresés **lapon jelennek** meg.

4. A találatok között kattintson az Eredmények **szűrése elemre,** és írja be a **Set-Mailbox (Postaláda beállítása)** mezőt a tevékenységszűrő mezőbe.

5. Jelöljön ki egy naplórekordot az eredmények között. A Részletek **úszó panelen** kattintson a További **információ elemre.** Az egyes naplórekordok részleteiben kell megállapítania, hogy a tevékenység kapcsolódik-e az e-mail-továbbításhoz.

   - **ObjectId:** A módosított postaláda aliasértéke.
   - **Paraméterek:** _A ForwardingSmtpAddress_ a cél e-mail-címet jelzi.
   - **UserId:** Az **ObjectId** mező postaládájában e-mail-továbbítást konfiguráló felhasználó.

További információ: Annak megállapítása, hogy ki állíthatja be az e-mail-továbbítást [egy postaládában.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
