---
title: Megnyitás Explorer nem működik
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419874"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="5028f-102">Megnyitás Explorer nem működik</span><span class="sxs-lookup"><span data-stu-id="5028f-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="5028f-103">Ha nem működik a **Megnyitás Intézővel** vagy **az Intéző nézetben** ellenőrizze, hogy a WebClient szolgáltatás **futtatásához** van beállítva, az alábbi lépéseket követve.</span><span class="sxs-lookup"><span data-stu-id="5028f-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="5028f-104">Például ha a szolgáltatás nem fut a SharePoint vagy a OneDrive könyvtár megnyitása hosszú ideig is eltarthat.</span><span class="sxs-lookup"><span data-stu-id="5028f-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="5028f-105">A Windows keresési mezőjében típus futtatni, jelölje be a Futtatás asztali alkalmazás, típus services.msc és majd **Enter**.</span><span class="sxs-lookup"><span data-stu-id="5028f-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="5028f-106">Görgessen le a webes ügyfélszolgáltatást, és ellenőrizze az **állapot** oszlopban.</span><span class="sxs-lookup"><span data-stu-id="5028f-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="5028f-107">A WebClient szolgáltatás állapota nem **fut**, kattintson duplán a szolgáltatásra, kattintson a **Start menüre**és kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="5028f-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="5028f-108">A szolgáltatás engedélyezése, ha szükséges, az **Indítás típusa** mezőben a **kézi** vagy **automatikus** kiválasztásával.</span><span class="sxs-lookup"><span data-stu-id="5028f-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="5028f-109">Explorer fájl megnyitásával kapcsolatos problémák elhárítása, lásd: [Nyissa meg az Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="5028f-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="5028f-110">Fedezze fel a Szinkronizáló jobb alternatíva: [az új OneDrive szinkronizálás ügyfél fájlok szinkronizálása SharePoint](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="5028f-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

