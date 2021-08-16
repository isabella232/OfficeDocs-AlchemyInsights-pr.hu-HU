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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044990"
---
# <a name="configure-and-customize-applications"></a>Alkalmazások konfigurálása és testreszabása

**Alkalmazások konfigurálása**

1. Rövid útmutató: Az alkalmazások tulajdonságainak konfigurálása [a Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) bérlői fiókban bemutatja, hogy miként konfigurálhatja egy alkalmazás néhány tulajdonságát.
2. Az alkalmazásoknak a Azure Active Directory való integrálása érdekében olyan oktatóanyagokat fejlesztettünk, amelyek végigsegítik [a](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) konfiguráláson.
3. [Az alkalmazásproxy-alkalmazások](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) konfigurálása segít megérteni, hogy miként konfigurálhatja az alkalmazásproxy-alkalmazásokat az Azure AD-ban, hogy a helyszíni alkalmazásokat elérhetővé tegye a felhőben.
4. Töltse le a [PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)alkalmazást, és konfigurálja az alkalmazást: A PingAccess konfigurálása az *Azure AD-hez* utasításokat követve védje Microsoft Azure AD Ping Identity webhelyen az alkalmazásproxyval közzétett alkalmazásokat, és töltse le a PingAccess legújabb verzióját.

**Helytelenül konfigurált alkalmazás (AADSTS650056) hibák**

1. Győződjön meg arról, hogy az alkalmazás tulajdonosa által megadott bejelentkezési címről fér hozzá az alkalmazáshoz. Ellenkező esetben a szokásos eljáráson keresztül jelentkezzen be az alkalmazásba. A legtöbb esetben ez a megoldás automatikusan magától megoldódik. Ha nem működik, ez a bejegyzés segíthet a hibaelhárításban és a megoldásban.
2. **Ha az alkalmazás az Ön tulajdonában van** (ami azt jelenti, hogy az alkalmazásregisztráció a szervezetnél van):
    - Legalább azt javasoljuk, hogy a Microsofttól származó vagy delegált engedélyt Graph `User.Read` `openid` meg. 
    - Győződjön meg arról, hogy az alkalmazáshoz és annak minden engedélyhez hozzájárult. Ezt az API-engedélyeken  belüli Alkalmazás-regisztráció Állapot oszlopában **ellenőrizheti.**
    - Bizonyos esetekben előfordulhat, hogy az alkalmazás lehet harmadik fél, de lehet, hogy regisztrálva van a szervezetben. Győződjön meg arról, hogy az alkalmazás szerepel-e az alkalmazás-regisztrációkban (nem nagyvállalati alkalmazásokban).
    - Ha továbbra is megjelenik ez a hibaüzenet. Ebben az esetben lehet, hogy létre kell hoznunk a 4. lépésben ismertetett jóváhagyási **URL-címet.**
3. **Ha nem a szervezete az** alkalmazás tulajdonosa, és külső alkalmazásként használja:
    - Ha Ön a globális/vállalati rendszergazda, a jóváhagyási képernyőt kell látnia. Jelölje be a "Hozzájárulás a szervezet **nevében" jelölőnégyzetet.**
    - Ha nem látja a beleegyezési képernyőt, törölje a Nagyvállalati alkalmazást, és próbálkozzon újra.
    - Ha továbbra is megjelenik ez a hibaüzenet. Ebben az esetben lehet, hogy létre kell hoznunk a 4. lépésben ismertetett jóváhagyási **URL-címet.**
4. **Manuálisan** kell felépítenie a használni kívánt jóváhagyási URL-címet: Ha az alkalmazás úgy lett kialakítva, hogy hozzáférjen egy adott erőforráshoz, előfordulhat, hogy nem használhatja az Azure Portal Hozzájárulás gombjait, manuálisan létre kell hoznia a saját hozzájárulási URL-címét, és ezt kell használnia.
    - Az alkalmazást és a tulajdonost is be kell `{App-Id}` `{App-Uri-Id}` szereznie. `{Tenant-Id}` a bérlő azonosítóját fogja tartalmazni. Ez vagy az `yourdomain.onmicrosoft.com` Ön címtárazonosítója.
    - Ha az alkalmazás az erőforráshoz fér hozzá, akkor az és `{App-Id}` `{App-Uri-Id}` ugyanaz lesz.
5. További információért lásd: Problémák [a bejelentkezés az SAML-alapú egyszeri bejelentkezéses alkalmazásokba.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Alkalmazások testreszabása**

- [Arculat](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) hozzáadása cége Azure Active Directory bejelentkezési lapjához – A szervezet emblémájával és egyéni színsémákkal egységes megjelenést adhat az Azure Active Directory (Azure AD) bejelentkezési lapjainak.
- [Egyéni tartománynév felvétele a Azure Active Directory portálon](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – Minden új Azure AD-bérlő kezdeti tartománynévvel rendelkezik. A kezdeti tartománynevet nem módosíthatja vagy törölheti, de felveheti a szervezet nevét. Az egyéni tartománynevek hozzáadásával olyan felhasználóneveket hozhat létre, amelyek már ismertek a felhasználók számára.
