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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084348"
---
# <a name="sso-connection-issues"></a>SSO-kapcsolati problémák

1. Az alkalmazás konfigurálához kövesse a [Rövid útmutató: Tulajdonságok](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) konfigurálása alkalmazás-útmutatóhoz útmutatót.
2. A választott alkalmazástól és az Egyszeri bejelentkezés [lehetőségtől](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) függően kövesse az alábbi útmutatást:
    - Ha egy helyszíni alkalmazást **SAML-alapú** egyszeri bejelentkezéshez konfigurálni, tekintse meg az **SAML** egyszeri bejelentkezést az alkalmazásproxyval telepített helyszíni [alkalmazásokhoz.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Ha felhőalapú **alkalmazást konfigurálni** a **jelszóalapú egyszeri bejelentkezéshez,** tekintse meg a Jelszó egyszeri bejelentkezésének [konfigurálása 2010-et.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Ha egy helyszíni alkalmazást **konfigurálni** az alkalmazásproxyn keresztüli egyszeri **bejelentkezéshez,** tekintse meg az Alkalmazásproxyval történő egyszeri bejelentkezés jelszótárba való [beállítását.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Alkalmazásproxyval** kapcsolatos hibák elhárítása : Azt javasoljuk, hogy először tekintse át a hibaelhárítási folyamatot, az [Alkalmazásproxy-összekötő](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)hibáinak hibakeresését, és állapítsa meg, hogy megfelelően vannak-e konfigurálva az alkalmazásproxy-összekötők. Ha továbbra is problémákat okoz az alkalmazáshoz való kapcsolódás, kövesse az Alkalmazásproxy hibakeresési alkalmazás problémáinak hibaelhárítási [folyamatát.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) A [CORS-problémákat a](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) böngésző hibakeresési eszközeivel azonosíthatja:
    - Indítsa el a böngészőt, és keresse meg a webalkalmazást.
    - Nyomja le **az F12 billentyűt** a hibakeresési konzolhoz való bekapcsoláshoz.
    - Próbálja meg reprodukálni a tranzakciót, és tekintse át a konzol üzenetét. A CORS-t megsértve konzolhiba történik a forrással kapcsolatban.
    - Néhány CORS-probléma nem oldható meg, például amikor az alkalmazás átirányítja login.microsoft.com hitelesítéshez, és a hozzáférési jogkivonat lejár. A CORS-hívás ekkor meghiúsul. Kerülő megoldásként meghosszabbíthatja a hozzáférési jogkivonat teljes élettartamát, hogy megakadályozza a lejáratát a felhasználó munkamenete során. Ennek mikéntje a Konfigurálható jogkivonat-élettartamok a [Microsoft Identitásplatform.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. **SAML-alapú** egyszeri bejelentkezés hibaelhárítása: Azt javasoljuk, hogy ellenőrizze a Problémák az [SAML-alapú](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)egyszeri bejelentkezéssel konfigurált alkalmazásokba való bejelentkezéssel kapcsolatban, hogy megtalálja a leggyakoribb problémák megoldását.
5. **A jelszóalapú** egyszeri bejelentkezés hibaelhárítása: Azt javasoljuk, hogy az [Azure AD-ban](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)a Jelszóalapú egyszeri bejelentkezés hibaelhárítása témakörben keresse meg a leggyakoribb problémák megoldását.
6. A VPN használata közbeni kapcsolódási problémákról az Egyszeri bejelentkezés használata VPN-en és kapcsolaton keresztül [Wi-Fi.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
