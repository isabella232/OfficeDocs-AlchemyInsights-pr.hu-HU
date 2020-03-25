---
title: SharePoint áttelepítési szabályozás 503-as hibákkal
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931660"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="e261f-102">SharePoint áttelepítési szabályozás 503-as hibákkal</span><span class="sxs-lookup"><span data-stu-id="e261f-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="e261f-103">**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben.</span><span class="sxs-lookup"><span data-stu-id="e261f-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e261f-104">Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások.</span><span class="sxs-lookup"><span data-stu-id="e261f-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e261f-105">Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="e261f-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e261f-106">Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon.</span><span class="sxs-lookup"><span data-stu-id="e261f-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e261f-107">Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben.</span><span class="sxs-lookup"><span data-stu-id="e261f-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e261f-108">Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.</span><span class="sxs-lookup"><span data-stu-id="e261f-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e261f-109">**503-as hibák a SharePoint Online-ra való áttéréskor**</span><span class="sxs-lookup"><span data-stu-id="e261f-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="e261f-110">Úgy tűnik, hogy a SharePoint Online-ra költözik, és 503-as hibákat kap.</span><span class="sxs-lookup"><span data-stu-id="e261f-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="e261f-111">Kérjük, kövesse az alábbi lépéseket, hogy a lehető leghamarabb segíthessünk Önnek.</span><span class="sxs-lookup"><span data-stu-id="e261f-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="e261f-112">Kattintson **a Kapcsolatfelvételi szolgáltatás**, majd **az Új szolgáltatáskérés parancsra.**</span><span class="sxs-lookup"><span data-stu-id="e261f-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="e261f-113">A cím és a leírás mezőbe írja be a **SharePoint áttelepítési szabályozását az 503-as sal.**</span><span class="sxs-lookup"><span data-stu-id="e261f-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="e261f-114">A jegy beküldése után kérjük, frissítse a következő információkkal:</span><span class="sxs-lookup"><span data-stu-id="e261f-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="e261f-115">Mennyi maradt a migrációból (például hány TB?).</span><span class="sxs-lookup"><span data-stu-id="e261f-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="e261f-116">Áttelepítés kezdő és záró dátuma.</span><span class="sxs-lookup"><span data-stu-id="e261f-116">Migration start and end date.</span></span>
    - <span data-ttu-id="e261f-117">Írja le, hogy honnan telepíti át a tartalmat, például a SharePoint Server, a Box, a GDrive, a Fájlmegosztások stb.</span><span class="sxs-lookup"><span data-stu-id="e261f-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="e261f-118">Becsülje meg a sávszélesség-szabályozási hibák számát (például x sávszélesség-szabályozás óránként?), és mikor történt a szabályozás.</span><span class="sxs-lookup"><span data-stu-id="e261f-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="e261f-119">Az ön által használt áttelepítési eszköz (például SPMT vagy ShareGate).</span><span class="sxs-lookup"><span data-stu-id="e261f-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


