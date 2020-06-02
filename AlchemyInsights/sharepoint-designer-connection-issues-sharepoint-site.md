---
title: A SharePoint Designer csatlakozási problémái
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
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511546"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="96d76-102">A SharePoint Designer csatlakozási problémái</span><span class="sxs-lookup"><span data-stu-id="96d76-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="96d76-103">Ha a SharePoint Designer kapcsolattal kapcsolatos problémákat tapasztal a SharePoint-webhelyekkel, próbálkozzon az alábbi gyakori megoldásokkal.</span><span class="sxs-lookup"><span data-stu-id="96d76-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="96d76-104">1. lépés: Ellenőrizze, hogy a SharePoint Designer 2013 frissítve van-e a [SharePoint Designer Service Pack 1 szervizcsomaggal](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) és a [2016.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)</span><span class="sxs-lookup"><span data-stu-id="96d76-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="96d76-105">2. lépés: A helyi gyorsítótárfájlok törlése:</span><span class="sxs-lookup"><span data-stu-id="96d76-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="96d76-106">Zárja be a SharePoint Designer 2013-at.</span><span class="sxs-lookup"><span data-stu-id="96d76-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="96d76-107">A helyi számítógépen távolítsa el az alábbi mappákban található összes fájlt.</span><span class="sxs-lookup"><span data-stu-id="96d76-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="96d76-108">%APPDATA%\Microsoft\Webkiszolgáló-bővítmények\Gyorsítótár</span><span class="sxs-lookup"><span data-stu-id="96d76-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="96d76-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="96d76-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="96d76-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="96d76-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="96d76-111">Nyissa meg a SharePoint Designer 2013-at, és írja be újra a fiókot, és nézze meg, hogy működik-e.</span><span class="sxs-lookup"><span data-stu-id="96d76-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="96d76-112">3. lépés: [Modern hitelesítés engedélyezése az Office 2013-hoz Windows-eszközökön](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="96d76-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="96d76-113">4. lépés: A SharePoint Designer-kapcsolat engedélyezéséhez a Rendszergazdák nak engedélyeznie kell az **egyéni parancsfájlt** a SharePoint Felügyeleti központ beállításaiban.</span><span class="sxs-lookup"><span data-stu-id="96d76-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="96d76-114">További információt az [Egyéni parancsfájl engedélyezése vagy lehetővé tévő engedélyezése](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="96d76-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


