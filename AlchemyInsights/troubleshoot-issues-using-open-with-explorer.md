---
title: Megnyitás Explorer használatával kapcsolatos problémák elhárítása
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 5be8a8f9f67939c7e2671855da259818269d9299
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293881"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="77470-102">Megnyitás Explorer problémáit</span><span class="sxs-lookup"><span data-stu-id="77470-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="77470-103">Dokumentumtár megnyitása a SharePoint- vagy OneDrive a **Megnyitás Intézővel** parancs használatával kapcsolatos gyakori problémák megoldásához:</span><span class="sxs-lookup"><span data-stu-id="77470-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="77470-p101">Használja az Internet Explorer 10 vagy 11 az Internet Explorer. **Megnyitás Intézővel** nem kompatibilis a Microsoft Edge, Google Chrome, Firefox és mások. **Megnyitás Intézővel** le van tiltva az Internet Explorer kivételével minden böngészőben.</span><span class="sxs-lookup"><span data-stu-id="77470-p101">Use Internet Explorer 10 or Internet Explorer 11. **Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others. **Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="77470-p102">**Megnyitás Intézővel** nem érhető el a SharePoint-tárak a modern élmény. **Az Intéző nézetben** használja. Jelölje ki a **Nézetbeállítások** \> **Intéző nézetben**. View fájl Explorer szoftvere nem kompatibilis a Microsoft Edge, Google Chrome, Firefox és mások. Az **Intéző nézetben** csak az Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="77470-p102">**Open with Explorer** is not available in the modern experience for SharePoint libraries. Use **View in File Explorer** instead. Select **View options** \> **View in File Explorer**. View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others. **View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="77470-p103">Ellenőrizze, hogy a WebClient szolgáltatást. A Windows Keresés mezőbe írja be a Futtatás jelölje be a Futtatás asztali alkalmazás, írja be a Services.msc parancsot, és nyomja le az ENTER billentyűt. Görgessen le a webes ügyfélszolgáltatást, és ellenőrizze, hogy az **állapot** oszlopában az "Fut". Ha nem, kattintson duplán a szolgáltatásra, kattintson a **Start**gombra, és kattintson az **OK gombra**. (Lehet, hogy szeretné engedélyezni a szolgáltatás **indítási típusa** mezőben a **kézi** vagy **automatikus** kiválasztásával.)</span><span class="sxs-lookup"><span data-stu-id="77470-p103">Make sure the WebClient service is running. In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter. Scroll down to the WebClient service and make sure the **Status** column displays "Running." If it doesn't, double-click the service, click **Start**, and then click **OK**. (You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="77470-p104">Könyvtár fájl Intéző megnyitása jól jöhet, ha meg szeretnénk másolni vagy áthelyezni, több fájlok és mappák után, de a könyvtárban rendszeresen használni kívánt, ajánlott szinkronizálása. Explorer fájl megnyitásával kapcsolatos problémák elhárítása, lásd: [Nyissa meg az Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Info: szinkronizálás beállítása [az új OneDrive szinkronizálás ügyfél fájlok szinkronizálása SharePoint](https://go.microsoft.com/fwlink/?linkid=871666)talál.</span><span class="sxs-lookup"><span data-stu-id="77470-p104">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it. To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="77470-120">Lásd a cikk [a "Megnyitás a Explorer" parancsot a problémák a SharePoint Online használatáról](https://support.office.com/en-us/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) további információt.</span><span class="sxs-lookup"><span data-stu-id="77470-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/en-us/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

