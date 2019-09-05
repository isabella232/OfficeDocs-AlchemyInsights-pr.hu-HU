---
title: Swap a Classic root oldalon egy modern site
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749262"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="c4e26-102">Swap a Classic root oldalon egy modern site</span><span class="sxs-lookup"><span data-stu-id="c4e26-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="c4e26-103">Ha a környezet beállítása április 2019 előtt történt, akkor a Microsoft PowerShell eszközzel megváltoztathatja a gyökérwebhelyet egy modern webhelyre:</span><span class="sxs-lookup"><span data-stu-id="c4e26-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="c4e26-104">Ha más webhely van, amelyet gyökérwebhelyként kíván használni, kicserélheti [a gyökérwebhelyet](https://docs.microsoft.com/sharepoint/modern-root-site) vele.</span><span class="sxs-lookup"><span data-stu-id="c4e26-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="c4e26-105">Az [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) használata segítségével kicserélheti egy webhely helyét egy másik webhelyre az eredeti webhely archiválása közben.</span><span class="sxs-lookup"><span data-stu-id="c4e26-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="c4e26-106">Elérhető mindkét csoportwebhelyhez (nem kapcsolódik csoporthoz) és kommunikációs webhelyhez.</span><span class="sxs-lookup"><span data-stu-id="c4e26-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="c4e26-107">A további képességek hamarosan bevezetésre kerülnek, amely lehetővé teszi, hogy folyamatosan használja a tartalmat az oldalon, de átalakítani a meglévő webhely kommunikációs site.</span><span class="sxs-lookup"><span data-stu-id="c4e26-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="c4e26-108">Ezek képességek lesz összecsavart ki fokozatosan.</span><span class="sxs-lookup"><span data-stu-id="c4e26-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="c4e26-109">A frissítésekért folytassa az Office 365 Message Center ellenőrzését.</span><span class="sxs-lookup"><span data-stu-id="c4e26-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="c4e26-110">A helyek swapping ismert problémái</span><span class="sxs-lookup"><span data-stu-id="c4e26-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="c4e26-111">A célwebhely rövid ideig "nem található" (HTTP 404) hibát ad vissza.</span><span class="sxs-lookup"><span data-stu-id="c4e26-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="c4e26-112">A keresési index frissítéséhez a tartalmat recrawled kell.</span><span class="sxs-lookup"><span data-stu-id="c4e26-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="c4e26-113">Manuális lépésekre nincs szükség-ezt automatikusan elvégzi.</span><span class="sxs-lookup"><span data-stu-id="c4e26-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="c4e26-114">A "statikus" hivatkozásokra (például a fájlszinkronizálás és a OneNote-fájlok) vonatkozó bármit manuálisan kell javítani.</span><span class="sxs-lookup"><span data-stu-id="c4e26-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="c4e26-115">Ha a forráswebhely egy szervezeti hírwebhely volt, frissítse az URL-címet.</span><span class="sxs-lookup"><span data-stu-id="c4e26-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="c4e26-116">Kap egy listát az összes szervezeti híroldalak.</span><span class="sxs-lookup"><span data-stu-id="c4e26-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="c4e26-117">Előfordulhat, hogy a Project Server webhelyeit érvényesíteni kell annak érdekében, hogy még mindig helyesen legyenek társítva.</span><span class="sxs-lookup"><span data-stu-id="c4e26-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





