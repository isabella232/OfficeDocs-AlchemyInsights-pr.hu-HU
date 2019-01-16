---
title: Törölt webhelycsoport visszaállítása
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: b3c72033dfcc093dd0c2837d2866c6a78d64449c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293578"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="23eee-102">Törölt webhelycsoport visszaállítása</span><span class="sxs-lookup"><span data-stu-id="23eee-102">Restore a deleted site collection</span></span>

<span data-ttu-id="23eee-p101">Ha egy rendszergazda törli a klasszikus helycsoportot, kerül a webhelycsoport lomtárába kerül, ahol tartják 93 nap előtt véglegesen törlődik. A webhelycsoport visszaállítása:</span><span class="sxs-lookup"><span data-stu-id="23eee-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="23eee-105">A klasszikus SharePoint felügyeleti központban kattintson a menüszalagon **Lomtár** .</span><span class="sxs-lookup"><span data-stu-id="23eee-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="23eee-106">Jelölje ki a visszaállítani kívánt webhelycsoport melletti jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="23eee-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="23eee-107">Kattintson a **Törölt elemek visszaállítása**parancsra.</span><span class="sxs-lookup"><span data-stu-id="23eee-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="23eee-p102">Törölt kommunikáció a webhely visszaállítása a SharePoint felügyeleti központ kép is használhatja. Ellenkező esetben szeretné használni a PowerShell. Az Office 365 csoporthoz tartozó webhely visszaállítása, állítsa vissza a csoportot az Exchange felügyeleti központban kell. Csoportok állíthatók vissza 30 napig, miután törölve van.</span><span class="sxs-lookup"><span data-stu-id="23eee-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  

