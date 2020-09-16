---
title: A SharePoint Designer kapcsolódási problémái
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727173"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="86855-102">A SharePoint Designer kapcsolódási problémái</span><span class="sxs-lookup"><span data-stu-id="86855-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="86855-103">Ha a SharePoint Designer a SharePoint-webhelyek kapcsolódási problémáit tapasztalja, próbálkozzon az alábbi általános megoldásokkal.</span><span class="sxs-lookup"><span data-stu-id="86855-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="86855-104">1. lépés: Ellenőrizze, hogy a SharePoint Designer 2013 frissült-e a [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) szervizcsomaggal és a sharepoint Designer [2013 augusztus 2-2016 frissítéssel](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="86855-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="86855-105">Második lépés: a helyi gyorsítótár-fájlok törlése:</span><span class="sxs-lookup"><span data-stu-id="86855-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="86855-106">Zárja be a SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="86855-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="86855-107">A helyi számítógépen távolítsa el az összes olyan fájlt, amely az alábbi mappákban található.</span><span class="sxs-lookup"><span data-stu-id="86855-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="86855-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="86855-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="86855-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="86855-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="86855-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="86855-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="86855-111">Nyissa meg a SharePoint Designer 2013 alkalmazást, és adja meg ismét a fiókot, és ellenőrizze, hogy működik-e.</span><span class="sxs-lookup"><span data-stu-id="86855-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="86855-112">3. lépés: [a modern hitelesítés engedélyezése a Windows rendszerű eszközökön futó Office 2013](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)-ban.</span><span class="sxs-lookup"><span data-stu-id="86855-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="86855-113">4. lépés: a SharePoint Designer-kapcsolat engedélyezéséhez a rendszergazdáknak engedélyeznie kell az **egyéni parancsfájlokat** a SharePoint felügyeleti központ beállításaiban.</span><span class="sxs-lookup"><span data-stu-id="86855-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="86855-114">További információt az [egyéni parancsfájlok engedélyezése vagy letiltása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="86855-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


