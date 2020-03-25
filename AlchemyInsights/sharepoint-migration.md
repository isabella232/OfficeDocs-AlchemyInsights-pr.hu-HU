---
title: Áttelepítési beállítások a SharePoint Online-ba
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932732"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="c5d43-102">Áttelepítési beállítások a SharePoint Online-ba</span><span class="sxs-lookup"><span data-stu-id="c5d43-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="c5d43-103">**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben.</span><span class="sxs-lookup"><span data-stu-id="c5d43-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c5d43-104">Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások.</span><span class="sxs-lookup"><span data-stu-id="c5d43-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c5d43-105">Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="c5d43-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c5d43-106">Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon.</span><span class="sxs-lookup"><span data-stu-id="c5d43-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c5d43-107">Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben.</span><span class="sxs-lookup"><span data-stu-id="c5d43-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c5d43-108">Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.</span><span class="sxs-lookup"><span data-stu-id="c5d43-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c5d43-109">**Áttelepítési beállítások**</span><span class="sxs-lookup"><span data-stu-id="c5d43-109">**Migration options**</span></span>

<span data-ttu-id="c5d43-110">A tartalom SharePoint Online-ba való áttelepítésére különböző lehetőségek állnak rendelkezésre, az áthelyezendő fájlok méretétől és mennyiségétől függően, lásd az [itt található](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online)lehetőségek listáját.</span><span class="sxs-lookup"><span data-stu-id="c5d43-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="c5d43-111">A tartalomáttelepítéssel kapcsolatos további információkért kérjük, látogasson el az alábbi linkekre.</span><span class="sxs-lookup"><span data-stu-id="c5d43-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="c5d43-112">Sharepoint áttelepítési eszköz</span><span class="sxs-lookup"><span data-stu-id="c5d43-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="c5d43-113">Első lépések az Áttelepítési kezelővel</span><span class="sxs-lookup"><span data-stu-id="c5d43-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="c5d43-114">SharePoint Online és ODB áttelepítési sebesség</span><span class="sxs-lookup"><span data-stu-id="c5d43-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="c5d43-115">A SharePoint Online-ban nem lehet szabályozni vagy letiltani.</span><span class="sxs-lookup"><span data-stu-id="c5d43-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="c5d43-116">SharePoint áttelepítési értékelő eszköz (SMAT)</span><span class="sxs-lookup"><span data-stu-id="c5d43-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="c5d43-117">**Megjegyzés:** Jelenleg a SharePoint áttelepítési eszköz csak a SharePoint 2010-ből és 2013-as áttelepítéseket támogatja.</span><span class="sxs-lookup"><span data-stu-id="c5d43-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="c5d43-118">A 2016-os vagy 2019-es verzió jelenleg nem támogatott.</span><span class="sxs-lookup"><span data-stu-id="c5d43-118">Version 2016 or 2019 are not supported at this time.</span></span>
