---
title: A Megnyitás Intézővel parancs nem működik
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694458"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="55805-102">A Megnyitás Intézővel nem végezhető műveletek</span><span class="sxs-lookup"><span data-stu-id="55805-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="55805-103">Ha a **Megnyitás Intézővel** vagy a **megtekintés a Fájlkezelőben** parancs nem működik, győződjön meg arról **, hogy a** WebClient szolgáltatás az alábbi lépésekkel van beállítva.</span><span class="sxs-lookup"><span data-stu-id="55805-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="55805-104">Hosszú időbe telik például a SharePoint-vagy OneDrive-tár megnyitása, ha a szolgáltatás nem fut.</span><span class="sxs-lookup"><span data-stu-id="55805-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="55805-105">A Windows Search mezőbe írja be a Futtatás parancsot, és válassza az asztali Futtatás alkalmazást, írja be a Services. msc parancsot, és válassza az **ENTER billentyűt**.</span><span class="sxs-lookup"><span data-stu-id="55805-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="55805-106">Görgessen le a WebClient szolgáltatáshoz, és ellenőrizze az **állapot** oszlopot.</span><span class="sxs-lookup"><span data-stu-id="55805-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="55805-107">Ha a WebClient szolgáltatás állapota nem **fut**, kattintson duplán a szolgáltatásra, kattintson a **Start**gombra, majd **az OK**gombra.</span><span class="sxs-lookup"><span data-stu-id="55805-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="55805-108">Engedélyezze a szolgáltatást, ha szükséges, az **indítási típus** mezőben válassza a **kézi** vagy az **automatikus** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="55805-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="55805-109">A Fájlkezelőben való megnyitással kapcsolatos hibák elhárításáról a [Megnyitás az Intézőben](https://go.microsoft.com/fwlink/?linkid=871665)című témakörben olvashat.</span><span class="sxs-lookup"><span data-stu-id="55805-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="55805-110">A szinkronizálás megismerése jobb alternatíva: [SharePoint-fájlok szinkronizálása az új OneDrive szinkronizálási ügyfélprogrammal](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="55805-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

