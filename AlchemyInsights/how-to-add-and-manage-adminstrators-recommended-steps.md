---
title: Rendszergazdák hozzáadása és kezelése – ajánlott lépések
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755837"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Rendszergazdák hozzáadása és kezelése – ajánlott lépések

A probléma leírása alapján megtalálunk egy megoldást. A legtöbb ügyfél saját maga oldhatja fel a problémát a dokumentációt követően.

**Az előfizetés-adminisztrátor vagy a munkatárs szerkesztése**

- A fiók rendszergazdája szerkesztheti mindkét szerepkört, míg az előfizetés rendszergazdája csak az [Azure portálon](https://ms.portal.azure.com/#home)tudja módosítani a rendszergazdákat.
- [Azure-előfizetés rendszergazdáinak hozzáadása vagy módosítása](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Az előfizetéses rendszergazda vagy a belső (LEVEGÕ) előfizetések Co-Administrator frissítése**

A szolgáltatás rendszergazdája vagy a társ-rendszergazda az alábbi lépésekkel hozhatja magával a műveletet:

1. Jelentkezzen be az [Azure-portálra](https://ms.portal.azure.com/#home) , és kattintson a **költség-kezelés + számlázás** elemre a bal oldali pengében.
2. Kattintson az előfizetéssel rendelkező sorba elemre. Ezzel megnyitja az előfizetés áttekintését.
3. Az **előfizetési** penge lapon kattintson a **Tulajdonságok** elemre. 
4. Kattintson a **szolgáltatás rendszergazdája** gombra.
5. Írja be annak a felhasználónak az e-mail-címét, akinek be szeretné állítani a szolgáltatás-rendszergazdaként választógombot, és kattintson **az OK gombra**.

**A rendszergazda hozzáadása/módosítása/eltávolítása**

1. Jelentkezzen be az [Azure portálra](https://ms.portal.azure.com/#home) szolgáltatás-rendszergazdaként.
2. Az [előfizetések](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) megnyitása (A társ-rendszergazdák csak az előfizetéses hatókörben rendelhetők hozzá.)
3. Navigálás a **következőben: hozzáférés-vezérlés (iam)** a  >  **klasszikus rendszergazdák**  >  **hozzáadásával**  >  a **társ-adminisztrátort** a Add **Co-** Administrator (ha le van tiltva a további rendszergazdai beállítás van letiltva)
4. Jelölje ki azt a felhasználót, akit fel szeretne venni, majd kattintson a **Hozzáadás** gombra.

**tudj meg többet:**
- [Rendszergazda hozzáadása](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Felügyelői munkatárs eltávolítása](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [A szolgáltatás rendszergazdájának módosítása](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [A fiók rendszergazdájának megtekintése](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Hozzáférés kezelése a RBAC és az Azure Portal segítségével](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Felhasználók hozzáadása és törlése az Azure Active Directory (AD) használatával**

Az Azure Active Directoryból (Azure AD) szervezetből új felhasználókat vehet fel, illetve törölheti a meglévő felhasználókat:

1. Új felhasználó hozzáadásához jelentkezzen be az Azure- [portálra](https://ms.portal.azure.com/#home) a szervezet felhasználói rendszergazdájaként.
2. Válassza az **Azure Active Directory** lehetőséget, válassza a **felhasználók** , majd az **új felhasználó** parancsot.
3. A **felhasználó** lapon adja meg a szükséges adatokat. Kattintson a **Létrehozás** gombra. A felhasználó létrehozta és felvette az Azure AD-bérlői webhelyére.

**További információ**:

- [Új felhasználó hozzáadása](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Felhasználó törlése](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Felhasználói profil adatainak hozzáadása vagy frissítése az Azure Active Directory segítségével](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Ajánlott dokumentumok**

- [Mi a szerepkör-alapú hozzáférés-vezérlés (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Az Azure-ban megjelenő különböző szerepkörök ismertetése](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Rendszergazdai szerepkör engedélyei az Azure Active Directoryban](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Oktatóprogram: hozzáférés biztosítása egy felhasználóhoz a RBAC és az Azure portál segítségével](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Az Azure RBAC hibaelhárítása](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Erőforrások rendszerezése Azure felügyeleti csoportokkal](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Az Azure-számlák másolatának kérése e-mailben](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Hitel-vagy bankkártya hozzáadása, frissítése vagy eltávolítása az Azure-ról](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Előfizetés kezelése (újraaktiválás/Mégse/kapcsoló)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



