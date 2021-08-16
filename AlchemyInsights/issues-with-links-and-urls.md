---
title: Hivatkozásokkal és URL-címekkel kapcsolatos problémák
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 1387d7e0cdf2e730b2812f3970181d2bf889d44b1faab9a351911840909defb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054800"
---
# <a name="issues-with-links-and-urls"></a>Hivatkozásokkal és URL-címekkel kapcsolatos problémák

Az átirányítási URI-k, illetve válaszolási URL-címek (ez a két kifejezés gyakorlatilag ugyanazt jelenti) azok az URL-címek, amelyeket a Microsoft identitásplatform használ az alkalmazások által kért jogkivonatok visszaküldéséhez. Ezekről az URL-címekről az alábbi cikkekben olvashat:

- [Hitelesítési folyamatok és alkalmazási helyzetek](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – információ az **Alkalmazásregisztráció** lapon látható átirányítási URI-król az egyes esetekben
- [Az átirányítási URI-ra/válaszolási URL-címre vonatkozó korlátozások és megkötések](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Nem tudom, hogyan regisztrálhatom a megfelelő átirányítási URI-t/válaszolási URL-címet az alkalmazásomhoz.**

Ha a fejlesztés alatt álló alkalmazásával való bejelentkezéskor megjelenik a bejelentkezési párbeszédpanelen az **AADSTS50011: A kérelemben megadott válaszolási URL nem egyezik az alkalmazáshoz konfigurált válaszolási URL-címekkel<your app ID>** üzenet, akkor fel kell vennie az alkalmazás regisztrációjába azt az átirányítási URI-t, amelyet a kódja a Microsoft identitásplatformnak küldött jogkivonat-kérelemben használt.

Válaszolási URL-cím megadásához válassza az Azure Portal **Alkalmazásregisztráció** lapján levő **Hitelesítés** lapfület, és vegyen fel egy bejegyzést az **Átirányítási URI-k** szakaszban. A beírandó érték attól függ, hogy milyen típusú alkalmazást készít, az alábbiak szerint:

- Egylapos alkalmazások és webalkalmazások esetében a válaszolási URL az alkalmazásban levő URL-címnek felel meg. Erről az [Egylapos alkalmazás regisztrálása](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) és a [Webalkalmazás regisztrálása az Azure Portal használatával](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal) című cikkben olvashat.
- Asztali alkalmazások esetében a kiválasztandó érték a következőktől függ:
    - a platformtól (MacOS esetén más érték szükséges, mint Windows vagy Linux esetén),
    - a jogkivonat beszerzési módjától (interaktív módon, az eszköz kódfolyamával, integrált Windows-hitelesítéssel vagy felhasználónév/jelszó megadásával).
    További részletek az [Asztali alkalmazások: alkalmazás regisztrálása – Átirányítási URI-k](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris) című cikkben olvashatók.
- Mobilalkalmazások esetében az átirányítási URI a következőktől függ:
    - a platformtól (iOS/Android/UWP),
    - az alkalmazás összeállításához használt információktól, például az iOS-hez használt csomagazonosítótól, illetve az Androidhoz használt csomagnévtől és aláírási kivonattól. Az Azure Portal alkalmazásregisztrációs felülete segít majd ebben. További részletek a [Platform konfigurálása és átirányítási URI-k](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris) című cikkben olvashatók.

> [!NOTE]
> A webes API-khoz és a jogkivonatok csendes módon való beszerzésének egyes módszereihez (integrált Windows-hitelesítés, illetve felhasználónév/jelszó) nincs szükség átirányítási URI-ra.

**Üzembe helyeztem a webalkalmazásomat, és a telepített alkalmazás tesztelésekor a válaszolási URL eltérésére figyelmeztető üzenet jelenik meg.**

Vegyen fel átirányítási URI-t minden olyan helyhez, ahol üzembe helyezi a webalkalmazást. További információ a [Webalkalmazás regisztrálása az Azure Portal használatával](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration) című cikkben olvasható.

> [!NOTE]
> Azonnal vegyen fel átirányítási URI-t az egyes helyekhez, amint üzembe helyezte az alkalmazást az adott helyen.

**Nem tudok elég válaszolási URL-címet regisztrálni.**

Ön internetszolgáltató, és mindegyik ügyfeléhez tartozik egy vagy több átirányítási URI. Szeretne áttérni az ADAL/Azure AD 1.0-s verziójáról az MSAL/Microsoft identitásplatform használatára, és elérte az [átirányítási URI-k maximális számát](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). A probléma megoldásához vegyen fel [átirányítási URI-kat az egyes ügyfeleinek megfelelő szolgáltatásnevekhez](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals).
