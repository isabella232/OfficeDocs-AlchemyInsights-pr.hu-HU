---
title: A keresési séma kezelése a SharePoint Online-ban
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770553"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="77e7b-102">A keresési séma kezelése a SharePoint Online-ban</span><span class="sxs-lookup"><span data-stu-id="77e7b-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="77e7b-103">A keresési séma szabályozza, hogy a felhasználók milyen módon kereshetnek, hogyan kereshetik meg a felhasználókat, és hogyan láthatják az eredményeket a keresési webhelyeken.</span><span class="sxs-lookup"><span data-stu-id="77e7b-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="77e7b-104">A [keresési séma kezelése a SharePoint Online-ban](https://docs.microsoft.com/sharepoint/manage-search-schema) című témakörből megtudhatja, hogyan végezheti el a következőket:</span><span class="sxs-lookup"><span data-stu-id="77e7b-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="77e7b-105">Módosítsa a keresési sémát.</span><span class="sxs-lookup"><span data-stu-id="77e7b-105">Change the search schema.</span></span>
- <span data-ttu-id="77e7b-106">Felügyelt tulajdonságok létrehozása</span><span class="sxs-lookup"><span data-stu-id="77e7b-106">Create managed properties.</span></span>
- <span data-ttu-id="77e7b-107">Bejárt megfeleltetések megfeleltetése a felügyelt tulajdonságoknak.</span><span class="sxs-lookup"><span data-stu-id="77e7b-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="77e7b-108">Vegye figyelembe a keresési séma kezelését érintő lépéseket:</span><span class="sxs-lookup"><span data-stu-id="77e7b-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="77e7b-109">Ha olyan figyelmeztetés jelenik meg, amely jelzi, hogy az alkalmazás a séma módosításakor **szüneteltetve** van, akkor ez a funkció csak akkor ideiglenes, ha a szolgáltatás karbantartása bekövetkezik.</span><span class="sxs-lookup"><span data-stu-id="77e7b-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="77e7b-110">Ha több mint 24 óra telt el, és továbbra is tapasztalja a figyelmeztetést, kérjük, jelentkezzen be támogatási ügyben.</span><span class="sxs-lookup"><span data-stu-id="77e7b-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="77e7b-111">A felügyelt tulajdonságok módosítása vagy újak felvétele esetén a módosítások csak a tartalom újbóli bejárása után lépnek életbe.</span><span class="sxs-lookup"><span data-stu-id="77e7b-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="77e7b-112">A SharePoint Online-ban a bejárás automatikusan a meghatározott bejárási ütemterv alapján történik.</span><span class="sxs-lookup"><span data-stu-id="77e7b-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="77e7b-113">Ha meg szeretne győződni arról, hogy a módosítások bejárást kaptak, külön [kérheti a lista vagy tár ismételt indexelését](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) .</span><span class="sxs-lookup"><span data-stu-id="77e7b-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="77e7b-114">A keresési séma teljes áttekintését a [keresési séma bemutatása](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/) című témakörben találhatja meg.</span><span class="sxs-lookup"><span data-stu-id="77e7b-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


