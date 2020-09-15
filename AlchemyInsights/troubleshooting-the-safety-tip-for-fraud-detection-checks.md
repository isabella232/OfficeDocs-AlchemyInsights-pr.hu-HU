---
title: A csalások észlelését ellenőrző biztonsági tippek hibaelhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658412"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="75d32-102">A csalások észlelését ellenőrző biztonsági tippek hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="75d32-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="75d32-103">Ha olyan biztonsági tippet kap, amely azt mondja, hogy "a feladó nem tudta a csalás észlelési vizsgálatát, és nem lehet, hogy kik jelennek meg", akkor a feladó nem tudta átadni a DKIM vagy az SPF-hitelesítési ellenőrzéseket.</span><span class="sxs-lookup"><span data-stu-id="75d32-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="75d32-104">A legjobb megoldás, ha a feladónak engedélyezni szeretné a feladót.</span><span class="sxs-lookup"><span data-stu-id="75d32-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="75d32-105">Ha a feladó az Ön nevében küldi el a feladót, engedélyeznie kell őket úgy, hogy hozzáadja a feladó IP-címét az SPF rekordhoz.</span><span class="sxs-lookup"><span data-stu-id="75d32-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="75d32-106">További információért olvassa el [a hibák elhárítása a vörös (gyanús) biztonsági tippekkel](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) című témakört.</span><span class="sxs-lookup"><span data-stu-id="75d32-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="75d32-107">Íme néhány további hivatkozás, amelyek segítséget nyújthatnak:</span><span class="sxs-lookup"><span data-stu-id="75d32-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="75d32-108">Hogyan használja a Microsoft a feladói házirend keretrendszert (SPF) a hamisítás megakadályozására</span><span class="sxs-lookup"><span data-stu-id="75d32-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="75d32-109">Az SPF beállítással megakadályozhatja a hamisítást</span><span class="sxs-lookup"><span data-stu-id="75d32-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
