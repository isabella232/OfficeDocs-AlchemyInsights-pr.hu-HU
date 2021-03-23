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
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="41274-102">Hitelesítési tárak használata</span><span class="sxs-lookup"><span data-stu-id="41274-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="41274-103">A Microsoft Authentication Library (MSAL) hiba elhárításához végezze el az alábbi ajánlott lépéseket:</span><span class="sxs-lookup"><span data-stu-id="41274-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="41274-104">**MSAL használata:** [Microsoft identitásplatform-hitelesítési](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) tárak – Ez a cikk a Microsoft hitelesítési könyvtár támogatását mutatja be több alkalmazástípus esetén.</span><span class="sxs-lookup"><span data-stu-id="41274-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="41274-105">A tár forráskódját mutató hivatkozásokat tartalmaz; hol szerezd be az app projektjéhez a csomagot; és hogy a tár támogatja-e a felhasználói bejelentkezést (hitelesítést), a védett webes API-khoz való hozzáférést (hitelesítést) vagy mindkettőt.</span><span class="sxs-lookup"><span data-stu-id="41274-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="41274-106">**Hitelesítéssel** kapcsolatos hibák elhárítása: Az MSAL számos hitelesítési folyamat használatát támogatja különböző alkalmazások esetén.</span><span class="sxs-lookup"><span data-stu-id="41274-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="41274-107">Attól függően, hogy az ügyfélalkalmazás hogyan épül fel, az MSAL a Microsoft identitásplatformja által támogatott hitelesítési folyamatokat használhatja.</span><span class="sxs-lookup"><span data-stu-id="41274-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="41274-108">Ezek a folyamatok többféle típusú jogkivonatot és engedélyezési kódot is tudnak készíteni, és a munkához különböző tokenek szükségesek.</span><span class="sxs-lookup"><span data-stu-id="41274-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="41274-109">**Hozzáférési jogkivonatok:** [Microsoft-identitásplatform-hozzáférési jogkivonatok](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Ismerje meg, hogy az API hogyan érvényesítheti és használhatja a hozzáférési jogkivonaton belül a jogcímeket.</span><span class="sxs-lookup"><span data-stu-id="41274-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="41274-110">A cikkben található összes dokumentáció(a feljegyzett kivételével) csak a regisztrált API-khoz kibocsátott jogkivonatokra vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="41274-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="41274-111">Nem vonatkozik a Microsoft tulajdonában lévő API-khoz kibocsátott jogkivonatokra, és nem is használhatók ezek a tokenek annak érvényesítésére, hogy a Microsoft identitásplatform hogyan fog jogkivonatokat kiállítani egy Ön által létrehozott API-hoz.</span><span class="sxs-lookup"><span data-stu-id="41274-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="41274-112">**Az Azure Active Directory Authentication Library (ADAL) támogatása**</span><span class="sxs-lookup"><span data-stu-id="41274-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="41274-113">**2020. június 30-án** kezdődően nem adjuk hozzá az új funkciókat az ADAL-hoz és az Azure AD Graphhoz.</span><span class="sxs-lookup"><span data-stu-id="41274-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="41274-114">A jövőben is biztosítani fogunk technikai támogatási és biztonsági frissítéseket, funkciófrissítéseket azonban nem.</span><span class="sxs-lookup"><span data-stu-id="41274-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="41274-115">**2022. június 30-án** véget ér az ADAL és az Azure AD Graph támogatása, és a továbbiakban nem nyújtunk technikai támogatást és biztonsági frissítéseket.</span><span class="sxs-lookup"><span data-stu-id="41274-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="41274-116">Az ADAL-t használó appok a meglévő operációs rendszerverziókban továbbra is működnek, de semmilyen technikai támogatást vagy biztonsági frissítést nem *fognak kapni.*</span><span class="sxs-lookup"><span data-stu-id="41274-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="41274-117">Előfordulhat, hogy ezen idő után az Azure AD Graph-et használó alkalmazások nem kapják meg a válaszokat az Azure AD Graph végponttól.</span><span class="sxs-lookup"><span data-stu-id="41274-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="41274-118">**ADAL-áttelepítés**</span><span class="sxs-lookup"><span data-stu-id="41274-118">**ADAL Migration**</span></span>

- <span data-ttu-id="41274-119">Javasoljuk, hogy frissítsen az MSAL-verzióra, amely a legújabb funkciókat és biztonsági frissítéseket tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="41274-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="41274-120">Ha Microsoft-appokat használ, tudja, hogy a Microsoft a támogatási határidő lejárta előtt át fogja átemelni az appokat az MSAL-be, így biztosítva, hogy kihasználják a MSAL folyamatos biztonsági és funkciófejlesztésének előnyét.</span><span class="sxs-lookup"><span data-stu-id="41274-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="41274-121">[Olvassa el az ADAL-gyakori kérdéseket.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="41274-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="41274-122">[Megtudhatja, hogy miként](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)lehet platformonként áttűnni az alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="41274-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="41274-123">Ha az app platformján található útmutató elolvasása után további kérdései vannak, közzéteheti a [Microsoft Q&A-on](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) [azure-ad-adal-deprecation] címkével, vagy megnyithat egy problémát a tár GitHub tárházában.</span><span class="sxs-lookup"><span data-stu-id="41274-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="41274-124">Az egyes [tárak](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) reposzira mutató hivatkozásokat az **MSAL** áttekintése című cikk Nyelvek és keretrendszerek című szakaszában talál.</span><span class="sxs-lookup"><span data-stu-id="41274-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="41274-125">Ha segítségre van szüksége annak megértéséhez, hogy melyik appja használja az **ADAL-t,** javasoljuk, hogy tekintse át az összes appja forráskódját.</span><span class="sxs-lookup"><span data-stu-id="41274-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="41274-126">Ha van ilyen, akkor a Független szoftvergyártókhoz vagy alkalmazásszolgáltatókhoz kell kapcsolatba k érnie.</span><span class="sxs-lookup"><span data-stu-id="41274-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="41274-127">A Microsoft terméktámogatási szolgálata a bérlői fiókban a nem Microsoft rendszerű ADAL-appok listáját is biztosítja.</span><span class="sxs-lookup"><span data-stu-id="41274-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







