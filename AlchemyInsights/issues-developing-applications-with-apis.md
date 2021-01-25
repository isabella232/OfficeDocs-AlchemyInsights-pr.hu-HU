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
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="383eb-102">Alkalmazások API-okkal való fejlesztésével kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="383eb-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="383eb-103">Az Azure Active Directory Graph API használatának megkezdéséhez tekintse meg az [Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) rövid útmutatóját, vagy tekintse meg az Azure AD Graph API interaktív [referenciadokumentációját.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)</span><span class="sxs-lookup"><span data-stu-id="383eb-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="383eb-104">**Az Azure Active Directory-hitelesítési könyvtár (ADAL) és az Azure AD Graph API (AAD Graph) támogatása**</span><span class="sxs-lookup"><span data-stu-id="383eb-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="383eb-105">**2020. június 30-án** kezdődően nem adjuk hozzá az ADAL és az Azure AD Graph új funkcióit.</span><span class="sxs-lookup"><span data-stu-id="383eb-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="383eb-106">Továbbra is nyújtunk technikai támogatást és biztonsági frissítéseket, de a továbbiakban nem biztosítunk funkciófrissítéseket.</span><span class="sxs-lookup"><span data-stu-id="383eb-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="383eb-107">**2022. június 30-án** véget ér az ADAL és az Azure AD Graph támogatása, és a továbbiakban nem nyújtunk technikai támogatást vagy biztonsági frissítéseket.</span><span class="sxs-lookup"><span data-stu-id="383eb-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="383eb-108">Az ADAL-t a meglévő operációs rendszerverziókban használó appok ez idő után is működnek, technikai támogatást és biztonsági frissítéseket azonban nem fognak kapni.</span><span class="sxs-lookup"><span data-stu-id="383eb-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="383eb-109">Az Azure AD Graph-et ezt követően használó appok a továbbiakban nem kaphatnak választ az Azure AD Graph-végponttól.</span><span class="sxs-lookup"><span data-stu-id="383eb-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="383eb-110">**ADAL-áttelepítés**</span><span class="sxs-lookup"><span data-stu-id="383eb-110">**ADAL Migration**</span></span>

<span data-ttu-id="383eb-111">Azt javasoljuk, hogy frissítsen a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)szolgáltatásra, amely a legújabb funkciókkal és biztonsági frissítésekkel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="383eb-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="383eb-112">Ha Microsoft-appokat használ, tudja, hogy a Microsoft a támogatási határidő lejárta előtt átemeli az alkalmazásait a MSAL szolgáltatásba, így biztosítva, hogy kihasználják a MSAL folyamatos biztonsági és funkciófejlesztésének hasznát.</span><span class="sxs-lookup"><span data-stu-id="383eb-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="383eb-113">[Olvassa el az ADAL gyakori kérdéseket.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="383eb-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="383eb-114">[Megtudhatja, hogy miként](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)lehet platformonként áttűnni az alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="383eb-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="383eb-115">Ha segítségre van szüksége annak megértéséhez, hogy melyik appja használja az ADAL-t, javasoljuk, hogy tekintse át az appok összes forráskódját, és ha lehetséges, bármely internetszolgáltatóhoz vagy alkalmazásszolgáltatóhoz.</span><span class="sxs-lookup"><span data-stu-id="383eb-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="383eb-116">A Microsoft ügyfélszolgálata emellett a bérlői fiókjában található nem Microsoft ADAL-appok listáját is meg tudja adni.</span><span class="sxs-lookup"><span data-stu-id="383eb-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="383eb-117">**AAD Graph-áttelepítés**</span><span class="sxs-lookup"><span data-stu-id="383eb-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="383eb-118">Az Azure AD Graph-et használó alkalmazások esetében kövesse az útmutatót az [Azure AD Graph-alkalmazások Microsoft Graphba való áttelepítéséhez.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="383eb-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="383eb-119">[Az áttelepítési ellenőrzőlistánk egy első lépésekre nyújt lehetőséget.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="383eb-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="383eb-120">Az Azure-app regisztrációs portálján látható, hogy mely alkalmazások használják az AAD Graphot.</span><span class="sxs-lookup"><span data-stu-id="383eb-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="383eb-121">Javasoljuk, hogy tekintse át az appok összes forráskódját, és ha lehetséges, bármely internetszolgáltatóhoz vagy alkalmazásszolgáltatóhoz.</span><span class="sxs-lookup"><span data-stu-id="383eb-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="383eb-122">A Microsoft ügyfélszolgálata az AAD Graph-használat teljes listáját is biztosítja a bérlői fiókjában.</span><span class="sxs-lookup"><span data-stu-id="383eb-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="383eb-123">Ahhoz, hogy az app hozzáférjen a Microsoft Graph adataihoz, a felhasználónak vagy a rendszergazdának a jóváhagyási folyamaton keresztül meg kell adnia neki a megfelelő engedélyeket.</span><span class="sxs-lookup"><span data-stu-id="383eb-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="383eb-124">A [Microsoft Graph engedélyeinek hivatkozása](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) felsorolja a Microsoft Graph API-k egyes fő készletével társított engedélyeket.</span><span class="sxs-lookup"><span data-stu-id="383eb-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="383eb-125">Útmutatást nyújt az engedélyek használatával kapcsolatban is.</span><span class="sxs-lookup"><span data-stu-id="383eb-125">It also provides guidance about how to use the permissions.</span></span>
