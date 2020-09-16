---
title: Teljesítménnyel kapcsolatos problémák – SharePoint vagy OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771903"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="ac248-102">A SharePoint és a OneDrive lassú, elérhetetlen vagy nem érhető el egyszerre több felhasználó esetében</span><span class="sxs-lookup"><span data-stu-id="ac248-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="ac248-103">Előfordulhat, hogy a SharePoint vagy a OneDrive lassú, elérhetetlen vagy elérhetetlen, vagy a szolgáltatás nem érhető el, vagy a 503 hibája, több okból kifolyólag:</span><span class="sxs-lookup"><span data-stu-id="ac248-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="ac248-104">Ha SharePoint-vagy OneDrive-webhelye lassú vagy késleltetett több felhasználó esetében, előfordulhat, hogy ideiglenes szolgáltatási probléma merül fel, ahol a felhasználók időnként késleltetve vagy navigációs hibákba ütköznek a SharePoint-webhelyek vagy a OneDrive-tartalmak elérésekor.</span><span class="sxs-lookup"><span data-stu-id="ac248-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="ac248-105">A [szolgáltatás állapota irányítópulton](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) ellenőrizheti, hogy a szervezete hatással van-e rá.</span><span class="sxs-lookup"><span data-stu-id="ac248-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="ac248-106">A felhasználók a SharePoint-vagy a OneDrive-webhelyeken való navigáláskor elfoglalt hibába ütközhet a *503-kiszolgálóval* .</span><span class="sxs-lookup"><span data-stu-id="ac248-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="ac248-107">Ezt a hibát a SharePoint-szolgáltatáson belüli szabályozás okozhatja.</span><span class="sxs-lookup"><span data-stu-id="ac248-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="ac248-108">A SharePoint Online a szabályozást használja a SharePoint Online szolgáltatás optimális teljesítményének és megbízhatóságának fenntartásához.</span><span class="sxs-lookup"><span data-stu-id="ac248-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="ac248-109">A szabályozás korlátozza a felhasználói műveletek vagy a párhuzamos hívások számát (parancsprogrammal vagy kóddal) az erőforrások túlzott felhasználásának megelőzése érdekében.</span><span class="sxs-lookup"><span data-stu-id="ac248-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="ac248-110">A szabályozással kapcsolatos további tudnivalókért olvassa el a [SharePoint Online-ban a letiltott vagy Letiltva](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="ac248-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="ac248-111">Ha gyenge teljesítményt tapasztal egy **klasszikus** vagy **modern** SharePoint-webhelyen vagy-lapon, használja a [lap diagnosztikai eszközét](https://aka.ms/perftool) a lapok elemzéséhez.</span><span class="sxs-lookup"><span data-stu-id="ac248-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="ac248-112">Ha továbbra is általános gyenge teljesítményt tapasztal, olvassa el a jelen cikk alján található forrásokat: [Bevezetés a SharePoint Online teljesítményének finomhangolásával](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="ac248-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  