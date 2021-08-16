---
title: Problémák a közvetlen egyszeri bejelentkezés és a helyszíni appokkal való integrálása során
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028294"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problémák a közvetlen egyszeri bejelentkezés és a helyszíni appokkal való integrálása során

A helyszíni alkalmazásokkal való zökkenőmentes egyszeri bejelentkezéssel kapcsolatos hibák elhárításához tegye a következőket:

**Ajánlott lépések**

1. Ha egy helyszíni alkalmazást **konfigurálni** az alkalmazásproxyn keresztüli egyszeri **bejelentkezéshez,** tekintse meg az Alkalmazásproxyval történő egyszeri bejelentkezés jelszótárba való [beállítását.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Alkalmazásproxyval** kapcsolatos hibák elhárítása: Azt javasoljuk, hogy először tekintse át a hibakeresési folyamatot, az [Alkalmazásproxy-összekötő](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)hibáit , és állapítsa meg, hogy megfelelően vannak-e konfigurálva az alkalmazásproxy-összekötők. Ha továbbra is problémákat okoz az alkalmazáshoz való kapcsolódás, kövesse az Alkalmazásproxyval kapcsolatos problémák hibaelhárítási [lépéseit.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) A [CORS-problémákat az](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) alábbi böngésző hibakeresési eszközökkel azonosíthatja:
    1. Indítsa el a böngészőt, és keresse meg a webalkalmazást.
    1. Nyomja le **az F12 billentyűt** a hibakeresési konzolhoz való bekapcsoláshoz.
    1. Próbálja meg reprodukálni a tranzakciót, és tekintse át a konzol üzenetét. A CORS-t megsértve konzolhiba történik a forrással kapcsolatban.
    1. Néhány CORS-probléma nem oldható meg, például amikor az alkalmazás átirányítja az login.microsoftonline.com hitelesítéshez, és a hozzáférési jogkivonat lejár. A CORS-hívás ekkor meghiúsul. Kerülő megoldásként meghosszabbíthatja a hozzáférési jogkivonat teljes élettartamát, hogy megakadályozza a lejáratát a felhasználó munkamenete során. Ennek mikéntje a Konfigurálható jogkivonat-élettartamok a [Microsoft Identitásplatform.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Ajánlott dokumentumok**

- [Egyszeri bejelentkezés beállítása alkalmazásproxy-alkalmazáshoz](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML egyszeri bejelentkezés helyszíni alkalmazásokhoz alkalmazásproxyval](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Az alkalmazásproxy CORS Azure Active Directory és megoldása](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [A Kerberos kényszeres delegálással kapcsolatos konfigurációinak elhárítása alkalmazásproxy esetén](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)