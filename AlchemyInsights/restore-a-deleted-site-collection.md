---
title: Törölt webhely visszaállítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: d37fd903c91c8cd6ac6137e815cb253f7edb4494
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912677"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="6cb1f-102">Törölt webhely visszaállítása</span><span class="sxs-lookup"><span data-stu-id="6cb1f-102">Restore a deleted site</span></span>

<span data-ttu-id="6cb1f-103">Amikor egy rendszergazda töröl egy SharePoint-webhelyet, az a Lomtárwebhely-csoportban kerül elhelyezésre, ahol 93 napig őrzi a rendszer, mielőtt véglegesen törölné.</span><span class="sxs-lookup"><span data-stu-id="6cb1f-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="6cb1f-104">A hely visszaállítása:</span><span class="sxs-lookup"><span data-stu-id="6cb1f-104">To restore the site:</span></span>
  
1. <span data-ttu-id="6cb1f-105">Az új SharePoint Felügyeleti központban kattintson a menüszalag **Lomtár** gombjára.</span><span class="sxs-lookup"><span data-stu-id="6cb1f-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="6cb1f-106">Jelölje be a visszaállítani kívánt webhelycsoport melletti jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="6cb1f-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="6cb1f-107">Kattintson **a Törölt elemek visszaállítása gombra.**</span><span class="sxs-lookup"><span data-stu-id="6cb1f-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="6cb1f-108">Törölt kommunikációs webhely visszaállításához használja az új SharePoint Felügyeleti központot.</span><span class="sxs-lookup"><span data-stu-id="6cb1f-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="6cb1f-109">Ellenkező esetben a Microsoft PowerShell t kell használnia.</span><span class="sxs-lookup"><span data-stu-id="6cb1f-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="6cb1f-110">A Microsoft 365-csoporthoz tartozó hely visszaállításához vissza kell állítania a csoportot az Exchange Felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="6cb1f-110">To restore a site that belongs to an Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="6cb1f-111">A csoportok a törlésük után 30 napig visszaállíthatók.</span><span class="sxs-lookup"><span data-stu-id="6cb1f-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

