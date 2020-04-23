---
title: A klasszikus gyökérwebhely felcserélése egy modern webhelyre
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741546"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="dc314-102">A klasszikus gyökérwebhely felcserélése egy modern webhelyre</span><span class="sxs-lookup"><span data-stu-id="dc314-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="dc314-103">Ha a környezet 2019 áprilisa előtt lett beállítva, a Microsoft PowerShell használatával modern webhelyre módosíthatja a gyökérwebhelyet:</span><span class="sxs-lookup"><span data-stu-id="dc314-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="dc314-104">Ha van egy másik webhely, amelyet gyökérwebhelyként szeretne használni, lecserélheti [(cserélheti) a gyökérwebhelyet.](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="dc314-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="dc314-105">[Az Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) segítségével az eredeti webhely archiválása közben cserélheti fel a webhely helyét egy másik hellyel.</span><span class="sxs-lookup"><span data-stu-id="dc314-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="dc314-106">A csoportwebhelyhez (csoporthoz nem kapcsolódó) és a kommunikációs helyhez egyaránt elérhető.</span><span class="sxs-lookup"><span data-stu-id="dc314-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="dc314-107">Hamarosan további képességek kerülnek bevezetésre, amelyek lehetővé teszik a webhely tartalmának további használatát, de a meglévő webhelyet kommunikációs webhelyre konvertálhatja.</span><span class="sxs-lookup"><span data-stu-id="dc314-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="dc314-108">Ezek a képességek fokozatosan kerülnek bevezetésre.</span><span class="sxs-lookup"><span data-stu-id="dc314-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="dc314-109">Folytassa a frissítéseket az Üzenetközpontban.</span><span class="sxs-lookup"><span data-stu-id="dc314-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="dc314-110">Ismert problémák a webhelyek cseréjével kapcsolatban</span><span class="sxs-lookup"><span data-stu-id="dc314-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="dc314-111">A célwebhely rövid ideig "nem található" (HTTP 404) hibát adhat vissza.</span><span class="sxs-lookup"><span data-stu-id="dc314-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="dc314-112">A keresési index frissítéséhez a tartalmat újra kell feltérképezni.</span><span class="sxs-lookup"><span data-stu-id="dc314-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="dc314-113">Nincs szükség manuális lépésre - ez automatikusan történik.</span><span class="sxs-lookup"><span data-stu-id="dc314-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="dc314-114">A "statikus" hivatkozásoktól (például a Fájlszinkronizálástól és a OneNote-fájloktól) függő minden hivatkozást manuálisan kell kijavítani.</span><span class="sxs-lookup"><span data-stu-id="dc314-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="dc314-115">Ha a forráswebhely szervezeti hírwebhely volt, frissítse az URL-címet.</span><span class="sxs-lookup"><span data-stu-id="dc314-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="dc314-116">Az összes szervezeti híroldal listájának beszereznie.</span><span class="sxs-lookup"><span data-stu-id="dc314-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="dc314-117">Előfordulhat, hogy a Project kiszolgáló helyhelyeit ellenőrizni kell annak érdekében, hogy azok továbbra is megfelelően legyenek társítva.</span><span class="sxs-lookup"><span data-stu-id="dc314-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
