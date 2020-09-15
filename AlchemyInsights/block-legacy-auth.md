---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685600"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="c78d4-102">Korábbi hitelesítés letiltása</span><span class="sxs-lookup"><span data-stu-id="c78d4-102">Blocking legacy authentication</span></span>

<span data-ttu-id="c78d4-103">A örökölt hitelesítés olyan kifejezés, amely az alábbiak által végzett hitelesítési kérésre hivatkozik:</span><span class="sxs-lookup"><span data-stu-id="c78d4-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="c78d4-104">Azok a régebbi Office-ügyfélprogramok, amelyek nem használják a modern hitelesítést (például az Office 2010 ügyfélprogramot).</span><span class="sxs-lookup"><span data-stu-id="c78d4-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="c78d4-105">Bármely olyan ügyfél, amely régebbi levelezési protokollt (például IMAP/SMTP/POP3) használ.</span><span class="sxs-lookup"><span data-stu-id="c78d4-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="c78d4-106">A régi hitelesítés és a modern hitelesítés engedélyezéséről a [régi hitelesítés letiltása](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)című témakörben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="c78d4-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="c78d4-107">Az Azure Active Directory biztonsági alapbeállításai (Azure AD) megkönnyítik a biztonság megőrzését, és segítséget nyújtanak a szervezet védelmében.</span><span class="sxs-lookup"><span data-stu-id="c78d4-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="c78d4-108">A biztonsági alapértékek előre beállított biztonsági beállításokat tartalmaznak a gyakori támadások számára.</span><span class="sxs-lookup"><span data-stu-id="c78d4-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="c78d4-109">Az alapértelmezett biztonsági beállításokról további információt a [biztonsági alapértékek?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="c78d4-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="c78d4-110">**Megjegyzés**: Ha a bérlői naptár október 22-én, 2019-ben lett létrehozva, akkor lehetséges, hogy az új, biztonságos működést tapasztalja, és már rendelkezik a bérlőben engedélyezett biztonsági alapbeállításokkal.</span><span class="sxs-lookup"><span data-stu-id="c78d4-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="c78d4-111">Az összes felhasználó védelme érdekében a biztonsági alapértékek minden újonnan létrehozott bérlő számára elérhetők.</span><span class="sxs-lookup"><span data-stu-id="c78d4-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
