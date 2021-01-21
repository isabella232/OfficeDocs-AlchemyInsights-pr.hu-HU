---
title: Tokenekkel kapcsolatos problémák
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
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916841"
---
# <a name="issues-with-tokens"></a>Tokenekkel kapcsolatos problémák

A jogkivonatokkal kapcsolatos problémák kezeléséhez végezze el az alábbi lépéseket:

1. Megadhatja a Microsoft identitásplatform által kibocsátott hozzáférési, azonosító- vagy SAML-jogkivonat élettartamát. Beállíthatja a jogkivonat élettartamát a szervezet összes appja, egy több-bérlős (több szervezetből álló) alkalmazás vagy egy adott szolgáltatásnév számára a szervezetben. További információt a Konfigurálható jogkivonat-élettartamok a [Microsoft identitásplatformján (előzetes verzió) található.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
2. A hozzáférési jogkivonatok lehetővé teszik az ügyfelek számára a védett webes API-k biztonságos hívását, és a webes API-k hitelesítést és hitelesítést hajtenek végre. Az OAuth-specifikáció szerint a hozzáférési jogkivonatok átlátszatlan karakterláncok beállított formátum nélkül – egyes identitásszolgáltatók GUID azonosítókat, mások titkosított blobokat használnak. A Microsoft identitásplatform számos hozzáférési jogkivonat-formátumot használ attól függően, hogy az API milyen konfigurációban fogadja el a jogkivonatot. Ha tudni szeretne arról, hogy az API miként érvényesítheti és használhatja a hozzáférési jogkivonaton belüli jogcímeket, olvassa el a [Microsoft identitásplatform-hozzáférési jogkivonatokat.](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint)
3. A Microsoft Authentication Library (MSAL) számos hitelesítési folyamat használatát támogatja a különböző alkalmazás helyzetekben. További információt a [Hitelesítés folyamatában.](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes)
4. Az OAuth 2.0 engedélyezési kód megadása az eszközön telepített appokban használható a védett erőforrásokhoz, például a webes API-khoz való hozzáféréshez. Az OAuth 2.0 Microsoft identitásplatformjának implementációja segítségével bejelentkezési és API-hozzáférést adhat a mobil- és asztali appok számára. A [Microsoft identitásplatformjának és az OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) engedélyezési kódfolyamának használatával közvetlenül az alkalmazás protokollja szerint, bármilyen nyelven programolhat.
5. Az OpenID Connect (OIDC) egy OAuth 2.0-ra készült hitelesítési protokoll, amely segítségével biztonságosan bejelentkezhet egy felhasználóba. Amikor a Microsoft identitásplatform végpontjának OpenID Connect-implementációját használja, bejelentkezési és API-hozzáférést adhat az appjaihoz. [A Microsoft identitásplatformja](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) és az OpenID Connect protokoll azt mutatja be, hogy ezt miként kell a nyelvtől függetlenül megtenni, és ismerteti, hogy miként küldhet és fogadhat HTTP-üzeneteket a Microsoft nyílt forráskódú tárak használata nélkül.
    - A UserInfo végpont az OIDC szabvány része, amely a hitelesített felhasználóra vonatkozó igények visszaadása érdekében készült. További információt a [Microsoft-identitásplatform UserInfo végpontján található.](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead)
    - A webalkalmazások Azure AD és [OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) használatával történő hívása minta bemutatja, hogy miként építhet fel egy Azure AD-t használó MVC-webalkalmazást az OpenID Connect protokoll használatával történő bejelentkezéshez, majd hogyan hívhat meg egy webes API-t a bejelentkezett felhasználó identitása alatt az OAuth 2.0-n keresztül kapott jogkivonatok használatával. Ez a minta az OpenID Connect ASP .Net OWIN middleware és az ADAL .Net szoftvert használja.
6. [Konfigurálhat egy alkalmazást a webes API-k](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) elérhetővé való beállítására – ebben a rövid útmutatóban regisztrál egy webes API-t a Microsoft identitásplatformján, és egy példa hatókör hozzáadásával elérhetővé teszi azt az ügyfélalkalmazások számára. Ha regisztrálja a webes API-t, és a hatókörök között ki is teszi, engedélyalapú hozzáférést biztosít az erőforrásaihoz az API-t elelérésre jogosult felhasználók és ügyfélalkalmazások számára.
7. Az Azure Active Directory B2C -ben (Azure AD B2C) az erőforrás-tulajdonosi jelszó hitelesítő adatai (ROPC) egy OAuth-szabványos hitelesítési folyamat. Ebben a folyamatban egy alkalmazás, más néven a függőben maradó fél érvényes hitelesítő adatokat ad a tokenekhez. A hitelesítő adatok közé tartozik egy felhasználói azonosító és egy jelszó. A visszaadott jogkivonat egy azonosítótoken, egy hozzáférési jogkivonat és egy frissítési jogkivonat. További információ: Erőforrás-tulajdonosi jelszó hitelesítő adatainak beállítása az [Azure Active Directory B2C szolgáltatásban.](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow) 

