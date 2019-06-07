---
title: Egy SharePoint-tárba hálózati meghajtó csatlakoztatása
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 7bb1f7d1b77ec5850109c9553ddfd894b3823946
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34754817"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="43055-102">Egy SharePoint-tárba hálózati meghajtó csatlakoztatása</span><span class="sxs-lookup"><span data-stu-id="43055-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="43055-103">A dokumentumtár hálózati meghajtóként leképezése szolgáltatás, ideiglenes, és csak az Internet Explorer böngészőn keresztül támogatott.</span><span class="sxs-lookup"><span data-stu-id="43055-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="43055-104">Esetenként az Internet Explorer programban nyissa meg a SharePoint-webhely és kell "aláírt tartózkodási" bejelölésével megakadályozhatja, hogy a munkamenet ne járjon le.</span><span class="sxs-lookup"><span data-stu-id="43055-104">You must occasionally open the SharePoint site in Internet Explorer and select "Stay signed in" to prevent the session from expiring.</span></span> <span data-ttu-id="43055-105">Ehelyett [Új ügyfél OneDrive szinkronizálása a SharePoint-fájlok szinkronizálása](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) </a> amely nyújt [Igény fájlokat](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span><span class="sxs-lookup"><span data-stu-id="43055-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="43055-106">OneDrive az összes fájl elérhető helyi tárolóhely használata nélkül.</span><span class="sxs-lookup"><span data-stu-id="43055-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="43055-107">Ha úgy dönt, hogy[az új OneDrive szinkronizálás ügyfél](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)helyett a meghajtókat, győződjön meg arról, hajtsa végre az alábbi cikkben.</span><span class="sxs-lookup"><span data-stu-id="43055-107">If you choose to map a drive instead of[using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="43055-108">**A csatlakoztatott hálózati meghajtók beállítása és hibaelhárítása**</span><span class="sxs-lookup"><span data-stu-id="43055-108">**How to configure and troubleshoot mapped network drives**</span></span>


- <span data-ttu-id="43055-109">[Konfigurálásához és hibaelhárításához csatlakoztatott hálózati meghajtók](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="43055-109">[Configure and to troubleshoot mapped network drives](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

<span data-ttu-id="43055-110">Megjegyzés: Az Internet Explorer 10 Windows 8 vagy a Windows 7, amely megjelenik a "Hozzáférés megtagadva" vagy "Elérési út nem érhető el." a meghajtó leképezésekor a gyorsjavítás telepítése a probléma megoldásához.</span><span class="sxs-lookup"><span data-stu-id="43055-110">NOTE:  For Internet Explorer 10 with Windows 8 or Windows 7 that receive "Access denied" or "Path is not accessible" when mapping a drive, install this hotfix to resolve this problem.</span></span> <span data-ttu-id="43055-111">[Nyissa meg a SharePoint-dokumentumtárhoz a Windows Intézőben, vagy rendeljen egy hálózati meghajtót a műsortárhoz, miután telepítette az Internet Explorer 10](https://support.microsoft.com/help/2846960)Ugrás.</span><span class="sxs-lookup"><span data-stu-id="43055-111">Go to [Error when you open a SharePoint Document Library in Windows Explorer or map a network drive to the library after you install Internet Explorer 10](https://support.microsoft.com/help/2846960).</span></span>
