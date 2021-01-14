---
title: Problémák a zökkenőmentes egyszeri bejelentkezés integrálásával a helyszíni appokkal
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868715"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problémák a zökkenőmentes egyszeri bejelentkezés integrálásával a helyszíni appokkal

A zökkenőmentes egyszeri bejelentkezés helyszíni alkalmazásokkal való integrálásával kapcsolatos hibák elhárításához tegye a következőket:

**Ajánlott lépések**

1. Ha egy **helyszíni alkalmazást konfigurálni** az alkalmazásproxyn keresztüli egyszeri bejelentkezéshez, tekintse meg az alkalmazásproxyval történő egyszeri bejelentkezéshez szükséges [jelszó-tárolót.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Alkalmazásproxyval** kapcsolatos hibák elhárítása: Azt javasoljuk, [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)hogy a hibakeresési folyamat, az alkalmazásproxy-összekötő hibáinak áttekintésével kezdje annak megállapítását, hogy az alkalmazásproxy-összekötők megfelelően vannak-e konfigurálva. Ha továbbra is problémákat okoz az alkalmazáshoz való kapcsolódás, kövesse a hibakeresési alkalmazásproxyval kapcsolatos problémák hibaelhárítási [lépéseit.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) A [CORS-problémákat az](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) alábbi böngésző hibakeresési eszközökkel azonosíthatja:
    1. Indítsa el a böngészőt, és keresse meg a webalkalmazást.
    1. Nyomja le **az F12 billentyűt** a hibakeresési konzolhoz való bekapcsoláshoz.
    1. Próbálja meg reprodukálni a tranzakciót, és tekintse át a konzolüzenetet. A CORS-szabálysértés konzolhiba esetén a forrással kapcsolatos hibát jelez.
    1. Egyes CORS-problémákat nem lehet megoldani, például amikor az app átirányítja a login.microsoftonline.com hitelesítéshez, és a hozzáférési jogkivonat lejár. A CORS-hívás ezután meghiúsul. Kerülő megoldásként meghosszabbíthatja a hozzáférési jogkivonat teljes élettartamát, hogy megakadályozza, hogy lejár a felhasználó munkamenete során. Ennek mikéntjeről a Konfigurálható jogkivonat-élettartamok a [Microsoft identitásplatformján olvashatók.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Ajánlott dokumentumok**

- [Egyszeri bejelentkezés beállítása alkalmazásproxy-alkalmazáshoz](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML egyszeri bejelentkezés helyszíni alkalmazásokhoz alkalmazásproxyval](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Az Azure Active Directory alkalmazásproxy CORS-problémáinak megoldása és használata](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [A Kerberos kényszeres delegálás konfigurálásával kapcsolatos hibák elhárítása alkalmazásproxy esetén](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)