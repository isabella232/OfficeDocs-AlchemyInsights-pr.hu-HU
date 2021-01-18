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
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885068"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Csoportok hozzárendelése Azure AD-szerepkörhöz

Ha Azure AD-szerepkörhöz szeretne azure AD-szerepkört hozzárendelni egy azure AD-szerepkörhöz, és az Azure AD-beli hitelesítésszolgáltatói csoportot hozzá szeretne rendelni, végezze el az alábbi lépéseket:

1. Új csoport létrehozása – Új csoport létrehozása:

    a. Jelentkezzen be az Azure AD Felügyeleti központba jogosultsággal rendelkező **szerepkörgazdával** vagy **globális rendszergazdai** engedélyekkel.
    b. Válassza az Azure Active Directory > csoportok > Új > **csoportban.**
    c. Hozza létre a csoportot.

2. Rendelje hozzá a szerepkört a csoporthoz a csoport létrehozásakor vagy a csoport létrehozása után.

    a. Ha a csoport létrehozásakor szerepkört szeretne hozzárendelni a csoporthoz, kapcsolja be az **Azure AD-szerepköröket** a csoporthoz rendelve és hozza létre a csoportot.
    b. Ha a létrehozása után hozzá szeretne rendelni egy  szerepkört a csoporthoz, nyissa meg az újonnan létrehozott csoport Hozzárendelt szerepkörök lapját, és rendelje hozzá a szerepkört a csoporthoz.  

**Azure AD-szerepkörhöz hozzárendelt csoport tagságának kezelése**

A jogosultságok kiterjesztésének megakadályozása érdekében alapértelmezés szerint csak a jogosultsággal rendelkező szerepkörgazdák és a globális rendszergazdák módosíthatják egy szerepkörhöz hozzárendelt csoport tagságát. Dönthetnek azonban úgy, hogy tulajdonost rendelnek egy ilyen csoporthoz, és delegálják ezt a feladatot.

A felhőcsoportok Azure AD-szerepkörökhöz való hozzárendelésének részleteiről az AD-szerepkörök hozzárendelése [a felhőcsoportokhoz.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) A felhőcsoportokhoz rendelt szerepkörök hibaelhárításáról további információt a felhőcsoportokhoz rendelt szerepkörök [hibaelhárítása témakörben talál.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





