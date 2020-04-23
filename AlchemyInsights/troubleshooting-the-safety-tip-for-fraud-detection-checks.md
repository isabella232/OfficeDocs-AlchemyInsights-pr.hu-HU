---
title: Hibaelhárítás a biztonsági tipp a csalások felderítése ellenőrzések
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759514"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="c1e8a-102">Hibaelhárítás a biztonsági tipp a csalások felderítése ellenőrzések</span><span class="sxs-lookup"><span data-stu-id="c1e8a-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="c1e8a-103">Ha olyan biztonsági tippet kap, amely szerint "A feladó megbukott a csalásészlelési ellenőrzéseken, és nem lehet az, akinek látszik", akkor a feladó nem tudta átadni a DKIM vagy az SPF hitelesítési ellenőrzéseket.</span><span class="sxs-lookup"><span data-stu-id="c1e8a-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="c1e8a-104">A megoldás legjobb módja az, ha a feladó engedélyezi magát.</span><span class="sxs-lookup"><span data-stu-id="c1e8a-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="c1e8a-105">Ha a feladó az Ön nevében küld, engedélyeznie kell őket a feladó IP-címének hozzáadásával az SPF-rekordhoz.</span><span class="sxs-lookup"><span data-stu-id="c1e8a-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="c1e8a-106">További információ [a csalásészlelési ellenőrzésekért olvassa el a piros (gyanús) biztonsági tipp hibaelhárítása](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) című témakört.</span><span class="sxs-lookup"><span data-stu-id="c1e8a-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="c1e8a-107">Íme néhány további link, amely segíthet:</span><span class="sxs-lookup"><span data-stu-id="c1e8a-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="c1e8a-108">Hogyan használja a Microsoft a feladói házirend keretrendszerét (SPF) a hamisítás megakadályozására?</span><span class="sxs-lookup"><span data-stu-id="c1e8a-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="c1e8a-109">Az SPF beállítása a hamisítás megakadályozása érdekében</span><span class="sxs-lookup"><span data-stu-id="c1e8a-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
