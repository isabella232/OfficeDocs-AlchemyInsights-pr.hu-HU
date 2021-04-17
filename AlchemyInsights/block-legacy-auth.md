---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820180"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="d84cf-102">A régi típusú hitelesítés letiltása</span><span class="sxs-lookup"><span data-stu-id="d84cf-102">Blocking legacy authentication</span></span>

<span data-ttu-id="d84cf-103">A régi típusú hitelesítés egy olyan kifejezés, amely a következő által kért hitelesítési kérésre hivatkozik:</span><span class="sxs-lookup"><span data-stu-id="d84cf-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="d84cf-104">Régebbi, modern hitelesítést nem felhasználó Office-ügyfelek (például Office 2010-ügyfél).</span><span class="sxs-lookup"><span data-stu-id="d84cf-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="d84cf-105">Bármely ügyfél, amely régebbi levelezési protokollokat (például IMAP/SMTP/POP3) használ.</span><span class="sxs-lookup"><span data-stu-id="d84cf-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="d84cf-106">A régi típusú hitelesítés letiltásával és a modern hitelesítés engedélyezésével kapcsolatos további információkért lásd: Régebbi hitelesítés [letiltása.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="d84cf-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="d84cf-107">Az Azure Active Directory (Azure AD) biztonsági alapértelmezései megkönnyítik a biztonság védelmét és a szervezet védelmét.</span><span class="sxs-lookup"><span data-stu-id="d84cf-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="d84cf-108">A biztonsági alapértelmezések előre konfigurált biztonsági beállításokat tartalmaznak a gyakori támadásokhoz.</span><span class="sxs-lookup"><span data-stu-id="d84cf-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="d84cf-109">A biztonsági alapértelmezésekkel kapcsolatos további információkért lásd: Mik azok a biztonsági [alapértelmezések?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="d84cf-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="d84cf-110">**Megjegyzés:** Ha a bérlői webhelyet 2019. október 22-én vagy azt követően hozták létre, lehetséges, hogy új alapértelmezett biztonsági viselkedést tapasztal, és már engedélyezve van a biztonsági alapértelmezett beállítások a bérlői webhelyen.</span><span class="sxs-lookup"><span data-stu-id="d84cf-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="d84cf-111">Az összes felhasználó védelme érdekében a biztonsági alapértelmezett beállításokat az összes újonnan létrehozott bérlői webhelyen ki lesz állítva.</span><span class="sxs-lookup"><span data-stu-id="d84cf-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
