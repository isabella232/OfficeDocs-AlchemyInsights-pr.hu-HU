---
title: SharePoint Online szabályozása
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958724"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="ecb45-102">SharePoint Online szabályozása</span><span class="sxs-lookup"><span data-stu-id="ecb45-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="ecb45-103">**Fontos:** Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is magas rendelkezésre állásúak maradjanak – további információkért látogasson el a [SharePoint Online ideiglenes szolgáltatásának korrekcióira.](https://aka.ms/ODSPAdjustments)</span><span class="sxs-lookup"><span data-stu-id="ecb45-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ecb45-104">**Az 503-as kiszolgáló foglalt hiba**</span><span class="sxs-lookup"><span data-stu-id="ecb45-104">**503 server is busy error**</span></span>

<span data-ttu-id="ecb45-105">Előfordulhat, hogy a felhasználók 503-as kiszolgálófoglalt hibaüzenetet kapnak, amikor SharePoint- vagy OneDrive-webhelyekre próbálnak navigálni.</span><span class="sxs-lookup"><span data-stu-id="ecb45-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="ecb45-106">Ezt a hibát a SharePoint szolgáltatáson belüli szabályozás okozhatja.</span><span class="sxs-lookup"><span data-stu-id="ecb45-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="ecb45-107">A SharePoint Online szabályozással állítja fenn a SharePoint Online-szolgáltatás optimális teljesítményét és megbízhatóságát.</span><span class="sxs-lookup"><span data-stu-id="ecb45-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="ecb45-108">Szabályozás korlátozza a felhasználói műveletek számát vagy egyidejű hívások (parancsfájl vagy kód) az erőforrások túlzott használatának megelőzése érdekében.</span><span class="sxs-lookup"><span data-stu-id="ecb45-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="ecb45-109">A szabályozásról további információt a [SharePoint Online-ban található Szabályozás elkerülése című témakörben](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)talál.</span><span class="sxs-lookup"><span data-stu-id="ecb45-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="ecb45-110">Ha úgy véli, hogy ez a hiba nem kapcsolódik a szabályozáshoz, ellenőrizheti, hogy a bérlőn aktív karbantartás történik-e, ha az [Üzenetközpontra](https://portal.office.com/adminportal/home#/MessageCenter)navigál.</span><span class="sxs-lookup"><span data-stu-id="ecb45-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="ecb45-111">Végül győződjön meg róla, hogy látogasson el a [Service Health](https://portal.office.com/adminportal/home#/servicehealth) oldalra, hogy ellenőrizze az esetlegesen előforduló tanácsokat/incidenseket.</span><span class="sxs-lookup"><span data-stu-id="ecb45-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

