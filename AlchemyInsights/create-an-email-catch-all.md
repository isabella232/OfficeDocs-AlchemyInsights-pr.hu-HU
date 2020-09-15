---
title: E-mail-fogás létrehozása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712988"
---
# <a name="create-an-email-catch-all"></a>E-mail-fogás létrehozása

Az összes fogás használata erősen ellenjavallt. Jobb, ha vissza szeretne térni a feladónak, hogy a feladók megismerjék az üzenetét, hogy a címzettek ne legyenek kézbesítve, így elvégezhetik őket. Úgy is korlátozhatja a figyelt postaládát, hogy csak a korábban érvényes e-mail-címeket kapja meg. 

Bármely fogás minden postaládában sok levélszemét fog megjelenni, és előfordulhat, hogy végül nem figyeltek meg. (Vannak fogadási korlátok.) 

Ha úgy dönt, hogy továbblép, kövesse az alábbi lépéseket:

1. Hozzon létre egy dinamikus terjesztési csoportot, & a "minden címzett típusa" szó szerepel.

2. Hozzon létre egy dedikált postaládát az e-mailek elfogásához, például catchall@domain.com.

3. Az adott tartomány esetében állítsa a DomainType a "InternalRelay" értékre. Ha később eltávolítja az egész fogást, győződjön meg arról, hogy a tartomány vissza a mérvadó értékre van állítva.

4. Hozzon létre egy Hibaelhárítóhttps://configure.Office.com/scenario.aspx?SID=12 átviteli szabályt az alábbiak szerint:

    - Ha a feladó "a szervezeten kívül"
    - Az üzenet átirányítása a Catchall@domain.com-ra
    - Kivéve, ha a címzett a allusers@domain.com tagja (a terjesztési csoport az összes tagot tartalmazza)
    - Annak ellenőrzése, hogy az új postaládák hozzá lettek-e adva a dinamikus terjesztési csoporthoz
