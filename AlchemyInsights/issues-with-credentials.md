---
title: Hitelesítő adatokkal kapcsolatos problémák
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
- "9004330"
- "7723"
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986821"
---
# <a name="issues-with-credentials"></a>Hitelesítő adatokkal kapcsolatos problémák

[Microsoft Identitásplatform OAuth 2.0-ügyfél](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) hitelesítőadat-adatfolyama azt ismerteti, hogy miként lehet közvetlenül az OAuth 2.0-ügyfél hitelesítő adataival programokat beprogramni.

**Hogyan kezelem egy alkalmazás jelszavát vagy a tanúsítvány hitelesítő adatait?**

Az Azure CLI szolgáltatásban az [ad-app](https://docs.microsoft.com/cli/azure/ad/app/credential) hitelesítő adataival törölheti, listába állíthatja, illetve alaphelyzetbe állíthatja egy alkalmazás jelszavát vagy tanúsítványának hitelesítő adatait.

**Hogyan állíthatják alaphelyzetbe a felhasználóim a jelszavukat?**

A felhasználóknak regisztrálniuk kell [az önkiszolgáló jelszó-visszaállításra,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) mielőtt alaphelyzetbe állíthatják jelszavukat. Miután regisztrált egy felhasználót, a következő cikkben található utasításokat követve alaphelyzetbe állíthatja a jelszavát: Munkahelyi vagy iskolai [jelszó alaphelyzetbe állítása.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Hogyan módosítják a felhasználóim a jelszavukat?**

A felhasználók az ebben a cikkben található lépéseket követve módosíthatjuk jelszavukat: [A jelszó módosítása.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Emellett a [kétlépéses ellenőrzés alkalmazásjelszavának kezelését is meg tudják kezelni.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**A felhasználó hibaüzenetet kap a jelszavuk módosításakor vagy alaphelyzetbe állításakor**

Ez a hivatkozás információkat nyújt azokkal a gyakori problémákkal kapcsolatban, amelyek a felhasználók jelszavának alaphelyzetbe állításakor merülhetnek fel: Gyakori problémák és [megoldásaik](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Probléma adva egy felhasználó jelszavának alaphelyzetbe állítása után**

- Győződjön meg arról, hogy jogosult a jelszavak alaphelyzetbe állítva. *Csak a globális, a jelszavak és a felhasználók rendszergazdái állíthatják alaphelyzetbe a felhasználói jelszavakat.* A globális rendszergazdák emellett más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.

- Győződjön meg arról, hogy megértette a licencelési követelményeket:

  - Legalább egy licencnek hozzá kell rendelnie a szervezetéhez:
    - **Csak felhőbeli felhasználók** – Office 365 (O365) díjért fizetett termékváltozat vagy Azure AD Basic
    - **Felhőbeli és/vagy** helyszíni felhasználók – Prémium P1 szintű Azure AD P2, Enterprise Mobility + Security (EMS) vagy Secure Productive Enterprise (SPE)
    - A licencelési követelményekről az [Azure AD önkiszolgáló jelszó-visszaállítási licenckövetelményei témakörben olvashat.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- A felhasználók jelszavának alaphelyzetbe állításához keresse meg a felhasználót az Azure AD szolgáltatásban. Ezután az adott felhasználó áttekintő paneljéhez kattintson a "Jelszó alaphelyzetbe állítása" gombra.

**A jelszó alaphelyzetbe állítva gomb szürkével kiszürkül**

Nem jogosult a felhasználó **jelszavának** alaphelyzetbe állítva. *Csak a globális, a jelszavak és a felhasználók rendszergazdái állíthatják alaphelyzetbe a felhasználói jelszavakat.* A globális rendszergazdák emellett más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.

**Nem látom a jelszó-visszaállítási blade-et**

Nem jogosult a jelszavak alaphelyzetbe állítani. *Csak a globális, a jelszavak és a felhasználók rendszergazdái állíthatják alaphelyzetbe a felhasználói jelszavakat.* A globális rendszergazdák emellett más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.

**Nem látom a helyszíni integrációs blade-t a jelszó-visszaállításban**

- A helyszíni integrációs blade csak hibrid környezetekben jelenik meg – ami azt jelenti, hogy jelszó-visszaírás használatával módosítja a helyszíni felhasználók jelszavát.

- Nem látja ezt a blade-et, ha:

  - Nem használ jelszó-visszaírást
  - Probléma van a jelszó-visszaírás telepítésével/csatlakoztatásával
  - Probléma van az Azure AD-szolgáltatások telepítésekor vagy csatlakoztatva Csatlakozás
  - A jelszó-visszaírással kapcsolatos problémák hibaelhárítási lépéseit a Jelszó-visszaírási [hibák elhárítása](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Nem tudom, hogyan állíthatok alaphelyzetbe egy felhasználó jelszavát**

1. Jelentkezzen be az Azure Portalba megfelelő rendszergazdaként.
2. A Felhasználók **és csoportok panelen** válassza a **Minden felhasználó lehetőséget.**
3. Jelöljön ki egy felhasználót a listából.
4. A kijelölt felhasználónál válassza **az** Áttekintés lehetőséget, majd a parancssávon válassza a Jelszó alaphelyzetbe **állítása lehetőséget.**
5. Válassza a **Jelszó alaphelyzetbe állítása** gombot, és kövesse a képernyőn megjelenő utasításokat.
    - Csak az Azure **Portal** támogatási jelszavának visszaírásával végrehajtott visszaállítások.

**Alaphelyzetbe állíthatom egy helyszíni felhasználó jelszavát a Office 365 Felügyelet portálról vagy Office 365 mobilalkalmazásból, de a felhasználó továbbra sem tud bejelentkezni**

A jelszó-visszaírást ez a portál nem támogatja. Állítsa alaphelyzetbe újra a felhasználó jelszavát az Azure Portalon.
