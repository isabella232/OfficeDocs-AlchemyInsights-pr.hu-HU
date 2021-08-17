---
title: SSPR hibaelhárítása
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038960"
---
# <a name="troubleshoot-sspr"></a>SSPR hibaelhárítása

**Probléma a jelszó-visszaállítás konfigurálásakor**

- Ha Ön rendszergazda, és az önkiszolgáló jelszó-visszaállítás engedélyezését keresi, tekintse meg az Oktatóprogram az [SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)engedélyezéséhez a jelszó alaphelyzetbe állításának konfigurálását a szervezetben. A licencelési követelményeket [is áttekintheti.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Legalább egy licencnek hozzá kell rendelnie a szervezetéhez.
    - **Csak felhőbeli felhasználók** – Office 365 (O365) díjért fizetett termékváltozat vagy Azure AD Basic
    - **Felhőbeli és/vagy** helyszíni felhasználók – Prémium P1 szintű Azure AD P2, Enterprise Mobility + Security (EMS) vagy Secure Productive Enterprise (SPE)
- Az önkiszolgáló jelszó-visszaállítással kapcsolatos további kérdésekért tekintse át a [gyakori kérdéseket.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Hibaüzenet jelenik meg**

A gyakori hibákat és megoldásukat a következő cikkben találja: [Az önkiszolgáló jelszó-visszaállítás hibaelhárítása](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Probléma van a jelszó-visszaállítási házirendmel**

- Ha a jelszó-visszaállítási házirend nem a várt módon működik, vagy ha kérdése van a jelszó-visszaállítási házirendekkel kapcsolatban, olvassa el a következő [cikket:](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)Jelszóházi házirendek és Azure Active Directory.
- A jelszó-visszaállítási házirendek nem vonatkoznak a rendszergazdákra. A Microsoft minden Azure-rendszergazdai szerepkörhöz érvényesít egy erős, két gates jelszó-visszaállítási házirendet. Győződjön meg arról, hogy olyan felhasználóval tesztel, aki nem rendszergazda. A rendszergazdai visszaállítási házirendről további információt a következő cikkben talál: [A rendszergazdai házirendek különbségei.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Nem szeretném, ha a felhasználóim további biztonsági adatokat regisztrálnak a jelszó-visszaállításhoz**

Egy API-t, PowerShellt vagy Azure AD-t használva előre kitöltheti a felhasználók adatait (e-mail- és telefonattribútumokat) Csatlakozás. További információ az olvasásról:

- [Jelszó alaphelyzetbe állítása regisztráció megkövetelése nélkül](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Milyen adatokat használ fel a jelszó-visszaállítás?](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Azt szeretném, hogy a felhasználók regisztrálják a további biztonsági adataikat a jelszó-visszaállításhoz**

1. Állítsa be a felhasználóinak, hogy regisztrálják a biztonsági adataikat önkiszolgáló jelszó-visszaállításhoz, és irányítsa őket a [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Miután a felhasználó (a felhasználó vagy a rendszergazda) feltölti [](https://passwordreset.microsoftonline.com/) az adatokat, iránya a felhasználót a aka.ms/sspr, hogy a felhasználók jogosultak legyen a saját jelszavuk alaphelyzetbe állítására.
1. Ha a felhasználók továbbra is problémákat tapasztalnak, valószínűleg összevont vagy jelszó-kivonatolással  **szinkronizált felhasználókat tapasztalnak.** Ez azt jelenti, hogy valószínűleg probléma van a Jelszóvisszaírás szolgáltatással.