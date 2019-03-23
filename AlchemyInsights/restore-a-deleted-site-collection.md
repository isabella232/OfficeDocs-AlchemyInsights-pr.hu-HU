---
title: Törölt webhelycsoport visszaállítása
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 1f9a66daf7bee43291b785b6260aec8725ee782f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753788"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="a0c44-102">Törölt webhelycsoport visszaállítása</span><span class="sxs-lookup"><span data-stu-id="a0c44-102">Restore a deleted site collection</span></span>

<span data-ttu-id="a0c44-103">Ha egy rendszergazda törli a klasszikus helycsoportot, kerül a webhelycsoport lomtárába kerül, ahol tartják 93 nap előtt véglegesen törlődik.</span><span class="sxs-lookup"><span data-stu-id="a0c44-103">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="a0c44-104">A webhelycsoport visszaállítása:</span><span class="sxs-lookup"><span data-stu-id="a0c44-104">To restore the site collection:</span></span>
  
1. <span data-ttu-id="a0c44-105">A klasszikus SharePoint felügyeleti központban kattintson a menüszalagon **Lomtár** .</span><span class="sxs-lookup"><span data-stu-id="a0c44-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="a0c44-106">Jelölje ki a visszaállítani kívánt webhelycsoport melletti jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="a0c44-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="a0c44-107">Kattintson a **Törölt elemek visszaállítása**parancsra.</span><span class="sxs-lookup"><span data-stu-id="a0c44-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="a0c44-108">Törölt kommunikáció a webhely visszaállítása a SharePoint felügyeleti központ kép is használhatja.</span><span class="sxs-lookup"><span data-stu-id="a0c44-108">To restore a deleted communication site, you can use the new SharePoint admin center preview.</span></span> <span data-ttu-id="a0c44-109">Ellenkező esetben szeretné használni a PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a0c44-109">Otherwise, you need to use PowerShell.</span></span> <span data-ttu-id="a0c44-110">Az Office 365 csoporthoz tartozó webhely visszaállítása, állítsa vissza a csoportot az Exchange felügyeleti központban kell.</span><span class="sxs-lookup"><span data-stu-id="a0c44-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="a0c44-111">Csoportok állíthatók vissza 30 napig, miután törölve van.</span><span class="sxs-lookup"><span data-stu-id="a0c44-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

