---
title: A SharePoint áttelepítési eszközével kapcsolatos problémák és hibák elhárítása
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931120"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="7ff4e-102">A SharePoint áttelepítési eszközével kapcsolatos problémák és hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="7ff4e-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="7ff4e-103">**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben.</span><span class="sxs-lookup"><span data-stu-id="7ff4e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="7ff4e-104">Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások.</span><span class="sxs-lookup"><span data-stu-id="7ff4e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="7ff4e-105">Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="7ff4e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="7ff4e-106">Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon.</span><span class="sxs-lookup"><span data-stu-id="7ff4e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="7ff4e-107">Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben.</span><span class="sxs-lookup"><span data-stu-id="7ff4e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="7ff4e-108">Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.</span><span class="sxs-lookup"><span data-stu-id="7ff4e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="7ff4e-109">**Gyakori problémák és hibák**</span><span class="sxs-lookup"><span data-stu-id="7ff4e-109">**Common issues and errors**</span></span>

<span data-ttu-id="7ff4e-110">A SharePoint áttelepítési eszköz (SPMT) használatakor gyakori problémák és hibák léphetnek fel.</span><span class="sxs-lookup"><span data-stu-id="7ff4e-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="7ff4e-111">További információkért kérjük, olvassa el az alábbi linkeket.</span><span class="sxs-lookup"><span data-stu-id="7ff4e-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="7ff4e-112">Gyakori SPMT-problémák és -hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="7ff4e-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="7ff4e-113">Az SPMT telepítésével kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="7ff4e-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)