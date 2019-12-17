---
title: Keresés a SharePoint Online szolgáltatásban
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044045"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="e70d6-102">Tartalomfeltérképezés és indexelés a SharePoint Online szolgáltatásban</span><span class="sxs-lookup"><span data-stu-id="e70d6-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="e70d6-103">A tartalmat bejárnia kell, és hozzá kell adnia a keresési indexhez ahhoz, hogy megtalálja a keresést a SharePoint Online szolgáltatásban.</span><span class="sxs-lookup"><span data-stu-id="e70d6-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="e70d6-104">A program a tartalmat előre definiált bejárási ütemezés alapján automatikusan feltérképezi (a bejárási ütemezés nem módosítható).</span><span class="sxs-lookup"><span data-stu-id="e70d6-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="e70d6-105">A webbejáró felveszi az utolsó bejárás óta módosult tartalmat, és frissíti az indexet.</span><span class="sxs-lookup"><span data-stu-id="e70d6-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="e70d6-106">A tartalombejárás és az index frissítése érdekében vegye figyelembe a következőket:</span><span class="sxs-lookup"><span data-stu-id="e70d6-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="e70d6-107">Győződjön meg arról, hogy tartalma megtalálható a [webhely tartalmának kereshetővé tétele](https://docs.microsoft.com/sharepoint/make-site-content-searchable)érdekében.</span><span class="sxs-lookup"><span data-stu-id="e70d6-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="e70d6-108">Miután módosította a felügyelt tulajdonságot, vagy módosította a bejárt és kezelt tulajdonságok hozzárendelését, a webhelyet újra kell bejárnia ahhoz, hogy a módosítások megjelenjenek a keresési indexben.</span><span class="sxs-lookup"><span data-stu-id="e70d6-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="e70d6-109">Mivel a módosítások a keresési sémában történtek, és nem az aktuális webhelyre, a webbejáró nem fogja automatikusan újra indexelni a webhelyet.</span><span class="sxs-lookup"><span data-stu-id="e70d6-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="e70d6-110">További információt a [webhelyek, tárak és listák kézi vagy újraindexelésének manuális kérése](https://docs.microsoft.com/sharepoint/crawl-site-conten)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="e70d6-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="e70d6-111">A bejárás és a teljes újraindex manuális kérése után várjon legalább 24 órát, és ellenőrizze, hogy a probléma továbbra is fennáll-e.</span><span class="sxs-lookup"><span data-stu-id="e70d6-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="e70d6-112">Ha több mint 24 óra telt el mióta kezdeményezte a feltérképezés és a teljes re-index, kérjük, jelentkezzen egy támogatási ügyben.</span><span class="sxs-lookup"><span data-stu-id="e70d6-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="e70d6-113">Sok esetben már dolgozunk a megoldásban.</span><span class="sxs-lookup"><span data-stu-id="e70d6-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="e70d6-114">Kérjük, hogy a megoldás befejezéséhez legalább 24 órát adjon nekünk.</span><span class="sxs-lookup"><span data-stu-id="e70d6-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e70d6-115">Ha egy webhelyet, dokumentumot (könyvtárat) vagy listát töröltek, és még mindig láthatók a keresési eredményekben, a felhasználóknak hibaüzenetet kell kapniuk, **404 a fájl nem található** , amikor megpróbálnak hozzáférni hozzá.</span><span class="sxs-lookup"><span data-stu-id="e70d6-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="e70d6-116">Ezt a kérdést a további kivizsgálás támogatási eseteként kell naplóznia.</span><span class="sxs-lookup"><span data-stu-id="e70d6-116">This issue should be logged as a support case for further investigation.</span></span> 



