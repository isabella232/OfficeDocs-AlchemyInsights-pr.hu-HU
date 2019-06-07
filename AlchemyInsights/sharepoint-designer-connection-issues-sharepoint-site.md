---
title: A SharePoint Online jogosultsági szintek
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760695"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="2482a-102">A SharePoint Designer kapcsolódási problémák</span><span class="sxs-lookup"><span data-stu-id="2482a-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="2482a-103">Ha SharePoint Designer SharePoint-webhelyekhez csatlakozási problémákat tapasztalja, kérjük próbálja meg a következő közös megoldásokat.</span><span class="sxs-lookup"><span data-stu-id="2482a-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="2482a-104">1. lépés: Ellenőrizze a SharePoint Designer frissül.</span><span class="sxs-lookup"><span data-stu-id="2482a-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="2482a-105">A SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="2482a-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="2482a-106">A SharePoint Designer Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="2482a-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="2482a-107">Frissítés a SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="2482a-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="2482a-108">2. lépés: A helyi gyorsítótárban található fájlok törlése</span><span class="sxs-lookup"><span data-stu-id="2482a-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="2482a-109">Zárja be a SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="2482a-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="2482a-110">A helyi számítógépen keresse meg a következő mappákban tárolt fájlok eltávolítása.</span><span class="sxs-lookup"><span data-stu-id="2482a-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="2482a-111">Kattintson a Start menü Futtatás és az egyes található összes fájl törlése az alábbi helyeken.</span><span class="sxs-lookup"><span data-stu-id="2482a-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="2482a-112">%APPDATA%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="2482a-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="2482a-113">Nyissa meg a SharePoint Designer 2013, és adja meg a fiók ismételten kattintva ellenőrizze, hogy az működik.</span><span class="sxs-lookup"><span data-stu-id="2482a-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="2482a-114">3. lépés: [a Modern Office 2013 eszköz a Windows-hitelesítés engedélyezése](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="2482a-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="2482a-115">4. lépés: A rendszergazdák kell egyéni parancsfájl engedélyezi a SharePoint Designer kapcsolat engedélyezésére.</span><span class="sxs-lookup"><span data-stu-id="2482a-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="2482a-116">Talál részletes leírást, példák és megfontolások [engedélyezése vagy tiltása egyéni parancsfájl](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="2482a-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


