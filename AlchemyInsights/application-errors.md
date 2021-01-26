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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984588"
---
# <a name="application-errors"></a>Alkalmazáshibák

Az Azure Active Directory (Azure AD) biztonsági jogkivonat-szolgáltatásból (STS) visszaadott **AADSTS-hibakódokat** keresi? Olvassa el az [Azure AD authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds.

Az engedélyezési hibák számos különböző hiba eredményeként jelenhetnek meg, amelyek nagy része 401-es vagy 403-as hibát generál. Az alábbiak például engedélyezési hibákhoz vezethetnek:

- Helytelen [hozzáférési jogkivonat-beszerzések](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Nem megfelelően konfigurált [engedélyhatókörök](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- A hozzájárulás [hiánya](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

A gyakori engedélyezési hibák megoldásához próbálkozzon az alábbi lépésekkel, amelyek a legjobban illeszkednek a kapott hibához. Több alkalmazás is alkalmazható.

**401 Jogosulatlan hiba: Érvényes a tokenje?**

Győződjön meg arról, hogy az alkalmazás érvényes hozzáférési jogkivonatot ad a Microsoft Graph-hoz a kérelem részeként. Ez a hiba gyakran azt jelenti, hogy a hozzáférési jogkivonat hiányzik a HTTP-hitelesítés kérésének fejlécében, vagy hogy a jogkivonat érvénytelen vagy lejárt. Kifejezetten javasoljuk, hogy a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) használatával használja a hozzáférési jogkivonat-beszerzést. Ez a hiba akkor fordulhat elő, ha egy személyes Microsoft-fiókhoz megadott delegált hozzáférési jogkivonatot próbál használni egy olyan API eléréséhez, amely csak munkahelyi vagy iskolai fiókokat (szervezeti fiókokat) támogat.

**403 Tiltott hiba: A megfelelő engedélykészletet választotta?**

Ellenőrizze, hogy a megfelelő engedélykészletet kérte-e az alkalmazáshívásai által fogadott Microsoft Graph API-k alapján. Az ajánlott legkevesebb jogosultsággal rendelkező engedélyeket a Microsoft Graph API referenciamódszer-témakörei biztosítják. Ezenkívül ezeket az engedélyeket egy felhasználónak vagy egy rendszergazdának kell megadnia az alkalmazásnak. Az engedélyek megadására általában egy jóváhagyási lapon vagy az Azure Portal alkalmazás regisztrációs paneljét használva lehet engedélyt adni. Az alkalmazás **Beállítások** panelen kattintson a **Kötelező** engedélyek elemre, majd az Engedélyek **megadása elemre.**

- [Microsoft Graph-engedélyek](https://docs.microsoft.com/graph/permissions-reference) 
- [Az Azure AD engedélyeinek és beleegyezésének ismertetése](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Tiltott hiba: Az app a kiválasztott engedélyeknek megfelelő jogkivonatot szerzett be?**

Győződjön meg arról, hogy a kért vagy megadott engedélyek típusa megegyezik az app által beszerzett hozzáférési jogkivonat-típussal. Előfordulhat, hogy alkalmazásengedélyeket kér és ad meg, delegált interaktív kódfolyam-jogkivonatokat használ az ügyfél hitelesítőadat-adatfolyam-tokenek helyett, vagy de delegált engedélyeket kér és ad meg, de ügyfél-hitelesítőadat-folyamat jogkivonatokat használ delegált kódfolyam-jogkivonatok helyett.

- [Hozzáférés a felhasználók és a delegált engedélyek nevében](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 – OAuth 2.0 engedélyezési kódfolyam](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Hozzáférés felhasználói (daemon-szolgáltatás) és alkalmazásengedélyek nélkül](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - OAuth 2.0-ügyfél hitelesítő adatok áramlása](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 – Tiltott hiba: Jelszó alaphelyzetbe állítása**

Jelenleg nincsenek olyan alkalmazásengedélyek, amelyek lehetővé teszik a felhasználói jelszavak alaphelyzetbe állítását. Ezek az API-k csak az interaktív delegált kódfolyamatok használatával támogatottak egy bejelentkezett rendszergazdával.

- [Microsoft Graph-engedélyek](https://docs.microsoft.com/graph/permissions-reference)

**403 Tiltott: Van hozzáférése a felhasználónak, és rendelkezik licenccel?**

Delegált kódfolyamatok esetén a Microsoft Graph kiértékeli, hogy a kérés engedélyezett-e az alkalmazásnak adott engedélyek és a bejelentkezett felhasználó által biztosított engedélyek alapján. Ez a hiba általában azt jelzi, hogy a felhasználó nincs elég jogosultsággal a kérés végrehajtásához, vagy hogy a felhasználó nem rendelkezik licenccel a megnyitott adatokhoz. A kérelmet csak a szükséges engedélyekkel vagy licencekkel rendelkező felhasználók kérhetik.

**403 Tiltott: A megfelelő erőforrás API-t választja?**

Az API-szolgáltatások, például a Microsoft Graph, ellenőrzik, hogy a kapott hozzáférési jogkivonatban aud claim (audience) megegyezik-e az elvárt értékkel, és ha nem, a 403 Tiltott hiba jelenik meg. A hibát gyakran az okozza, hogy megpróbál egy Azure AD Graph API-khoz, Outlook API-khoz vagy SharePoint/OneDrive API-khoz beszerzett jogkivonatot használni a Microsoft Graph hívásához (vagy fordítva). Győződjön meg arról, hogy az erőforrás (vagy a hatókör) az app által hívott API-hoz tartozó jogkivonatot szerez be.

**400 Bad Request vagy 403 Tiltott: Betartja a felhasználó a szervezet feltételes hozzáférési szabályzatát?**

A szervezet hitelesítésszolgáltatói szabályzata alapján előfordulhat, hogy az alkalmazáson keresztül Microsoft Graph-erőforrásokhoz hozzáférő felhasználók további információkért nem hatnak az app által eredetileg beszerzett hozzáférési jogkivonatban. Ebben az esetben az app egy 400-as interaction_required kap a *hozzáférési* jogkivonat beszerzésekor, illetve egy 403-as insufficient_claims microsoft Graph-híváskor.  A hibare adott válasz mindkét esetben további információkat tartalmaz, amelyek bemutathatóak a végpontnak, hogy a felhasználó további információkat (például többtényezős hitelesítést vagy eszközregisztrálást) igényelni tudjanak.

- [A feltételes hozzáféréssel kapcsolatos kihívások kezelése mSAL használatával ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Fejlesztői útmutató az Azure Active Directory feltételes hozzáféréséhez](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
