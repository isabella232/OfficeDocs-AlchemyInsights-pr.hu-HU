---
title: SharePoint-dokumentumtár elemeinek másolása és áthelyezése
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: b8324f596b6830998bb7e659d561a015a7ba2b1a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715670"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="afe06-102">SharePoint-dokumentumtár elemeinek másolása és áthelyezése</span><span class="sxs-lookup"><span data-stu-id="afe06-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="afe06-103">A dokumentumtár különböző helyein fájlokat, mappákat és hivatkozásokat másolhat és helyezhet át.</span><span class="sxs-lookup"><span data-stu-id="afe06-103">You can copy and move files, folders, and links to different locations within a document library.</span></span> <span data-ttu-id="afe06-104">Az elemeket webhelyek között is másolhatja.</span><span class="sxs-lookup"><span data-stu-id="afe06-104">You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="afe06-105">A böngészőben tallózással keresse meg az áthelyezni kívánt fájlokat, mappákat vagy hivatkozásokat, majd kattintson a **Másolás ide** vagy **az Áthelyezés gombra.**</span><span class="sxs-lookup"><span data-stu-id="afe06-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="afe06-106">A SharePoint Online klasszikus élményének használata esetén a **Másolás a másodjára** és az **Áthelyezés** nem érhető el.</span><span class="sxs-lookup"><span data-stu-id="afe06-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="afe06-107">A **Hely kiválasztása csoportban**válassza ki azt a helyet, ahhoz az elemet másolni vagy áthelyezni, vagy kattintson a **Webhelyek tallózása gombra** a webhelyek teljes listájának megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="afe06-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="afe06-108">Ha az elemek másolásakor nem jelenik meg más webhelyek listája, a webhelyek közötti másolás nincs konfigurálva.</span><span class="sxs-lookup"><span data-stu-id="afe06-108">If you don't see other sites listed when you copy items, copying across sites hasn't been configured.</span></span> <span data-ttu-id="afe06-109">Az engedélyezéshez nyissa meg a SharePoint Felügyeleti központ beállítási lapját, és kattintson az **OK**gombra.</span><span class="sxs-lookup"><span data-stu-id="afe06-109">To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="afe06-110">Új mappa létrehozásához jelöljön ki egy helyet a mappahierarchiában, kattintson az **Új mappa**gombra, adja meg a mappa nevét, majd a bejelöléssel mentse a nevet.</span><span class="sxs-lookup"><span data-stu-id="afe06-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="afe06-111">Kattintson **a Másolás gombra,** vagy **itt mozoghat.**</span><span class="sxs-lookup"><span data-stu-id="afe06-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="afe06-112">Egyszerre legfeljebb 500 MB fájlt és mappát másolhat.</span><span class="sxs-lookup"><span data-stu-id="afe06-112">You can copy up to 500 MB of files and folders at one time.</span></span> <span data-ttu-id="afe06-113">> Ha olyan dokumentumokat másol, amelyek verzióelőzményekkel rendelkeznek, csak a legújabb verzió tmásolja.</span><span class="sxs-lookup"><span data-stu-id="afe06-113">>  When you copy documents that have version history, only the latest version is copied.</span></span> <span data-ttu-id="afe06-114">Dokumentumok áthelyezésekekekénél az előzmények is átkerülnek.</span><span class="sxs-lookup"><span data-stu-id="afe06-114">When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="afe06-115">Amikor egy fájl mozog, akkor is megjelenik a forráskönyvtárban, amíg teljesen át nem kerül a célhelyre, majd törlődik.</span><span class="sxs-lookup"><span data-stu-id="afe06-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="afe06-116">A fájl az áthelyezés után a forráshelyeken marad a lomtárban, és a szokásos újrahasznosítási ütemezés vonatkozik rá, kivéve, ha a felhasználó helyreállítja azt a lomtárból.</span><span class="sxs-lookup"><span data-stu-id="afe06-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="afe06-117">További információ:</span><span class="sxs-lookup"><span data-stu-id="afe06-117">For more information, see:</span></span>

 - <span data-ttu-id="afe06-118">[Fájlok áthelyezése vagy másolása a SharePointban](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (office-támogatási cikk)</span><span class="sxs-lookup"><span data-stu-id="afe06-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="afe06-119">[Fájlok áthelyezése bármely mappából](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blogcikk)</span><span class="sxs-lookup"><span data-stu-id="afe06-119">[Move files from any folder](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  