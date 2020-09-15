---
title: Törölt webhely visszaállítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692045"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="c3af4-102">Törölt webhely visszaállítása</span><span class="sxs-lookup"><span data-stu-id="c3af4-102">Restore a deleted site</span></span>

<span data-ttu-id="c3af4-103">Ha egy rendszergazda töröl egy SharePoint-webhelyet, az a webhelycsoport – Lomtár mappában található, ahol az 93-ös napok a végleges törlés előtt maradnak.</span><span class="sxs-lookup"><span data-stu-id="c3af4-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="c3af4-104">A webhely visszaállítása:</span><span class="sxs-lookup"><span data-stu-id="c3af4-104">To restore the site:</span></span>
  
1. <span data-ttu-id="c3af4-105">Az új SharePoint felügyeleti központban kattintson a **Lomtár** elemre a menüszalagon.</span><span class="sxs-lookup"><span data-stu-id="c3af4-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="c3af4-106">Jelölje be a visszaállítani kívánt webhelycsoport melletti jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="c3af4-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="c3af4-107">Kattintson a **törölt elemek visszaállítása**gombra.</span><span class="sxs-lookup"><span data-stu-id="c3af4-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="c3af4-108">Ha vissza szeretne állítani egy törölt kommunikációs webhelyet, használhatja az új SharePoint felügyeleti központot.</span><span class="sxs-lookup"><span data-stu-id="c3af4-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="c3af4-109">Egyéb esetben a Microsoft PowerShellt kell használnia.</span><span class="sxs-lookup"><span data-stu-id="c3af4-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="c3af4-110">Ha vissza szeretne állítani egy Microsoft 365-csoportba tartozó webhelyet, vissza kell állítania a csoportot az Exchange felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="c3af4-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="c3af4-111">A csoportok a törlésük után 30 napig visszaállíthatók.</span><span class="sxs-lookup"><span data-stu-id="c3af4-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

