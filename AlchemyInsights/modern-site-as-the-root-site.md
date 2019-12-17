---
title: A modern weboldal a gyökérwebhely
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054704"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="35be1-102">A modern weboldal mint Gyökéroldal</span><span class="sxs-lookup"><span data-stu-id="35be1-102">Modern site as root site</span></span>

<span data-ttu-id="35be1-103">Megkezdtük a kínálatból egy új funkció, amely lehetővé teszi, hogy a [swap a klasszikus webhely gyökere egy modern oldalon](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="35be1-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="35be1-104">Az [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) használata segítségével kicserélheti egy webhely helyét egy másik webhelyre az eredeti webhely archiválása közben.</span><span class="sxs-lookup"><span data-stu-id="35be1-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="35be1-105">Elérhető mindkét csoportwebhelyhez (nem kapcsolódik csoporthoz) és kommunikációs webhelyhez.</span><span class="sxs-lookup"><span data-stu-id="35be1-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="35be1-106">A klasszikus gyökérwebhelyet ne törölje, hogy modern kommunikációs webhelyet hozzon létre.</span><span class="sxs-lookup"><span data-stu-id="35be1-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="35be1-107">Ezt a Microsoft nem támogatja.</span><span class="sxs-lookup"><span data-stu-id="35be1-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="35be1-108">A gyökérwebhely törlésével minden felhasználó számára hozzáférhetetlenné válik a szervezet összes SharePoint-webhelye, amíg vissza nem állítja a webhelyet, vagy ha ugyanazon az URL-címen új webhelyet hoz létre.</span><span class="sxs-lookup"><span data-stu-id="35be1-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="35be1-109">Mi lesz kommunikálni ezt a funkciót keresztül az üzenetközpont.</span><span class="sxs-lookup"><span data-stu-id="35be1-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="35be1-110">A szolgáltatás hamarosan bekapcsolódik a bérlőbe.</span><span class="sxs-lookup"><span data-stu-id="35be1-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="35be1-111">A helyek swapping ismert problémái</span><span class="sxs-lookup"><span data-stu-id="35be1-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="35be1-112">A célwebhely rövid ideig "nem található" (HTTP 404) hibát ad vissza.</span><span class="sxs-lookup"><span data-stu-id="35be1-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="35be1-113">A keresési index frissítéséhez a tartalmat recrawled kell.</span><span class="sxs-lookup"><span data-stu-id="35be1-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="35be1-114">Nincs kézi lépés szükséges itt, ez automatikusan megtörténik.</span><span class="sxs-lookup"><span data-stu-id="35be1-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="35be1-115">A "statikus" hivatkozásokra (például a fájlszinkronizálás és a OneNote-fájlok) vonatkozó bármit manuálisan kell javítani.</span><span class="sxs-lookup"><span data-stu-id="35be1-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="35be1-116">Előfordulhat, hogy a Project Server webhelyeit érvényesíteni kell annak érdekében, hogy még mindig helyesen legyenek társítva.</span><span class="sxs-lookup"><span data-stu-id="35be1-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
