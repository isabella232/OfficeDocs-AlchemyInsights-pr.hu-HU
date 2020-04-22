---
title: A tartalom nem jelenik meg a SharePoint keresési eredményei között
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705663"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="64d49-102">A tartalom nem jelenik meg a SharePoint keresési eredményei között</span><span class="sxs-lookup"><span data-stu-id="64d49-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="64d49-103">Kövesse az alábbi hibaelhárítási lépéseket, ha a várt tartalom nem jelenik meg a keresési eredmények között:</span><span class="sxs-lookup"><span data-stu-id="64d49-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="64d49-104">Ellenőrizze, hogy a várt tartalmat tartalmazó **webhely** úgy van-e beállítva, hogy a tartalom megjelenjen a keresési eredmények között.</span><span class="sxs-lookup"><span data-stu-id="64d49-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="64d49-105">Kövesse a [Tartalom megjelenítése a webhelyen](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)a keresési eredmények között című részben leírt lépéseket.</span><span class="sxs-lookup"><span data-stu-id="64d49-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="64d49-106">Ellenőrizze, hogy a várt tartalmat tartalmazó **lista** vagy **tár** úgy van-e beállítva, hogy a tartalom megjelenjen a keresési eredmények között.</span><span class="sxs-lookup"><span data-stu-id="64d49-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="64d49-107">Kövesse a [Tartalom megjelenítése listákból vagy tárakból](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)a keresési eredmények között című részben leírt lépéseket.</span><span class="sxs-lookup"><span data-stu-id="64d49-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="64d49-108">Ellenőrizze, hogy az oldal, a dokumentum vagy az egyéni lapelrendezés **főverzióként van-e közzétéve.**</span><span class="sxs-lookup"><span data-stu-id="64d49-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="64d49-109">Kövesse a [Keresés](https://go.microsoft.com/fwlink/?linkid=874525)3.</span><span class="sxs-lookup"><span data-stu-id="64d49-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="64d49-110">Ellenőrizze, hogy a felhasználó **rendelkezik-e engedéllyel** a tartalom megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="64d49-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="64d49-111">Kövesse a [SharePoint engedélyszintek ismertsék el ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels)című témakör lépéseit.</span><span class="sxs-lookup"><span data-stu-id="64d49-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="64d49-112">Ha a keresési sémát új felügyelt tulajdonság hozzáadásával, felügyelt tulajdonság szerkesztésével vagy egy felügyelt tulajdonság eltávolításával módosították, akkor bejárást és újraindexelést kell kérnie.</span><span class="sxs-lookup"><span data-stu-id="64d49-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="64d49-113">A tartalom **újbóli indexelése** a [Webhely, tár vagy lista bejárásának és újraindexelésének kézi kérése című lépéslépéseit követve.](https://docs.microsoft.com/sharepoint/crawl-site-content)</span><span class="sxs-lookup"><span data-stu-id="64d49-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="64d49-114">Ez eltarthat egy ideig, várjon 24 órát, mielőtt újra ellenőrizné az eredményeket.</span><span class="sxs-lookup"><span data-stu-id="64d49-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="64d49-115">További információt a Tartalom keresése a webhelyen című [témakörben talál.](https://docs.microsoft.com/sharepoint/make-site-content-searchable)</span><span class="sxs-lookup"><span data-stu-id="64d49-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
