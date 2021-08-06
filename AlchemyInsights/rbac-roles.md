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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923133"
---
# <a name="rbac-rules"></a>RBAC-szabályok

Ha az engedélyre vonatkozó hibaüzenet jelenik meg: 

- Az objektumazonosítóval rendelkező ügyfélnek nincs engedélye a műveletek elvégzésére hatókör **(kód: AuthorizationFailed) esetén:** amikor erőforrást próbál létrehozni, ellenőrizze, hogy be van-e jelentkezve egy olyan felhasználóval, aki írási engedéllyel rendelkezik a választott hatókörben lévő erőforráshoz. Egy erőforráscsoport virtuális gépeit például az erőforráscsoport [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) virtuális számítógép-közreműködői szerepkörével (vagy szülőhatókörével) kell felügyelni. Az egyes beépített szerepkörök engedélyeinek listáját Az [Azure-erőforrások](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)beépített szerepkörei.
- Nincs engedélye támogatási kérelem létrehozására: ha támogatási jegyet próbál létrehozni vagy frissíteni, ellenőrizze, hogy be van-e jelentkezve egy Olyan felhasználónál, aki microsoft.support/supportTickets/write engedéllyel rendelkezik (például támogatási kérelem közreműködője). [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Nem lehet több szerepkör-hozzárendelést **létrehozni (kód: RoleAssignmentLimitExceeded):** Amikor megpróbál hozzárendelni egy szerepkört, próbáljon meg csökkenteni a szerepkör-hozzárendelések számát úgy, hogy ehelyett szerepköröket rendel a csoportokhoz. Az Azure előfizetésenként **legfeljebb 2000** szerepkör-hozzárendelést támogat.

Az Azure RBAC-szerepkörökről további információt Az [Azure RBAC-szerepkörök](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)szolgáltatásban talál.
