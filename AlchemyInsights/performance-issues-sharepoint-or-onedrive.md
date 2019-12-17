---
title: Teljesítménnyel kapcsolatos problémák-SharePoint vagy OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068406"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="104b4-102">A SharePoint vagy az OneDrive lassú, elérhetetlen vagy nem érhető el több felhasználó számára</span><span class="sxs-lookup"><span data-stu-id="104b4-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="104b4-103">A SharePoint vagy az OneDrive lelassulhat, hozzáférhetetlen vagy nem érhető el, és több okból is elérhetetlenné vagy 503 hibát okozhat:</span><span class="sxs-lookup"><span data-stu-id="104b4-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="104b4-104">Ha a SharePoint vagy az OneDrive webhelye lassú, vagy több felhasználó számára késik, előfordulhat, hogy átmeneti szolgáltatási probléma áll fenn, ahol a felhasználók a SharePoint-webhelyek vagy az OneDrive-tartalom elérése közben időszakos késleltetést vagy navigációs hibákat tapasztalnak.</span><span class="sxs-lookup"><span data-stu-id="104b4-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="104b4-105">Ellenőrizze a [szolgáltatás állapotirányítópultját](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , hogy a szervezet érintett-e.</span><span class="sxs-lookup"><span data-stu-id="104b4-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="104b4-106">Használók május kap egy *503 szolgál van elfoglalt* hiba mikor kísérlet-hoz hajózik-hozSharepoint vagy OneDrive telek.</span><span class="sxs-lookup"><span data-stu-id="104b4-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="104b4-107">Ez a hiba a SharePoint-szolgáltatásban történő fojtás esetén is okozhatja.</span><span class="sxs-lookup"><span data-stu-id="104b4-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="104b4-108">A SharePoint Online az optimális teljesítmény és megbízhatóság fenntartására használja a SharePoint Online szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="104b4-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="104b4-109">A fojtás korlátozza a felhasználói műveletek számát vagy az egyidejű hívásokat (parancsfájlokkal vagy kóddal) az erőforrások túlzott használatának megakadályozása érdekében.</span><span class="sxs-lookup"><span data-stu-id="104b4-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="104b4-110">A szabályozásra vonatkozó további információért [Kerülje a SharePoint Online szolgáltatásban a sávszélesség vagy a Letiltás elkerülését](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="104b4-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="104b4-111">Ha a **klasszikus** vagy a **modern** SharePoint-webhellyel vagy-weblapokkal lassú teljesítményt tapasztal, használja az [oldaldiagnosztikai eszközt](https://aka.ms/perftool) az oldalak elemzéséhez.</span><span class="sxs-lookup"><span data-stu-id="104b4-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="104b4-112">Ha továbbra is lassú a teljesítmény, tekintse át a cikk alján található forrásokat: [Bevezetés a SharePoint Online teljesítményhangolásához](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="104b4-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  