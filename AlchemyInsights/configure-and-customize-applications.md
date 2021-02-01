---
title: Alkalmazások konfigurálása és testreszabása
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063657"
---
# <a name="configure-and-customize-applications"></a>Alkalmazások konfigurálása és testreszabása

**Alkalmazások konfigurálása**

1. [Gyorsútmutató: Egy](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) alkalmazás tulajdonságainak konfigurálása az Azure Active Directory (Azure AD) bérlői fiókban azt mutatja be, hogy miként konfigurálhatja egy alkalmazás néhány tulajdonságát.
2. Az alkalmazások Azure Active Directoryval való integrálása érdekében fejlesztettünk egy olyan oktatóanyag-gyűjteményt, amely végigsegíti [a](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) konfiguráción.
3. [Az alkalmazásproxy-alkalmazások](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) konfigurálása segít megérteni, hogy miként konfigurálhatja az alkalmazásproxy-alkalmazásokat az Azure AD-ban, hogy a helyszíni alkalmazásokat elérhetővé tegye a felhőben.
4. Töltse le a PingAccess fájlt, és konfigurálja [az alkalmazást:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)A PingAccess konfigurálása az Azure AD-hez parancsra vonatkozó utasításokat követve védje a Ping Identity webhelyen a Microsoft Azure AD alkalmazásproxyval közzétett alkalmazásokat, és töltse le a *PingAccess* legújabb verzióját.

**Helytelenül konfigurált alkalmazás (AADSTS650056) hibák**

1. Győződjön meg arról, hogy az alkalmazás tulajdonosa által megadott bejelentkezési címről fér hozzá az alkalmazáshoz. Ellenkező esetben a szokásos eljáráson keresztül jelentkezzen be az alkalmazásba. A legtöbb esetben ez magától magától megoldódik. Ha nem, akkor ez a bejegyzés segíthet a hibaelhárításban és a megoldásában.
2. **Ha az alkalmazás az Ön tulajdonában van** (ami azt jelenti, hogy az alkalmazásregisztráció a szervezetnél van):
    - Azt javasoljuk, hogy legalább a Microsoft Graphtól származó vagy `User.Read` `openid` delegált engedélyt is hozzáadja. 
    - Győződjön meg arról, hogy az alkalmazás és az összes engedélye hozzájárult. Ezt az API-engedélyekben  az Alkalmazásregisztráció Állapot oszlopában **ellenőrizheti.**
    - Bizonyos esetekben előfordulhat, hogy az alkalmazás külső fél, de előfordulhat, hogy regisztrálva van a szervezetében. Győződjön meg arról, hogy az alkalmazás szerepel-e az alkalmazásregisztrációkban (nem nagyvállalati alkalmazásokban).
    - Ha továbbra is megjelenik ez a hibaüzenet. Ezután előfordulhat, hogy létre kell hoznunk a 4. lépésben ismertetett jóváhagyási **URL-címet.**
3. **Ha a szervezete nem az alkalmazás tulajdonosa,** és azt külső alkalmazásként használja:
    - Ha Ön a globális/vállalati rendszergazda, látnia kell a jóváhagyási képernyőt. Jelölje be a "Jóváhagyás a szervezet **nevében" jelölőnégyzetet.**
    - Ha nem látja a beleegyezési képernyőt, törölje a Nagyvállalati alkalmazást, és próbálkozzon újra.
    - Ha továbbra is megjelenik ez a hibaüzenet. Ezután előfordulhat, hogy létre kell hoznunk a 4. lépésben ismertetett jóváhagyási **URL-címet.**
4. **Manuálisan** hozza létre a használni kívánt jóváhagyási URL-címet: Ha az alkalmazás egy adott erőforrás elérésére van tervezve, előfordulhat, hogy nem tudja használni az Azure Portalon található Jóváhagyási gombokat, manuálisan kell létrehoznia a saját jóváhagyási URL-címét, és ezt kell használnia.
    - Meg kell szereznie az alkalmazást és a `{App-Id}` `{App-Uri-Id}` tulajdonost. `{Tenant-Id}` azonosító lesz a bérlői webhelyen. Ez vagy a `yourdomain.onmicrosoft.com` címtárazonosítója lesz.
    - Ha az alkalmazás saját maga fér hozzá az erőforráshoz, akkor az és `{App-Id}` `{App-Uri-Id}` ugyanaz lesz.
5. További információt az [SAML-alapú](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)egyszeri bejelentkezéshez konfigurált alkalmazásokba való bejelentkezés problémáiról tartalmaz.

**Alkalmazások testreszabása**

- [Arculat](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) hozzáadása a szervezet Azure Active Directory bejelentkezési lapjához – A szervezet emblémája és egyéni színsémák használatával egységes megjelenést és megjelenést biztosít az Azure Active Directory (Azure AD) bejelentkezési lapjaihoz.
- [Egyéni tartománynév felvétele az Azure Active Directory portálon](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – Minden új Azure AD-bérlő kezdeti tartománynévvel rendelkezik. A kezdeti tartománynevet nem módosíthatja vagy törölheti, de hozzáadhatja a szervezete nevét. Az egyéni tartománynevek hozzáadásával olyan felhasználóneveket hozhat létre, amelyek ismerősek a felhasználóknak.
