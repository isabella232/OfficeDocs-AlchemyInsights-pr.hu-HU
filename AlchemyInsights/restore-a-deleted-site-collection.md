---
title: Törölt webhely visszaállítása
ms.author: kaarins
author: kaarins
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: a1fb15869b9f576696de4eda4c0b2101bd6cca17
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768550"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="e0645-102">Törölt webhely visszaállítása</span><span class="sxs-lookup"><span data-stu-id="e0645-102">Restore a deleted site</span></span>

<span data-ttu-id="e0645-103">Amikor egy admin töröl egy SharePoint-webhelyet, az a webhelycsoport lomtárába kerül, ahol 93 napig őrzi meg a végleges törlés előtt.</span><span class="sxs-lookup"><span data-stu-id="e0645-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="e0645-104">A webhely visszaállításához:</span><span class="sxs-lookup"><span data-stu-id="e0645-104">To restore the site:</span></span>
  
1. <span data-ttu-id="e0645-105">Az új SharePoint felügyeleti központban kattintson a **Lomtár** gombra a menüszalagon.</span><span class="sxs-lookup"><span data-stu-id="e0645-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="e0645-106">Jelölje be a jelölőnégyzetet a visszaállítani kívánt webhelycsoport mellett.</span><span class="sxs-lookup"><span data-stu-id="e0645-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="e0645-107">Kattintson a **törölt elemek visszaállítása**gombra.</span><span class="sxs-lookup"><span data-stu-id="e0645-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="e0645-108">A törölt kommunikációs hely visszaállításához használhatja az új SharePoint felügyeleti központot.</span><span class="sxs-lookup"><span data-stu-id="e0645-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="e0645-109">Ellenkező esetben a Microsoft PowerShellt kell használnia.</span><span class="sxs-lookup"><span data-stu-id="e0645-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="e0645-110">Az Office 365-csoportokhoz tartozó webhelyek visszaállításához vissza kell állítania a csoportot az Exchange felügyeleti központjában.</span><span class="sxs-lookup"><span data-stu-id="e0645-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="e0645-111">A csoportok a törlés után 30 nappal visszaállíthatók.</span><span class="sxs-lookup"><span data-stu-id="e0645-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

