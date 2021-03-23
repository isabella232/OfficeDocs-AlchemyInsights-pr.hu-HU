---
title: Hitelesítési tárak használata
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035830"
---
# <a name="working-with-authentication-libraries"></a>Hitelesítési tárak használata

A Microsoft Authentication Library (MSAL) hiba elhárításához végezze el az alábbi ajánlott lépéseket:

1. **MSAL használata:** [Microsoft identitásplatform-hitelesítési](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) tárak – Ez a cikk a Microsoft hitelesítési könyvtár támogatását mutatja be több alkalmazástípus esetén. A tár forráskódját mutató hivatkozásokat tartalmaz; hol szerezd be az app projektjéhez a csomagot; és hogy a tár támogatja-e a felhasználói bejelentkezést (hitelesítést), a védett webes API-khoz való hozzáférést (hitelesítést) vagy mindkettőt.

2. **Hitelesítéssel** kapcsolatos hibák elhárítása: Az MSAL számos hitelesítési folyamat használatát támogatja különböző alkalmazások esetén. Attól függően, hogy az ügyfélalkalmazás hogyan épül fel, az MSAL a Microsoft identitásplatformja által támogatott hitelesítési folyamatokat használhatja. Ezek a folyamatok többféle típusú jogkivonatot és engedélyezési kódot is tudnak készíteni, és a munkához különböző tokenek szükségesek.

3. **Hozzáférési jogkivonatok:** [Microsoft-identitásplatform-hozzáférési jogkivonatok](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Ismerje meg, hogy az API hogyan érvényesítheti és használhatja a hozzáférési jogkivonaton belül a jogcímeket. A cikkben található összes dokumentáció(a feljegyzett kivételével) csak a regisztrált API-khoz kibocsátott jogkivonatokra vonatkozik. Nem vonatkozik a Microsoft tulajdonában lévő API-khoz kibocsátott jogkivonatokra, és nem is használhatók ezek a tokenek annak érvényesítésére, hogy a Microsoft identitásplatform hogyan fog jogkivonatokat kiállítani egy Ön által létrehozott API-hoz.

**Az Azure Active Directory Authentication Library (ADAL) támogatása**

- **2020. június 30-án** kezdődően nem adjuk hozzá az új funkciókat az ADAL-hoz és az Azure AD Graphhoz. A jövőben is biztosítani fogunk technikai támogatási és biztonsági frissítéseket, funkciófrissítéseket azonban nem.
- **2022. június 30-án** véget ér az ADAL és az Azure AD Graph támogatása, és a továbbiakban nem nyújtunk technikai támogatást és biztonsági frissítéseket.
- Az ADAL-t használó appok a meglévő operációs rendszerverziókban továbbra is működnek, de semmilyen technikai támogatást vagy biztonsági frissítést nem *fognak kapni.*
- Előfordulhat, hogy ezen idő után az Azure AD Graph-et használó alkalmazások nem kapják meg a válaszokat az Azure AD Graph végponttól.

**ADAL-áttelepítés**

- Javasoljuk, hogy frissítsen az MSAL-verzióra, amely a legújabb funkciókat és biztonsági frissítéseket tartalmaz.
- Ha Microsoft-appokat használ, tudja, hogy a Microsoft a támogatási határidő lejárta előtt át fogja átemelni az appokat az MSAL-be, így biztosítva, hogy kihasználják a MSAL folyamatos biztonsági és funkciófejlesztésének előnyét.

1. [Olvassa el az ADAL-gyakori kérdéseket.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Megtudhatja, hogy miként](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)lehet platformonként áttűnni az alkalmazásokat.
3. Ha az app platformján található útmutató elolvasása után további kérdései vannak, közzéteheti a [Microsoft Q&A-on](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) [azure-ad-adal-deprecation] címkével, vagy megnyithat egy problémát a tár GitHub tárházában. Az egyes [tárak](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) reposzira mutató hivatkozásokat az **MSAL** áttekintése című cikk Nyelvek és keretrendszerek című szakaszában talál.
4. Ha segítségre van szüksége annak megértéséhez, hogy melyik appja használja az **ADAL-t,** javasoljuk, hogy tekintse át az összes appja forráskódját. Ha van ilyen, akkor a Független szoftvergyártókhoz vagy alkalmazásszolgáltatókhoz kell kapcsolatba k érnie. A Microsoft terméktámogatási szolgálata a bérlői fiókban a nem Microsoft rendszerű ADAL-appok listáját is biztosítja.







