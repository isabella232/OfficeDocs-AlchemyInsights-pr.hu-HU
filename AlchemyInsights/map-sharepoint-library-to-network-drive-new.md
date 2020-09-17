---
title: SharePoint-tár megfeleltetése hálózati meghajtóként
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
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 9115a3ab8d1234127a95628a9a49679ef06f6d39
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806185"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="81997-102">SharePoint-tár megfeleltetése hálózati meghajtóként</span><span class="sxs-lookup"><span data-stu-id="81997-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="81997-103">A tárak hálózati meghajtóként való megfeleltetése ideiglenes, és csak az Internet Explorerben támogatott.</span><span class="sxs-lookup"><span data-stu-id="81997-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="81997-104">Alkalmanként meg kell nyitnia a SharePoint-webhelyet az Internet Explorerben, és a bejelentkezett marad lehetőséget választva megakadályozhatja, hogy a munkamenet **lemaradjon** .</span><span class="sxs-lookup"><span data-stu-id="81997-104">You must occasionally open the SharePoint site in Internet Explorer and select **Stay signed in** to prevent the session from expiring.</span></span> <span data-ttu-id="81997-105">Ehelyett [szinkronizálja a SharePoint-fájlokat az új OneDrive szinkronizálási ügyfélprogrammal](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) , </a> amely [igény szerinti fájlokat](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)biztosít.</span><span class="sxs-lookup"><span data-stu-id="81997-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="81997-106">A OneDrive-on lévő összes fájl eléréséhez helyi tárterület használata nélkül.</span><span class="sxs-lookup"><span data-stu-id="81997-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="81997-107">Ha úgy dönt, hogy [az új OneDrive szinkronizálási ügyfélalkalmazás](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)helyett egy meghajtót rendel, gondoskodjon arról, hogy kövesse az alábbi cikk lépéseit.</span><span class="sxs-lookup"><span data-stu-id="81997-107">If you choose to map a drive instead of [using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="81997-108">**A megfeleltetett hálózati meghajtók beállítása és hibaelhárítása**</span><span class="sxs-lookup"><span data-stu-id="81997-108">**How to configure and troubleshoot mapped network drives**</span></span>


<span data-ttu-id="81997-109">Lásd: [a SharePoint Online-hoz kapcsolódó csatlakoztatott hálózati meghajtók hibaelhárítása](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="81997-109">See [Troubleshoot mapped network drives that connect to SharePoint Onlines](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>

<span data-ttu-id="81997-110">Megjegyzés: Ha Windows 8 vagy Windows 7 rendszerű Internet Explorer 10 böngészőt használ, és a **hozzáférés megtagadva** vagy **az elérési út nem érhető** el egy meghajtó hozzárendelésekor, telepítse [ezt a gyorsjavítást](https://support.microsoft.com/help/2846960) a probléma megoldásához.</span><span class="sxs-lookup"><span data-stu-id="81997-110">NOTE:  If you use Internet Explorer 10 with Windows 8 or Windows 7, and receive **Access denied** or **Path is not accessible** when mapping a drive, install [this hotfix](https://support.microsoft.com/help/2846960) to resolve this problem.</span></span> 
