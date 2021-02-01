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
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="2ffae-102">A hitelesítési tárakkal kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="2ffae-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="2ffae-103">[A Microsoft identitásplatform-hitelesítési tárai](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) a Microsoft által támogatott és kompatibilis ügyfél- és middleware-tárak listáját sorolják fel.</span><span class="sxs-lookup"><span data-stu-id="2ffae-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="2ffae-104">A Microsoft Authentication Library (MSAL) számos hitelesítési folyamat használatát támogatja [különböző](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) alkalmazások esetén.</span><span class="sxs-lookup"><span data-stu-id="2ffae-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="2ffae-105">A tokenek hitelesítéséhez és megszerzéséhez inicializálni kell egy új nyilvános vagy bizalmas ügyfélalkalmazást a kódban.</span><span class="sxs-lookup"><span data-stu-id="2ffae-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="2ffae-106">Ha inicializálja az ügyfélalkalmazást a Microsoft Authentication Library (MSAL) alkalmazásban, több konfigurációs beállítást is meg lehet állítani.</span><span class="sxs-lookup"><span data-stu-id="2ffae-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="2ffae-107">További információt az [Alkalmazáskonfigurációs beállításokban olvashat.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)</span><span class="sxs-lookup"><span data-stu-id="2ffae-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="2ffae-108">**Az Azure Active Directory-hitelesítési könyvtár (ADAL) és az Azure AD Graph API (AAD Graph) támogatása**</span><span class="sxs-lookup"><span data-stu-id="2ffae-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="2ffae-109">**2020. június 30-án** kezdődően nem adjuk hozzá az ADAL és az Azure AD Graph új funkcióit.</span><span class="sxs-lookup"><span data-stu-id="2ffae-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="2ffae-110">A jövőben is biztosítani fogunk technikai támogatási és biztonsági frissítéseket, funkciófrissítéseket azonban nem.</span><span class="sxs-lookup"><span data-stu-id="2ffae-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="2ffae-111">**2022. június 30-án** véget ér az ADAL és az Azure AD Graph támogatása, és a továbbiakban nem nyújtunk technikai támogatást vagy biztonsági frissítéseket.</span><span class="sxs-lookup"><span data-stu-id="2ffae-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="2ffae-112">Az ADAL-t a meglévő operációs rendszerverziókban használó appok ez idő után is működnek, technikai támogatást és biztonsági frissítéseket azonban nem *fognak kapni.*</span><span class="sxs-lookup"><span data-stu-id="2ffae-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="2ffae-113">Az Azure AD Graph-et ezt követően használó appok a továbbiakban nem kaphatnak választ az Azure AD Graph-végponttól.</span><span class="sxs-lookup"><span data-stu-id="2ffae-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="2ffae-114">**ADAL-áttelepítés**</span><span class="sxs-lookup"><span data-stu-id="2ffae-114">**ADAL Migration**</span></span>

<span data-ttu-id="2ffae-115">Javasoljuk, hogy frissítsen a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) szolgáltatásra, amely a legújabb funkciókat és biztonsági frissítéseket használja.</span><span class="sxs-lookup"><span data-stu-id="2ffae-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="2ffae-116">Ha Microsoft-appokat használ, tudja, hogy a Microsoft a támogatási határidő lejárta előtt átemeli az alkalmazásait a MSAL szolgáltatásba, és gondoskodik arról, hogy kihasználják a MSAL folyamatos biztonsági és funkciófejlesztésének előnyét.</span><span class="sxs-lookup"><span data-stu-id="2ffae-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="2ffae-117">További információ:</span><span class="sxs-lookup"><span data-stu-id="2ffae-117">For more information, see:</span></span>

1. [<span data-ttu-id="2ffae-118">Az ADAL GYIK elolvasása</span><span class="sxs-lookup"><span data-stu-id="2ffae-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="2ffae-119">További információ az appok áttelepítéséről platformonként</span><span class="sxs-lookup"><span data-stu-id="2ffae-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="2ffae-120">Ha segítségre van szüksége annak megértéséhez, hogy melyik appja használja az ADAL-t, javasoljuk, hogy tekintse át az appok összes forráskódját, és ha lehetséges, bármely internetszolgáltatóhoz vagy alkalmazásszolgáltatóhoz.</span><span class="sxs-lookup"><span data-stu-id="2ffae-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="2ffae-121">A Microsoft terméktámogatási szolgálata a bérlői fiókban a nem Microsoft rendszerű ADAL-appok listáját is biztosítja.</span><span class="sxs-lookup"><span data-stu-id="2ffae-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="2ffae-122">**AAD Graph-áttelepítés**</span><span class="sxs-lookup"><span data-stu-id="2ffae-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="2ffae-123">Az Azure AD Graph-et használó alkalmazások esetében kövesse az útmutatót az [Azure AD Graph-alkalmazások Microsoft Graphba való áttelepítéséhez.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="2ffae-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="2ffae-124">Az áttelepítés ellenőrzőlistája egy első lépés.</span><span class="sxs-lookup"><span data-stu-id="2ffae-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="2ffae-125">Az Azure-appok regisztrációs portálján látható, hogy mely alkalmazások használják az AAD Graphot.</span><span class="sxs-lookup"><span data-stu-id="2ffae-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="2ffae-126">Javasoljuk, hogy tekintse át az összes app forráskódját, és ha lehetséges, forduljon bármely szoftverszolgáltatóhoz vagy alkalmazásszolgáltatóhoz.</span><span class="sxs-lookup"><span data-stu-id="2ffae-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="2ffae-127">A Microsoft ügyfélszolgálata az AAD Graph-használat teljes listáját is biztosítja a bérlői fiókjában.</span><span class="sxs-lookup"><span data-stu-id="2ffae-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="2ffae-128">Ahhoz, hogy az app hozzáférjen a Microsoft Graph adataihoz, a felhasználónak vagy a rendszergazdának a jóváhagyási folyamaton keresztül meg kell adnia neki a megfelelő engedélyeket.</span><span class="sxs-lookup"><span data-stu-id="2ffae-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="2ffae-129">A [Microsoft Graph engedélyeinek hivatkozása](https://docs.microsoft.com/graph/permissions-reference) felsorolja a Microsoft Graph API-k egyes fő készletével társított engedélyeket.</span><span class="sxs-lookup"><span data-stu-id="2ffae-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="2ffae-130">Útmutatást nyújt az engedélyek használatával kapcsolatban is.</span><span class="sxs-lookup"><span data-stu-id="2ffae-130">It also provides guidance about how to use the permissions.</span></span>
