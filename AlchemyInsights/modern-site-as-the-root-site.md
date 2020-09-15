---
title: Modern webhely root-webhelyként
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666872"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="99cff-102">Modern webhely root-webhelyként</span><span class="sxs-lookup"><span data-stu-id="99cff-102">Modern site as root site</span></span>

<span data-ttu-id="99cff-103">Kezdtük egy új funkció kiépítését, amely lehetővé teszi, hogy a [klasszikus webhely gyökerét egy modern](https://docs.microsoft.com/sharepoint/modern-root-site)webhelyre cserélje.</span><span class="sxs-lookup"><span data-stu-id="99cff-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="99cff-104">A [SPOSiteSwap hivatkozhat](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) arra, hogy a webhely helyét egy másik webhelyre cseréli az eredeti webhely archiválása közben.</span><span class="sxs-lookup"><span data-stu-id="99cff-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="99cff-105">Mindkét csoportwebhely számára elérhető (nem kapcsolódhat egy csoporthoz) és egy kommunikációs webhelyhez.</span><span class="sxs-lookup"><span data-stu-id="99cff-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="99cff-106">A modern kommunikációs webhelyek létrehozásához ne törölje a klasszikus root-webhelyét.</span><span class="sxs-lookup"><span data-stu-id="99cff-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="99cff-107">Ezt a Microsoft nem támogatja.</span><span class="sxs-lookup"><span data-stu-id="99cff-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="99cff-108">A legfelső szintű webhely törlésekor a szervezet összes SharePoint-webhelye nem érhető el az összes felhasználó számára, amíg vissza nem állítja a webhelyet, illetve nem hozhat létre új webhelyet ugyanazon az URL-címen.</span><span class="sxs-lookup"><span data-stu-id="99cff-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="99cff-109">Ezt a funkciót az üzenetközpont segítségével fogjuk kommunikálni.</span><span class="sxs-lookup"><span data-stu-id="99cff-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="99cff-110">Várnia kell, hogy a funkció hamarosan be legyen kapcsolva a bérlői webhelyére.</span><span class="sxs-lookup"><span data-stu-id="99cff-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="99cff-111">A webhelyek cseréjével kapcsolatos ismert problémák</span><span class="sxs-lookup"><span data-stu-id="99cff-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="99cff-112">Előfordulhat, hogy a cél egy rövid időre "not found" (HTTP 404) hibát ad vissza.</span><span class="sxs-lookup"><span data-stu-id="99cff-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="99cff-113">A keresési index frissítéséhez a tartalmat újra kell bejárni.</span><span class="sxs-lookup"><span data-stu-id="99cff-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="99cff-114">Ebben az esetben nincs szükség kézi lépésre, ezt automatikusan elvégezheti.</span><span class="sxs-lookup"><span data-stu-id="99cff-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="99cff-115">A "statikus" hivatkozásokkal (például a fájlok szinkronizálására és a OneNote-fájlokra) függő bármit manuálisan kell kijavítani.</span><span class="sxs-lookup"><span data-stu-id="99cff-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="99cff-116">Előfordulhat, hogy a Project Server-webhelyek érvényesítése szükséges ahhoz, hogy a rendszer továbbra is megfelelően társítsa őket.</span><span class="sxs-lookup"><span data-stu-id="99cff-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
