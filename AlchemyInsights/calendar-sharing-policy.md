---
title: 618 Naptármegosztási szabályzat
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373001"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Házirendhiba naptár megosztásakor

1. Az adott helyzetnek megfelelően tegye a következők egyikét:
    - Csatlakozzon az Exchange Online-hoz a Távoli PowerShell használatával. További információt a [Csatlakozás az Exchange Online-hoz távoli PowerShell használatával című](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)témakörben talál.
    - A helyszíni kiszolgálón nyissa meg az Exchange Management Shell t.
2. Határozza meg a felhasználóhoz rendelt megosztási házirendet. Ehhez futtassa a következő parancsot, és vegye figyelembe a visszaadott házirendet:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Frissítse a felhasználó megosztási házirendjeit. Ehhez kövesse az alábbi lépéseket:
    - Nyissa meg az Exchange Felügyeleti központot.
    - Kattintson a **Szervezet**elemre, majd kattintson duplán arra a házirendre, amely az Egyéni megosztás csoportban van a felhasználóhoz **rendelve.** Ez az a házirend, amelyet a 2.
    - A Megosztási szabály lapon jelölje ki a megosztani kívánt **adatok megadása**csoportban az engedélyezni kívánt naptármegosztási szintet. kattintson a **Mentés gombra.**

További információ: ["A házirend nem engedélyezi az engedélyek megadását ezen a szinten egy vagy több címzett(ek)nek" hibaüzenet jelenik](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)meg, amikor a felhasználó megpróbálja megosztani a naptárat.
