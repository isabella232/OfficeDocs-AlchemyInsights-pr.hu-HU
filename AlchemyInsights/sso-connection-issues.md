---
title: SSO-kapcsolati problémák
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
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935151"
---
# <a name="sso-connection-issues"></a>SSO-kapcsolati problémák

1. Kövesse [a rövid útmutatót: Az alkalmazás-útmutató tulajdonságainak](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) konfigurálása az alkalmazás konfigurálához.
2. Attól függően, hogy milyen alkalmazást és [egyszeri bejelentkezést](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) választott, kövesse az alábbi megfelelő útmutatást:
    - Ha egy  helyszíni alkalmazást **konfigurálni a SAML-alapú** egyszeri bejelentkezéshez, tekintse meg a SAML egyszeri bejelentkezést az alkalmazásproxyval telepített helyszíni [alkalmazásokhoz.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - A **felhőalapú alkalmazás** jelszóalapú egyszeri bejelentkezéshez való konfigurálásról további tudni **fogja,** hogy konfigurálja a jelszó [egyszeri bejelentkezését.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Ha egy **helyszíni alkalmazást konfigurálni** az alkalmazásproxyn keresztüli egyszeri bejelentkezéshez, tekintse meg az alkalmazásproxyval történő egyszeri bejelentkezéshez szükséges [jelszó-tárolót.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Alkalmazásproxyval** kapcsolatos problémák elhárítása: Azt javasoljuk, [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)hogy először tekintse át a hibaelhárítási folyamatot, az alkalmazásproxy-összekötő hibáit, és állapítsa meg, hogy az alkalmazásproxy-összekötők megfelelően vannak-e konfigurálva. Ha továbbra is problémákat okoz az alkalmazáshoz való kapcsolódás, kövesse a hibakeresési [alkalmazásproxyval](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)kapcsolatos problémák hibaelhárítási folyamatát. A [KORI-problémákat a](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) böngésző hibakeresési eszközeivel azonosíthatja:
    - Indítsa el a böngészőt, és keresse meg a webalkalmazást.
    - Nyomja le **az F12 billentyűt** a hibakeresési konzolhoz való bekapcsoláshoz.
    - Próbálja meg reprodukálni a tranzakciót, és tekintse át a konzolüzenetet. A CORS-szabálysértés konzolhiba esetén a forrással kapcsolatos hibát jelez.
    - Egyes CORS-problémákat nem lehet megoldani, például amikor az app átirányítja a login.microsoft.com hitelesítéshez, és a hozzáférési jogkivonat lejár. A CORS-hívás ezután meghiúsul. Kerülő megoldásként meghosszabbíthatja a hozzáférési jogkivonat teljes élettartamát, hogy megakadályozza, hogy lejár a felhasználó munkamenete során. Ennek mikéntjeről a Konfigurálható jogkivonat-élettartamok a [Microsoft identitásplatformján olvashatók.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. **AZ SAML-alapú egyszeri** bejelentkezéssel kapcsolatos hibák elhárítása: Azt javasoljuk, hogy ellenőrizze az [SAML-alapú](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)egyszeri bejelentkezéssel konfigurált alkalmazásokba való bejelentkezéssel kapcsolatos problémákat, hogy megtalálja a leggyakoribb problémák megoldását.
5. **Jelszóalapú egyszeri** bejelentkezéssel kapcsolatos hibák elhárítása: Azt javasoljuk, hogy az [Azure AD-ban](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)a jelszóalapú egyszeri bejelentkezés hibaelhárítása témakörben keresse meg a valószínűleg felmerülő problémák megoldását.
6. A VPN használata közbeni kapcsolódási problémákról az Egyszeri bejelentkezés használata VPN-en és Wi-Fi [keresztül.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
