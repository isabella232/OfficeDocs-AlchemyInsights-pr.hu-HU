---
title: A SharePoint Designer kapcsolódási problémák
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508425"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="ce1c1-102">A SharePoint Designer kapcsolódási problémák</span><span class="sxs-lookup"><span data-stu-id="ce1c1-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="ce1c1-103">Ha a SharePoint Designer SharePoint-webhelyekhez csatlakozási problémákat tapasztalja, próbálkozzon a következő közös megoldásokat.</span><span class="sxs-lookup"><span data-stu-id="ce1c1-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="ce1c1-104">1. lépés: Ellenőrizze, hogy a SharePoint Designer 2013 frissül [a SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) és a [2016. augusztus 2. frissítés a SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="ce1c1-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="ce1c1-105">2. lépés: A helyi gyorsítótárban található fájlok törlése:</span><span class="sxs-lookup"><span data-stu-id="ce1c1-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="ce1c1-106">Zárja be a SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="ce1c1-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="ce1c1-107">A helyi számítógépen a következő mappákban található összes fájl eltávolításához.</span><span class="sxs-lookup"><span data-stu-id="ce1c1-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="ce1c1-108">%APPDATA%\Microsoft\Web server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="ce1c1-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="ce1c1-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="ce1c1-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="ce1c1-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="ce1c1-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="ce1c1-111">Nyissa meg a SharePoint Designer 2013, és adja meg a fiók ismételten kattintva ellenőrizze, hogy az működik.</span><span class="sxs-lookup"><span data-stu-id="ce1c1-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="ce1c1-112">3. lépés: a [Modern Office 2013 eszköz a Windows-hitelesítés engedélyezése](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="ce1c1-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="ce1c1-113">4. lépés: Rendszergazdák kell **Egyéni parancsfájl engedélyezi** a SharePoint felügyeleti központ beállításaiban a SharePoint Designer kapcsolat engedélyezésére.</span><span class="sxs-lookup"><span data-stu-id="ce1c1-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="ce1c1-114">Lásd a [engedélyezése vagy tiltása egyéni parancsfájl](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) további információt.</span><span class="sxs-lookup"><span data-stu-id="ce1c1-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


