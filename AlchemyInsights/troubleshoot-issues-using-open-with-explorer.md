---
title: A Megnyitás az Intéző programmal szolgáltatással kapcsolatos problémák elhárítása
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742735"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="8bee0-102">Megerősít probléma-val nyit-val Felfedező</span><span class="sxs-lookup"><span data-stu-id="8bee0-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="8bee0-103">Erősít mindennapi probléma-val megüresedett állás egy dokumentum könyvtár-ban SharePoint vagy OneDrive használ a **nyit-val Felfedező** követel:</span><span class="sxs-lookup"><span data-stu-id="8bee0-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="8bee0-104">Használja az Internet Explorer 10 vagy az Internet Explorer 11 böngészőt.</span><span class="sxs-lookup"><span data-stu-id="8bee0-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="8bee0-105">**Megnyitás az Explorer** nem kompatibilis a Microsoft Edge, Google Chrome, Firefox és mások.</span><span class="sxs-lookup"><span data-stu-id="8bee0-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="8bee0-106">Az **Intéző** az Internet Explorer kivételével minden böngészőben le van tiltva.</span><span class="sxs-lookup"><span data-stu-id="8bee0-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="8bee0-107">**Nyitott az Explorer** nem áll rendelkezésre a modern élményt SharePoint könyvtárak.</span><span class="sxs-lookup"><span data-stu-id="8bee0-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="8bee0-108">Ehelyett használja **a Fájltallózó nézetet** .</span><span class="sxs-lookup"><span data-stu-id="8bee0-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="8bee0-109">**A fájltallózó**nézetben válassza a **nézet beállításai** \> nézetet.</span><span class="sxs-lookup"><span data-stu-id="8bee0-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="8bee0-110">Kilátás-ban Reszelő Felfedező van nem összeegyeztethető-val Mikroszkóp él, Google Króm, Kilő és másikak.</span><span class="sxs-lookup"><span data-stu-id="8bee0-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="8bee0-111">**Kilátás-ban Reszelő Felfedező** -ban elérhető egyetlen-ban Internet Felfedező.</span><span class="sxs-lookup"><span data-stu-id="8bee0-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="8bee0-112">Ellenőrizze, hogy a webes ügyfélszolgáltatás fut-e.</span><span class="sxs-lookup"><span data-stu-id="8bee0-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="8bee0-113">-Ban Windows kutatás doboz, típus fuss, kiválaszt a fuss iskolapad app, típus Services. msc, aztán nyomjon entert.</span><span class="sxs-lookup"><span data-stu-id="8bee0-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="8bee0-114">Görgesse le a webes ügyfélszolgáltatást, és győződjön meg róla, hogy az **állapot** oszlopban a "Futtatás" jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="8bee0-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="8bee0-115">Ha nem, kattintson duplán a szolgáltatásra, kattintson a **Start**gombra, majd kattintson **az OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="8bee0-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="8bee0-116">(Előfordulhat, hogy először engedélyeznie kell a szolgáltatást, ha az **Indítás típusa** mezőben a **manuális** vagy az **automatikus** lehetőséget választja.)</span><span class="sxs-lookup"><span data-stu-id="8bee0-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8bee0-117">Ha egyszerre több fájlt és mappát kell átmásolnia vagy áthelyeznia, de ha rendszeresen szeretne dolgozni a tárban, javasoljuk, hogy szinkronizálja a könyvtárat a fájlkezelő alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="8bee0-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="8bee0-118">A Fájltallózón történő megnyitási problémák elhárításához tekintse [meg a Megnyitás az Intézőben](https://go.microsoft.com/fwlink/?linkid=871665)című témakört.</span><span class="sxs-lookup"><span data-stu-id="8bee0-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="8bee0-119">A szinkronizálás beállításáról további információt a következő témakörben talál: [SharePoint-fájlok szinkronizálása az új OneDrive Sync-ügyféllel](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="8bee0-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="8bee0-120">További információért olvassa el a ["Megnyitás az Intéző segítségével" parancsot a SharePoint Online problémáinak elhárításáról](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="8bee0-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

