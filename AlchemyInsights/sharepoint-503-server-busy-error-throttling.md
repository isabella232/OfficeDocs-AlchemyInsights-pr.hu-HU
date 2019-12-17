---
title: SharePoint Online-szabályozás
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: ed3598dc92a7c36c9c9b077db0ab31f63537ef60
ms.sourcegitcommit: 14894a09db1c4101e48ff720d878d1c9f7b1dac8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/16/2019
ms.locfileid: "40065560"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="97474-102">SharePoint Online-szabályozás</span><span class="sxs-lookup"><span data-stu-id="97474-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="97474-103">Használók május kap egy 503 szolgál van elfoglalt hiba mikor kísérlet-hoz hajózik-hoz SharePoint vagy OneDrive telek.</span><span class="sxs-lookup"><span data-stu-id="97474-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="97474-104">Ez a hiba a SharePoint-szolgáltatásban történő fojtás esetén is okozhatja.</span><span class="sxs-lookup"><span data-stu-id="97474-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="97474-105">A SharePoint Online az optimális teljesítmény és megbízhatóság fenntartására használja a SharePoint Online szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="97474-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="97474-106">A fojtás korlátozza a felhasználói műveletek számát vagy az egyidejű hívásokat (parancsfájlokkal vagy kóddal) az erőforrások túlzott használatának megakadályozása érdekében.</span><span class="sxs-lookup"><span data-stu-id="97474-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="97474-107">A szabályozásra vonatkozó további információért [Kerülje a SharePoint Online szolgáltatásban a sávszélesség vagy a Letiltás elkerülését](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="97474-107">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="97474-108">Ha úgy gondolja, hogy ez a hiba nem kapcsolódik a fojtáshoz, akkor ellenőrizze, hogy van-e aktív karbantartás a bérlőnél az [Üzenetközpontba](https://portal.office.com/adminportal/home#/MessageCenter)való navigálással.</span><span class="sxs-lookup"><span data-stu-id="97474-108">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="97474-109">Végül, biztosít ön látogat a [szolgáltatás egészség](https://portal.office.com/adminportal/home#/servicehealth) oldal-hoz ellenőriz részére akármi figyelmeztetéseket/eset amit május előfordul.</span><span class="sxs-lookup"><span data-stu-id="97474-109">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

