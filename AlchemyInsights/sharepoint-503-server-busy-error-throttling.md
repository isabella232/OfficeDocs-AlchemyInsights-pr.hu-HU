---
title: A SharePoint Online szabályozása
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761261"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="7c1ca-102">A SharePoint Online szabályozása</span><span class="sxs-lookup"><span data-stu-id="7c1ca-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="7c1ca-103">Jelenhet meg egy 503 kiszolgáló foglalt hiba, menjen el a OneDrive vagy a SharePoint-webhelyek tett kísérlet közben.</span><span class="sxs-lookup"><span data-stu-id="7c1ca-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="7c1ca-104">Ezt a hibát okozhatja a SharePoint szolgáltatáson belül szabályozását.</span><span class="sxs-lookup"><span data-stu-id="7c1ca-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="7c1ca-105">A SharePoint Online használ szabályozását az optimális teljesítmény és a SharePoint Online szolgáltatás megbízhatóságának fenntartására.</span><span class="sxs-lookup"><span data-stu-id="7c1ca-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="7c1ca-106">Szabályozási határértékek a száma, a felhasználói műveletek vagy egyidejű hívások (parancsfájl vagy kód) által erőforrások túlfelhasználást megakadályozása érdekében.</span><span class="sxs-lookup"><span data-stu-id="7c1ca-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="7c1ca-107">Ha Ön kap folyamatban, 99 %-ában egyéni kód miatt van.</span><span class="sxs-lookup"><span data-stu-id="7c1ca-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="7c1ca-108">További információt lásd, [ne beolvasása folyamatban, vagy blokkolja a SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)-szabályozás.</span><span class="sxs-lookup"><span data-stu-id="7c1ca-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="7c1ca-109">Ha úgy gondolja, hogy ez a hiba akkor független a sávszélesség-szabályozás, ha nincs aktív karbantartási [Message center](https://portal.office.com/adminportal/home#/MessageCenter)navigáljon a bérlő bekövetkező ellenőrizheti.</span><span class="sxs-lookup"><span data-stu-id="7c1ca-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="7c1ca-110">Végezetül ellenőrizze, akkor látogassa meg a [Egészségügyi szolgáltatás](https://portal.office.com/adminportal/home#/servicehealth) , amely felmerülhet tanácsadók/események ellenőrzése.</span><span class="sxs-lookup"><span data-stu-id="7c1ca-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

