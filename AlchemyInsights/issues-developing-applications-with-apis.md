---
title: Alkalmazások api-okkal való fejlesztésével kapcsolatos problémák
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013462"
---
# <a name="issues-developing-applications-with-apis"></a>Alkalmazások api-okkal való fejlesztésével kapcsolatos problémák

Az Azure Active Directory Graph API használatának megkezdéséhez tekintse meg az [Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) rövid útmutatóját , vagy tekintse meg az Azure AD Graph API interaktív [dokumentációját.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Az Azure Active Directory Authentication Library (ADAL) és az Azure AD Graph API (AAD-hitelesítés) támogatása Graph)**

**2020. június 30-án** kezdődően nem adjuk hozzá az új funkciókat az ADAL-hoz és az Azure AD-Graph. A jövőben is biztosítani fogunk technikai támogatási és biztonsági frissítéseket, funkciófrissítéseket azonban nem.

**2022.** június 30-ával kezdődően véget ér az ADAL és az Azure AD Graph támogatása, és a továbbiakban nem nyújtunk technikai támogatást és biztonsági frissítéseket.

Az ADAL-t már meglévő operációs rendszereken használó appok ezután is működnek, de sem technikai támogatásban, sem biztonsági frissítésben nem részesülnek.

Az Azure AD-t használó Graph ezt követően előfordulhat, hogy a továbbiakban nem kap válaszokat az Azure AD Graph végponttól.

**ADAL-áttelepítés**

Javasoljuk, hogy frissítsen a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) szolgáltatásra, amely a legújabb funkciókat és biztonsági frissítéseket használja.

Ha Microsoft-appokat használ, tudja, hogy a Microsoft a támogatási határidő lejárta előtt át fogja átemelni az alkalmazásait a MSAL-be, így biztosítva, hogy kihasználják a MSAL folyamatos biztonsági és funkciófejlesztések nyújtotta előnyöket.

1. [Olvassa el az ADAL-gyakori kérdéseket.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Megtudhatja, hogy miként](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)lehet platformonként áttűnni az alkalmazásokat.
1. Ha segítségre van szüksége annak megértéséhez, hogy melyik appja használja az ADAL-t, javasoljuk, hogy tekintse át az összes app forráskódját, és ha lehetséges, bármilyen internetszolgáltatóhoz vagy alkalmazásszolgáltatóhoz is érdemes segítséget kérnie. A Microsoft terméktámogatási szolgálata a bérlői fiókban a nem Microsoft rendszerű ADAL-appok listáját is biztosítja.

**AAD Graph-áttelepítés**

Az Azure AD Graph-t használó alkalmazások esetén kövesse az Azure AD Graph-appok microsoftos [Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Az áttelepítési ellenőrzőlista segít az első lépésekben](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Az Azure-appok regisztrációs portálján látható, hogy mely alkalmazások használják az AAD Graphot. Javasoljuk, hogy tekintse át az összes app forráskódját, és ha lehetséges, forduljon bármely szoftverszolgáltatóhoz vagy alkalmazásszolgáltatóhoz. A Microsoft ügyfélszolgálata a bérlői fiókjában az AAD-használat Graph listáját is meg tudja Önnek adni.
1. Ahhoz, hogy az app hozzáférjen az adatokhoz a Microsoft Graph-ban, a felhasználónak vagy a rendszergazdának egy jóváhagyási folyamaton keresztül meg kell adnia neki a megfelelő engedélyeket. A [Microsoft Graph az](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) engedélyekre vonatkozó hivatkozás felsorolja az egyes microsoftos Graph API-khoz társított engedélyeket. Útmutatást is nyújt az engedélyek használatára vonatkozóan.
