---
title: Az OIDC-alapú zökkenőmentes egyszeri bejelentkezéssel kapcsolatos problémák elhárítása
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745023"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Az OIDC-alapú zökkenőmentes egyszeri bejelentkezéssel kapcsolatos problémák elhárítása

- Ha meg szeretne tudni, hogy miként adhat hozzá egy OIDC-alapú appot azure-bérlőjéhez, olvassa el a rövid [útmutató: OIDC-alapú](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)egyszeri bejelentkezés beállítása egy alkalmazáshoz az Azure Active Directory (Azure AD) bérlői fiókban.
- Az OpenID Connect standardot az egyszeri bejelentkezés implementálja appokkal kapcsolatos további részletekért lásd az [OIDC-alapú egyszeri bejelentkezés használata.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Ha arra az esetre, ha úgy dönt, hogy a kódot közvetlenül a HTTP-kérelmek küldésével és kezelésével írja meg, vagy egy külső gyártótól származó nyílt forráskódú tárat használ egy nyílt forráskódú tár használata helyett, tekintse meg az [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)és az OpenID Connect protokollokat a Microsoft identitásplatformján.

**Protokollok**

1. [Microsoft-identitásplatform](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) és implicit grant flow – Az implicit grant meghatározása az, hogy a tokeneket (azonosítótokeneket vagy hozzáférési jogkivonatokat) közvetlenül a /authorize végpontról adja vissza a rendszer a /token végpont helyett. Ezt gyakran használják az engedélyezési kód folyamatának részeként, a **"hibrid folyamat"** részeként – a /authorize kérésen az azonosítókód lekérése egy engedélyezési kóddal együtt. Ez a cikk azt ismerteti, hogy miként programolhat közvetlenül az alkalmazás protokollja alapján, és hogyan kérhet jogkivonatokat az Azure AD-től.
2. [Microsoft-identitásplatform és OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) engedélyezési kódfolyam – Az OAuth 2.0 engedélyezési kód megadása az eszközön telepített appokban használható a védett erőforrásokhoz, például a webes API-khoz való hozzáféréshez. Az OAuth 2.0 Microsoft-identitásplatformjának implementációja segítségével bejelentkezési és API-hozzáférést adhat a mobil- és **asztali alkalmazásokhoz.** Ez a cikk azt ismerteti, hogy miként programozni közvetlenül az alkalmazás protokollja ellen bármilyen nyelven.
3. [Microsoft identitásplatform](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) és OpenID Connect protokoll – Ha a Microsoft identitásplatform OpenID Connect-implementációját használja, hozzáadhat bejelentkezést és API-hozzáférést az appjaihoz. Ebből a cikkből megtudhatja, hogy ezt hogyan kell a nyelvtől függetlenül megtenni, és ismerteti, hogy miként küldhet és fogadhat HTTP-üzeneteket a Microsoft nyílt forráskódú **tárainak használata nélkül.**
4. [Microsoft-identitásplatform és OAuth 2.0-ügyfél](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) hitelesítőadat-forgalom – Az RFC 6749 szabványban (más néven kétlevelű **OAuth)** megadott OAuth 2.0-ügyfél hitelesítő adatokkal elérheti a webes erőforrásokat egy alkalmazás identitásával. Ezt a fajta támogatástípust általában kiszolgálók közötti interakciókhoz használják, amelyek a háttérben kell futniuk anélkül, hogy azonnali interakcióba esnek a felhasználókkal. Az ilyen típusú alkalmazásokat gyakran **daemonnak vagy szolgáltatásfióknak** **nevezik.** Ez a cikk azt ismerteti, hogy miként programozni közvetlenül az alkalmazás protokollja ellen.
