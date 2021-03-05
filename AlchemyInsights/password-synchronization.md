---
title: Jelszó-szinkronizálás
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482036"
---
# <a name="password-synchronization"></a>Jelszó-szinkronizálás

**A jelszó kivonat-szinkronizálása egyáltalán nem működik**

Egyes gyakori problémák az ügyfeleknél akkor találkoznak, ha a jelszó kivonat-szinkronizálása nem működik:

- Az Azure AD Connect által a helyszíni Active Directoryval való  kommunikációhoz  használt Active Directory-fiók nem kap replikált címtárbeli módosításokat és replikált címtár-módosításokat minden engedélyt, amelyek a jelszó-szinkronizáláshoz szükségesek – ezt úgy kell kijavítani, hogy megadja ezeket az engedélyeket az Active Directory-fióknak.
- A jelszó-kivonat szinkronizálása le van tiltva,  miután egy rendszergazda módosította a Felhasználói Sign-In-módszert jelszó-szinkronizálásról egy másik beállításra,  például az Összevonás az **AD FS** szolgáltatással az Azure AD Connect varázslóban – ezt az Azure AD Connect varázsló jelszó-kivonat-szinkronizálási funkciójának újra engedélyezésével oldhatja meg.
- Kapcsolódási probléma a helyszíni Active Directoryval. Egyes tartományvezérlők például nem érhetők el az Azure [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) AD Connect által, vagy a tűzfal blokkolja a szükséges portokat. Ezt úgy kell megoldania, hogy az Azure AD Connect-kiszolgáló és a helyszíni Active Directory közötti kapcsolat megfelelően működik.
- Az Azure AD Connect-kiszolgáló jelenleg előkészítési módban van, ezért a kiszolgáló nem fogja tudni megadni a jelszó-előjeleket. A probléma megoldásához kövesse az [Azure AD](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Connect-szinkronizálással való jelszó-szinkronizálás hibaelhárítása című szakasz lépéseit . A rendszer nem szinkronizál jelszavakat.

**A jelszó kivonat-szinkronizálása nem működik egyes felhasználóknál**

1. Ha azt vette észre, hogy egy felhasználó jelszavas  kivonata nem szinkronizálódik, az Azure AD Connect hibaelhárítási feladatával kivizsgálhatja és megoldhatja a problémát. Végezze el az alábbi műveleteket:

    a. [A hibaelhárítási feladat futtatása a varázslóban](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [A hibaelhárítási parancsmag használatával vizsgálja meg egy adott használat jelszó kivonatszinkronizálási problémáit.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. A helyszíni Active Directory user objektum engedélyezve van a Felhasználó számára, és a következő **bejelentkezéskor módosítania** kell a jelszót. Ha ez a beállítás engedélyezve van, a felhasználóhoz egy ideiglenes jelszó lesz rendelve, és a rendszer kérni fogja, hogy módosítsa a jelszót a következő bejelentkezéskor. Az Azure AD Connect nem szinkronizálja az ideiglenes jelszavakat az Azure AD-be.

A fenti probléma megoldásához végezze el az alábbi műveletek egyikét:

- Kérje meg a felhasználót, hogy jelentkezzen be a helyszíni alkalmazásba (például asztali Windowsba), és módosítsa a jelszót. Az új jelszó szinkronizálva lesz az Azure AD-vel.
- A következő bejelentkezéskor a felhasználónak módosítania kell a jelszót, és meg kell osztania a felhasználóval az új jelszót. 

3. A helyszíni Active Directory-felhasználó  objektum nincs megfelelően konfigurálva az objektum-szinkronizáláshoz vagy a jelszó-szinkronizáláshoz. A probléma megoldásához kövesse az Azure AD Connect szinkronizálásával való jelszó-kivonat-szinkronizálás hibaelhárítása [témakörben leírt lépéseket.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







