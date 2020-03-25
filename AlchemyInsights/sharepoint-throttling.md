---
title: SharePoint Online szabályozása
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931444"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="852a7-102">SharePoint Online szabályozása</span><span class="sxs-lookup"><span data-stu-id="852a7-102">SharePoint Online throttling</span></span>

<span data-ttu-id="852a7-103">**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben.</span><span class="sxs-lookup"><span data-stu-id="852a7-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="852a7-104">Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások.</span><span class="sxs-lookup"><span data-stu-id="852a7-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="852a7-105">Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="852a7-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="852a7-106">Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon.</span><span class="sxs-lookup"><span data-stu-id="852a7-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="852a7-107">Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben.</span><span class="sxs-lookup"><span data-stu-id="852a7-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="852a7-108">Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.</span><span class="sxs-lookup"><span data-stu-id="852a7-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="852a7-109">**SharePoint Online szabályozása**</span><span class="sxs-lookup"><span data-stu-id="852a7-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="852a7-110">A SharePoint Online szabályozással állítja fenn a SharePoint Online-szolgáltatás optimális teljesítményét és megbízhatóságát.</span><span class="sxs-lookup"><span data-stu-id="852a7-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="852a7-111">Szabályozás korlátozza a felhasználói műveletek számát vagy egyidejű hívások (parancsfájl vagy kód) az erőforrások túlzott használatának megelőzése érdekében.</span><span class="sxs-lookup"><span data-stu-id="852a7-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="852a7-112">További információkért kérjük, látogasson el az alábbi linkekre.</span><span class="sxs-lookup"><span data-stu-id="852a7-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="852a7-113">A SharePoint Online-ban nem lehet szabályozni vagy letiltani.</span><span class="sxs-lookup"><span data-stu-id="852a7-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="852a7-114">Adatáttelepítés és SPO-szabályozás</span><span class="sxs-lookup"><span data-stu-id="852a7-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="852a7-115">A SharePoint Online és a OneDrive áttelepítési sebessége</span><span class="sxs-lookup"><span data-stu-id="852a7-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="852a7-116">SharePoint Online-szabályozás leválasztása exponenciális visszaválasztással</span><span class="sxs-lookup"><span data-stu-id="852a7-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="852a7-117">Kapacitástervezés és terheléstesztelés a SharePoint Online-ban</span><span class="sxs-lookup"><span data-stu-id="852a7-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

