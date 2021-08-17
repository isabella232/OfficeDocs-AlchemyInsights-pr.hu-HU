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
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080748"
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
