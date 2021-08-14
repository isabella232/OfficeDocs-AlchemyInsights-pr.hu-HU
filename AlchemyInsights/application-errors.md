---
title: Alkalmazáshibák
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931451"
---
# <a name="application-errors"></a>Alkalmazáshibák

Az Azure Active Directory (Azure AD) biztonsági jogkivonat-szolgáltatásból (STS) visszaadott **AADSTS-hibakódokat** keresi? Olvassa [el az Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds.

Az engedélyezési hibák több különböző hiba következtében léphetnek fel, amelyek nagy része 401-es vagy 403-as hibát generál. Az alábbi hibák például engedélyezési hibákhoz vezethetnek:

- Helytelen [hozzáférési jogkivonat beszerzési folyamatok](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Rosszul konfigurált [engedély hatókörök](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- [Jóváhagyás](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) hiánya

A gyakori engedélyezési hibák elhárításához próbálkozzon az alábbi lépésekkel, amelyek a leginkább illeszkednek a kapott hibához. Több alkalmazás is alkalmazható.

**401 Jogosulatlan hozzáférési hiba: Érvényes a jogkivonata?**

Győződjön meg arról, hogy az alkalmazás érvényes hozzáférési jogkivonatot ad a Microsoft Graph a kérés részeként. Ez a hiba gyakran azt jelzi, hogy a hozzáférési jogkivonat hiányzik a HTTP hitelesítési kérés fejlécében, vagy hogy a jogkivonat érvénytelen vagy lejárt. Határozottan javasoljuk, hogy a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) használatával használja a hozzáférési jogkivonat beszerzését. Ez a hiba akkor fordulhat elő, ha személyes Microsoft-fiókhoz biztosított delegált hozzáférési jogkivonatot próbál használni egy olyan API eléréséhez, amely csak munkahelyi vagy iskolai fiókokat (szervezeti fiókokat) támogat.

**403 Tiltott művelet: A megfelelő engedélykészletet választotta ki?**

Ellenőrizze, hogy a megfelelő engedélykészletet kérte-e az alkalmazáshívások microsoftos Graph API-k alapján. Az ajánlott legkevesebb jogosultsági jogosultságot a Microsoft Graph API referenciamódszerekkel kapcsolatos témakörében biztosítjuk. Ezenkívül ezeket az engedélyeket egy felhasználónak vagy egy rendszergazdának kell megadnia az alkalmazásnak. Az engedélyek megadása általában egy jóváhagyási lapon történik, vagy az Azure Portal alkalmazás regisztrációs blade használatával engedélyek felhasználásával. Az alkalmazás **Beállítások** panelén kattintson a **Szükséges engedélyek** elemre, majd kattintson az **Engedélyek megadása** lehetőségre.

- [Microsoft Graph-engedélyek](https://docs.microsoft.com/graph/permissions-reference) 
- [Az Azure AD engedélyeinek és hozzájárulásainak ismertetése](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Tiltott művelet: Beszerezte az appja a választott engedélyeknek megfelelő jogkivonatot?**

Győződjön meg arról, hogy a kért vagy megadott engedélyek típusa megegyezik az app által beszerzett hozzáférési jogkivonat-típussal. Lehetséges, hogy alkalmazásengedélyeket kér és ad meg, delegált interaktív kódfolyam-jogkivonatokat használ ügyfél-hitelesítőadat-folyamatkódok helyett, vagy delegált engedélyeket kér és ad ki, de ügyféloldali hitelesítőadat-jogkivonatokat használ delegált kód-folyamatkódok helyett.

- [Hozzáférés kérése a felhasználók nevében és meghatalmazott engedélyek](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 – OAuth 2.0 engedélyezési kódfolyam](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Hozzáférés kérése felhasználó (daemon szolgáltatás) és alkalmazásengedélyek nélkül](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 – OAuth 2.0-ügyfél hitelesítőadat-folyam](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Tiltott művelet: Jelszó visszaállítása**

Jelenleg nincsenek olyan alkalmazásengedélyek, amelyek lehetővé teszik a felhasználói jelszavak visszaállítását. Ezek az API-k csak bejelentkezett rendszergazda interaktív delegált kódfolyamával támogatottak.

- [Microsoft Graph-engedélyek](https://docs.microsoft.com/graph/permissions-reference)

**403 Tiltott művelet: Van hozzáférése a felhasználónak, és rendelkezik licenccel?**

A delegált kódfolyamatok esetén a Microsoft Graph kiértékeli, hogy a kérés engedélyezett-e az alkalmazásnak adott engedélyek és a bejelentkezett felhasználó által megadott engedélyek alapján. Ez a hiba általában azt jelzi, hogy a felhasználó nem rendelkezik elegendő jogosultsággal ahhoz, hogy végrehajtsa a kérést, vagy hogy a felhasználónak nincs licence a hozzáfért adatokhoz. Csak a szükséges engedélyekkel vagy licencekkel rendelkező felhasználók tudnak sikeresen kérelmezni.

**403 Tiltott művelet: Megfelelő forrás API-t választott ki?**

Az API-szolgáltatások, mint például a Microsoft Graph ellenőrzik, hogy a kapott hozzáférési jogkivonatban a felhasználó által elvárt érték megegyezik-e a várt értékkel, és ha nem, a 403-as "Tiltott" hibát okozza. Gyakori hiba, amely következtében egy Azure AD Graph API-khoz, Outlook API-khoz vagy SharePoint/OneDrive API-khoz beszerzett jogkivonatot hibásan próbál használni a Microsoft Graph hívásához (vagy fordítva). Győződjön meg arról, hogy az adott erőforrás (vagy hatókör) egy olyan jogkivonatot szerez be, amely megfelel az app által hívott API-nak.

**400 Hibás kérelem vagy 403 Tiltott művelet: Megfelel a felhasználó a szervezete feltételes hozzáférésre (CA) vonatkozó irányelveinek?**

A szervezet hitelesítésszolgáltatói szabályzata alapján előfordulhat, hogy egy, a Microsoft Graph-erőforrásokhoz az alkalmazáson keresztül hozzáférő felhasználó esetén további információkra lehet szükség, amelyek nem találhatóak meg az app eredetileg beszerzett hozzáférési jogkivonatában. Ebben az esetben az appban egy 400-as, *interaction_required* típusú hiba történik a hozzáférési jogkivonat beszerzésekor, vagy egy 403-as, *insufficient_claims* típusú Microsoft Graph hívása esetén. A hibare adott válasz mindkét esetben további információkat tartalmaz, amelyek bemutatják a végpont engedélyezése számára, hogy a felhasználónak további információkat (például többtényezős hitelesítést vagy eszköz regisztrálását) is ki kell mondania.

- [A feltételes hozzáféréssel kapcsolatos kihívások kezelése MSAL segítségével ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Fejlesztői útmutató az Azure Active Directory feltételes hozzáféréséhez](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
