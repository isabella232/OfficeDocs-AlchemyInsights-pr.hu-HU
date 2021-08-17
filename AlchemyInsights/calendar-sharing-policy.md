---
title: 618 Naptármegosztási házirend
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091605"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Házirendhiba naptárak megosztásakor

1. A helyzetnek megfelelően tegye az alábbiak egyikét:
    - Csatlakozás a Exchange Online PowerShell használatával. További információt a Távoli [PowerShell Csatlakozás Exchange Online történő használatának be-](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)és Exchange Online.
    - A helyszíni kiszolgálón nyissa meg a Exchange Management Shellt.
2. Határozza meg a felhasználóhoz rendelt megosztási házirendet. Ehhez futtassa az alábbi parancsot, és jegyezze fel a visszaadott házirendet:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Frissítse a felhasználó megosztási házirendját. Ehhez hajtsa végre a következő lépéseket:
    - Nyissa meg Exchange Felügyeleti központot.
    - Kattintson **a Szervezet** elemre, majd kattintson duplán a felhasználóhoz rendelt házirendre az Egyéni megosztás **csoportban.** Ez a 2. lépésben visszaadott házirend.
    - A Megosztási szabály lapon válassza ki az engedélyezni kívánt naptármegosztási szintet a Megosztani kívánt **információk megadása csoportban;** kattintson a **Mentés gombra.**

További információ: "A házirend nem teszi lehetővé engedélyek megadását ezen a szinten egy vagy több [címzett(k)nek"](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)hibaüzenet jelenik meg, amikor a felhasználó megpróbálja megosztani a naptárt.
