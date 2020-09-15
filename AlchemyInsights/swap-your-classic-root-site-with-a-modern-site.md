---
title: A klasszikus root webhely cseréje modern webhellyel
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691181"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="38a58-102">A klasszikus root webhely cseréje modern webhellyel</span><span class="sxs-lookup"><span data-stu-id="38a58-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="38a58-103">Ha a környezete az 2019 áprilisa előtt volt beállítva, a Microsoft PowerShell segítségével módosíthatja a legfelső szintű webhelyet a modern webhelyekhez:</span><span class="sxs-lookup"><span data-stu-id="38a58-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="38a58-104">Ha egy másik webhelyet szeretne használni a legfelső szintű webhelyként, lecserélheti [(felcserélheti) a legfelső szintű webhelyét](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="38a58-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="38a58-105">A [SPOSiteSwap hivatkozhat](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) arra, hogy a webhely helyét egy másik webhelyre cseréli az eredeti webhely archiválása közben.</span><span class="sxs-lookup"><span data-stu-id="38a58-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="38a58-106">Mindkét csoportwebhely számára elérhető (nem kapcsolódhat egy csoporthoz) és egy kommunikációs webhelyhez.</span><span class="sxs-lookup"><span data-stu-id="38a58-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="38a58-107">A további lehetőségeket hamarosan bevezetjük, amelyek lehetővé teszik a webhely tartalmának használatát, de a meglévő webhelyet konvertálja egy kommunikációs webhelyre.</span><span class="sxs-lookup"><span data-stu-id="38a58-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="38a58-108">Ezek a funkciók fokozatosan jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="38a58-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="38a58-109">Továbbra is ellenőrizze az üzenetközpont frissítéseit.</span><span class="sxs-lookup"><span data-stu-id="38a58-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="38a58-110">A webhelyek cseréjével kapcsolatos ismert problémák</span><span class="sxs-lookup"><span data-stu-id="38a58-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="38a58-111">Előfordulhat, hogy a cél egy rövid időre "not found" (HTTP 404) hibát ad vissza.</span><span class="sxs-lookup"><span data-stu-id="38a58-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="38a58-112">A keresési index frissítéséhez a tartalmat újra kell bejárni.</span><span class="sxs-lookup"><span data-stu-id="38a58-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="38a58-113">Nincs szükség kézi lépésre – ezt automatikusan elvégzi a program.</span><span class="sxs-lookup"><span data-stu-id="38a58-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="38a58-114">A "statikus" hivatkozásokkal (például a fájlok szinkronizálására és a OneNote-fájlokra) függő bármit manuálisan kell kijavítani.</span><span class="sxs-lookup"><span data-stu-id="38a58-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="38a58-115">Ha a forrás webhelye szervezeti hírkiszolgáló volt, frissítse az URL-címet.</span><span class="sxs-lookup"><span data-stu-id="38a58-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="38a58-116">Az összes szervezeti híroldalak listájának beszerzése.</span><span class="sxs-lookup"><span data-stu-id="38a58-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="38a58-117">Előfordulhat, hogy a Project Server-webhelyek érvényesítése szükséges ahhoz, hogy a rendszer továbbra is megfelelően társítsa őket.</span><span class="sxs-lookup"><span data-stu-id="38a58-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
