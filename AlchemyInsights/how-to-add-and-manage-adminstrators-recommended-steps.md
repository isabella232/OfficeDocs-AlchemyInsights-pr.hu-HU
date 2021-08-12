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
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963789"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Rendszergazdák hozzáadása és kezelése – ajánlott lépések

A probléma leírása alapján megoldást találtunk az Ön számára. A legtöbb ügyfél a dokumentációt követően egyedül megoldotta a problémát.

**Az előfizetési rendszergazda vagy a társ-rendszergazda szerkesztése**

- A fiók rendszergazdája mindkét szerepkört szerkesztheti, míg az előfizetési rendszergazda csak a társ-rendszergazdákat módosíthatja az [Azure Portalon.](https://ms.portal.azure.com/#home)
- [Azure-előfizetés rendszergazdáinak hozzáadása vagy módosítása](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Az Előfizetés-rendszergazda vagy a Co-Administrator (AIRS) előfizetések frissítése**

A szolgáltatás rendszergazdája vagy a társ-rendszergazda saját maga is használhatja ezt a műveletet az alábbi lépésekkel:

1. Jelentkezzen be az [Azure Portalba, és](https://ms.portal.azure.com/#home) a bal oldali panelen kattintson a **Költségkezelés +** Számlázás elemre.
2. Kattintson az előfizetéssel kapcsolatos sortételre. Ezzel megnyitja az előfizetése Overview (Áttekintés) lapját.
3. Az Előfizetés **panelen** kattintson a Tulajdonságok **elemre.** 
4. Kattintson a **Szolgáltatás-rendszergazda gombra.**
5. Írja be annak a felhasználónak az e-mail-címét, akit szolgáltatás-rendszergazdaként be szeretne állítani, majd kattintson az **OK gombra.**

**Add/Change/Remove Co-administrator**

1. Jelentkezzen be az [Azure Portalba](https://ms.portal.azure.com/#home) szolgáltatás-rendszergazdaként.
2. Nyissa [meg az Előfizetések](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 2010-et, és válasszon egy előfizetést. (A társ-rendszergazdák csak az előfizetési hatókörben rendelhetők hozzá.)
3. Nyissa meg az **Access-vezérlő (IAM)** klasszikus rendszergazdáit: Adja hozzá a Rendszergazda hozzáadása lehetőséget a Társfelügyelő hozzáadása panel megnyitásához (Ha a Rendszergazda hozzáadása lehetőség le van tiltva, az azt jelenti, hogy Ön nem rendelkezik  >    >    >   engedélyekkel). 
4. Jelölje ki a hozzáadni kívánt felhasználót, és kattintson a Hozzáadás **gombra.**

**tudj meg többet:**
- [Társ-rendszergazda hozzáadása](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Társ-rendszergazda eltávolítása](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [A szolgáltatás rendszergazdájának módosítása](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [A fiók rendszergazdájának megtekintése](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Hozzáférés kezelése RBAC és Azure Portal használatával](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Felhasználók felvétele és törlése Azure Active Directory (AD) használatával**

Hozzáadhat új felhasználókat, vagy törölheti a meglévő felhasználókat a Azure Active Directory (Azure AD) szervezetből:

1. Új felhasználó hozzáadásához jelentkezzen be az [Azure Portalra](https://ms.portal.azure.com/#home) a szervezet rendszergazdájaként.
2. Válassza **Azure Active Directory**, válassza a **Felhasználók,** majd az Új **felhasználó lehetőséget.**
3. A Felhasználó **lapon** adja meg a szükséges adatokat. Kattintson a **Létrehozás gombra.** A felhasználó létrejön, és hozzáadódik az Ön Azure AD-bérlőjéhez.

**További információ:**

- [Új felhasználó hozzáadása](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Felhasználó törlése](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Felhasználók profilinformációinak hozzáadása vagy frissítése a Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Ajánlott dokumentumok**

- [Mit jelent a szerepköralapú hozzáférés-vezérlés?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [A különböző szerepkörök az Azure-ban](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Rendszergazdai szerepkör engedélyei a Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Oktatóprogram: Hozzáférés megadása egy felhasználónak az RBAC és az Azure Portal használatával](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Az RbAC hibaelhárítása az Azure-ban](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Az erőforrások rendszerezése Azure felügyeleti csoportokkal](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Azure-számla másolatának kérése e-mailben](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Hitelkártya vagy bankkártya hozzáadása, frissítése vagy eltávolítása az Azure-ból](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Előfizetés kezelése (újraaktiválás/lemondás/váltás)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



