---
title: Az áttelepítési teljesítményt ismertető általános útmutató
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932481"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="63985-102">Az áttelepítési teljesítményt ismertető általános útmutató</span><span class="sxs-lookup"><span data-stu-id="63985-102">General migration performance guidance</span></span>

<span data-ttu-id="63985-103">**Fontos**: A SharePoint Online és a OneDrive számos felhasználója futtat a háttérben üzleti szempontból kritikus fontosságú alkalmazásokat a szolgáltatáson.</span><span class="sxs-lookup"><span data-stu-id="63985-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="63985-104">Ezek közé tartoznak a tartalom áttelepítésére, az adatvesztés megelőzésére (DLP) és a biztonsági mentésre szolgáló megoldások.</span><span class="sxs-lookup"><span data-stu-id="63985-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="63985-105">Ezekben a példátlan időkben különböző lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatás továbbra is magas rendelkezésre állással és megbízhatóan működjön a felhasználók számára, akik a távmunkára épülő helyzetekben minden eddiginél jobban függnek a szolgáltatástól.</span><span class="sxs-lookup"><span data-stu-id="63985-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="63985-106">E cél elérése érdekében szigorúbb leszabályozási korlátokat vezettünk be a háttérben futó alkalmazásokra (áttelepítési, DLP- és biztonsági mentési megoldásokra) vonatkozóan hétköznap a nappali órákban.</span><span class="sxs-lookup"><span data-stu-id="63985-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="63985-107">Számítania kell arra, hogy ezek az alkalmazások nagyon korlátozott átviteli sebességet biztosítanak majd ezekben az időszakokban.</span><span class="sxs-lookup"><span data-stu-id="63985-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="63985-108">Az adott régió esti és hétvégi időszakaiban azonban a szolgáltatás készen áll arra, hogy lényegesen nagyobb mennyiségű, a háttéralkalmazásoktól érkező kérést dolgozzon fel.</span><span class="sxs-lookup"><span data-stu-id="63985-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="63985-109">**Az áttelepítési teljesítményt ismertető útmutató**</span><span class="sxs-lookup"><span data-stu-id="63985-109">**Migration performance guidance**</span></span>

<span data-ttu-id="63985-110">Az áttelepítési teljesítményt befolyásolhatja a hálózati infrastruktúra, a fájlok mérete, az áttelepítés időpontja és a leszabályozás.</span><span class="sxs-lookup"><span data-stu-id="63985-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="63985-111">Ezek megértése segítséget nyújthat az áttelepítés megtervezéséhez és a lehető leghatékonyabb elvégzéséhez.</span><span class="sxs-lookup"><span data-stu-id="63985-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="63985-112">Az áttelepítési teljesítményt ismertető általános útmutató</span><span class="sxs-lookup"><span data-stu-id="63985-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
