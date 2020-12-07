---
title: 'RBAC szerepkörök '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583547"
---
# <a name="rbac-rules"></a>RBAC szabályok

Ha az engedélyről tájékoztató hibaüzenet jelenik meg: 

- **Az objektum-azonosítóval rendelkező ügyfél nem engedélyezte a hatókör feletti műveletet (kód: AuthorizationFailed)**: amikor megkísérel létrehozni egy erőforrást, ellenőrizze, hogy van-e bejelentkezve olyan felhasználóval, akinek van írási engedélye az erőforráshoz a kijelölt hatókörben. Ha például egy erőforráscsoport virtuális számítógépeit szeretné kezelni, akkor a [virtuális gép közreműködői](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) szerepkört kell tartalmaznia az erőforráscsoport (vagy a szülő hatóköre) számára. Az egyes beépített szerepkörök engedélyeinek listáját a [beépített szerepkörök az Azure-források esetében](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)című témakörben találhatja meg.
- **Nincs engedélye arra, hogy támogatási kérést hozzon létre**: Ha egy támogatási jegyet próbál létrehozni vagy frissíteni, ellenőrizze, hogy jelenleg be van-e jelentkezve egy olyan felhasználóval, akinek van hozzárendelve a Microsoft. support/supportTickets/írási engedélye (például [támogatási kérelem munkatárs](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)).
- **Nem hozhatók létre több szerepkör-hozzárendelés (kód: RoleAssignmentLimitExceeded)**: amikor megpróbál hozzárendelni egy szerepkört, próbálja meg csökkenteni a szerepkör-hozzárendelések számát úgy, hogy a szerepköröket kiosztja a csoportokba. Az Azure támogatja az **2000** szerepkör-hozzárendeléseinek előfizetését.

Az Azure RBAC szerepköreiről további információt az [Azure RBAC szerepkörei](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)című témakörben talál.
