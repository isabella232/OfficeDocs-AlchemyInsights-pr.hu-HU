---
title: Elemek másolása vagy áthelyezése a SharePoint-dokumentumtárban
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
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: d7aa865a6b3db0871a57313dd7d6f5b0213ca0e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807121"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="0abdd-102">Elemek másolása vagy áthelyezése a SharePoint-dokumentumtárban</span><span class="sxs-lookup"><span data-stu-id="0abdd-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="0abdd-103">A dokumentumtárban lévő fájlokat, mappákat és hivatkozásokat átmásolhatja és áthelyezheti a különböző helyekre.</span><span class="sxs-lookup"><span data-stu-id="0abdd-103">You can copy and move files, folders, and links to different locations within a document library.</span></span> <span data-ttu-id="0abdd-104">Az elemeket a webhelyek között is másolhatja.</span><span class="sxs-lookup"><span data-stu-id="0abdd-104">You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="0abdd-105">A böngészőben tallózással keresse meg az áthelyezni kívánt fájlokat, mappákat vagy hivatkozásokat, majd kattintson a **Másolás** vagy **a áthelyezés**parancsra.</span><span class="sxs-lookup"><span data-stu-id="0abdd-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="0abdd-106">Ha a SharePoint Online klasszikus felületét használja, a **Másolás** és a **Áthelyezés** lehetőség nem érhető el.</span><span class="sxs-lookup"><span data-stu-id="0abdd-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="0abdd-107">A **válasszon egy**helyet csoportban válassza ki azt a helyet, ahová az elemeket másolni vagy áthelyezni szeretné, vagy a webhelyek **tallózása** gombra kattintva jelenítse meg a webhelyek teljes listáját.</span><span class="sxs-lookup"><span data-stu-id="0abdd-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="0abdd-108">Ha nem láthatók az elemek másolásakor felsorolt egyéb webhelyek, akkor a másolás nem volt konfigurálva a webhelyek között.</span><span class="sxs-lookup"><span data-stu-id="0abdd-108">If you don't see other sites listed when you copy items, copying across sites hasn't been configured.</span></span> <span data-ttu-id="0abdd-109">A beállítás engedélyezéséhez nyissa meg a SharePoint felügyeleti központ Beállítások lapját, és kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="0abdd-109">To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="0abdd-110">Új mappa létrehozásához jelöljön ki egy helyet a mappa hierarchiájában, kattintson az **új mappa**elemre, írja be a mappa nevét, és a név mentéséhez jelölje be a jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="0abdd-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="0abdd-111">Kattintson a **Másolás ide** vagy az **Áthelyezés ide**gombra.</span><span class="sxs-lookup"><span data-stu-id="0abdd-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="0abdd-112">Egyszerre csak 500 MB-nyi fájlok és mappák másolhatók.</span><span class="sxs-lookup"><span data-stu-id="0abdd-112">You can copy up to 500 MB of files and folders at one time.</span></span> <span data-ttu-id="0abdd-113">> a korábbi verziók másolásakor csak a legújabb verziót másolja a program.</span><span class="sxs-lookup"><span data-stu-id="0abdd-113">>  When you copy documents that have version history, only the latest version is copied.</span></span> <span data-ttu-id="0abdd-114">Dokumentumok áthelyezésekor a program az előzményeket is áthelyezi.</span><span class="sxs-lookup"><span data-stu-id="0abdd-114">When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="0abdd-115">Ha egy fájl át van helyezve, az továbbra is megjelenik a forrás könyvtárában, amíg a teljes helyre nem kerül a célhelyre, majd törlődik.</span><span class="sxs-lookup"><span data-stu-id="0abdd-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="0abdd-116">A fájl a forrás webhelyek Lomtárában marad az áthelyezés befejezése után, kivéve, ha egy felhasználó visszanyeri azt a Lomtárból.</span><span class="sxs-lookup"><span data-stu-id="0abdd-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="0abdd-117">További információ:</span><span class="sxs-lookup"><span data-stu-id="0abdd-117">For more information, see:</span></span>

 - <span data-ttu-id="0abdd-118">[Fájlok áthelyezése vagy másolása a SharePointban](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office-támogatási cikk)</span><span class="sxs-lookup"><span data-stu-id="0abdd-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="0abdd-119">[Fájlok áthelyezése bármely mappából](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span><span class="sxs-lookup"><span data-stu-id="0abdd-119">[Move files from any folder](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  