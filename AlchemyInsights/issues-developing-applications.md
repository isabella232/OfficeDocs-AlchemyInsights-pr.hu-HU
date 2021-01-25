---
title: Alkalmazások fejlesztésével kapcsolatos problémák
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974473"
---
# <a name="issues-developing-applications"></a>Alkalmazások fejlesztésével kapcsolatos problémák

Az Azure Active Directory (AD) alkalmazásokkal kapcsolatos leggyakoribb problémák megoldásához tekintse át az alábbi cikkeket:

- [Problémákat látok a csak Chrome böngészővel való alkalmazás(ak)ba való bejelentkezés során](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Nem tudom, hogyan változtathatom meg az alkalmazás jogkivonat-élettartamának alapértelmezett beállítását](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Nem tudom, hogyan működik az alkalmazáshoz való hozzájárulás](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Nem tudom, hogyan adhatok engedélyeket az alkalmazásomnak](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Nem tudom, mi a különbség a delegált és az alkalmazásengedélyek között](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Az Azure Active Directory-hitelesítési könyvtár (ADAL) és az Azure AD Graph API (AAD Graph) táma-**

- 2020. június 30-án kezdődően nem adjuk hozzá új funkciókat az Azure Active Directory hitelesítési tárhoz (ADAL) és az Azure AD Graph API-hoz (AAD Graph). Továbbra is nyújtunk technikai támogatást és biztonsági frissítéseket, de a továbbiakban nem biztosítunk funkciófrissítéseket.

- 2022. június 30-án véget ér az ADAL és az AAD Graph támogatása, és a továbbiakban nem nyújtunk technikai támogatást vagy biztonsági frissítéseket. A feltétel következtében a következő következményekkel jár:

    - Az ADAL-t a meglévő operációs rendszerverziókban használó appok ez idő után is működnek, technikai támogatást és biztonsági frissítéseket azonban nem fognak kapni.

    - Előfordulhat, hogy az AAD Graphot ezt követően használó appok nem kapják meg a válaszokat az AAD Graph-végponttól

_ *ADAL-áttelepítés**

Ha Microsoft-alkalmazásokat használ, javasoljuk, hogy frissítsen a Microsoft Authentication Library (MSAL) szolgáltatásra, amely a legújabb funkciókkal és biztonsági frissítésekkel rendelkezik. Ez a javaslat abban az összefüggésben van, hogy a Microsoft a támogatási határidő végéig elindítja az appok MSAL-re való áttelepítését. 

A Microsoft alkalmazásai MSAL-be való áttelepítése biztosítja, hogy az appok kihasználják az MSAL folyamatos biztonsági és funkciófejlesztésének előnyét.

1. [Olvassa el az ADAL-lal kapcsolatos gyakori kérdéseket](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Megtudhatja, hogy miként lehet platformonként áttűnni az alkalmazásokat](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Ha segítségre van szüksége annak megértéséhez, hogy mely appok használják az ADAL-t, javasoljuk, hogy tekintse át az appok összes forráskódját, és ha lehetséges, bármely független szoftverszállítóhoz (ISV- vagy alkalmazásszolgáltatóhoz) kapcsolatba. A Microsoft ügyfélszolgálata emellett a bérlői fiókjában található nem Microsoft ADAL-appok listáját is meg tudja adni.

**AAD Graph-áttelepítés**

Az AAD Graphot használó alkalmazások esetében kövesse az AAD Graph-appok Microsoft Graphba való áttelepítéséhez szükséges útmutatást:

1. [Az áttelepítési ellenőrzőlistánk egy első lépésekre nyújt lehetőséget.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
2. Az Azure-app regisztrációs portálján látható, hogy mely alkalmazások használják az AAD Graphot. Azt javasoljuk, hogy tekintse át az appok összes forráskódját, és ha lehetséges, bármely független szoftverszállítóhoz vagy alkalmazásszolgáltatóhoz kapcsolatba. A Microsoft ügyfélszolgálata a bérlői fiók AAD Graph-használatáról is tájékoztatást tud nyújtani.







