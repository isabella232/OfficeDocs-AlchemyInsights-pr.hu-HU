---
title: Probléma a jelszó alaphelyzetbe állításával
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039968"
---
# <a name="problems-resetting-password"></a>Problémák a jelszó alaphelyzetbe állításával

Az alábbiakban néhány olyan problémát talál, amely a jelszó alaphelyzetbe állításakor előfordulhat, és a lehetséges megoldások:

**A jelszó-visszaállítást nem fedezi a többi kategória**

- Győződjön meg arról, hogy jogosult a jelszavak alaphelyzetbe állítva. Csak a globális, a jelszavak és a felhasználók rendszergazdái állíthatják alaphelyzetbe a felhasználói jelszavakat. A globális rendszergazdák emellett más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.
- Győződjön meg arról, hogy megértette a licencelési követelményeket:
    - Legalább egy licencnek hozzá kell rendelnie a szervezetéhez
        - Csak felhőbeli felhasználók – Office 365 (O365) fizetős termékváltozat vagy Azure AD Basic
        - Felhőbeli és/vagy helyszíni felhasználók – Prémium P1 szintű Azure AD P2, Enterprise Mobility + Security (EMS) vagy Secure Productive Enterprise (SPE)
        - A licencelési követelményekről az [Azure AD önkiszolgáló jelszó-visszaállítási](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)követelményeinek licencelési követelményei témakörben olvashat bővebben.

**Problémákat tapasztalok a beállított jelszó-visszaállítási házirend tesztelése során**

- A legutóbb alkalmazott házirendek replikálása az összes adatközpontban és végponton néhány percig is eltarthat. Az adatközponttól való fizikai távolság is befolyásolja a változások alkalmazását.
- Tesztelje a tesztet egy végfelhasználóval, ne rendszergazdával, és tesztelje kis felhasználókészletekkel. Az Azure Portalon konfigurált házirendek csak a végfelhasználókra vonatkoznak, a rendszergazdákra nem. A Microsoft erős, két gate-s jelszó-visszaállítási házirendet érvényesít minden Azure-rendszergazdai szerepkörhöz (például: Globális rendszergazda, ügyfélszolgálati rendszergazda, jelszókezelő stb.).
    - További információ a [rendszergazdáknak készült házirendekről.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Szeretném telepíteni a jelszó alaphelyzetbe állítását, de nem szeretném, ha a felhasználóim további biztonsági adatokat regisztrálnak**

Töltse ki előre a felhasználók adatait, hogy ne is szükséges adatokat feltölteniük! – Rendszergazdaként beállíthatja a telefonszám és a levelezés tulajdonságait a felhasználóknak, mielőtt a jelszavak alaphelyzetbe állítását vezetjük be a szervezetben. Ezt egy API-, PowerShell- vagy Azure AD-parancsprogrammal Csatlakozás. További információ itt:
- [Jelszó alaphelyzetbe állítása regisztráció megkövetelése nélkül](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Milyen adatokat használ fel a jelszó-visszaállítás?](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**A jelszó alaphelyzetbe állítva gomb szürkével kiszürkül**

Nem jogosult a felhasználó jelszavának alaphelyzetbe állítva. Csak a globális, a jelszavak és a felhasználók rendszergazdái állíthatják alaphelyzetbe a felhasználói jelszavakat. A globális rendszergazdák emellett más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.

**Nem látom a jelszó-visszaállítási blade-et**

Nem jogosult a jelszavak alaphelyzetbe állítani. Csak a globális, a jelszavak és a felhasználók rendszergazdái állíthatják alaphelyzetbe a felhasználói jelszavakat. A globális rendszergazdák emellett más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.

**Nem látom a helyszíni integrációs blade-t a jelszó-visszaállításban**

- A helyszíni integrációs blade csak hibrid környezetekben jelenik meg – ami azt jelenti, hogy jelszó-visszaírás használatával módosítja a helyszíni felhasználók jelszavát.
- Nem látja ezt a blade-et, ha:
    - Nem használ jelszó-visszaírást
    - Probléma van a jelszó-visszaírás telepítésével/csatlakoztatásával
    - Probléma van az Azure AD-szolgáltatások telepítésekor vagy csatlakoztatva Csatlakozás
    - A jelszó-visszaírással kapcsolatos problémák hibaelhárítási lépéseit a Jelszóvisszaírási [hibák elhárítása című szakaszban láthatja.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nem tudom, hogyan állíthatok alaphelyzetbe egy felhasználó jelszavát**

1. Jelentkezzen be az Azure Portalba megfelelő rendszergazdaként.
1. A Felhasználók és csoportok panelen válassza a **Minden felhasználó lehetőséget.**
1. Jelöljön ki egy felhasználót a listából.
1. A kijelölt felhasználónál válassza **az** Áttekintés lehetőséget, majd a parancssávon kattintson a Jelszó alaphelyzetbe **állítása elemre.**
1. Kövesse a képernyőn megjelenő utasításokat.
    - Csak az Azure Portal támogatási jelszavának visszaírásával végrehajtott visszaállítások.

**Alaphelyzetbe állíthatom egy helyszíni felhasználó jelszavát a Office 365 Felügyelet portálról vagy Office 365 mobilalkalmazásból, de a felhasználó továbbra sem tud bejelentkezni**

A jelszó-visszaírást ez a portál nem támogatja. A felhasználó jelszavának alaphelyzetbe állítása az Azure Portalon – portal.azure.com

