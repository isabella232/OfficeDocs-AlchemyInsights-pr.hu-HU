---
title: Modern oldal, mint a gyökér hely
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713793"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="43866-102">Modern webhely gyökérhelyként</span><span class="sxs-lookup"><span data-stu-id="43866-102">Modern site as root site</span></span>

<span data-ttu-id="43866-103">Elkezdtünk egy új funkciót kivonni, amely lehetővé teszi, hogy [a klasszikus webhely gyökérwebhelyét egy modern webhelyre cserélje.](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="43866-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="43866-104">[Az Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) segítségével az eredeti webhely archiválása közben cserélheti fel a webhely helyét egy másik hellyel.</span><span class="sxs-lookup"><span data-stu-id="43866-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="43866-105">A csoportwebhelyhez (csoporthoz nem kapcsolódó) és a kommunikációs helyhez egyaránt elérhető.</span><span class="sxs-lookup"><span data-stu-id="43866-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="43866-106">Ne törölje a klasszikus gyökérwebhelyet, hogy modern kommunikációs webhelyet hozzon létre.</span><span class="sxs-lookup"><span data-stu-id="43866-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="43866-107">Ezt a Microsoft nem támogatja.</span><span class="sxs-lookup"><span data-stu-id="43866-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="43866-108">A gyökérwebhely törlésével a szervezet összes SharePoint-webhelye elérhetetlenné válik minden felhasználó számára, amíg vissza nem állítja a webhelyet, vagy nem hoz létre új webhelyet ugyanazon az URL-címen.</span><span class="sxs-lookup"><span data-stu-id="43866-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="43866-109">Ezt a funkciót az üzenetközponton keresztül fogjuk közlöm.</span><span class="sxs-lookup"><span data-stu-id="43866-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="43866-110">Azt kell várni, hogy a szolgáltatás be van kapcsolva a bérlő hamarosan.</span><span class="sxs-lookup"><span data-stu-id="43866-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="43866-111">Ismert problémák a webhelyek cseréjével kapcsolatban</span><span class="sxs-lookup"><span data-stu-id="43866-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="43866-112">A célwebhely rövid ideig "nem található" (HTTP 404) hibát adhat vissza.</span><span class="sxs-lookup"><span data-stu-id="43866-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="43866-113">A keresési index frissítéséhez a tartalmat újra kell feltérképezni.</span><span class="sxs-lookup"><span data-stu-id="43866-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="43866-114">Itt nincs szükség manuális lépésre, ez automatikusan megtörténik.</span><span class="sxs-lookup"><span data-stu-id="43866-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="43866-115">A "statikus" hivatkozásoktól (például a Fájlszinkronizálástól és a OneNote-fájloktól) függő minden hivatkozást manuálisan kell kijavítani.</span><span class="sxs-lookup"><span data-stu-id="43866-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="43866-116">Előfordulhat, hogy a Project kiszolgáló helyhelyeit ellenőrizni kell annak érdekében, hogy azok továbbra is megfelelően legyenek társítva.</span><span class="sxs-lookup"><span data-stu-id="43866-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
