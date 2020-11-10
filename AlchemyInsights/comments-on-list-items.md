---
title: Megjegyzések listaelemekhez
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
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982491"
---
# <a name="comments-on-list-items"></a>Megjegyzések listaelemekhez

A felhasználók hamarosan hozzáadhatnak és törölhetnek megjegyzéseket a listaelemekhez. A felhasználók megtekinthetik a listaelemek minden megjegyzését, és szűrhetik az egy elemhez kapcsolódó megjegyzéseket vagy tevékenységeket megjelenítő nézetek között.

**Időzítés** :

**Célzott kiadás** : fokozatos kilépés az októberi közép-és első lépésekkel – november közepéig

**Szokásos kiadás** : fokozatos Kilépés a novemberi közép-és a decemberi első lépésekkel

**Bevezetés** : célzott kiadás a teljes szervezet számára

A felhasználóknak a megjegyzések hozzáadásához és törléséhez a következőket kell megjegyezniük:

- A megjegyzések a SharePointban rejlő jogosultsági beállításokat követik.
- A modern felhasználói felületeken, például a feladatlistákban még nem megjelenő klasszikus listák nem fogják tartalmazni a megjegyzések hozzáfűzését.
- Ebben a kiadásban nem érhető el megjegyzések a Teams listáihoz.
- A megjegyzéseket a keresés nem indexeli.

A rendszergazdák a **set-SPOTenant PowerShell-** parancsmagban a **CommentsOnListItemsDisabled** paraméter módosításával letilthatják ezt a funkciót szervezeti szinten.

A webhely vagy a lista szintjén jelenleg nem lehet letiltani a megjegyzéseket. Reméljük, hogy ezeket a vezérlőket egy későbbi frissítésben, az 2021 első negyedévében kell megnyitnia.
