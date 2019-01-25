---
title: Ellenőrzi a biztonsági tipp csalások felderítésével kapcsolatos hibaelhárítás
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473491"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="8009c-102">Ellenőrzi a biztonsági tipp csalások felderítésével kapcsolatos hibaelhárítás</span><span class="sxs-lookup"><span data-stu-id="8009c-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="8009c-p101">Ha Ön kap egy biztonsági tipp, amely szerint "a feladó nem sikerült a csalás észlelése ellenőrzések és tűnnek, aki nem lehet", majd a feladó nem sikerült átadni a DKIM vagy SPF hitelesítési ellenőrzést. Ennek megoldására a legjobb módszer a feladót, hogy engedélyezik a maguk szolgál. A feladó küld az Ön nevében, ha azokat a feladó IP-címe az SPF-rekord hozzáadásával engedélyezni kell.</span><span class="sxs-lookup"><span data-stu-id="8009c-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="8009c-106">További információ a [ellenőrzi a piros (gyanús) biztonsági tipp csalások felderítésével kapcsolatos hibaelhárítást](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) talál.</span><span class="sxs-lookup"><span data-stu-id="8009c-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="8009c-107">Az alábbiakban néhány egyéb hivatkozások, amelyek segítik:</span><span class="sxs-lookup"><span data-stu-id="8009c-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="8009c-108">Hogyan Office 365 használja megakadályozásához tartalomhamisítást lehetővé tévő keretet küldő (SPF)</span><span class="sxs-lookup"><span data-stu-id="8009c-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="8009c-109">SPF beállítása az Office 365-ben a hamisítás megelőzéséhez</span><span class="sxs-lookup"><span data-stu-id="8009c-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

