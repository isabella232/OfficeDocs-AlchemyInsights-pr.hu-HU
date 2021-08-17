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
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105780"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Az OIDC-alapú zökkenőmentes egyszeri bejelentkezéssel kapcsolatos problémák elhárítása

- Ha meg szeretne tudni, hogy miként adhat hozzá egy OIDC-alapú appot azure-bérlőjéhez, olvassa el a Rövid [útmutató: OIDC-alapú](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)egyszeri bejelentkezés beállítása egy alkalmazáshoz az Azure Active Directory -bérlőben (Azure AD) bérlői fiókban.
- Az OpenID Csatlakozás-alapú egyszeri bejelentkezés implementálja appokkal kapcsolatos további részletekért lásd: [Az OIDC-alapú](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)egyszeri bejelentkezés használata.
- Ha arra az esetre, ha a http-kérelmek közvetlen küldésével és kezelésével írna kódot, vagy egy külső gyártótól származó nyílt forráskódú tárat használna egy nyílt forráskódú tár használata helyett, tekintse át az [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)és az OpenID Csatlakozás protokollokat a Microsoft Identitásplatform.

**Protokollok**

1. [Microsoft Identitásplatform és implicit grant flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) – Az implicit grant meghatározása az, hogy a tokeneket (azonosítótokeneket vagy hozzáférési jogkivonatokat) közvetlenül a /authorize végpontról adja vissza a rendszer a /token végpont helyett. Ezt gyakran használják az engedélyezési kód folyamatának részeként, a **"hibrid folyamat"** részeként – a /authorize kérésen az azonosítókód lekérése egy engedélyezési kóddal együtt. Ez a cikk azt ismerteti, hogy miként programolhat közvetlenül az alkalmazás protokollja alapján, és hogyan kérhet jogkivonatokat az Azure AD-től.
2. Microsoft Identitásplatform és [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) engedélyezési kódfolyam – Az OAuth 2.0 engedélyezési kód megadása az eszközön telepített appokban használható a védett erőforrásokhoz, például a webes API-khoz való hozzáféréshez. Az OAuth 2.0 Microsoft Identitásplatform implementációja segítségével hozzáadhatja a bejelentkezést és az API-hozzáférést a mobil- és asztali **alkalmazásokhoz.** Ez a cikk azt ismerteti, hogy miként programozni közvetlenül az alkalmazás protokollja ellen bármilyen nyelven.
3. [Microsoft Identitásplatform és OpenID Csatlakozás protokoll](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – Ha az Microsoft Identitásplatform OpenID Csatlakozás implementációját használja, hozzáadhatja az alkalmazásokhoz a bejelentkezést és az API-hozzáférést. Ebből a cikkből megtudhatja, hogy ezt hogyan kell a nyelvtől függetlenül megtenni, és ismerteti, hogy miként küldhet és fogadhat HTTP-üzeneteket a Microsoft nyílt forráskódú **tárainak használata nélkül.**
4. Microsoft Identitásplatform és [az OAuth 2.0-ügyfél](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) hitelesítőadat-adatfolyama – Az RFC 6749 szabványban (rfC 6749) megadott OAuth 2.0-s ügyfél hitelesítő adatokkal egy alkalmazás identitásával férhet hozzá a webes erőforrásokhoz.  Ezt a fajta támogatástípust általában kiszolgálók közötti interakciókhoz használják, amelyek a háttérben kell futniuk anélkül, hogy azonnali interakcióba esnek a felhasználókkal. Az ilyen típusú alkalmazásokat gyakran **daemonnak vagy szolgáltatásfióknak** **nevezik.** Ez a cikk azt ismerteti, hogy miként programozni közvetlenül az alkalmazás protokollja ellen.
