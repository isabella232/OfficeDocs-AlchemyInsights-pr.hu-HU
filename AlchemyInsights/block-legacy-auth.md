---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: e7bff5f9fcf6f2f2c77e93c2f27f585f2cc18bea
ms.sourcegitcommit: 98231a228ecb2bf14ec3b96d4dd4ccf2507617a3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/01/2020
ms.locfileid: "43079262"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="cebde-102">Örökölt hitelesítés blokkolása</span><span class="sxs-lookup"><span data-stu-id="cebde-102">Blocking legacy authentication</span></span>

<span data-ttu-id="cebde-103">Az örökölt hitelesítés olyan kifejezés, amely a következő hitelesítési kérelemre hivatkozik:</span><span class="sxs-lookup"><span data-stu-id="cebde-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="cebde-104">Régebbi Office-ügyfelek, amelyek nem használnak modern hitelesítést (például Office 2010-ügyfél).</span><span class="sxs-lookup"><span data-stu-id="cebde-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="cebde-105">Minden olyan ügyfél, amely örökölt leveli protokollokat használ, például IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="cebde-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="cebde-106">Az örökölt hitelesítés blokkolásával és a modern hitelesítés engedélyezésével kapcsolatos további információkért olvassa el [az örökölt hitelesítés blokkolása](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)című.</span><span class="sxs-lookup"><span data-stu-id="cebde-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="cebde-107">Az Azure Active Directory (Azure AD) biztonsági beállításai megkönnyítik a biztonságot és a szervezet védelmét.</span><span class="sxs-lookup"><span data-stu-id="cebde-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="cebde-108">A biztonsági alapértelmezések előre konfigurált biztonsági beállításokat tartalmaznak a gyakori támadásokhoz.</span><span class="sxs-lookup"><span data-stu-id="cebde-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="cebde-109">A biztonsági alapértékekről a [Mik a biztonsági alapértelmezések?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="cebde-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="cebde-110">**Megjegyzés:** Ha a bérlő2019. október 22-én vagy azt követően jött létre, lehetséges, hogy az új biztonságos alapértelmezett viselkedést tapasztalja, és már engedélyezve van a bérlőben a biztonsági alapértelmezések.</span><span class="sxs-lookup"><span data-stu-id="cebde-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="cebde-111">Annak érdekében, hogy megvédje az összes felhasználó, biztonsági alapértelmezett a rendszer gördült ki az összes új bérlő létrehozott.</span><span class="sxs-lookup"><span data-stu-id="cebde-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
