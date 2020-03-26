---
title: Áttérés a SharePoint Online-ra az Áttelepítéskezelő használatával
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
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932181"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="c6926-102">Áttérés a SharePoint Online-ra az Áttelepítéskezelő használatával</span><span class="sxs-lookup"><span data-stu-id="c6926-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="c6926-103">**Fontos**: A SharePoint Online és a OneDrive számos felhasználója futtat a háttérben üzleti szempontból kritikus fontosságú alkalmazásokat a szolgáltatáson.</span><span class="sxs-lookup"><span data-stu-id="c6926-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c6926-104">Ezek közé tartoznak a tartalom áttelepítésére, az adatvesztés megelőzésére (DLP) és a biztonsági mentésre szolgáló megoldások.</span><span class="sxs-lookup"><span data-stu-id="c6926-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c6926-105">Ezekben a példátlan időkben különböző lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatás továbbra is magas rendelkezésre állással és megbízhatóan működjön a felhasználók számára, akik a távmunkára épülő helyzetekben minden eddiginél jobban függnek a szolgáltatástól.</span><span class="sxs-lookup"><span data-stu-id="c6926-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c6926-106">E cél elérése érdekében szigorúbb leszabályozási korlátokat vezettünk be a háttérben futó alkalmazásokra (áttelepítési, DLP- és biztonsági mentési megoldásokra) vonatkozóan hétköznap a nappali órákban.</span><span class="sxs-lookup"><span data-stu-id="c6926-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c6926-107">Számítania kell arra, hogy ezek az alkalmazások nagyon korlátozott átviteli sebességet biztosítanak majd ezekben az időszakokban.</span><span class="sxs-lookup"><span data-stu-id="c6926-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c6926-108">Az adott régió esti és hétvégi időszakaiban azonban a szolgáltatás készen áll arra, hogy lényegesen nagyobb mennyiségű, a háttéralkalmazásoktól érkező kérést dolgozzon fel.</span><span class="sxs-lookup"><span data-stu-id="c6926-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c6926-109">**Áttelepítéskezelő**</span><span class="sxs-lookup"><span data-stu-id="c6926-109">**Migration Manager**</span></span>

<span data-ttu-id="c6926-110">A modern SharePoint Felügyeleti központban található Áttelepítéskezelő végigvezeti az ügyfelek beállításának és a feladatok létrehozásának lépésein.</span><span class="sxs-lookup"><span data-stu-id="c6926-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="c6926-111">Megadhat globális vagy feladatszintű beállításokat, megtekintheti az összes feladat előrehaladását, és letölthet összesített eredményeket mutató összefoglaló, illetve feladatszintű jelentéseket.</span><span class="sxs-lookup"><span data-stu-id="c6926-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="c6926-112">Első lépések az Áttelepítéskezelővel</span><span class="sxs-lookup"><span data-stu-id="c6926-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="c6926-113">Áttelepítéskezelő-ügyfelek beállítása</span><span class="sxs-lookup"><span data-stu-id="c6926-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="c6926-114">Az Áttelepítéskezelő beállításai</span><span class="sxs-lookup"><span data-stu-id="c6926-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
