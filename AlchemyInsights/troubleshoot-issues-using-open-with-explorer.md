---
title: A Megnyitás Intézővel parancs használatával kapcsolatos problémák elhárítása
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659060"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="20128-102">A Megnyitás Intézővel kapcsolatos problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="20128-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="20128-103">A SharePointban vagy a OneDrive-ban az **Open with Explorer** paranccsal megnyitható gyakori problémák megoldása:</span><span class="sxs-lookup"><span data-stu-id="20128-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="20128-104">Használja az Internet Explorer 10 vagy az Internet Explorer 11 alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="20128-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="20128-105">**A Megnyitás Intézővel** nem kompatibilis a Microsoft Edge, a Google Chrome, a Firefox és a többiekkel.</span><span class="sxs-lookup"><span data-stu-id="20128-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="20128-106">A **Megnyitás Intézővel** le van tiltva az összes böngészőben, kivéve az Internet Explorert.</span><span class="sxs-lookup"><span data-stu-id="20128-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="20128-107">A **Megnyitás Intézővel** lehetőség nem érhető el a SharePoint-tárak modern felületén.</span><span class="sxs-lookup"><span data-stu-id="20128-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="20128-108">Használja inkább **a nézetet a Fájlkezelőben** .</span><span class="sxs-lookup"><span data-stu-id="20128-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="20128-109">Válassza a **nézet beállításai** \> **nézet lehetőséget a Fájlkezelőben**.</span><span class="sxs-lookup"><span data-stu-id="20128-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="20128-110">A megtekintés a Fájlkezelőben nem kompatibilis a Microsoft Edge, a Google Chrome, a Firefox és a többiekkel.</span><span class="sxs-lookup"><span data-stu-id="20128-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="20128-111">A **fájlkezelőben** csak az Internet Explorerben érhető el nézet.</span><span class="sxs-lookup"><span data-stu-id="20128-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="20128-112">Ellenőrizze, hogy fut-e a WebClient szolgáltatás.</span><span class="sxs-lookup"><span data-stu-id="20128-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="20128-113">A Windows Search mezőbe írja be a Futtatás parancsot, és válassza az asztali Futtatás alkalmazást, írja be a Services. msc parancsot, és nyomja le az ENTER billentyűt.</span><span class="sxs-lookup"><span data-stu-id="20128-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="20128-114">Görgessen le a WebClient szolgáltatáshoz, és győződjön meg arról, hogy az **állapot** oszlopban a "Futtatás" szó látható.</span><span class="sxs-lookup"><span data-stu-id="20128-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="20128-115">Ha nem, kattintson duplán a szolgáltatásra, kattintson a **Start**gombra, majd az **OK**gombra.</span><span class="sxs-lookup"><span data-stu-id="20128-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="20128-116">(Előfordulhat, hogy először engedélyeznie kell a szolgáltatást az **indítási típus** mezőben lévő **kézi** vagy **automatikus** elem kiválasztásával.)</span><span class="sxs-lookup"><span data-stu-id="20128-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="20128-117">Ha egy tár megnyitása a Fájlkezelőben akkor hasznos, ha egyszerre több fájlt és mappát kell másolni vagy áthelyeznie, de ha rendszeresen dolgozni szeretne a tárban, azt javasoljuk, hogy szinkronizálja.</span><span class="sxs-lookup"><span data-stu-id="20128-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="20128-118">A Fájlkezelőben való megnyitással kapcsolatos hibák elhárításáról a [Megnyitás az Intézőben](https://go.microsoft.com/fwlink/?linkid=871665)című témakörben olvashat.</span><span class="sxs-lookup"><span data-stu-id="20128-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="20128-119">A szinkronizálás beállításáról további információt a [SharePoint-fájlok szinkronizálása az új OneDrive szinkronizálási ügyfélprogrammal](https://go.microsoft.com/fwlink/?linkid=871666)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="20128-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="20128-120">További információért olvassa el a [SharePoint Online problémáinak elhárítása című témakört a "Megnyitás Intézővel" paranccsal](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="20128-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

