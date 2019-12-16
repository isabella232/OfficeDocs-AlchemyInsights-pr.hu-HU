---
title: SharePoint Designer-csatlakozási problémák
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051715"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="c2f80-102">SharePoint Designer-csatlakozási problémák</span><span class="sxs-lookup"><span data-stu-id="c2f80-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="c2f80-103">Ha a SharePoint Designer kapcsolódási problémákat tapasztal a SharePoint-webhelyeken, próbálja meg a következő közös megoldásokat.</span><span class="sxs-lookup"><span data-stu-id="c2f80-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="c2f80-104">1. lépés: Ellenőrizze, hogy a SharePoint Designer 2013 a [SharePoint Designer Service Pack 1 csomaggal](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) frissítve van-e és az [augusztusi 2, 2016 a SharePoint Designer 2013 frissítés](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="c2f80-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="c2f80-105">2. lépés: a helyi gyorsítótárfájlok törlése:</span><span class="sxs-lookup"><span data-stu-id="c2f80-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="c2f80-106">Zárja be a SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="c2f80-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="c2f80-107">A helyi számítógépen távolítsa el a következő mappákban található fájlokat.</span><span class="sxs-lookup"><span data-stu-id="c2f80-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="c2f80-108">%APPDATA%\Microsoft\Web szolgál Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="c2f80-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="c2f80-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="c2f80-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="c2f80-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="c2f80-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="c2f80-111">Nyit SharePoint Tervező 2013 és belép a számla újra-hoz lát ha ez szerkezet.</span><span class="sxs-lookup"><span data-stu-id="c2f80-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="c2f80-112">Lép 3: [képessé tesz korszerű hitelesítés részére hivatal 2013-ra Windows berendezés](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="c2f80-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="c2f80-113">4. lépés: a rendszergazdáknak engedélyezni kell az **egyéni parancsfájl** beállítást a SharePoint Admin Center beállításaiban a SharePoint Designer-kapcsolat engedélyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="c2f80-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="c2f80-114">További információt az [egyéni parancsfájl engedélyezése vagy tiltása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="c2f80-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


