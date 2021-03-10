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
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694377"
---
# <a name="problems-resetting-password"></a>Problémák a jelszó alaphelyzetbe állításával

Az alábbiakban néhány olyan problémát talál, amely a jelszó alaphelyzetbe állításakor és a lehetséges megoldások során előfordulhat:

**A jelszó-visszaállítás más kategóriákban nem szereplő problémáim vannak**

- Győződjön meg arról, hogy jogosult a jelszavak alaphelyzetbe állításra. Csak a globális, a jelszó és a felhasználói rendszergazdák állíthatják alaphelyzetbe a felhasználói jelszavakat. A globális rendszergazdák más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.
- Győződjön meg arról, hogy megértette a licencelési követelményeket:
    - A szervezetéhez legalább egy licencnek hozzá kell rendelnie
        - Csak felhőbeli felhasználók – Bármely Office 365 -ös (O365) fizetős termékváltozat vagy Azure AD Basic
        - Felhőbeli és/vagy helyszíni felhasználók – Azure AD Premium P1 vagy P2, Enterprise Mobility + Security (EMS) vagy Secure Productive Enterprise (SPE)
        - A licencelési követelményekről az Azure AD önkiszolgáló jelszó-visszaállítási licenckövetelményei [között olvashat bővebben.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Problémákat tapasztalok a beállított jelszó-visszaállítási házirend tesztelése során**

- A legutóbb alkalmazott házirendek replikálása az összes adatközpontban és végponton néhány percig is eltarthat. Az adatközponttól való fizikai távolság is befolyásolja, hogy milyen gyorsan alkalmazza a program a módosításokat.
- Tesztelje a tesztet egy végfelhasználóval, ne rendszergazdával, és tesztelje a tesztelést néhány felhasználóval. Az Azure Portalon konfigurált házirendek csak a végfelhasználókra vonatkoznak, a rendszergazdákra nem. A Microsoft erős alapértelmezett kétoldali jelszó-visszaállítási házirendet érvényesít minden Azure-rendszergazdai szerepkörhöz (például: globális rendszergazda, ügyfélszolgálati rendszergazda, jelszókezelő stb.).
    - További információ a [rendszergazdákra vonatkozó házirendekről.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Jelszó-visszaállítást szeretnék telepíteni, de nem szeretném, ha a felhasználóim további biztonsági adatokat regisztrálnak**

Töltse ki előre a felhasználók adatait, hogy ne szükséges nekik! Rendszergazdaként beállíthatja a telefon- és e-mail-tulajdonságokat a felhasználóknak, mielőtt jelszó-visszaállítást vezet be a szervezetében. Ezt egy API, PowerShell vagy Azure AD Connect használatával tudja megtenni. További információ:
- [Jelszó-visszaállítás telepítése a felhasználók regisztrálásának előírása nélkül](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [A jelszó-visszaállítás által használt adatok](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**A jelszó-visszaállítás gomb szürkével kiszürkül**

Ön nem jogosult a felhasználó jelszavának alaphelyzetbe állítania. Csak a globális, a jelszó és a felhasználói rendszergazdák állíthatják alaphelyzetbe a felhasználói jelszavakat. A globális rendszergazdák más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.

**Nem látom a jelszó-visszaállítási panelt**

Ön nem jogosult a jelszavak alaphelyzetbe állításra. Csak a globális, a jelszó és a felhasználói rendszergazdák állíthatják alaphelyzetbe a felhasználói jelszavakat. A globális rendszergazdák más jogosultsággal rendelkező rendszergazdák jelszavát is alaphelyzetbe állíthatják.

**Nem látom a helyszíni integrációs panelt a jelszó-visszaállításban**

- A helyszíni integrációs blade csak hibrid környezetekben jelenik meg – ami azt jelenti, hogy jelszóvisszaírást használ a helyszíni felhasználók jelszavának a módosítása érdekében.
- A következő esetben nem látja ezt a blade-et:
    - Nem használ jelszó-visszaírást
    - Probléma van a jelszó-visszaírás telepítésével/csatlakoztatásával
    - Probléma van az Azure AD Connect telepítésével/csatlakoztatásával
    - A jelszó-visszaírással kapcsolatos problémák hibaelhárítási lépéseit a Jelszóvisszaírási hibák [elhárítása című szakaszban láthatja.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nem tudom, hogyan állíthatom alaphelyzetbe egy felhasználó jelszavát**

1. Jelentkezzen be az Azure Portalba megfelelő rendszergazdaként.
1. A Felhasználók és csoportok panelen válassza a **Minden felhasználó lehetőséget.**
1. Válasszon ki egy felhasználót a listából.
1. A kijelölt felhasználónál válassza az **Áttekintés** lehetőséget, majd a parancssávon kattintson a **Jelszó alaphelyzetbe állítása parancsra.**
1. Kövesse a képernyőn megjelenő utasításokat.
    - Csak az Azure Portal támogatási jelszavának visszaírásán keresztül végrehajtott visszaállítások.

**Alaphelyzetbe állíthatom egy helyszíni felhasználó jelszavát az Office 365 Felügyeleti portálról vagy az Office 365 mobilalkalmazásból, de a felhasználó továbbra sem tud bejelentkezni**

Ebben a portálban nem támogatott a jelszó-visszaírás. A felhasználó jelszavának alaphelyzetbe állítása az Azure Portalon – portal.azure.com

