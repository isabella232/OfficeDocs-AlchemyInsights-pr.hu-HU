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
# <a name="issues-developing-applications"></a><span data-ttu-id="3c6a8-102">Alkalmazások fejlesztésével kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="3c6a8-102">Issues developing applications</span></span>

<span data-ttu-id="3c6a8-103">Az Azure Active Directory (AD) alkalmazásokkal kapcsolatos leggyakoribb problémák megoldásához tekintse át az alábbi cikkeket:</span><span class="sxs-lookup"><span data-stu-id="3c6a8-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="3c6a8-104">Problémákat látok a csak Chrome böngészővel való alkalmazás(ak)ba való bejelentkezés során</span><span class="sxs-lookup"><span data-stu-id="3c6a8-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="3c6a8-105">Nem tudom, hogyan változtathatom meg az alkalmazás jogkivonat-élettartamának alapértelmezett beállítását</span><span class="sxs-lookup"><span data-stu-id="3c6a8-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="3c6a8-106">Nem tudom, hogyan működik az alkalmazáshoz való hozzájárulás</span><span class="sxs-lookup"><span data-stu-id="3c6a8-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="3c6a8-107">Nem tudom, hogyan adhatok engedélyeket az alkalmazásomnak</span><span class="sxs-lookup"><span data-stu-id="3c6a8-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="3c6a8-108">Nem tudom, mi a különbség a delegált és az alkalmazásengedélyek között</span><span class="sxs-lookup"><span data-stu-id="3c6a8-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="3c6a8-109">\***Az Azure Active Directory-hitelesítési könyvtár (ADAL) és az Azure AD Graph API (AAD Graph) táma-**</span><span class="sxs-lookup"><span data-stu-id="3c6a8-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="3c6a8-110">2020. június 30-án kezdődően nem adjuk hozzá új funkciókat az Azure Active Directory hitelesítési tárhoz (ADAL) és az Azure AD Graph API-hoz (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="3c6a8-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="3c6a8-111">Továbbra is nyújtunk technikai támogatást és biztonsági frissítéseket, de a továbbiakban nem biztosítunk funkciófrissítéseket.</span><span class="sxs-lookup"><span data-stu-id="3c6a8-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="3c6a8-112">2022. június 30-án véget ér az ADAL és az AAD Graph támogatása, és a továbbiakban nem nyújtunk technikai támogatást vagy biztonsági frissítéseket.</span><span class="sxs-lookup"><span data-stu-id="3c6a8-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="3c6a8-113">A feltétel következtében a következő következményekkel jár:</span><span class="sxs-lookup"><span data-stu-id="3c6a8-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="3c6a8-114">Az ADAL-t a meglévő operációs rendszerverziókban használó appok ez idő után is működnek, technikai támogatást és biztonsági frissítéseket azonban nem fognak kapni.</span><span class="sxs-lookup"><span data-stu-id="3c6a8-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="3c6a8-115">Előfordulhat, hogy az AAD Graphot ezt követően használó appok nem kapják meg a válaszokat az AAD Graph-végponttól</span><span class="sxs-lookup"><span data-stu-id="3c6a8-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="3c6a8-116">_ *ADAL-áttelepítés*\*</span><span class="sxs-lookup"><span data-stu-id="3c6a8-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="3c6a8-117">Ha Microsoft-alkalmazásokat használ, javasoljuk, hogy frissítsen a Microsoft Authentication Library (MSAL) szolgáltatásra, amely a legújabb funkciókkal és biztonsági frissítésekkel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="3c6a8-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="3c6a8-118">Ez a javaslat abban az összefüggésben van, hogy a Microsoft a támogatási határidő végéig elindítja az appok MSAL-re való áttelepítését.</span><span class="sxs-lookup"><span data-stu-id="3c6a8-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="3c6a8-119">A Microsoft alkalmazásai MSAL-be való áttelepítése biztosítja, hogy az appok kihasználják az MSAL folyamatos biztonsági és funkciófejlesztésének előnyét.</span><span class="sxs-lookup"><span data-stu-id="3c6a8-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="3c6a8-120">Olvassa el az ADAL-lal kapcsolatos gyakori kérdéseket</span><span class="sxs-lookup"><span data-stu-id="3c6a8-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="3c6a8-121">Megtudhatja, hogy miként lehet platformonként áttűnni az alkalmazásokat</span><span class="sxs-lookup"><span data-stu-id="3c6a8-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="3c6a8-122">Ha segítségre van szüksége annak megértéséhez, hogy mely appok használják az ADAL-t, javasoljuk, hogy tekintse át az appok összes forráskódját, és ha lehetséges, bármely független szoftverszállítóhoz (ISV- vagy alkalmazásszolgáltatóhoz) kapcsolatba.</span><span class="sxs-lookup"><span data-stu-id="3c6a8-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="3c6a8-123">A Microsoft ügyfélszolgálata emellett a bérlői fiókjában található nem Microsoft ADAL-appok listáját is meg tudja adni.</span><span class="sxs-lookup"><span data-stu-id="3c6a8-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="3c6a8-124">**AAD Graph-áttelepítés**</span><span class="sxs-lookup"><span data-stu-id="3c6a8-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="3c6a8-125">Az AAD Graphot használó alkalmazások esetében kövesse az AAD Graph-appok Microsoft Graphba való áttelepítéséhez szükséges útmutatást:</span><span class="sxs-lookup"><span data-stu-id="3c6a8-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="3c6a8-126">[Az áttelepítési ellenőrzőlistánk egy első lépésekre nyújt lehetőséget.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="3c6a8-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="3c6a8-127">Az Azure-app regisztrációs portálján látható, hogy mely alkalmazások használják az AAD Graphot.</span><span class="sxs-lookup"><span data-stu-id="3c6a8-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="3c6a8-128">Azt javasoljuk, hogy tekintse át az appok összes forráskódját, és ha lehetséges, bármely független szoftverszállítóhoz vagy alkalmazásszolgáltatóhoz kapcsolatba.</span><span class="sxs-lookup"><span data-stu-id="3c6a8-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="3c6a8-129">A Microsoft ügyfélszolgálata a bérlői fiók AAD Graph-használatáról is tájékoztatást tud nyújtani.</span><span class="sxs-lookup"><span data-stu-id="3c6a8-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







