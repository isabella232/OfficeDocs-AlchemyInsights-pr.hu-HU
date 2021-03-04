---
title: Az SSPR hibaelhárítása
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
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429718"
---
# <a name="troubleshoot-sspr"></a>Az SSPR hibaelhárítása

**Problémáim vannak a jelszó-visszaállítás konfigurálásával**

- Ha Ön rendszergazda, és azt szeretné tudni, hogy miként engedélyezheti az önkiszolgáló jelszó-visszaállítást, az oktatóanyag engedélyezi az [SSPR-t,](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)és konfigurálja a jelszó-visszaállítást a szervezetében. A licencelési követelményeket is [áttekintheti.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Legalább egy licencnek hozzá kell rendelnie a szervezetéhez.
    - **Csak felhőbeli felhasználók** – Bármely Office 365 -ös (O365) fizetős termékváltozat vagy Azure AD Basic
    - **Felhőbeli és/vagy helyszíni** felhasználók – Azure AD Premium P1 vagy P2, Enterprise Mobility + Security (EMS) vagy Secure Productive Enterprise (SPE)
- Az önkiszolgáló jelszó-visszaállítással kapcsolatos további kérdésekért tekintse át [a gyakori kérdéseket.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Hibaüzenet jelenik meg**

A gyakori hibák és megoldásuk megkeresése: Az [önkiszolgáló jelszó-visszaállítás hibaelhárítása](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Probléma van a jelszó-visszaállítási házirendmel**

- Ha a jelszó-visszaállítási házirend nem a várt módon működik, vagy ha kérdése van a jelszó-visszaállítási házirendekkel kapcsolatban, olvassa el a következő cikket: Jelszóházirakok és -korlátozások az [Azure Active Directoryban.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- A jelszó-visszaállítási házirendek nem vonatkoznak a rendszergazdákra. A Microsoft minden Azure-rendszergazdai szerepkörhöz erős alapértelmezett kétoldali jelszó-visszaállítási házirendet kényszerít. Győződjön meg arról, hogy olyan felhasználóval tesztel, aki nem rendszergazda. A rendszergazdai alaphelyzetbe állítási házirendről további információt a következő cikkben talál: A rendszergazdák alaphelyzetbe [állítási házirendje közötti különbségek.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Nem szeretném, ha a felhasználóim további biztonsági adatokat regisztrálnak a jelszó-visszaállításhoz**

Api,PowerShell vagy Azure AD Connect használatával előre kitöltheti felhasználói adatait (e-mail- és telefonattribútumát). További információ az olvasásról:

- [Jelszó-visszaállítás telepítése a felhasználók regisztrálásának előírása nélkül](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [A jelszó-visszaállítás által használt adatok](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Azt szeretném, hogy a felhasználók regisztrálják a további biztonsági adataikat a jelszó alaphelyzetbe állításához**

1. Állítsa be a felhasználóknak, hogy regisztrálják biztonsági adataikat önkiszolgáló [jelszó-visszaállításhoz,](https://mysignins.microsoft.com/security-info)és irányt állítsanak aka.ms/ssprsetup.
1. Miután a felhasználó (a felhasználó vagy a rendszergazda) feltölti [](https://passwordreset.microsoftonline.com/) az adatokat, iránya a aka.ms/sspr, hogy a felhasználók jogosultak legyen a saját jelszavuk alaphelyzetbe állítására.
1. Ha a felhasználók továbbra is problémákat tapasztalnak, valószínűleg összevont vagy jelszó-kivonatot szinkronizált **felhasználók.**  Ez azt jelenti, hogy valószínűleg probléma van a Jelszóvisszaírás szolgáltatással.