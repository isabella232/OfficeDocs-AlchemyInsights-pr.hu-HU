---
title: A csalás észlelésével kapcsolatos biztonsági tipp hibaelhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834733"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="f28d1-102">A csalás észlelésével kapcsolatos biztonsági tipp hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="f28d1-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="f28d1-103">Ha egy biztonsági tipp jelenik meg arról, hogy "A feladó nem sikerült a csalás észlelésére vonatkozó ellenőrzéseket végezni, és előfordulhat, hogy nem az, akinek kikiált", akkor a feladó nem tudta átadni a DKIM vagy az SPF hitelesítési ellenőrzéseket.</span><span class="sxs-lookup"><span data-stu-id="f28d1-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="f28d1-104">A probléma megoldásának legjobb módja, ha a feladónak engedélyeznie kell magát.</span><span class="sxs-lookup"><span data-stu-id="f28d1-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="f28d1-105">Ha a feladó az Ön nevében küld üzenetet, engedélyeznie kell azt úgy, hogy hozzáadja a feladó IP-címét az SPF rekordhoz.</span><span class="sxs-lookup"><span data-stu-id="f28d1-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="f28d1-106">További [információt A vörös (gyanús) biztonsági](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) tipp hibaelhárítása csalás észleléséhez témakörben kaphat.</span><span class="sxs-lookup"><span data-stu-id="f28d1-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="f28d1-107">Íme néhány további hivatkozás, amely segíthet:</span><span class="sxs-lookup"><span data-stu-id="f28d1-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="f28d1-108">Hogyan használja a Microsoft a feladói házirend keretrendszerét (SPF) a hamisítás megelőzéséhez?</span><span class="sxs-lookup"><span data-stu-id="f28d1-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="f28d1-109">SPF beállítása a hamisítás megelőzéséhez</span><span class="sxs-lookup"><span data-stu-id="f28d1-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
