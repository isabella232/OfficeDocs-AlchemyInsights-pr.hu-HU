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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724156"
---
# <a name="comments-on-list-items"></a>Megjegyzések listaelemekhez

A felhasználók megtekinthetik a listaelemek minden megjegyzését, és szűrhetik az egy elemhez kapcsolódó megjegyzéseket vagy tevékenységeket megjelenítő nézetek között.

A felhasználóknak a megjegyzések hozzáadásához és törléséhez a következőket kell megjegyezniük:

- A megjegyzések a SharePointban rejlő jogosultsági beállításokat követik.
- A modern felhasználói felületeken, például a feladatlistákban még nem megjelenő klasszikus listák nem fogják tartalmazni a megjegyzések hozzáfűzését.
- Ebben a kiadásban nem érhető el megjegyzések a Teams listáihoz.
- A megjegyzéseket a keresés nem indexeli.

A rendszergazdák a **set-SPOTenant PowerShell-** parancsmagban a **CommentsOnListItemsDisabled** paraméter módosításával letilthatják ezt a funkciót szervezeti szinten.

A webhely vagy a lista szintjén jelenleg nem lehet letiltani a megjegyzéseket. Reméljük, hogy ezeket a vezérlőket egy későbbi frissítésben, az 2021 első negyedévében kell megnyitnia.
