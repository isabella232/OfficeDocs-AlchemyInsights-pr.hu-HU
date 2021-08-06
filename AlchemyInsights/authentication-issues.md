---
title: Hitelesítési problémák
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: c7e6d96940f8d7052ee4b49b22c0d1d7d5bd5f9277f4a7eff709def1da2e13af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019510"
---
# <a name="authentication-issues"></a>Hitelesítési problémák

**Az Azure Active Directory (Azure AD) biztonsági jogkivonat-szolgáltatásból (STS) visszaküldött AADSTS-hibakódok adatait keresi?** További információt az AADSTS hibaleírásokról, javításokról és néhány javasolt kerülő megoldás megkereséséről az [Azure AD hitelesítés és engedélyezés](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) című cikkben talál.

Az engedélyezési hibák több különböző hiba következtében léphetnek fel, amelyek nagy része 401-es vagy 403-as hibát generál. Például az alábbi problémák engedélyezési hibákhoz vezethetnek:

- Helytelen [hozzáférési jogkivonat beszerzési folyamatok](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Rosszul konfigurált [engedély hatókörök](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- [Jóváhagyás](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent) hiánya

A gyakori engedélyezési hibák megoldásához próbálkozzon az alábbi lépésekkel valamelyikével, amely a legjobban megfelel a kapott hibának. Több lépés is alkalmazható lehet a kapott hibára.

**401 Jogosulatlan hozzáférési hiba: Érvényes a jogkivonata?**

Győződjön meg arról, hogy az app a kérés részeként érvényes hozzáférési jogkivonatot ad a Microsoft Graph-hoz. Ez a hiba gyakran azt jelzi, hogy a hozzáférési jogkivonat hiányzik a HTTP hitelesítési kérés fejlécében, vagy hogy a jogkivonat érvénytelen vagy lejárt. Kifejezetten javasoljuk, hogy a Microsoft Authentication Library (MSAL) használatával szerezze be a hozzáférési jogkivonatot. Ez a hiba akkor is előfordulhat, ha egy személyes Microsoft-fióknak megadott meghatalmazási jogkivonatot próbál használni egy olyan API eléréséhez, amely csak munkahelyi vagy iskolai fiókokat (szervezeti fiókokat) támogat.

**403 Tiltott művelet: A megfelelő engedélykészletet választotta ki?**

Ellenőrizze, hogy megfelelő engedélykészletet kérte-e az alkalmazás által hívott Microsoft Graph API-k alapján. Az ajánlott kevésbé kiváltságos engedélyeket a Microsoft Graph API-k összes referenciamódszer-témakörében biztosítjuk. Ezenkívül ezeket az engedélyeket egy felhasználónak vagy egy rendszergazdának kell megadnia az alkalmazásnak. Az engedélyek megadása általában egy jóváhagyási lapon vagy az Azure Portal alkalmazásregisztrációs szolgáltatásának használatával történik. Az alkalmazás **Beállítások** panelén kattintson a **Szükséges engedélyek** elemre, majd kattintson az **Engedélyek megadása** lehetőségre. További információ:

- [Microsoft Graph-engedélyek](https://docs.microsoft.com/graph/permissions-reference) 
- [Az Azure AD engedélyeinek és hozzájárulásainak ismertetése](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Tiltott művelet: Beszerezte az appja a választott engedélyeknek megfelelő jogkivonatot?**

Ellenőrizze, hogy a kért vagy megadott engedélytípusok megegyeznek-e az app által megszerzett hozzáférési jogkivonat-típussal. Előfordulhat, hogy alkalmazásengedélyeket kér és ad ki, de delegált interaktív kódfolyamkódokat használ az ügyfélbeli hitelesítőadat-forgalom jogkivonatai helyett, illetve delegált engedélyeket kér és ad ki, de ügyfél hitelesítőadat-folyam jogkivonatokat használ a delegált kódfolyam jogkivonatok helyett.

A jogkivonatok beszerzésével kapcsolatos további információért lásd:

- [Hozzáférés kérése a felhasználók nevében és meghatalmazott engedélyek](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 – OAuth 2.0 engedélyezési kódfolyam](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Hozzáférés kérése felhasználó (daemon szolgáltatás) és alkalmazásengedélyek nélkül](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 – OAuth 2.0-ügyfél hitelesítőadat-folyam](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Tiltott művelet: Jelszó visszaállítása**

Jelenleg nincsenek olyan alkalmazásengedélyek, amelyek lehetővé teszik a felhasználói jelszavak visszaállítását. Ezek az API-k csak bejelentkezett rendszergazda interaktív delegált kódfolyamával támogatottak. További információt a [Microsoft Graph engedélyek](https://docs.microsoft.com/graph/permissions-reference) lapján találhat.

**403 Tiltott művelet: Van hozzáférése a felhasználónak, és rendelkezik licenccel?**

A delegált kódfolyamatok esetén a Microsoft Graph értékeli, hogy a kérés engedélyezett-e az appnak adott engedélyek és a bejelentkezett felhasználó által biztosított engedélyek alapján. Ez a hiba általában azt jelzi, hogy a felhasználó nem rendelkezik elegendő jogosultsággal ahhoz, hogy végrehajtsa a kérést, **vagy** hogy a felhasználónak nincs licence a hozzáfért adatokhoz. Csak a szükséges engedélyekkel vagy licencekkel rendelkező felhasználók tudnak sikeresen kérelmezni.

**403 Tiltott művelet: Megfelelő forrás API-t választott ki?**

Az API-szolgáltatások, például a Microsoft Graph, ellenőrzik, hogy az *aud* igény (közönség) a kapott hozzáférési jogkivonatban megegyezik-e a várt értékkel, és ha nem, a 403-as Tiltott művelet hiba történik. Gyakori hiba, amely következtében egy Azure AD Graph API-khoz, Outlook API-khoz vagy SharePoint/OneDrive API-khoz beszerzett jogkivonatot hibásan próbál használni a Microsoft Graph hívásához (vagy fordítva). Győződjön meg arról, hogy az adott erőforrás (vagy hatókör) egy olyan jogkivonatot szerez be, amely megfelel az app által hívott API-nak.

**400 Hibás kérelem vagy 403 Tiltott művelet: Megfelel a felhasználó a szervezete feltételes hozzáférésre (CA) vonatkozó irányelveinek?**

A szervezet feltételes hozzáférésre vonatkozó házirendje (CA) alapján előfordulhat, hogy egy felhasználó az Ön appján keresztüli hozzáférése a Microsoft Graph-erőforrásokhoz olyan további adatokat igényel, amelyek nem szerepelnek a hozzáférési jogkivonatban, amelyet az app eredetileg megszerzett. Ebben az esetben az appban egy **400-as, *interaction_required*** típusú hiba történik a hozzáférési jogkivonat beszerzésekor, vagy egy **403-as, *insufficient_claims*** típusú Microsoft Graph hívása esetén. A hiba megjelenése mindkét esetben további információkat tartalmaz, amelyek bemutatják az engedélyezett végpontnak, hogy a felhasználótól további információkat (például többtényezős hitelesítés vagy eszközregisztrálás) igényeljen.

A feltételes hozzáféréssel kapcsolatos további információkért lásd:

- [A feltételes hozzáféréssel kapcsolatos kihívások kezelése az MSAL segítségével](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Fejlesztői útmutató az Azure Active Directory feltételes hozzáféréséhez](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***Az Azure Active Directory Authentication Library (ADAL) és az Azure AD Graph API (AAD-hitelesítés) támogatása Graph)***

- 2020. június 30-tól kezdődően nem adunk hozzá új funkciókat az Azure Active Directory-hitelesítési tár (ADAL) és az Azure AD Graph API (AAD Graph) szolgáltatáshoz. A jövőben is biztosítani fogunk technikai támogatási és biztonsági frissítéseket, funkciófrissítéseket azonban nem.
- 2022. június 30-tól kezdődően véget vetünk az ADAL- és az AAD Graph-támogatásnak, és a továbbiakban nem biztosítunk technikai támogatást és biztonsági frissítéseket.
    - Az ADAL-t már meglévő operációs rendszereken használó appok ezután is működnek, de sem technikai támogatásban, sem biztonsági frissítésben nem részesülnek.
    - Előfordulhat, hogy az AAD Graphot használó appok ezt követően nem kapnak választ az AAD Graph-végponttól.

**ADAL-áttelepítés**

Javasoljuk, hogy frissítsen a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) szolgáltatásra, amely a legújabb funkciókat és biztonsági frissítéseket használja. Ezt azzal kapcsolatban javasoljuk, hogy a Microsoft az alkalmazásait MSAL-re telepíti át a támogatás megszűnésének határidejére. A Microsoft-appok MSAL-be való áttelepítésének célja annak biztosítása, hogy az appok kihasználják az MSAL folyamatos biztonsági és funkciófejlesztéseit.

- [Az ADAL GYIK elolvasása](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [További információ az appok áttelepítéséről platformonként](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Ha segítségre van szüksége annak megértéséhez, hogy mely alkalmazásai használják az ADAL-t, javasoljuk, hogy tekintse át valamennyi app forráskódját, és ha lehetséges, független szoftvergyártóktól (ISV-k) vagy alkalmazásszolgáltatóktól is segítséget kérhet. A Microsoft terméktámogatási szolgálata a bérlői fiókban a nem Microsoft rendszerű ADAL-appok listáját is biztosítja.

**AAD Graph-áttelepítés**

Az AAD Graphot használó alkalmazások esetén kövesse az [Azure AD Graph-appok áttelepítése a Microsoft Graphba](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true) témakörben leírtakat.

- [Az áttelepítési ellenőrzőlista segít az első lépésekben](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Az Azure-appok regisztrációs portálján látható, hogy mely alkalmazások használják az AAD Graphot. Javasoljuk, hogy tekintse át az összes app forráskódját, és ha lehetséges, forduljon bármely szoftverszolgáltatóhoz vagy alkalmazásszolgáltatóhoz. A Microsoft terméktámogatási szolgálata a bérlői fiókban található összes AAD Graph-használatra vonatkozó adatokat is biztosítja.

 










