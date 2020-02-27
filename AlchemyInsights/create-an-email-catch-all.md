---
title: Hozzon létre egy e-mail fogás az összes
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286195"
---
# <a name="create-an-email-catch-all"></a>Hozzon létre egy e-mail fogás az összes

Használata a fogás minden erősen ellenszegül. Sokkal jobb, hogy egy visszapattanó vissza a feladó tudatja, hogy az üzenetet nem lehet kézbesíteni a címzett, így azok lépéseket. A figyelt postaládát úgy is korlátozhatja, hogy csak a korábban érvényes e-mail-címek foghatók. 

Minden fogás minden postaláda kap egy jó adag spam, és végül töltse ki, ha nem szorosan figyelemmel kíséri. (Vannak fogadási korlátok.) 

Ha úgy dönt, hogy folytatja, kövesse az alábbi lépéseket:

1. Hozzon létre egy dinamikus terjesztési csoportot, & tartalmazza a "Minden címzett típusa" című &.

2. Hozzon létre egy dedikált postaládát az e-mailek, például a catchall@domain.com.

3. Az adott tartományhoz állítsa a DomainType programot "InternalRelay" beállításra. Ha később eltávolítja az összes fogást, állítsa vissza a tartományt Mérvadó szintre.

4. Hozzon létre egy Mailflow átviteli szabályt az alábbiak szerint:

    - Ha a feladó "szervezeten kívül"
    - Az üzenet átirányítása Catchall@domain.com
    - Kivéve, ha a címzett tagja a allusers@domain.com (Distribution Group tartalmazza az összes tagja)
    - Annak ellenőrzése, hogy új postaládák kerültek-e a dinamikus terjesztési csoportba
