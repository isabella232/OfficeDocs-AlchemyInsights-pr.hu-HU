---
title: Keresés a SharePoint Online-ban
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f790efbe6ed445786933efa3fc980f974693d1d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770769"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="b9367-102">Tartalmak bejárása és indexelése a SharePoint Online-ban</span><span class="sxs-lookup"><span data-stu-id="b9367-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="b9367-103">A tartalmat be kell járni, és hozzá kell adni a keresési indexhez, hogy a felhasználók megtalálják, amit keresnek a SharePoint Online-ban.</span><span class="sxs-lookup"><span data-stu-id="b9367-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span>

- <span data-ttu-id="b9367-104">Ellenőrizze, hogy a tartalom kereshető-e a [webhely tartalma](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="b9367-104">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="b9367-105">Ha módosította a felügyelt tulajdonságot, vagy ha módosította a bejárt és felügyelt tulajdonságok megfeleltetését, a webhelyet újra be kell bejárásra, mielőtt a módosítások megjelennek a keresési indexben.</span><span class="sxs-lookup"><span data-stu-id="b9367-105">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span>

- <span data-ttu-id="b9367-106">További információt a [webhely, tár vagy lista bejárásának vagy újraindexelésének manuális kérése](https://docs.microsoft.com/sharepoint/crawl-site-content)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="b9367-106">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span>

- <span data-ttu-id="b9367-107">Várjon legalább 24 órát a bejárási és a teljes újraindexelési kérés után annak megállapításához, hogy továbbra is tapasztalja-e a problémát.</span><span class="sxs-lookup"><span data-stu-id="b9367-107">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span>

- <span data-ttu-id="b9367-108">Ha több mint 24 óra telt el, mióta a bejárást kezdeményezte, és a teljes újraindexelést kezdeményezte, kérjük, jelentkezzen be támogatási ügyben.</span><span class="sxs-lookup"><span data-stu-id="b9367-108">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="b9367-109">Sok esetben már dolgozunk a megoldáson.</span><span class="sxs-lookup"><span data-stu-id="b9367-109">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b9367-110">Kérjük, hogy végezze el a megfelelő megoldást legalább 24 óráig.</span><span class="sxs-lookup"><span data-stu-id="b9367-110">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="b9367-111">**Fontos**: Ha egy webhely, dokumentum (tár) vagy lista törlődött, és továbbra is megjelenik a találatok között, a felhasználók **nem találnak hibaüzenetet a 404-fájlok** elérésének megkísérlésekor.</span><span class="sxs-lookup"><span data-stu-id="b9367-111">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="b9367-112">A problémát a további vizsgálatokhoz támogatási esetként kell naplózni.</span><span class="sxs-lookup"><span data-stu-id="b9367-112">This issue should be logged as a support case for further investigation.</span></span>



