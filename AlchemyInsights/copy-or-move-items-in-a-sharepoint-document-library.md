---
title: Elemek másolása vagy áthelyezése egy SharePoint-dokumentumtárban
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 5/24/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: 6e14260d3670eb15f73e92dc5b0c86e0e842974a
ms.sourcegitcommit: efdde3c24a0c1adfb8b6f5f59dcae435fb5c53a8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38711758"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="c06e7-102">Elemek másolása vagy áthelyezése egy SharePoint-dokumentumtárban</span><span class="sxs-lookup"><span data-stu-id="c06e7-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="c06e7-103">A dokumentumtáron belül különböző helyekre másolhat és mozgathatja a fájlokat, mappákat és hivatkozásokat.</span><span class="sxs-lookup"><span data-stu-id="c06e7-103">You can copy and move files, folders, and links to different locations within a document library.</span></span> <span data-ttu-id="c06e7-104">Az elemeket több hely között is átmásolhatja.</span><span class="sxs-lookup"><span data-stu-id="c06e7-104">You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="c06e7-105">A böngészőben tallózva keresse meg az áthelyezni kívánt fájlokat, mappákat vagy hivatkozásokat, majd kattintson a **Másolás** vagy **Áthelyezés**gombra.</span><span class="sxs-lookup"><span data-stu-id="c06e7-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c06e7-106">Ha a SharePoint Online klasszikus élményét használja, a **Másolás** és a **mozgás** nem érhető el.</span><span class="sxs-lookup"><span data-stu-id="c06e7-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="c06e7-107">A **célhely kiválasztása**területen jelölje ki azt a helyet, ahová másolni vagy áthelyezni szeretné az elemeket, vagy kattintson a helyek közötti **Keresés** gombra a webhelyek teljes listájának megtekintéséhez.</span><span class="sxs-lookup"><span data-stu-id="c06e7-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c06e7-108">Ha nem látja az elemek másolásakor felsorolt más webhelyeket, akkor a helyek közötti másolás nem lett konfigurálva.</span><span class="sxs-lookup"><span data-stu-id="c06e7-108">If you don't see other sites listed when you copy items, copying across sites hasn't been configured.</span></span> <span data-ttu-id="c06e7-109">-Hoz képessé tesz ez, megy a elintézés oldal-ból SharePoint admin központ és kettyenés **rendben van**.</span><span class="sxs-lookup"><span data-stu-id="c06e7-109">To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="c06e7-110">Új mappa létrehozásához jelöljön ki egy helyet a mappahierarchiában, kattintson az **új mappa**elemre, adja meg a mappa nevét, majd kattintson a jelölőnégyzetbe a név mentéséhez.</span><span class="sxs-lookup"><span data-stu-id="c06e7-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="c06e7-111">Kettyenés **másol itt** vagy **mozog itt**.</span><span class="sxs-lookup"><span data-stu-id="c06e7-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c06e7-112">Egyszerre akár 500 MB fájlokat és mappákat is másolhat.</span><span class="sxs-lookup"><span data-stu-id="c06e7-112">You can copy up to 500 MB of files and folders at one time.</span></span> <span data-ttu-id="c06e7-113">> a korábbi verziójú dokumentumok másolásakor a program csak a legújabb verziót másolja.</span><span class="sxs-lookup"><span data-stu-id="c06e7-113">>  When you copy documents that have version history, only the latest version is copied.</span></span> <span data-ttu-id="c06e7-114">A dokumentumok áthelyezésekor előzményei is áthelyezhetők.</span><span class="sxs-lookup"><span data-stu-id="c06e7-114">When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="c06e7-115">Amikor egy fájl áthelyezhető, a forráskönyvtárban továbbra is megjelenik, amíg teljesen el nem kerül a célhelyre, majd törli azt.</span><span class="sxs-lookup"><span data-stu-id="c06e7-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="c06e7-116">A reszelő akarat marad-ban forrás telek újra feldolgoz tartó után a mozog van kiegészít és lenni azzal a szokásos újra feldolgoz táblázat hacsak egy felhasználó visszanyer ez-ból újra feldolgoz tartó.</span><span class="sxs-lookup"><span data-stu-id="c06e7-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="c06e7-117">További információ:</span><span class="sxs-lookup"><span data-stu-id="c06e7-117">For more information, see:</span></span>

 - <span data-ttu-id="c06e7-118">[Áthelyezni vagy másolni a fájlokat a SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office támogatási cikke)</span><span class="sxs-lookup"><span data-stu-id="c06e7-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="c06e7-119">[Mozog fájlokat-ból akármi dosszié hivatalban 365](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (mikroszkóp tech Közösség blog cikk)</span><span class="sxs-lookup"><span data-stu-id="c06e7-119">[Move files from any folder in Office 365](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  