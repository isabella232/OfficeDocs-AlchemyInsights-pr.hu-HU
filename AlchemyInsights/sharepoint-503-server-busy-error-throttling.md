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
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559843"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="67136-102">A SharePoint Online szabályozása</span><span class="sxs-lookup"><span data-stu-id="67136-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="67136-103">Jelenhet meg egy 503 kiszolgáló foglalt hiba, menjen el a OneDrive vagy a SharePoint-webhelyek tett kísérlet közben.</span><span class="sxs-lookup"><span data-stu-id="67136-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="67136-104">Ezt a hibát okozhatja a SharePoint szolgáltatáson belül szabályozását.</span><span class="sxs-lookup"><span data-stu-id="67136-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="67136-105">A SharePoint Online használ szabályozását az optimális teljesítmény és a SharePoint Online szolgáltatás megbízhatóságának fenntartására.</span><span class="sxs-lookup"><span data-stu-id="67136-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="67136-106">Szabályozási határértékek a száma, a felhasználói műveletek vagy egyidejű hívások (parancsfájl vagy kód) által erőforrások túlfelhasználást megakadályozása érdekében.</span><span class="sxs-lookup"><span data-stu-id="67136-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="67136-107">Ha Ön kap folyamatban, 99 %-ában egyéni kód miatt van.</span><span class="sxs-lookup"><span data-stu-id="67136-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="67136-108">További információt lásd, [ne beolvasása folyamatban, vagy blokkolja a SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)-szabályozás.</span><span class="sxs-lookup"><span data-stu-id="67136-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="67136-109">Ha úgy gondolja, hogy ez a hiba akkor független a sávszélesség-szabályozás, ha nincs aktív karbantartási [Message center](https://portal.office.com/adminportal/home#/MessageCenter)navigáljon a bérlő bekövetkező ellenőrizheti.</span><span class="sxs-lookup"><span data-stu-id="67136-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="67136-110">Végezetül ellenőrizze, akkor látogassa meg a [Egészségügyi szolgáltatás](https://portal.office.com/adminportal/home#/servicehealth) , amely felmerülhet tanácsadók/események ellenőrzése.</span><span class="sxs-lookup"><span data-stu-id="67136-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

