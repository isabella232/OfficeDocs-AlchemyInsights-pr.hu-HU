---
title: Problémák az Intune felügyeleti konzoljának használatával
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555383"
---
# <a name="problems-using-the-intune-admin-console"></a>Problémák az Intune felügyeleti konzoljának használatával

**"Hozzáférés megtagadva" az Intune felügyeleti portálján való navigáláskor.**

- Ha egy Intune-alapú egyéni szerepkör tagja, győződjön meg arról, hogy egy Intune-vagy Enterprise Mobility Suite (EMS) licenc van hozzárendelve a fiókjához.
- Ha a Configuration Manager segítségével kezeli az eszközöket, ellenőrizze, hogy nem tagja-e az Intune MDM-nek az Intune felhasználói gyűjteményében.
- Ellenőrizze, hogy rendelkezik-e a megfelelő szerepköralapú felügyeleti vezérlő (RBAC) engedélyekkel az Intune szerepkörök panelen.
- Ellenőrizze, hogy a használt csoport nem terjesztési lista-e. Az Intune az Azure Portalon csak az Azure Active Directory biztonsági csoportjaihoz tartozó felhasználói fiókokat támogatja. Tekintse át a csoportokat az Azure Portalon > **az Intune-csoportokban,**  >  **Groups**illetve az Azure Portalon > az Azure **Active Directoryban.**

**A felhasználó túl sok engedéllyel rendelkezik a hozzárendelt Intune-szerepkörhöz**

Azt tanácsolja a **Intune**felhasználónak, hogy lépjen az  >  **Intune-szerepkörök**saját  >  **engedélyek**  >  **rekettel** a megadott engedélyek áttekintéséhez.

**Hozzáadtam egy hatókörcsoportot egy szerepkörhöz, de a szerepkörben lévő felhasználók továbbra is láthatják a többi felhasználót vagy eszközt.**

A hatókörcsoportok nem szűrik ki a felhasználókat vagy az eszközöket. Hatókörcsoportok:

- Korlátozhatja, hogy a felhasználók kihez rendelhetnek házirendeket vagy alkalmazásokat.
- Csak bizonyos felhasználók futtathatnak távoli feladatokat az eszközökön.

A hatókörcsoportokról további információt a [Szerepköralapú hozzáférés-vezérlés (RBAC) és a Microsoft Intune (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)című témakörben talál.

**Hozzáadtam egy felhasználót egy Intune-szerepkörhöz, de továbbra is teljes hozzáféréssel rendelkeznek az Intune felügyeleti konzoljához.**

Nyissa meg az Intune **>-felhasználók at** az Azure Portalon, és ellenőrizze, hogy a felhasználó nincs-e hozzárendelve az alábbi szerepkörök egyikéhez az Azure Portalon:

- Globális rendszergazda
- Az Intune szolgáltatás rendszergazdája
- SharePoint-rendszergazda

További információt a [Szerepköralapú hozzáférés-vezérlés (RBAC) és a Microsoft Intune című témakörben talál.](https://docs.microsoft.com/intune/role-based-access-control)

**Hozzáférési problémák**

További információt az [Office 365-be, az Azure-ba vagy az Intune-ba való bejelentkezés nem tud bejelentkezni.](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)