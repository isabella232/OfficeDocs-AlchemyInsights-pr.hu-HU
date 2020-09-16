---
title: A Microsoft Edge használata a eDiscovery exportálásához a Chromium böngészők alapján
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 64aebb7f048dba37eef8cd1fa6286b36823d3f0f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734517"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="01b14-102">A Microsoft Edge használata a eDiscovery exportálásához a Chromium böngészők alapján</span><span class="sxs-lookup"><span data-stu-id="01b14-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="01b14-103">A legutóbbi változtatások miatt a Microsoft Edge böngészőknek alapértelmezés szerint nincs engedélyezve a ClickOnce támogatása.</span><span class="sxs-lookup"><span data-stu-id="01b14-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="01b14-104">A Microsoft 365 eDiscovery exportálási eszközének folytatásához a Microsoft Internet Explorer böngészőt kell használnia, vagy engedélyeznie kell a ClickOnce támogatást a Microsoft Edge-ben.</span><span class="sxs-lookup"><span data-stu-id="01b14-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="01b14-105">A ClickOnce támogatás engedélyezése a Microsoft Edge-ben a Chromium alapján:</span><span class="sxs-lookup"><span data-stu-id="01b14-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="01b14-106">A Microsoft Edge böngészőjében keresse fel a edge://flags/#edge – egyszer.</span><span class="sxs-lookup"><span data-stu-id="01b14-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="01b14-107">A ClickOnce támogatás beállításnál módosítsa az **alapértelmezett** vagy a **letiltott** érték beállítás értékét az **engedélyezve**értékre.</span><span class="sxs-lookup"><span data-stu-id="01b14-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="01b14-108">A böngészőablak alján válassza az **Újraindítás**gombot.</span><span class="sxs-lookup"><span data-stu-id="01b14-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="01b14-109">A módosítások a Microsoft Edge újraindítása után lépnek életbe.</span><span class="sxs-lookup"><span data-stu-id="01b14-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="01b14-110">Az exportálási eszköz telepítésével kapcsolatos további tudnivalókért olvassa el a tartalmi találatok [ exportálása](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)című témakört.</span><span class="sxs-lookup"><span data-stu-id="01b14-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>