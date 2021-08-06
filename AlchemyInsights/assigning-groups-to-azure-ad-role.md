---
title: Csoportok hozzárendelése Azure AD-szerepkörhöz
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036242"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Csoportok hozzárendelése Azure AD-szerepkörhöz

Ha Azure AD-szerepkörhöz szeretne Azure AD-szerepkört hozzárendelni egy azure ad-beli hitelesítésszolgáltatóval rendelkező Azure AD-csoporthoz, végezze el az alábbi lépéseket:

1. Új csoport létrehozása – Új csoport létrehozása:

    a. Jelentkezzen be az Azure AD Felügyeleti központba jogosultsággal rendelkező **rendszergazdai** vagy globális **rendszergazdai** engedélyekkel.
    b. Válassza **Azure Active Directory > Csoportok > Csoport > csoportban lehetőséget.**
    c. Hozza létre a csoportot.

2. Rendelje hozzá a szerepkört a csoporthoz a csoport létrehozása során vagy a csoport létrehozása után.

    a. Ha a csoport létrehozásakor szerepkört szeretne hozzárendelni a csoporthoz, kapcsolja be az **Azure AD-szerepköröket** hozzá lehet rendelni a csoporthoz, és létre kell hoznia a csoportot.
    b. Ha a létrehozása után hozzá szeretne rendelni egy  szerepkört a csoporthoz, lépjen az újonnan létrehozott csoportHoz rendelt szerepkörök lapra, és rendelje hozzá a szerepkört a csoporthoz.  

**Azure AD-szerepkörhöz hozzárendelt csoport tagságának kezelése**

A jogosultságok jogosultságok kiterjesztésének megakadályozása érdekében alapértelmezés szerint csak a jogosultságokkal rendelkező szerepkörgazdák és a globális rendszergazdák módosíthatják a szerepkörhöz rendelt csoportok tagságát. Dönthetnek azonban úgy, hogy tulajdonost rendelnek egy ilyen csoporthoz, és átruházják ezt a feladatot.

A felhőcsoportok Azure AD-szerepkörökhöz való hozzárendelésének részleteit AD-szerepkörök hozzárendelése felhőcsoporthoz ( AD-szerepkörök hozzárendelése a felhőcsoportokhoz) (lásd: [AD-szerepkörök hozzárendelése a felhőcsoportokhoz)](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) A felhőcsoportokhoz rendelt szerepkörök hibaelhárításáról további információt A felhőcsoportokhoz rendelt szerepkörök hibaelhárítása [témakörben talál.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





