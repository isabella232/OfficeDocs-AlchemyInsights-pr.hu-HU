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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013426"
---
# <a name="issues-developing-applications"></a>Alkalmazások fejlesztésével kapcsolatos problémák

Az alábbi cikkekből tudja elhárítani az Azure Active Directory (AD) alkalmazások kiépítésekor gyakran megjelenő hibákat:

- [Problémákat látok a csak a Chrome böngészővel való alkalmazás(ak)ba való bejelentkezés során](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Nem tudom, hogyan változtathatom meg a jogkivonat élettartamának alapértelmezett alapértelmezett beállítását az alkalmazásomhoz](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Nem tudom, hogyan működik az alkalmazás-hozzájárulás](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Nem tudom, hogyan adhatok engedélyeket az alkalmazásomnak](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Nem tudom mi a különbség a delegált és az alkalmazásengedélyek között](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Az Azure Active Directory Authentication Library (ADAL) és az Azure AD Graph API (AAD-hitelesítés) támogatása Graph)***

- 2020. június 30-tól kezdődően nem adunk hozzá új funkciókat az Azure Active Directory-hitelesítési tár (ADAL) és az Azure AD Graph API (AAD Graph) szolgáltatáshoz. A jövőben is biztosítani fogunk technikai támogatási és biztonsági frissítéseket, funkciófrissítéseket azonban nem.

- 2022. június 30-tól kezdődően véget vetünk az ADAL- és az AAD Graph-támogatásnak, és a továbbiakban nem biztosítunk technikai támogatást és biztonsági frissítéseket. A feltétel eredménye a következő:

    - Az ADAL-t már meglévő operációs rendszereken használó appok ezután is működnek, de sem technikai támogatásban, sem biztonsági frissítésben nem részesülnek.

    - Előfordulhat, hogy az AAD-Graph ezt követően nem kap választ az AAD-Graph válaszaitól

**ADAL-áttelepítés**

Ha Microsoft-appokat használ, javasoljuk, hogy frissítsen a Microsoft Authentication Library (MSAL) szolgáltatásra, amely a legújabb funkciókat és biztonsági frissítéseket tartalmaz. Ez a javaslat olyan helyzetben van, amikor a Microsoft a támogatási határidő végéig elindítja az appok MSAL-re való áttelepítését. 

A Microsoft alkalmazásai MSAL-be való áttelepítése gondoskodik arról, hogy az appok kihasználják az MSAL folyamatos biztonsági és funkciófejlesztésének előnyét.

1. [Az ADAL GYIK elolvasása](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [További információ az appok áttelepítéséről platformonként](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Ha segítségre van szüksége annak megértéséhez, hogy az appok melyik használják az ADAL-t, javasoljuk, hogy tekintse át az összes app forráskódját, és ha lehetséges, bármilyen független szoftverszállítóhoz vagy alkalmazásszolgáltatóhoz. A Microsoft terméktámogatási szolgálata a bérlői fiókban a nem Microsoft rendszerű ADAL-appok listáját is biztosítja.

**AAD Graph-áttelepítés**

Az AAD-t használó alkalmazások Graph az AAD-alkalmazások microsoftos Graph microsoftos Graph:

1. [Az áttelepítési ellenőrzőlista segít az első lépésekben](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Az Azure-appok regisztrációs portálján látható, hogy mely alkalmazások használják az AAD Graphot. Javasoljuk, hogy tekintse át az összes app forráskódját, és ha lehetséges, kapcsolatba kell vele érnie bármely független szoftverszállítóval vagy alkalmazásszolgáltatóval. A Microsoft ügyfélszolgálata az AAD-nek a bérlői fiókban Graph használatáról is tud információkat nyújtani.







