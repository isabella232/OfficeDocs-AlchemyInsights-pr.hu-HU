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
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063679"
---
# <a name="issues-with-credentials"></a>Hitelesítő adatokkal kapcsolatos problémák

[A Microsoft identitásplatformja és az OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) ügyfél hitelesítő adatok áramlása azt ismerteti, hogy miként lehet közvetlenül az OAuth 2.0-ügyfél hitelesítő adataival programokat beprogramni.

**Hogyan kezelem egy alkalmazás jelszavát vagy tanúsítványának hitelesítő adatait?**

Az Azure CLI szolgáltatásban az [ad app](https://docs.microsoft.com/cli/azure/ad/app/credential) hitelesítő adataival törölheti, listálhatja vagy alaphelyzetbe állíthatja egy alkalmazás jelszavát vagy tanúsítványának hitelesítő adatait.

**Hogyan állíthatják alaphelyzetbe a felhasználóim a jelszavukat?**

A felhasználóknak regisztrálniuk kell [az önkiszolgáló jelszó-visszaállításra,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) mielőtt alaphelyzetbe állíthatják jelszavukat. Miután regisztrált egy felhasználó, a felhasználó a cikkben található utasításokat követve alaphelyzetbe állíthatja a jelszavát: Állítsa alaphelyzetbe munkahelyi vagy [iskolai jelszavát.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Hogyan módosítják a felhasználóim a jelszavukat?**

A felhasználók a cikkben található lépéseket követve módosíthatjak a jelszavukat: A [jelszó módosítása.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
A [kétlépéses ellenőrzés alkalmazásjelszavát is kezelhetik.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**A felhasználó hibaüzenetet kap a jelszavuk módosításakor vagy alaphelyzetbe állításakor**

Ez a hivatkozás információkat nyújt a felhasználók jelszavának alaphelyzetbe állításakor felmerülő gyakori problémákról: Gyakori problémákról és [megoldásukról](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Probléma adva egy felhasználó jelszavának alaphelyzetbe állítása után**

- Győződjön meg arról, hogy jogosult a jelszavak alaphelyzetbe állításra. *Csak a globális, a jelszó és a felhasználói rendszergazdák állíthatják alaphelyzetbe a felhasználói jelszavakat.* A globális rendszergazdák más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.

- Győződjön meg arról, hogy megértette a licencelési követelményeket:

  - A szervezetéhez legalább egy licencnek hozzá kell rendelnie:
    - **Csak felhőbeli felhasználók** – Bármely Office 365 -ös (O365) fizetős termékváltozat vagy Azure AD Basic
    - **Felhőbeli és/vagy helyszíni** felhasználók – Azure AD Premium P1 vagy P2, Enterprise Mobility + Security (EMS) vagy Secure Productive Enterprise (SPE)
    - A licencelési követelményekről az [Azure AD önkiszolgáló jelszó-visszaállítási licenckövetelményei között olvashat bővebben.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- A felhasználók jelszavának alaphelyzetbe állításához keresse meg a felhasználót az Azure AD-ban. Ezután kattintson a felhasználó áttekintő paneljének "Jelszó alaphelyzetbe állítása" gombjára.

**A jelszó-visszaállítás gomb szürkével kiszürkül**

Ön nem jogosult a  felhasználó jelszavának alaphelyzetbe állítania. *Csak a globális, a jelszó és a felhasználói rendszergazdák állíthatják alaphelyzetbe a felhasználói jelszavakat.* A globális rendszergazdák más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.

**Nem látom a jelszó-visszaállítási panelt**

Ön nem jogosult a jelszavak alaphelyzetbe állításra. *Csak a globális, a jelszó és a felhasználói rendszergazdák állíthatják alaphelyzetbe a felhasználói jelszavakat.* A globális rendszergazdák más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.

**Nem látom a helyszíni integrációs panelt a jelszó-visszaállításban**

- A helyszíni integrációs blade csak hibrid környezetekben jelenik meg – ami azt jelenti, hogy jelszó-visszaírást használ a helyszíni felhasználók jelszavának a módosítása érdekében.

- Ez a kés nem látható, ha:

  - Nem jelszó-visszaírást használ
  - Probléma van a jelszó-visszaírás telepítésével/csatlakoztatásával
  - Probléma van az Azure AD Connect telepítésével/csatlakoztatásával
  - A jelszóvisszaírással kapcsolatos hibák hibaelhárítási lépéseit a Jelszóvisszaírási hibák [elhárítása témakörben láthatja.](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Nem tudom, hogyan állíthatom alaphelyzetbe egy felhasználó jelszavát**

1. Jelentkezzen be az Azure Portalba megfelelő rendszergazdaként.
2. A Felhasználók és **csoportok panelen** válassza a **Minden felhasználó lehetőséget.**
3. Jelöljön ki egy felhasználót a listából.
4. A kijelölt felhasználónál válassza az **Áttekintés** lehetőséget, majd a parancssávon válassza a **Jelszó alaphelyzetbe állítása lehetőséget.**
5. Válassza a **Jelszó alaphelyzetbe állítása** gombot, és kövesse a képernyőn megjelenő utasításokat.
    - Csak az Azure **Portal** támogatási jelszavának visszaírásán keresztül végrehajtott visszaállítások.

**Alaphelyzetbe állíthatom egy helyszíni felhasználó jelszavát az Office 365 Felügyeleti portálról vagy az Office 365 mobilalkalmazásból, de a felhasználó továbbra sem tud bejelentkezni**

Ebben a portálban nem támogatott a jelszó-visszaírás. Állítsa alaphelyzetbe ismét a felhasználó jelszavát az Azure Portalon.
