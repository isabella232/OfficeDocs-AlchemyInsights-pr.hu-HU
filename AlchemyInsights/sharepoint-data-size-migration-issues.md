---
title: Problémák az adatok SharePoint Online-ba való áttelepítése közben
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931696"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="bd619-102">Problémák az adatok SharePoint Online-ba való áttelepítése közben</span><span class="sxs-lookup"><span data-stu-id="bd619-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="bd619-103">**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben.</span><span class="sxs-lookup"><span data-stu-id="bd619-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="bd619-104">Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások.</span><span class="sxs-lookup"><span data-stu-id="bd619-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="bd619-105">Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="bd619-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="bd619-106">Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon.</span><span class="sxs-lookup"><span data-stu-id="bd619-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="bd619-107">Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben.</span><span class="sxs-lookup"><span data-stu-id="bd619-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="bd619-108">Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.</span><span class="sxs-lookup"><span data-stu-id="bd619-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="bd619-109">**Több mint 100 TB adat áttelepítése**</span><span class="sxs-lookup"><span data-stu-id="bd619-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="bd619-110">Úgy tűnik, több mint 100 TB adatot telepít át a SharePoint Online-ba.</span><span class="sxs-lookup"><span data-stu-id="bd619-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="bd619-111">Kérjük, kövesse az alábbi lépéseket, hogy a lehető leghamarabb segíthessünk Önnek.</span><span class="sxs-lookup"><span data-stu-id="bd619-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="bd619-112">Válassza az **Új szolgáltatáskérelem**, majd **az Új szolgáltatáskérelem lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="bd619-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="bd619-113">Hagyja a címet és a leírást **SharePoint-áttelepítésként 100 TB-nál is.**</span><span class="sxs-lookup"><span data-stu-id="bd619-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="bd619-114">A jegy beküldése után kérjük, frissítse a következő információkkal:</span><span class="sxs-lookup"><span data-stu-id="bd619-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="bd619-115">Az áttelepítés becsült mérete.</span><span class="sxs-lookup"><span data-stu-id="bd619-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="bd619-116">Becslés abból, hogy mikor szeretné elindítani és befejezni az áttelepítést.</span><span class="sxs-lookup"><span data-stu-id="bd619-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="bd619-117">Írja le, hogy honnan telepíti át a tartalmat, például a SharePoint Server, a Box, a GDrive, a Fájlmegosztások stb.</span><span class="sxs-lookup"><span data-stu-id="bd619-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

