---
title: A modern webhelyre, ahol a legfelső szintű webhely
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232717"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="e49b6-102">A modern webhelyre, ahol a legfelső szintű webhely</span><span class="sxs-lookup"><span data-stu-id="e49b6-102">Modern site as root site</span></span>

<span data-ttu-id="e49b6-103">Ezért megkezdődött, bevezetés egy új szolgáltatás, amely lehetővé teszi, hogy a klasszikus webhely legfelső szintű webhely modern hellyel felcserélése.</span><span class="sxs-lookup"><span data-stu-id="e49b6-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="e49b6-104">[Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) segítségével felcserélése egy másik webhelyet a webhely helyét az eredeti helyre archiválás során.</span><span class="sxs-lookup"><span data-stu-id="e49b6-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="e49b6-105">A csoportwebhely (nem kapcsolódik egy csoport) és a kommunikációs hely áll rendelkezésre.</span><span class="sxs-lookup"><span data-stu-id="e49b6-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="e49b6-106">Ne törölje a klasszikus legfelső szintű webhely a modern kommunikációs webhelyet hozhat létre.</span><span class="sxs-lookup"><span data-stu-id="e49b6-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="e49b6-107">Ez a Microsoft által nem támogatott.</span><span class="sxs-lookup"><span data-stu-id="e49b6-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="e49b6-108">A legfelső szintű webhely törlése tesz minden SharePoint-webhely a szervezet nem érhető el minden felhasználó számára addig, amíg a webhely visszaállítása, vagy hozzon létre egy új helyet azonos URL-címen.</span><span class="sxs-lookup"><span data-stu-id="e49b6-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="e49b6-109">Fogja azt közlő üzenet közepén keresztül ezt a szolgáltatást.</span><span class="sxs-lookup"><span data-stu-id="e49b6-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="e49b6-110">A funkció segítségével kapcsolható be a bérlő röviddel számíthatunk.</span><span class="sxs-lookup"><span data-stu-id="e49b6-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="e49b6-111">Csere helyek kapcsolatos ismert problémák</span><span class="sxs-lookup"><span data-stu-id="e49b6-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="e49b6-112">A célwebhely vissza "nem található" hiba (HTTP 404) egy rövid ideig.</span><span class="sxs-lookup"><span data-stu-id="e49b6-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="e49b6-113">Tartalom kell frissíteni a keresési indexben kell recrawled.</span><span class="sxs-lookup"><span data-stu-id="e49b6-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="e49b6-114">Nem szükséges itt kézi művelet van, ez automatikusan megtörténik.</span><span class="sxs-lookup"><span data-stu-id="e49b6-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="e49b6-115">Semmit sem függ a "statikus" hivatkozások (például fájlszinkronizálás és a OneNote-fájlok) manuálisan kell javítani kell.</span><span class="sxs-lookup"><span data-stu-id="e49b6-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="e49b6-116">A Project Server-webhelyek kell annak biztosítása érdekében, hogy még az társított érvényesíthető.</span><span class="sxs-lookup"><span data-stu-id="e49b6-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
