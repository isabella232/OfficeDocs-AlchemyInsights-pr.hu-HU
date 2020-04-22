---
title: Nem működik a Megnyitás az Intézővel
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713036"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="176e8-102">Nem működik a Megnyitás az Intézővel</span><span class="sxs-lookup"><span data-stu-id="176e8-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="176e8-103">Ha **a Megnyitás explorerrel** vagy **a Fájlkezelőben való megtekintés** sel nem működik, ellenőrizze, hogy a WebClient szolgáltatás futása beállítással **fut-e** az alábbi lépések végrehajtásával.</span><span class="sxs-lookup"><span data-stu-id="176e8-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="176e8-104">Ha például a szolgáltatás nem fut, hosszú időbe telhet egy SharePoint- vagy OneDrive-tár megnyitása.</span><span class="sxs-lookup"><span data-stu-id="176e8-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="176e8-105">A Windows keresőmezőjében írja be a futtatás t, jelölje be az Asztali alkalmazás futtatása jelölőnégyzetet, írja be a services.msc parancsot, majd válassza **az Enter lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="176e8-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="176e8-106">Görgessen le a WebClient szolgáltatáshoz, és ellenőrizze az **Állapot** oszlopot.</span><span class="sxs-lookup"><span data-stu-id="176e8-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="176e8-107">Ha a WebClient szolgáltatás állapota nem **fut,** kattintson duplán a szolgáltatásra, kattintson a **Start**gombra, majd az **OK**gombra.</span><span class="sxs-lookup"><span data-stu-id="176e8-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="176e8-108">Szükség esetén engedélyezze a szolgáltatást az Indítás **típusa** mezőben a **Kézi** vagy az **Automatikus** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="176e8-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="176e8-109">A Fájlkezelőben megnyitott problémák elhárításáról a [Megnyitás az Intézőben című témakörben](https://go.microsoft.com/fwlink/?linkid=871665)található.</span><span class="sxs-lookup"><span data-stu-id="176e8-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="176e8-110">A szinkronizálás jobb alternatívaként való [felfedezése: SharePoint-fájlok szinkronizálása az új OneDrive szinkronizálási ügyfélalkalmazással](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="176e8-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

