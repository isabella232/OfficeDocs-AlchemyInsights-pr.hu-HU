---
title: Tartalom nem jelenik meg a SharePoint-találatok
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517033"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="ff1f2-102">Tartalom nem jelenik meg a SharePoint-találatok</span><span class="sxs-lookup"><span data-stu-id="ff1f2-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="ff1f2-103">Hajtsa végre az alábbi lépéseket, ha a várt tartalom nem jelenik meg a keresési eredmények között:</span><span class="sxs-lookup"><span data-stu-id="ff1f2-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="ff1f2-104">Ellenőrizze, hogy a várt tartalom tartalmazó **webhely** beállításai lehetővé teszik a tartalom jelenjen meg a keresési eredmények között.</span><span class="sxs-lookup"><span data-stu-id="ff1f2-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="ff1f2-105">Kövesse [a keresési eredmények között a webhely tartalmának megjelenítése](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="ff1f2-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="ff1f2-106">Ellenőrizze, hogy a **lista** vagy **dokumentumtár** , amely tartalmazza a várt tartalom beállításai lehetővé teszik a tartalom jelenjen meg a keresési eredmények között.</span><span class="sxs-lookup"><span data-stu-id="ff1f2-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="ff1f2-107">Kövesse a [listák vagy tárak a keresési eredmények között a tartalom megjelenítése](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="ff1f2-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="ff1f2-108">Ellenőrizze, hogy a lap, dokumentum vagy egyéni lap elrendezése is közzétételre kerülnek a **főverzió.**</span><span class="sxs-lookup"><span data-stu-id="ff1f2-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="ff1f2-109">Hajtsa végre a 3 a [Keresés nem ad vissza a SharePoint Online összes eredmény](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="ff1f2-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="ff1f2-110">Győződjön meg arról, hogy a felhasználó rendelkezik-e **engedéllyel** a tartalom megtekintését.</span><span class="sxs-lookup"><span data-stu-id="ff1f2-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="ff1f2-111">Kövesse a [SharePoint jogosultsági szintek ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="ff1f2-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="ff1f2-112">Ha a Keresés séma megváltozott, egy új felügyelt tulajdonság hozzáadása, felügyelt tulajdonság szerkesztése, vagy egy kezelt tulajdonságnak, majd a bejárás kérő eltávolításával és újraindexeli lesz szükség.</span><span class="sxs-lookup"><span data-stu-id="ff1f2-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="ff1f2-113">**Újraindexelni** a tartalmat [kézzel a bejárási és indexelési újra a hely, a tár vagy lista kérése](https://docs.microsoft.com/sharepoint/crawl-site-content)utasításait követve.</span><span class="sxs-lookup"><span data-stu-id="ff1f2-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="ff1f2-114">Ez lehet, hogy hosszabb ideig eltarthat, Várjon 24 órát az eredmények ismételt ellenőrzés előtt.</span><span class="sxs-lookup"><span data-stu-id="ff1f2-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="ff1f2-115">További tudnivalókért tanulmányozza [a helyszínen kell kereshető tartalom engedélyezése](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="ff1f2-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
