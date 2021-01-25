---
title: Alkalmazások API-okkal való fejlesztésével kapcsolatos problémák
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974620"
---
# <a name="issues-developing-applications-with-apis"></a>Alkalmazások API-okkal való fejlesztésével kapcsolatos problémák

Az Azure Active Directory Graph API használatának megkezdéséhez tekintse meg az [Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) rövid útmutatóját, vagy tekintse meg az Azure AD Graph API interaktív [referenciadokumentációját.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Az Azure Active Directory-hitelesítési könyvtár (ADAL) és az Azure AD Graph API (AAD Graph) támogatása**

**2020. június 30-án** kezdődően nem adjuk hozzá az ADAL és az Azure AD Graph új funkcióit. Továbbra is nyújtunk technikai támogatást és biztonsági frissítéseket, de a továbbiakban nem biztosítunk funkciófrissítéseket.

**2022. június 30-án** véget ér az ADAL és az Azure AD Graph támogatása, és a továbbiakban nem nyújtunk technikai támogatást vagy biztonsági frissítéseket.

Az ADAL-t a meglévő operációs rendszerverziókban használó appok ez idő után is működnek, technikai támogatást és biztonsági frissítéseket azonban nem fognak kapni.

Az Azure AD Graph-et ezt követően használó appok a továbbiakban nem kaphatnak választ az Azure AD Graph-végponttól.

**ADAL-áttelepítés**

Azt javasoljuk, hogy frissítsen a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)szolgáltatásra, amely a legújabb funkciókkal és biztonsági frissítésekkel rendelkezik.

Ha Microsoft-appokat használ, tudja, hogy a Microsoft a támogatási határidő lejárta előtt átemeli az alkalmazásait a MSAL szolgáltatásba, így biztosítva, hogy kihasználják a MSAL folyamatos biztonsági és funkciófejlesztésének hasznát.

1. [Olvassa el az ADAL gyakori kérdéseket.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Megtudhatja, hogy miként](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)lehet platformonként áttűnni az alkalmazásokat.
1. Ha segítségre van szüksége annak megértéséhez, hogy melyik appja használja az ADAL-t, javasoljuk, hogy tekintse át az appok összes forráskódját, és ha lehetséges, bármely internetszolgáltatóhoz vagy alkalmazásszolgáltatóhoz. A Microsoft ügyfélszolgálata emellett a bérlői fiókjában található nem Microsoft ADAL-appok listáját is meg tudja adni.

**AAD Graph-áttelepítés**

Az Azure AD Graph-et használó alkalmazások esetében kövesse az útmutatót az [Azure AD Graph-alkalmazások Microsoft Graphba való áttelepítéséhez.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Az áttelepítési ellenőrzőlistánk egy első lépésekre nyújt lehetőséget.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
1. Az Azure-app regisztrációs portálján látható, hogy mely alkalmazások használják az AAD Graphot. Javasoljuk, hogy tekintse át az appok összes forráskódját, és ha lehetséges, bármely internetszolgáltatóhoz vagy alkalmazásszolgáltatóhoz. A Microsoft ügyfélszolgálata az AAD Graph-használat teljes listáját is biztosítja a bérlői fiókjában.
1. Ahhoz, hogy az app hozzáférjen a Microsoft Graph adataihoz, a felhasználónak vagy a rendszergazdának a jóváhagyási folyamaton keresztül meg kell adnia neki a megfelelő engedélyeket. A [Microsoft Graph engedélyeinek hivatkozása](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) felsorolja a Microsoft Graph API-k egyes fő készletével társított engedélyeket. Útmutatást nyújt az engedélyek használatával kapcsolatban is.
