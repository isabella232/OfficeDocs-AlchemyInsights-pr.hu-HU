---
title: Az összes e-mail fogó létrehozása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816202"
---
# <a name="create-an-email-catch-all"></a>Az összes e-mail fogó létrehozása

A minden kifogó használata kifejezetten ellenzi ezt. Jobb, ha visszapattan a feladóhoz, és tudatja a feladóval, hogy az üzenetet nem lehetett címzettként kézbesíteni, hogy meg tudjanak oldani a lépéseket. A figyelt postaládát úgy is korlátozhatja, hogy csak a korábban érvényes e-mail-címeket elfogja. 

Minden elfogható postaláda sok levélszemetet kap, és végül kitöltheti őket, ha nem figyelik rendszeresen. (Vannak fogadási korlátozások.) 

Ha a folytatásról dönt, kövesse az alábbi lépéseket:

1. Dinamikus terjesztési csoport létrehozása & "Minden címzetttípus" gombra.

2. Létrehozhat egy dedikált postaládát az e-mailek (például e-mailek) catchall@domain.com.

3. Az adott tartományhoz állítsa a DomainType tulajdonságot "InternalRelay" (Belső átfedés) beállításra. Ha később eltávolítja a "Minden" halmazt, állítsa vissza a tartományt Mérvadóra.

4. Hozzon létre egy levélcsordulási átviteli szabályt az alábbiak szerint:

    - Ha a Feladó "Szervezeten kívül"
    - Az üzenet átirányítása a Catchall@domain.com
    - Kivéve, ha a címzett tagja az allusers@domain.com (a terjesztési csoport az összes tagot tartalmazza)
    - Ellenőrizze, hogy az új postaládák bekerülnek-e a dinamikus terjesztési csoportba
