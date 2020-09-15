---
title: Nem jelenik meg a tartalom a SharePoint keresési eredményei között
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713132"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="ef01f-102">Nem jelenik meg a tartalom a SharePoint keresési eredményei között</span><span class="sxs-lookup"><span data-stu-id="ef01f-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="ef01f-103">Kövesse ezeket a hibaelhárítási lépéseket, ha a várt tartalom nem jelenik meg a keresési eredmények között:</span><span class="sxs-lookup"><span data-stu-id="ef01f-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="ef01f-104">Ellenőrizze, hogy a várt tartalmat tartalmazó **webhely** be van-e állítva a tartalom keresési eredményekben való megjelenítésére.</span><span class="sxs-lookup"><span data-stu-id="ef01f-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="ef01f-105">Kövesse a [webhely tartalmának megjelenítése a keresési eredményekben](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)című témakör lépéseit.</span><span class="sxs-lookup"><span data-stu-id="ef01f-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="ef01f-106">Ellenőrizze, hogy a várt tartalmat tartalmazó **lista** vagy **tár** van-e beállítva, hogy a tartalom a találatok között jelenjen meg.</span><span class="sxs-lookup"><span data-stu-id="ef01f-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="ef01f-107">Kövesse a [találatok között a listák vagy tárak tartalmának megjelenítése](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)című témakör lépéseit.</span><span class="sxs-lookup"><span data-stu-id="ef01f-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="ef01f-108">Ellenőrizze, hogy a lap, a dokumentum vagy az egyéni lapelrendezés megjelenik-e **fő verzióként.**</span><span class="sxs-lookup"><span data-stu-id="ef01f-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="ef01f-109">Kövesse a 3. lépés a [találatok között a SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525)-ban című témakört.</span><span class="sxs-lookup"><span data-stu-id="ef01f-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="ef01f-110">Ellenőrizze, hogy a felhasználó rendelkezik-e **engedélyekkel** a tartalom megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="ef01f-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="ef01f-111">Kövesse a [SharePoint jogosultsági szintjeinek ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels)című témakör lépéseit.</span><span class="sxs-lookup"><span data-stu-id="ef01f-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="ef01f-112">Ha a keresési sémát egy új felügyelt tulajdonság hozzáadásával módosította, a felügyelt tulajdonság szerkesztésével vagy egy felügyelt tulajdonság eltávolításával, majd a bejárási és újraindexelési kéréssel szükséges.</span><span class="sxs-lookup"><span data-stu-id="ef01f-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="ef01f-113">**A tartalom újraindexeléséhez** kövesse a [webhely, tár vagy lista bejárásának vagy újraindexelésének manuális kérése című szakasz](https://docs.microsoft.com/sharepoint/crawl-site-content)lépéseit.</span><span class="sxs-lookup"><span data-stu-id="ef01f-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="ef01f-114">Ez eltarthat egy darabig, várjon 24 órát, mielőtt ismét ellenőrizni fogja az eredményeket.</span><span class="sxs-lookup"><span data-stu-id="ef01f-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="ef01f-115">További tudnivalókat a [webhelyen kereshető tartalmak engedélyezése](https://docs.microsoft.com/sharepoint/make-site-content-searchable)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="ef01f-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
