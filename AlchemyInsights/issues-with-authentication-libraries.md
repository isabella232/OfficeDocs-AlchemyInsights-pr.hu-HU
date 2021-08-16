---
title: A hitelesítési tárakkal kapcsolatos problémák
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028006"
---
# <a name="issues-with-authentication-libraries"></a>A hitelesítési tárakkal kapcsolatos problémák

1. Microsoft Identitásplatform a hitelesítő [tárak](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) a Microsoft által támogatott és kompatibilis ügyfél- és középsőprogramtárakat sorolják fel.
2. A Microsoft Authentication Library (MSAL) számos hitelesítési folyamat használatát támogatja különböző alkalmazások esetén. [](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows)
3. A tokenek hitelesítéséhez és megszerzéséhez inicializál egy új nyilvános vagy bizalmas ügyfélalkalmazást a kódban. Az ügyfélalkalmazás Microsoft Authentication Library (MSAL) alkalmazásban való inicializálásakor számos konfigurációs beállítás meg van állítva. További információ: [Alkalmazáskonfigurációs beállítások](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Az Azure Active Directory Authentication Library (ADAL) és az Azure AD Graph API (AAD-hitelesítés) támogatása Graph)**

**2020. június 30-án** kezdődően nem adjuk hozzá az új funkciókat az ADAL-hoz és az Azure AD-Graph. A jövőben is biztosítani fogunk technikai támogatási és biztonsági frissítéseket, funkciófrissítéseket azonban nem.

**2022.** június 30-ával kezdődően véget ér az ADAL és az Azure AD Graph támogatása, és a továbbiakban nem nyújtunk technikai támogatást és biztonsági frissítéseket.

Az ADAL-t használó appok a meglévő operációs rendszerverziókban továbbra is működnek, de semmilyen technikai támogatást vagy biztonsági frissítést nem *fognak kapni.*

Az Azure AD-t használó Graph ezt követően előfordulhat, hogy a továbbiakban nem kap válaszokat az Azure AD Graph végponttól.

**ADAL-áttelepítés**

Javasoljuk, hogy frissítsen a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) szolgáltatásra, amely a legújabb funkciókat és biztonsági frissítéseket használja.

Ha Microsoft-appokat használ, tudja, hogy a Microsoft a támogatási határidő lejárta előtt át fogja átemelni az alkalmazásait az MSAL-be, hogy kihasználják a MSAL folyamatos biztonsági és funkciófejlesztésekkel kapcsolatos előnyét.

További információ:

1. [Az ADAL GYIK elolvasása](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [További információ az appok áttelepítéséről platformonként](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ha segítségre van szüksége annak megértéséhez, hogy melyik appja használja az ADAL-t, javasoljuk, hogy tekintse át az összes app forráskódját, és ha lehetséges, bármilyen internetszolgáltatóhoz vagy alkalmazásszolgáltatóhoz is érdemes segítséget kérnie. A Microsoft terméktámogatási szolgálata a bérlői fiókban a nem Microsoft rendszerű ADAL-appok listáját is biztosítja.

**AAD Graph-áttelepítés**

Az Azure AD Graph-t használó alkalmazások esetén kövesse az Azure AD Graph-appok microsoftos [Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Az áttelepítés ellenőrzőlistája segítséget nyújt az első lépésekhez.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Az Azure-appok regisztrációs portálján látható, hogy mely alkalmazások használják az AAD Graphot. Javasoljuk, hogy tekintse át az összes app forráskódját, és ha lehetséges, forduljon bármely szoftverszolgáltatóhoz vagy alkalmazásszolgáltatóhoz. A Microsoft ügyfélszolgálata a bérlői fiókjában az AAD-használat Graph listáját is meg tudja Önnek adni.
3. Ahhoz, hogy az app hozzáférjen az adatokhoz a Microsoft Graph-ban, a felhasználónak vagy a rendszergazdának egy jóváhagyási folyamaton keresztül meg kell adnia neki a megfelelő engedélyeket. A [Microsoft Graph az](https://docs.microsoft.com/graph/permissions-reference) engedélyekre vonatkozó hivatkozás felsorolja az egyes microsoftos Graph API-khoz társított engedélyeket. Útmutatást is nyújt az engedélyek használatára vonatkozóan.
