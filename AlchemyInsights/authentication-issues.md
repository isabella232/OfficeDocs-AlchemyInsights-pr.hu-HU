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
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974487"
---
# <a name="authentication-issues"></a>Hitelesítési problémák

**Az Azure Active Directory (Azure AD) biztonsági jogkivonat-szolgáltatásból (STS) visszaadott AADSTS-hibakódokkal kapcsolatban keres információkat?** Az [Azure AD authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds.

Az engedélyezési hibák számos különböző hiba eredményeként jelenhetnek meg, amelyek nagy része 401-es vagy 403-as hibát generál. Az alábbi problémák például engedélyezési hibákhoz vezethetnek:

- Helytelen [hozzáférési jogkivonat-beszerzések](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Nem megfelelően konfigurált [engedélyhatókörök](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- A hozzájárulás [hiánya](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

A gyakori engedélyezési hibák megoldásához próbálkozzon az alábbi lépésekkel, amelyek a legjobban megfelelnek a kapott hibának. Előfordulhat, hogy egynél több lépés is jelentkezik a hibaüzenet miatt.

- **401 Jogosulatlan hiba: Érvényes a tokenje?**

Győződjön meg arról, hogy az app érvényes hozzáférési jogkivonatot ad a Microsoft Graph-hoz a kérelem részeként. Ez a hiba gyakran azt jelenti, hogy a hozzáférési jogkivonat hiányzik a HTTP-hitelesítés kérésének fejlécében, vagy hogy a jogkivonat érvénytelen vagy lejárt. Kifejezetten javasoljuk, hogy a Microsoft Authentication Library (MSAL) használatával használja a hozzáférési jogkivonat-beszerzést. Ez a hiba akkor is előfordulhat, ha egy személyes Microsoft-fiókhoz megadott delegált hozzáférési jogkivonattal próbál hozzáférni egy olyan API-hoz, amely csak munkahelyi vagy iskolai fiókokat (szervezeti fiókokat) támogat.

**403 Tiltott hiba: A megfelelő engedélykészletet választotta?**

Győződjön meg arról, hogy a megfelelő engedélykészletet kérte az alkalmazáshívásai által biztosított Microsoft Graph API-k alapján. Az ajánlott, legkevesebb jogosultsággal rendelkező engedélyeket a Microsoft Graph API referenciamódszer-témakörei biztosítják. Ezenkívül ezeket az engedélyeket egy felhasználónak vagy egy rendszergazdának kell megadnia az alkalmazásnak. Az engedélyek megadására általában egy jóváhagyási lapon vagy az Azure Portal alkalmazás regisztrációs panelének használatával van szükség. Az alkalmazás **Beállítások** panelen kattintson a **Kötelező** engedélyek elemre, majd az Engedélyek **megadása elemre.** További információ:

- [Microsoft Graph-engedélyek](https://docs.microsoft.com/graph/permissions-reference) 
- [Az Azure AD engedélyeinek és beleegyezésének ismertetése](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Tiltott hiba: Az app a kiválasztott engedélyeknek megfelelő jogkivonatot szerzett be?**

Győződjön meg arról, hogy a kért vagy megadott engedélytípusok megegyeznek az app által beszerzett hozzáférési jogkivonat-típussal. Előfordulhat, hogy alkalmazásengedélyeket kér és ad meg, delegált interaktív kódfolyam-jogkivonatokat használ az ügyfél hitelesítőadat-adatfolyam-tokenek helyett, vagy de delegált engedélyeket kér és ad meg, de ügyfél-hitelesítőadat-folyamat jogkivonatokat használ delegált kódfolyam-jogkivonatok helyett.

A jogkivonatok beszerzésével kapcsolatos további információkért lásd:

- [Hozzáférés a felhasználók és a delegált engedélyek nevében](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 – OAuth 2.0 engedélyezési kódfolyam](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Hozzáférés felhasználói (daemon-szolgáltatás) és alkalmazásengedélyek nélkül](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - OAuth 2.0-ügyfél hitelesítő adatok áramlása](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 – Tiltott hiba: Jelszó alaphelyzetbe állítása**

Jelenleg nincsenek olyan alkalmazásengedélyek, amelyek lehetővé teszik a felhasználói jelszavak alaphelyzetbe állítását. Ezek az API-k csak az interaktív delegált kódfolyamatok használatával támogatottak egy bejelentkezett rendszergazdával. További információ: [Microsoft Graph-engedélyek.](https://docs.microsoft.com/graph/permissions-reference)

**403 Tiltott: Van hozzáférése a felhasználónak, és rendelkezik licenccel?**

Delegált kódfolyamatok esetén a Microsoft Graph kiértékeli, hogy engedélyezve van-e a kérés az appnak adott engedélyek és a bejelentkezett felhasználó engedélyei alapján. Ez a hiba általában azt jelzi, hogy a felhasználó  nincs elég jogosultsággal a kérés végrehajtásához, vagy hogy a felhasználó nem rendelkezik licenccel a megnyitott adatokhoz. A kérelmet csak a szükséges engedélyekkel vagy licencekkel rendelkező felhasználók kérhetik.

**403 Tiltott: A megfelelő erőforrás API-t választja?**

Az API-szolgáltatások, például a Microsoft Graph, ellenőrzik, hogy *a* kapott hozzáférési jogkivonatban aud claim (audience) megegyezik-e az elvárt értékkel, és ha nem, 403-as tiltott hiba történik. A hibát gyakran az okozza, hogy megpróbál egy Azure AD Graph API-khoz, Outlook API-khoz vagy SharePoint/OneDrive API-khoz beszerzett jogkivonatot használni a Microsoft Graph hívásához (vagy fordítva). Győződjön meg arról, hogy az erőforrás (vagy a hatókör) az app által hívott API-hoz tartozó jogkivonatot szerez be.

**400 Bad Request vagy 403 Tiltott: Betartja a felhasználó a szervezet feltételes hozzáférési szabályzatát?**

A szervezet feltételes hozzáférési szabályzata alapján előfordulhat, hogy az appon keresztül a Microsoft Graph-erőforrásokhoz hozzáférő felhasználók további információkért nem hatnak az app eredetileg beszerzett hozzáférési jogkivonatában. Ebben az esetben az app **egy  400-as** interaction_required kap a hozzáférési jogkivonat beszerzésekor, illetve **egy 403-as** insufficient_claims microsoft Graph-híváskor. A hibare adott válasz mindkét esetben további információkat tartalmaz, amelyek bemutathatóak az engedélyezett végpontnak, hogy a felhasználó további információkat (például többtényezős hitelesítést vagy eszköz regisztrálását) igényelni tudjanak.

A feltételes hozzáféréssel kapcsolatos további információkért lásd:

- [A feltételes hozzáféréssel kapcsolatos kihívások kezelése mSAL használatával](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Fejlesztői útmutató az Azure Active Directory feltételes hozzáféréséhez](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Az Azure Active Directory-hitelesítési könyvtár (ADAL) és az Azure AD Graph API (AAD Graph) táma-_*

- 2020. június 30-án kezdődően nem adjuk hozzá új funkciókat az Azure Active Directory hitelesítési tárhoz (ADAL) és az Azure AD Graph API-hoz (AAD Graph). Továbbra is nyújtunk technikai támogatást és biztonsági frissítéseket, de a továbbiakban nem biztosítunk funkciófrissítéseket.
- 2022. június 30-án véget ér az ADAL és az AAD Graph támogatása, és a továbbiakban nem nyújtunk technikai támogatást vagy biztonsági frissítéseket.
    - Az ADAL-t a meglévő operációs rendszerverziókban használó appok ez idő után is működnek, technikai támogatást és biztonsági frissítéseket azonban nem fognak kapni.
    - Előfordulhat, hogy az AAD Graphot ezt követően használó appok a továbbiakban nem kapják meg a válaszokat az AAD Graph-végponttól.

_ *ADAL-áttelepítés**

Azt javasoljuk, hogy frissítsen a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)szolgáltatásra, amely a legújabb funkciókkal és biztonsági frissítésekkel rendelkezik. Ez a javaslat abban a kontextusban van, hogy a Microsoft a támogatási határidő végéig átemeli az alkalmazásait mSAL-re. A Microsoft-appok MSAL-be való áttelepítésének célja, hogy az appok kihasználják a MSAL folyamatos biztonsági és funkciófejlesztésének előnyét.

- [Olvassa el az ADAL-lal kapcsolatos gyakori kérdéseket](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Megtudhatja, hogy miként lehet platformonként áttűnni az alkalmazásokat](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Ha segítségre van szüksége annak megértéséhez, hogy melyik appja használja az ADAL-t, javasoljuk, hogy tekintse át az appok összes forráskódját, és ha lehetséges, bármely független szoftverszállítóhoz vagy alkalmazásszolgáltatóhoz kapcsolatba kell kérnie. A Microsoft ügyfélszolgálata emellett a bérlői fiókjában található nem Microsoft ADAL-appok listáját is meg tudja adni.

**AAD Graph-áttelepítés**

Az AAD Graphot használó alkalmazások esetében kövesse az útmutatót az Azure AD Graph-appok Microsoft Graphba való [áttelepítéséhez.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true)

- [Az áttelepítési ellenőrzőlistánk egy első lépésekre nyújt lehetőséget.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
- Az Azure-app regisztrációs portálján látható, hogy mely alkalmazások használják az AAD Graphot. Javasoljuk, hogy tekintse át az appok összes forráskódját, és ha lehetséges, bármely internetszolgáltatóhoz vagy alkalmazásszolgáltatóhoz. A Microsoft ügyfélszolgálata a bérlői fiókjában az AAD Graph-használattal kapcsolatos információkat is meg tudja adni.

 










