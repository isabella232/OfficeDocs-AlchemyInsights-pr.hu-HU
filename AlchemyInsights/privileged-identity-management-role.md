---
title: Privileged Identity Management szerepkör
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973231"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM) szerepkör

**Jogosultságok nem adhatók meg a szerepkör aktiválása után**

Amikor aktivál egy szerepkört az Azure AD Privileged Identity Management (PIM) szolgáltatásban, előfordulhat, hogy az aktiválás nem propagálható azonnal az összes olyan portálon, amely szükséges a jogosultsági szerepkörhöz. Néha még a módosítás propagálása esetén is előfordulhat, hogy a portálon való webes gyorsítótárazás azt eredményezi, hogy a módosítás nem lép azonnal hatályba.

Ha az aktiválás késik, kövesse az alábbi lépéseket:

1. Jelentkezzen ki az Azure Portalról, majd jelentkezzen be újra. Azure AD-szerepkör vagy Azure-erőforrás-szerepkör aktiválásakor láthatja az aktiválás fázisokat. Ha az összes szakasz elkészült, látni fog egy Kijelentkezás hivatkozást. Erre a hivatkozásra kattintva kijelentkezhet. Ez megoldja a legtöbb esetben az aktiválási késleltetést.
2. A PiM-listában ellenőrizze, hogy Ön szerepel-e a szerepkörben.
3. Ha a rendszergazdai rendszergazdai Exchange, jelentkezzen ki, majd jelentkezzen be újra. Ha a probléma nem szűnik meg, nyisson egy támogatási jegyet, és emelje fel a problémát. Ha a Biztonsági és megfelelőségi központ Exchange rendszergazdai szerepkört használja, tekintse meg a következő lépést.
4. Ha a Biztonsági és megfelelőségi központ eléréséhez aktivál egy szerepkört, vagy ha az SharePoint Rendszergazda szerepkört aktiválja, néhány perctől néhány óráig némi aktiválási késleltetést tapasztal. Ez egy ismert probléma, és aktívan dolgozunk ezekkel a csoportokkal a probléma lehető leghamarabbi megoldása érdekében.

További információ:

- [Azure AD-szerepkörök aktiválása a felhasználói környezetben](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Azure-erőforrás-szerepkörök aktiválása a piM-ban](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**A szerepkör inaktiválásának vagy a szerepkör aktiválásának lejárata után a rendszer nem távolítja el az engedélyeket.**

Ha inaktivál egy szerepkört az Azure AD-ban Privileged Identity Management vagy lejár egy szerepkör aktiválási időszaka, előfordulhat, hogy egy késedelem, amikor továbbra is hozzáfér.

Ha az inaktiválás késik, kövesse az alábbi lépéseket:

1. Ha a Exchange-rendszergazdai szerepkört inaktiválja, vagy ha lejár a szerepkör aktiválási időszaka, és jelentős késést figyel fel az engedélyek eltávolítása előtt, nyisson egy támogatási jegyet, és mondja meg a támogatási szakembernek, hogy segítsen a jogosultsággal rendelkező hozzáférés kezelését (PAM) Office-csoportnál a hiba érvénybe lépéséhez.
2. Ha az aktiválási időszak lejárt, de még meg van nyitva a böngésző munkamenete, zárja be a böngészőt. A szerepkört mindaddig használhatja, amíg be nem zárja a munkamenetet. Ez egy ismert probléma, és jelenleg egy lehetséges javítást folytatunk annak érdekében, hogy az aktiválás lejárta után aktívan visszavonjuk az egyes munkameneteket.

Ha a késése eltér a fenti két helyzettől, nyisson egy támogatási jegyet.
