---
title: A Megnyitás intézővel című programmal kapcsolatos problémák elhárítása
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759694"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="3f95f-102">Az Open with Explorer programmal kapcsolatos problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="3f95f-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="3f95f-103">Javítsa ki a SharePoint vagy a OneDrive dokumentumtárának megnyitásával kapcsolatos gyakori problémákat a **Megnyitás az Intézővel** paranccsal:</span><span class="sxs-lookup"><span data-stu-id="3f95f-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="3f95f-104">Használja az Internet Explorer 10-et vagy az Internet Explorer 11-et.</span><span class="sxs-lookup"><span data-stu-id="3f95f-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="3f95f-105">**A Open with Explorer** nem kompatibilis a Microsoft Edge, a Google Chrome, a Firefox és mások alkalmazásával.</span><span class="sxs-lookup"><span data-stu-id="3f95f-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="3f95f-106">**Az Intézővel megnyitva** minden böngészőben le van tiltva, kivéve az Internet Explorert.</span><span class="sxs-lookup"><span data-stu-id="3f95f-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="3f95f-107">**A Nyitott az Intézővel** program nem érhető el a SharePoint-tárak modern élményében.</span><span class="sxs-lookup"><span data-stu-id="3f95f-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="3f95f-108">Használja inkább **a Nézet a Fájlkezelőben** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3f95f-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="3f95f-109">Válassza **a Nézet lehetőséget** \> **a Fájlkezelőben**.</span><span class="sxs-lookup"><span data-stu-id="3f95f-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="3f95f-110">View in File Explorer nem kompatibilis a Microsoft Edge, a Google Chrome, a Firefox és mások.</span><span class="sxs-lookup"><span data-stu-id="3f95f-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="3f95f-111">**A Fájlkezelőben** csak az Internet Explorer ben érhető el.</span><span class="sxs-lookup"><span data-stu-id="3f95f-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="3f95f-112">Ellenőrizze, hogy fut-e a WebClient szolgáltatás.</span><span class="sxs-lookup"><span data-stu-id="3f95f-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="3f95f-113">A Windows keresőmezőjében írja be a futtatás t, jelölje be az Asztali alkalmazás futtatása jelölőnégyzetet, írja be a services.msc parancsot, majd nyomja le az Enter billentyűt.</span><span class="sxs-lookup"><span data-stu-id="3f95f-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="3f95f-114">Görgessen le a WebClient szolgáltatáshoz, és győződjön meg arról, hogy az **Állapot** oszlopban a "Futás" látható.</span><span class="sxs-lookup"><span data-stu-id="3f95f-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="3f95f-115">Ha nem, kattintson duplán a szolgáltatásra, kattintson a **Start**gombra, majd az **OK**gombra.</span><span class="sxs-lookup"><span data-stu-id="3f95f-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="3f95f-116">(Előfordulhat, hogy először engedélyeznie kell a szolgáltatást, ha az **Indítás típusa** mezőben a **Kézi** vagy az **Automatikus** lehetőséget választja.)</span><span class="sxs-lookup"><span data-stu-id="3f95f-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="3f95f-117">A Fájlkezelőben megnyitegy tárat, ha egyszer több fájlt és mappát kell másolnia vagy áthelyeznie, de ha rendszeresen szeretne dolgozni a tárban, javasoljuk, hogy szinkronizálja azt.</span><span class="sxs-lookup"><span data-stu-id="3f95f-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="3f95f-118">A Fájlkezelőben megnyitott problémák elhárításáról a [Megnyitás az Intézőben című témakörben](https://go.microsoft.com/fwlink/?linkid=871665)található.</span><span class="sxs-lookup"><span data-stu-id="3f95f-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="3f95f-119">A szinkronizálás beállításáról a [SharePoint-fájlok szinkronizálása az új OneDrive szinkronizálási ügyfélalkalmazással](https://go.microsoft.com/fwlink/?linkid=871666)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="3f95f-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="3f95f-120">További információt a ["Megnyitás explorerrel" paranccsal a SharePoint Online-ban felmerülő problémák elhárítására](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) című cikkben talál.</span><span class="sxs-lookup"><span data-stu-id="3f95f-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

