---
title: A Microsoft Edge használata Chromium-böngészők alapján elektronikus adatfeladatokat exportálható
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834373"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="e9988-102">A Microsoft Edge használata Chromium-böngészők alapján elektronikus adatfeladatokat exportálható</span><span class="sxs-lookup"><span data-stu-id="e9988-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="e9988-103">Egy nemrégiben történt változás miatt a Microsoft Edge böngészőkben alapértelmezés szerint nem engedélyezett a ClickOnce támogatása.</span><span class="sxs-lookup"><span data-stu-id="e9988-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="e9988-104">A Microsoft 365 Elektronikus adatok észlelése exportálási eszköz használatának folytatásához vagy a Microsoft Internet Explorert kell használnia, vagy engedélyeznie kell a ClickOnce-támogatást a Microsoft Edge-ben.</span><span class="sxs-lookup"><span data-stu-id="e9988-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="e9988-105">A ClickOnce-támogatás engedélyezése a Microsoft Edge-ben Chromium alapján:</span><span class="sxs-lookup"><span data-stu-id="e9988-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="e9988-106">A Microsoft Edge böngészőben látogasson el a edge://flags/#edge-click-once.</span><span class="sxs-lookup"><span data-stu-id="e9988-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="e9988-107">A ClickOnce támogatási csoportban módosítsa  az Alapértelmezett vagy a Letiltva értéket **Engedélyezve** **értékre.**</span><span class="sxs-lookup"><span data-stu-id="e9988-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="e9988-108">A böngészőablak alján válassza az Újraindítás **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e9988-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="e9988-109">A módosítás a Microsoft Edge újraindítása után lép érvénybe.</span><span class="sxs-lookup"><span data-stu-id="e9988-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="e9988-110">Erről és az exportálási eszköz telepítésének lépéséről a Tartalomkeresés [eredményének exportálásacímben található további információ.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="e9988-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>