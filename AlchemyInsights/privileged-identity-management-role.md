---
title: Privilegizált identitás-kezelési szerepkör
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088882"
---
# <a name="privileged-identity-managementpim-role"></a>Jogosultsági jogosultságok kezelése (PIM) szerepkör

**A szerepkör aktiválása után a rendszer nem biztosít engedélyeket**

Ha aktiválja az Azure AD privilegizált Identitáskezelő (PIM) szerepkörét, előfordulhat, hogy az aktiválás nem terjed ki azonnal az összes olyan portálra, amely a kiváltságos szerepkört igényli. Előfordulhat, hogy a módosítás propagálása még akkor is, ha a módosítás nem azonnal lép életbe a portálon.

Ha késik az aktiválás, kövesse az alábbi lépéseket:

1. Kijelentkezhet az Azure portálról, majd ismét bejelentkezhet. Az Azure AD szerepkör vagy az Azure Resource szerepkör aktiválása után az aktiválás szakaszai láthatók. Miután minden szakasz befejeződött, megjelenik egy "kijelentkezés" hivatkozás. Ez a hivatkozás a kijelentkezésre használható. Ez megoldja a legtöbb esetet az aktiválás késleltetése során.
2. A PIM-ban győződjön meg arról, hogy a szerepkör tagjaként szerepel a listában.
3. Ha aktiválja az Exchange-rendszergazdai szerepkört, győződjön meg arról, hogy kijelentkezik, majd újra bejelentkezik. Ha a probléma nem szűnik meg, nyisson meg egy támogatási jegyet, és emelje fel ezt a problémát. Ha az Exchange-rendszergazda szerepkört használja a biztonsági és megfelelőségi központ eléréséhez, olvassa el a következő lépést.
4. Ha egy szerepkört aktivál a biztonsági és megfelelőségi központ eléréséhez, vagy ha aktiválja a SharePoint-rendszergazdai szerepkört, néhány perccel az aktiválási késleltetést néhány percen belül megtapasztalhatja. Ez egy ismert probléma, és aktívan dolgozunk ezekkel a csapatokkal a probléma mielőbbi megoldásához.

További információ:

- [Az Azure AD-szerepkörök aktiválása a PIM-ban](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Az Azure Resource-szerepkörök aktiválása a PIM-ban](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Az engedélyek nem törlődnek a szerepkör inaktiválása vagy a szerepkör-aktiválás lejárta után**

Ha inaktiválja az Azure AD-jogosultságok kezelésének szerepkörét, vagy ha lejár egy szerepkör-aktiválási időszak, akkor lehet, hogy késés van, ahol továbbra is hozzáférése van.

Ha késik a deaktiválása, kövesse az alábbi lépéseket:

1. Ha inaktívvá teszi az Exchange-rendszergazdai szerepkört vagy a szerepkör-aktiválási időszakot, és jelentős késést tapasztal az engedélyek eltávolítása előtt, nyisson meg egy támogatási jegyet, és mondja el a támogatási szakemberének, hogy segítsen Önnek jegyet benyújtani az Office-ban az Office-szal kapcsolatos kiváltságos hozzáférés-kezelési (PAM) csapattal.
2. Ha az aktiválási időszak lejárt, de továbbra is meg van nyitva a böngészési folyamat, zárja be a böngészőt. Addig is használhatja a szerepkört, amíg be nem zárja a munkamenetet. Ez egy ismert probléma, és az aktiválás lejárta után egy esetleges javítást keresünk.

Ha a késése eltér a két forgatókönyvtől, kérjük, nyisson meg egy támogatási jegyet.
