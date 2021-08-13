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
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960837"
---
# <a name="password-synchronization"></a>Jelszó-szinkronizálás

**A jelszó kivonat-szinkronizálása egyáltalán nem működik**

Az ügyfeleknél a következő gyakori problémákat okozhatja, ha a jelszó kivonat-szinkronizálása nem működik:

- Az Azure AD Csatlakozás által a helyszíni Active Directoryval való kommunikációra használt  Active Directory-fiók nem kap Replikált címtár-módosítások és Replikált címtár-módosítások minden olyan engedélyt, amely szükséges a jelszó-szinkronizáláshoz – ezt úgy kell kijavítani, hogy megadja ezeket az engedélyeket az Active Directory-fióknak. 
- A jelszó kivonatszinkronizálása le van tiltva, miután egy rendszergazda módosította a Felhasználó Sign-In-módszert jelszó-szinkronizálásról egy másik beállításra, például  az Összevonás az **AD FS** szolgáltatással az Azure AD Csatlakozás varázslóban – ezt úgy oldhatja meg, hogy újra engedélyezi a jelszó kivonatszinkronizálási funkcióját az Azure AD Csatlakozás varázslóban. 
- Kapcsolódási probléma a helyszíni Active Directoryval. Például egyes tartományvezérlők nem érhetők el az Azure AD [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Csatlakozás, vagy a tűzfal blokkolja a portokat – Ezt úgy kell megoldania, hogy megfelelően működik a kapcsolat az Azure AD Csatlakozás-kiszolgáló és a helyszíni Active Directory között.
- Az Azure AD Csatlakozás-kiszolgáló jelenleg átmeneti üzemmódban van, amelynek következtében a kiszolgáló nem tudja a jelszó-előjeleket használni – A probléma megoldásához kövesse A jelszó-szinkronizálás az [Azure AD Csatlakozás](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)szinkronizálásával – Nincs jelszó szinkronizálva című szakaszban leírt lépéseket.

**A jelszó kivonat-szinkronizálása nem működik néhány felhasználómnál**

1. Ha azt észlelte, hogy egy felhasználó jelszavas  kivonata nem szinkronizálódik, az Azure AD szolgáltatás hibaelhárítási Csatlakozás vizsgálja meg és oldja meg a problémát. Végezze el az alábbi műveleteket:

    a. [A hibaelhárítási feladat futtatása a varázslóban](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [A hibaelhárítási parancsmag használatával vizsgálja meg egy adott használat jelszó kivonatszinkronizálási problémáit](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. A helyszíni Active Directory User objektum engedélyezve van a Felhasználónak a következő **bejelentkezési beállításnál módosítania kell a jelszót.** Ha ez a beállítás engedélyezve van, a felhasználóhoz kap egy ideiglenes jelszót, és a rendszer kérni fogja, hogy módosítsa a jelszót a következő bejelentkezéskor. Az Azure AD Csatlakozás nem szinkronizálja az ideiglenes jelszavakat az Azure AD-be.

A fenti probléma megoldásához végezze el az alábbi műveletek egyikét:

- Kérje meg a felhasználót, hogy jelentkezzen be a helyszíni alkalmazásba (például az asztali Windows), és módosítsa a jelszót. A rendszer szinkronizálja az új jelszót az Azure AD szolgáltatásba.
- Rendszergazdai jogosultságot kell megadnia a felhasználó jelszavának frissítéséhez a következő bejelentkezéskor a felhasználó jelszavának módosítása **nélkül,** és az új jelszót meg kell osztania a felhasználóval.

3. A helyszíni Active Directory User  objektum nincs megfelelően konfigurálva az objektum-szinkronizáláshoz vagy a jelszó-szinkronizáláshoz. A probléma megoldásához kövesse Az Azure AD-címtárral való jelszó-szinkronizálási hibák elhárítása [és Csatlakozás lépéseket.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







