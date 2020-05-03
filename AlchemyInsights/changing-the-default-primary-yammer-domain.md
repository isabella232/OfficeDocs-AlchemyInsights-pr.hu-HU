---
title: Az alapértelmezett Yammer-tartomány módosítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 099feb5c58a2b1068a2ec501ff966c6ac73d804d
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991197"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Az alapértelmezett/elsődleges Yammer-tartomány módosítása

A Yammer URL-címe tartalmazza a Yammer-hálózat aktuális elsődleges tartománynevét. Előfordulhat, hogy ez a tartománynév nem egyezik meg az Office 365-ben vagy az Azure AD szolgáltatásban beállított elsődleges tartománynévvel. Különbségek vannak a viselkedésben, a bérlőhöz hozzáadott egyéni tartományok száma alapján, illetve attól függően, hogy a Yammer egy támogatott konfigurációban van-e (1 bérlő: 1 hálózat vagy 1:1). A [Yammer tartományokra és az Office 365-re](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) vonatkozó dokumentáció elérhető.

Ha helytelen tartományt lát, annak leggyakoribb oka az, hogy több Yammer-hálózat létezik, és össze kell vonni ezeket. Ehhez fontos első lépést jelent [az egyetlen hálózatba való összevonás](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) a hálózati áttelepítési eszközzel. Ezt végezze el, mielőtt megpróbálná beállítani az elsődleges tartományát.

**Nincsenek egyéni tartományok**

Új bérlők esetében a bérlő alapértelmezett tartománya (pl. fabrikam.onmicrosoft.com) lesz felhasználva a Yammerhez. Az elsődleges tartomány a yammer.com/fabrikam.onmicrosoft.com értékre van állítva.

**Egy egyéni tartomány**

A Yammer automatikusan kiválasztja az egyéni tartományt (pl. fabrikam.com) a bérlőről a Yammer elsődleges tartományaként. Ez a yammer.com/fabrikam.com értékre van állítva. Ezt a módosítást a tartományszinkronizálási szolgáltatás végzi, és érvénybe lépése akár 24 órát is igénybe vehet.

**Több egyéni tartomány**

A Yammernek lehet olyan elsődleges tartománya, amely nem azonos az alapértelmezett bérlői tartománnyal. Mivel több egyéni tartomány is van, a Yammer nem kísérli meg a megfelelő tartomány kiválasztását a rendelkezésre álló tartományokból. Támogatási esetet kell nyitnia annak kéréséhez, hogy az elsődleges tartománynevet az Ön által választott elsődleges tartományra módosítsuk.

**További hibaelhárítási információk**

Bizonyos esetekben előfordulhat, hogy a tartományok át lettek helyezve a bérlők között, és a tartomány szinkronizálási szolgáltatása nem tudott sikeresen futni. Előfordulhat, hogy bejelentkezési vagy egyéb problémákat tapasztal a helytelen elsődleges tartományon kívül. A probléma megoldásához lehetséges, hogy át kell helyeznie a tartományokat a megfelelő hálózatba a Microsoft ügyfélszolgálatának segítségével. Ez a helyzet közvetlen segítséget igényel, és eltarthat egy kis ideig a megoldása, különösen akkor, ha a tartománynevek listája nagyon hosszú. Nyisson egy támogatási esetet, hogy segítséget kapjon az ilyen típusú problémák megoldásához.

A támogatási szakember, akivel dolgozik, ellenőrizni fogja, hogy a tartományok igazoltak-e egy, az Ön ellenőrzése alatt álló bérlőn. Feltehet Önnek további ellenőrző kérdéseket is a tartományaira vonatkozóan, ha azok hozzá vannak adva a bérlőjéhez, de nincsenek DNS-sel igazolva. Kérjük, gondoskodjon arról, hogy a tartományok DNS-sel legyenek igazolva a folyamat felgyorsításához.
