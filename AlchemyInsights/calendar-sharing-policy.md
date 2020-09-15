---
title: 618 naptár-megosztási házirend
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684232"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Házirend-hiba a naptár megosztásakor

1. A helyzetnek megfelelően végezze el az alábbi műveletek egyikét:
    - Csatlakozás az Exchange Online-hoz távoli PowerShell használatával. További információt a [Csatlakozás az Exchange Online-hoz távoli PowerShell használatával](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)című témakörben talál.
    - Nyissa meg az Exchange Management shellt a helyszíni kiszolgálón.
2. Határozza meg a felhasználóhoz rendelt megosztási házirendet. Ehhez futtassa a következő parancsot, és jegyezze fel a visszaadott házirendet:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. A felhasználó megosztási házirendjének frissítése Ehhez hajtsa végre a következő lépéseket:
    - Nyissa meg az Exchange felügyeleti központot.
    - Kattintson a **szervezet**elemre, majd kattintson duplán arra a házirendre, amely az **Egyéni megosztás**csoportban van hozzárendelve a felhasználóhoz. Ez a házirend, amely a 2. lépésben tért vissza.
    - A megosztási szabály lapon válassza ki az engedélyezni kívánt naptár megosztási szintjét az **adja meg, hogy milyen információkat szeretne megosztani**; kattintson a **Mentés**gombra.

További információt a következő témakörben talál: ["a házirend nem engedélyezi az engedélyeket a címzett (ek) nek egy vagy több címzett számára" hibaüzenet jelenik meg, amikor a felhasználó megpróbálja megosztani a naptárat](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
