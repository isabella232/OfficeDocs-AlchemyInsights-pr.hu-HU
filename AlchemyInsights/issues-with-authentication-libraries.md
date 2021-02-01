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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063609"
---
# <a name="issues-with-authentication-libraries"></a>A hitelesítési tárakkal kapcsolatos problémák

1. [A Microsoft identitásplatform-hitelesítési tárai](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) a Microsoft által támogatott és kompatibilis ügyfél- és middleware-tárak listáját sorolják fel.
2. A Microsoft Authentication Library (MSAL) számos hitelesítési folyamat használatát támogatja [különböző](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) alkalmazások esetén.
3. A tokenek hitelesítéséhez és megszerzéséhez inicializálni kell egy új nyilvános vagy bizalmas ügyfélalkalmazást a kódban. Ha inicializálja az ügyfélalkalmazást a Microsoft Authentication Library (MSAL) alkalmazásban, több konfigurációs beállítást is meg lehet állítani. További információt az [Alkalmazáskonfigurációs beállításokban olvashat.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Az Azure Active Directory-hitelesítési könyvtár (ADAL) és az Azure AD Graph API (AAD Graph) támogatása**

**2020. június 30-án** kezdődően nem adjuk hozzá az ADAL és az Azure AD Graph új funkcióit. A jövőben is biztosítani fogunk technikai támogatási és biztonsági frissítéseket, funkciófrissítéseket azonban nem.

**2022. június 30-án** véget ér az ADAL és az Azure AD Graph támogatása, és a továbbiakban nem nyújtunk technikai támogatást vagy biztonsági frissítéseket.

Az ADAL-t a meglévő operációs rendszerverziókban használó appok ez idő után is működnek, technikai támogatást és biztonsági frissítéseket azonban nem *fognak kapni.*

Az Azure AD Graph-et ezt követően használó appok a továbbiakban nem kaphatnak választ az Azure AD Graph-végponttól.

**ADAL-áttelepítés**

Javasoljuk, hogy frissítsen a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) szolgáltatásra, amely a legújabb funkciókat és biztonsági frissítéseket használja.

Ha Microsoft-appokat használ, tudja, hogy a Microsoft a támogatási határidő lejárta előtt átemeli az alkalmazásait a MSAL szolgáltatásba, és gondoskodik arról, hogy kihasználják a MSAL folyamatos biztonsági és funkciófejlesztésének előnyét.

További információ:

1. [Az ADAL GYIK elolvasása](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [További információ az appok áttelepítéséről platformonként](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ha segítségre van szüksége annak megértéséhez, hogy melyik appja használja az ADAL-t, javasoljuk, hogy tekintse át az appok összes forráskódját, és ha lehetséges, bármely internetszolgáltatóhoz vagy alkalmazásszolgáltatóhoz. A Microsoft terméktámogatási szolgálata a bérlői fiókban a nem Microsoft rendszerű ADAL-appok listáját is biztosítja.

**AAD Graph-áttelepítés**

Az Azure AD Graph-et használó alkalmazások esetében kövesse az útmutatót az [Azure AD Graph-alkalmazások Microsoft Graphba való áttelepítéséhez.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Az áttelepítés ellenőrzőlistája egy első lépés.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Az Azure-appok regisztrációs portálján látható, hogy mely alkalmazások használják az AAD Graphot. Javasoljuk, hogy tekintse át az összes app forráskódját, és ha lehetséges, forduljon bármely szoftverszolgáltatóhoz vagy alkalmazásszolgáltatóhoz. A Microsoft ügyfélszolgálata az AAD Graph-használat teljes listáját is biztosítja a bérlői fiókjában.
3. Ahhoz, hogy az app hozzáférjen a Microsoft Graph adataihoz, a felhasználónak vagy a rendszergazdának a jóváhagyási folyamaton keresztül meg kell adnia neki a megfelelő engedélyeket. A [Microsoft Graph engedélyeinek hivatkozása](https://docs.microsoft.com/graph/permissions-reference) felsorolja a Microsoft Graph API-k egyes fő készletével társított engedélyeket. Útmutatást nyújt az engedélyek használatával kapcsolatban is.
