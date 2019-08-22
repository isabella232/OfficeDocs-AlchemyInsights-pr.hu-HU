---
title: A klasszikus Modern webhely legfelső szintű webhely felcserélése
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
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501081"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="2646c-102">A klasszikus Modern webhely legfelső szintű webhely felcserélése</span><span class="sxs-lookup"><span data-stu-id="2646c-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="2646c-103">A környezet április 2019 előtt hozták létre, ha a Microsoft PowerShell használatával módosíthatja a legfelső szintű webhely modern webhely:</span><span class="sxs-lookup"><span data-stu-id="2646c-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="2646c-104">Ha a legfelső szintű webhely használni kívánt másik helyre, (swap) a legfelső szintű webhely cserélheti vele.</span><span class="sxs-lookup"><span data-stu-id="2646c-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="2646c-105">[Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) segítségével felcserélése egy másik webhelyet a webhely helyét az eredeti helyre archiválás során.</span><span class="sxs-lookup"><span data-stu-id="2646c-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="2646c-106">A csoportwebhely (nem kapcsolódik egy csoport) és a kommunikációs hely áll rendelkezésre.</span><span class="sxs-lookup"><span data-stu-id="2646c-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="2646c-107">További lehetőségeket fogják bevezetni legrövidebb időn belül, amely lehetővé teszi a tovább használni a tartalmat a webhelyen, de a meglévő webhely átalakítása kommunikációs hely.</span><span class="sxs-lookup"><span data-stu-id="2646c-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="2646c-108">Ezek a funkciók lesznek-e vetítve fokozatosan.</span><span class="sxs-lookup"><span data-stu-id="2646c-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="2646c-109">Továbbra is az Office 365 Message Center frissítések ellenőrzése.</span><span class="sxs-lookup"><span data-stu-id="2646c-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="2646c-110">Csere helyek kapcsolatos ismert problémák</span><span class="sxs-lookup"><span data-stu-id="2646c-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="2646c-111">A célwebhely vissza "nem található" hiba (HTTP 404) egy rövid ideig.</span><span class="sxs-lookup"><span data-stu-id="2646c-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="2646c-112">Tartalom kell frissíteni a keresési indexben kell recrawled.</span><span class="sxs-lookup"><span data-stu-id="2646c-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="2646c-113">Nincs szükség kézi lépés van – ez automatikusan történik.</span><span class="sxs-lookup"><span data-stu-id="2646c-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="2646c-114">Semmit sem függ a "statikus" hivatkozások (például fájlszinkronizálás és a OneNote-fájlok) manuálisan kell javítani kell.</span><span class="sxs-lookup"><span data-stu-id="2646c-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="2646c-115">Ha a forráswebhely egy szervezeti híreket tartalmazó webhely volt, az URL-cím frissítése</span><span class="sxs-lookup"><span data-stu-id="2646c-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="2646c-116">Szervezeti hírcsoporthelyek listájának megjelenítése.</span><span class="sxs-lookup"><span data-stu-id="2646c-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="2646c-117">A Project Server-webhelyek kell annak biztosítása érdekében, hogy még az társított érvényesíthető.</span><span class="sxs-lookup"><span data-stu-id="2646c-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





