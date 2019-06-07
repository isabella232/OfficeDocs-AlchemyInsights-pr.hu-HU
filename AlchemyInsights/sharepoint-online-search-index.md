---
title: A SharePoint Online keresés szótárak kezelése
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 5319c2f1edc3e61074301f039736d2aa96bda47b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758768"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="0e2fb-102">A SharePoint Online keresés</span><span class="sxs-lookup"><span data-stu-id="0e2fb-102">Search in SharePoint Online</span></span>

<span data-ttu-id="0e2fb-103">Tartalom bejárása legyen, és hozzáadódnak a keresési index számára, hogy mi azok keres a SharePoint Online keresése.</span><span class="sxs-lookup"><span data-stu-id="0e2fb-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="0e2fb-104">Automatikusan a bejárt tartalmat alapján előre definiált bejárási ütemezés (a bejárás ütemezése nem lehet módosítani).</span><span class="sxs-lookup"><span data-stu-id="0e2fb-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="0e2fb-105">A webbejáró veszi fel tartalmat, amely a legutóbbi bejárás óta megváltozott, és frissíti az indexet.</span><span class="sxs-lookup"><span data-stu-id="0e2fb-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="0e2fb-106">A bejárt tartalmat, és az index frissítése érdekében kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="0e2fb-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="0e2fb-107">Ellenőrizze, hogy azáltal, hogy a webhely tartalma kereshető tartalom található.</span><span class="sxs-lookup"><span data-stu-id="0e2fb-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="0e2fb-108">További információért lásd [a helyszínen kell kereshető tartalom engedélyezése](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="0e2fb-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="0e2fb-109">Felügyelt tulajdonság módosítása után, vagy ha megváltoztatta hozzárendelése bejárt és kezelt tulajdonságai, a webhely bejárását előtt kell a változások megjelennek a keresési indexben.</span><span class="sxs-lookup"><span data-stu-id="0e2fb-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="0e2fb-110">A módosítások megjelennek a keresési sémában, és nem a tényleges hely, mert a webbejáró nem automatikusan újra indexeli a webhelyet.</span><span class="sxs-lookup"><span data-stu-id="0e2fb-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="0e2fb-111">További információért lásd: [manuálisan kérheti a bejárási és indexelési újra a hely, a tár vagy lista](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="0e2fb-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="0e2fb-112">Várjon, amíg manuálisan a bejárás és teljes újraindexelése megtekintéséhez, ha még mindig fennáll a probléma bekérése után legalább 24 órán keresztül.</span><span class="sxs-lookup"><span data-stu-id="0e2fb-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="0e2fb-113">Ha 24 óránál hosszabb idő telt el azóta a bejárás és a teljes újraindexelése kezdeményezett, jelentkezzen be a támogatási eset.</span><span class="sxs-lookup"><span data-stu-id="0e2fb-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="0e2fb-114">Sok esetben azt már dolgozik a megoldáson.</span><span class="sxs-lookup"><span data-stu-id="0e2fb-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="0e2fb-115">Adja meg a megoldás végrehajtásához legalább 24 órán keresztül.</span><span class="sxs-lookup"><span data-stu-id="0e2fb-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="0e2fb-116">**Fontos**: Ha hely, a dokumentum (könyvtár) vagy a lista volt a törölt és továbbra is megjeleníti a keresési eredmények között, a felhasználók kell kapnia egy hiba 404 fájl nem található mikor megpróbáljuk elérni.</span><span class="sxs-lookup"><span data-stu-id="0e2fb-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="0e2fb-117">A probléma további vizsgálatához támogatási eset kell naplózásra.</span><span class="sxs-lookup"><span data-stu-id="0e2fb-117">This issue should be logged as a support case for further investigation.</span></span> 



