---
title: Az OAuth 2.0 és az OpenID Connect protokollal kapcsolatos hibák elhárítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036406"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Az OAuth 2.0 és az OpenID Connect protokollal kapcsolatos hibák elhárítása

Az OAuth 2.0 és az OpenID Connect problémáinak megoldásához végezze el az alábbi ajánlott lépéseket:

Az OAuth 2.0 és az OpenID Connect protokoll konfigurációját és hibaelhárítását az alábbi cikkekben talál:

- [Microsoft identitásplatform és OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) engedélyezési kódfolyam – Ez a cikk azt ismerteti, hogy miként programozni közvetlenül a kód grant **(PKCE)** folyamaton keresztül, bármilyen nyelven.
- [Microsoft-identitásplatform és OAuth 2.0-ügyfél](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) hitelesítőadat-forgalom –  Ez a cikk azt ismerteti, hogy miként programozni közvetlenül az ügyfél hitelesítőadat-adatfolyamához az alkalmazásban.
- [A Microsoft identitásplatformja és az OAuth 2.0 erőforrás-tulajdonosi](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) jelszó hitelesítő adatai – Ez a cikk azt ismerteti, hogy miként programozni közvetlenül az alkalmazás **ROPC-folyamatába.**
    - A Microsoft identitásplatform csak Azure AD-bérlők roPC-használatát támogatja, személyes fiókok esetében nem. Ez azt jelenti, hogy bérlőspecifikus végpontot **( https://login.microsoftonline.com/{TenantId_or_Name})** vagy a **szervezeti végpontot) kell** használnia.
    - Az Azure AD-bérlőkbe meghívott személyes fiókok nem használhatnak ROPC-t.
    - A jelszóval nem rendelkező fiókok nem tudnak bejelentkezni roPC-n keresztül. Ebben az esetben azt javasoljuk, hogy használjon helyettük egy másik folyamatot az apphoz.
    - Ha a felhasználóknak többtényezős hitelesítést [(MFA) kell](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) használnia az alkalmazásba való bejelentkezéshez, a rendszer letiltja őket.
    - A roPC nem [](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) támogatott hibrid identitás-összevonási forgatókönyvekben (például a helyszíni fiókok hitelesítéséhez használt Azure AD és ADFS). Ha a felhasználók teljes lapra vannak átirányítva egy helyszíni identitásszolgáltatóhoz, az Azure AD nem tudja tesztelni a felhasználónevet és a jelszót az adott identitásszolgáltatóval. [A roPC azonban](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) támogatja az áteső hitelesítést.
    - Kivételt képeznek a hibrid identitás-összevonási esetek: Ha a Home Realm Discovery házirend az **AllowCloudPasswordValidation** beállítás **IGAZ** értékű, akkor a ROPC-forgalom működni fog az összevont felhasználók számára, amikor a helyszíni jelszó szinkronizálva van a felhővel. További információt az Összevont felhasználók közvetlen ROPC-hitelesítésének engedélyezése a [régi alkalmazásokhoz](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Microsoft identitásplatform és OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) – Ez a cikk azt ismerteti, hogy miként programozni közvetlenül az alkalmazáson belül a más nevében történő **(STB)-adatfolyamon** keresztül.
- [Microsoft identitásplatform](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) és OpenID Connect protokoll – Ebből a cikkből megtudhatja, hogy miként implementálja az OpenID Connect protokollt a nyelvtől függetlenül, és azt is bemutatja, hogy miként küldhet és fogadhat HTTP-üzeneteket a Microsoft nyílt forráskódú tárainak használata nélkül.

**Hozzáférési jogkivonatok**

[Microsoft identitásplatform-hozzáférési jogkivonatok](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Ismerje meg, hogy az API hogyan érvényesítheti és használhatja a jogcímeket egy hozzáférési jogkivonaton belül. A cikkben található összes dokumentáció(a feljegyzett kivételével) csak a regisztrált API-khoz kibocsátott jogkivonatokra vonatkozik. Nem vonatkozik a Microsoft tulajdonában lévő API-khoz kibocsátott jogkivonatokra, és nem is használhatók ezek a tokenek annak érvényesítésére, hogy a Microsoft identitásplatform hogyan fog jogkivonatokat kiállítani egy Ön által létrehozott API-hoz.

**Alkalmazáskonfiguráció**

[URI (válasz URL-cím) korlátozásai és korlátainak átirányítása](https://docs.microsoft.com/azure/active-directory/develop/reply-url) – Itt megtudhatja, hogy miként konfigurálhatja az átirányítási URI-t (válasz URL-címét). Az átirányítási URI-t (más szóval válasz URL-címét) az a hely, ahová az engedélyezési kiszolgáló elküldi a felhasználót, miután az appot sikeresen engedélyezte, és hozzáférési kódot vagy hozzáférési jogkivonatot adott a felhasználónak. Az engedélyezési kiszolgáló elküldi a kódot vagy a jogkivonatot az átirányítási URI azonosítónak; ezért fontos, hogy az alkalmazás-regisztrációs folyamat részeként regisztrálja a megfelelő helyet.

**Alkalmazás kiépítése**

[Oktatóprogram: SCIM-végpont](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) kiépítésének kidolgozása és megtervezése – Ez a cikk ismerteti, hogy miként építhet fel egy SCIM-végpontot, és hogyan integrálhatja azt az AAD kiépítési szolgáltatásával.


