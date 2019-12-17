---
title: A keresési séma kezelése a SharePoint Online szolgáltatásban
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042965"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="a5fa3-102">A keresési séma kezelése a SharePoint Online szolgáltatásban</span><span class="sxs-lookup"><span data-stu-id="a5fa3-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="a5fa3-103">A keresési séma határozza meg, hogy mely felhasználók kereshetnek, hogyan kereshetnek az adott felhasználó, és hogyan jelenhetnek meg az eredmények a keresési webhelyeken.</span><span class="sxs-lookup"><span data-stu-id="a5fa3-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="a5fa3-104">A [keresési séma kezelése a SharePoint Online szolgáltatásban](https://docs.microsoft.com/sharepoint/manage-search-schema) című témakör ismerteti a következő tudnivalókat:</span><span class="sxs-lookup"><span data-stu-id="a5fa3-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="a5fa3-105">Módosítsa a keresési sémát.</span><span class="sxs-lookup"><span data-stu-id="a5fa3-105">Change the search schema.</span></span>
- <span data-ttu-id="a5fa3-106">Felügyelt tulajdonságok létrehozása.</span><span class="sxs-lookup"><span data-stu-id="a5fa3-106">Create managed properties.</span></span>
- <span data-ttu-id="a5fa3-107">Megfeleltetett leképezés bejárt térképhez a felügyelt tulajdonságokhoz.</span><span class="sxs-lookup"><span data-stu-id="a5fa3-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="a5fa3-108">A keresési séma kezelésével kapcsolatban vegye figyelembe az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="a5fa3-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="a5fa3-109">Ha a sémamódosítások során figyelmeztetés jelenik meg **az alkalmazás szüneteltetésekor** , ez csak ideiglenes, mivel a szolgáltatás karbantartása bekövetkezik.</span><span class="sxs-lookup"><span data-stu-id="a5fa3-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="a5fa3-110">Ha több mint 24 óra telt el, és még mindig tapasztalja a figyelmeztetést, kérjük, jelentkezzen be a támogatási ügyben.</span><span class="sxs-lookup"><span data-stu-id="a5fa3-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="a5fa3-111">Felügyelt tulajdonságok módosítása vagy újak hozzáadása esetén a módosítások csak a tartalom ismételt bejárását követően lépnek érvénybe.</span><span class="sxs-lookup"><span data-stu-id="a5fa3-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="a5fa3-112">A SharePoint Online szolgáltatásban a bejárás automatikusan megtörténik a megadott bejárási ütemezés alapján.</span><span class="sxs-lookup"><span data-stu-id="a5fa3-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="a5fa3-113">Annak érdekében, hogy a módosítások bejárhatók legyenek, külön [kérheti a lista vagy tár újraindexelését](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) .</span><span class="sxs-lookup"><span data-stu-id="a5fa3-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="a5fa3-114">A keresési séma teljes áttekintéséhez lásd: a [keresési séma bemutatása](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="a5fa3-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


