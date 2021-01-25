---
title: Hivatkozásokkal és URL-címekkel kapcsolatos problémák
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974466"
---
# <a name="issues-with-links-and-urls"></a>Hivatkozásokkal és URL-címekkel kapcsolatos problémák

Az URI-/válasz URL-címek (mindkét kifejezés felcserélhetők) a Microsoft identitásplatform által az app által kért jogkivonatok visszaadása érdekében használt URL-címek. Ezekről az URL-címekről az alábbi cikkekben talál további információt:

- [Authentication flow and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIS in the **App registration** page for each scenario.
- [Az URI/válasz URL-címére vonatkozó korlátozások és korlátozások átirányítása](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Nem tudom, hogyan regisztrálható a megfelelő átirányítási URI/válasz URL-cím az alkalmazásomhoz**

Ha a fejlesztetlen alkalmazással jelentkezik be, és a bejelentkezési párbeszédpanelen megjelenik az **AADSTS50011: <your app ID>** A kérésben megadott válasz URL-cím nem egyezik az alkalmazáshoz konfigurált válasz URL-címével, hozzá kell adni az alkalmazás regisztrációját, a tokenkérésben használt kód által használt URI-t a Microsoft identitásplatformhoz.

Válasz URL-címének hozzáadásához  az Azure  Portal alkalmazásregisztrációs lapján a Hitelesítés lapon vegyen fel egy bejegyzést az **URI-k átirányítása szakaszban.** Az átirányítási URI-k be vannak gépelve (webes vagy mobil/asztali). Az érték, amit meg kell adnia, attól függ, hogy milyen típusú alkalmazást épít, az alábbiak szerint:

- Egyoldalas alkalmazások és webalkalmazások esetén a válasz URL-címe az alkalmazás URL-címe. [Egyoldalas alkalmazásregisztráció vagy](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) [webalkalmazás regisztrálása](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal) az Azure Portal használatával
- Az asztali appok esetében a választania kell érték a következőtől függ:
    - a platform (a MacOS eltér a Windowstól vagy a Linuxtól)
    - a jogkivonat megszerzésének módja (interaktív módon, eszközkód-forgalommal, integrált Windows-hitelesítéssel [IWA] vagy felhasználónévvel/jelszóval).
    Részleteket az asztali [alkalmazások – alkalmazásregisztráció – URi átirányítása](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Mobilappok esetében az átirányítási URI a következőtől függ:
    - platform (iOS/Android/UWP)
    - az app felépítéséhez használt információk, például az iOS csomagazonosítója és az Android csomagneve és aláírási kivonata Az Azure Portal app regisztrációja segít. Részletes információkért lásd [a platformkonfigurációt és az URI-k átirányítását.](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)

> [!NOTE]
> A webes API-k és a tokenek beszerzésének néhány csendes módja (IWA és felhasználónév/jelszó) nem igényel átirányítási URI-t.

**Üzembe helyeztem a webalkalmazást, és amikor tesztelem a telepített appot, hibaüzenet jelenik meg a válasz URL-címével való eltérésről**

Adjon hozzá átirányítási URI-okat az összes olyan helyhez, ahol telepíti a webalkalmazást. További információ: [Webalkalmazás regisztrálása](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)az Azure Portal használatával.

> [!NOTE]
> Adja hozzá az átirányítási URI-t egy helyhez közvetlenül azt követően, hogy telepítette az alkalmazást az adott helyen.

**Nem tudok elegendő válasz URL-t regisztrálni**

Ön isv- és egy vagy több átirányítási URI-vel van minden ügyfél számára. Az ADAL/Azure AD 1.0-s verziójáról MSAL/a Microsoft-identitásplatformra szeretne áttérni, és a maximális számú átirányítási [URI-t kell látnia.](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris) A probléma megoldásához adjon [átirányítási URI-t](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) az egyes ügyfeleknek megfelelő egyszerű szolgáltatásnévhez.
