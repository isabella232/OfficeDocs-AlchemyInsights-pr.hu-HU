---
title: Megnyitás Explorer nem működik
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293065"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="c3b39-102">Megnyitás Explorer nem működik</span><span class="sxs-lookup"><span data-stu-id="c3b39-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="c3b39-p101">Ha nem működik a **Megnyitás Intézővel** vagy **az Intéző nézetben** ellenőrizze, hogy a WebClient szolgáltatás **futtatásához** van beállítva, az alábbi lépéseket követve. Például ha a szolgáltatás nem fut a SharePoint vagy a OneDrive könyvtár megnyitása hosszú ideig is eltarthat.</span><span class="sxs-lookup"><span data-stu-id="c3b39-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="c3b39-105">A Windows keresési mezőjében típus futtatni, jelölje be a Futtatás asztali alkalmazás, típus services.msc és majd **Enter**.</span><span class="sxs-lookup"><span data-stu-id="c3b39-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="c3b39-p102">Görgessen le a webes ügyfélszolgáltatást, és ellenőrizze az **állapot** oszlopban. A WebClient szolgáltatás állapota nem **fut**, kattintson duplán a szolgáltatásra, kattintson a **Start menüre**és kattintson az **OK gombra**. A szolgáltatás engedélyezése, ha szükséges, az **Indítás típusa** mezőben a **kézi** vagy **automatikus** kiválasztásával.</span><span class="sxs-lookup"><span data-stu-id="c3b39-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="c3b39-p103">Explorer fájl megnyitásával kapcsolatos problémák elhárítása, lásd: [Nyissa meg az Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Fedezze fel a Szinkronizáló jobb alternatíva: [az új OneDrive szinkronizálás ügyfél fájlok szinkronizálása SharePoint](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="c3b39-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

