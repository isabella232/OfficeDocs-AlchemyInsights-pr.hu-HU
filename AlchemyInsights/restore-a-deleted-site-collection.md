---
title: Törölt a webhely visszaállítása
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
ms.openlocfilehash: 0cf10a3a0effc1774d8a07c5d0be96384362c175
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747780"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="9b533-102">Törölt a webhely visszaállítása</span><span class="sxs-lookup"><span data-stu-id="9b533-102">Restore a deleted site</span></span>

<span data-ttu-id="9b533-103">Ha egy rendszergazda törli egy webhely, kerül a webhelycsoport lomtárába kerül, ahol tartják 93 nap előtt véglegesen törlődik.</span><span class="sxs-lookup"><span data-stu-id="9b533-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="9b533-104">A webhely visszaállítása:</span><span class="sxs-lookup"><span data-stu-id="9b533-104">To restore the site:</span></span>
  
1. <span data-ttu-id="9b533-105">Az új SharePoint-felügyeleti központ, a **Lomtár** parancsra a menüszalagon.</span><span class="sxs-lookup"><span data-stu-id="9b533-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="9b533-106">Jelölje ki a visszaállítani kívánt webhelycsoport melletti jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="9b533-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="9b533-107">Kattintson a **Törölt elemek visszaállítása**parancsra.</span><span class="sxs-lookup"><span data-stu-id="9b533-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="9b533-108">Törölt kommunikáció a webhely visszaállítása, használhatja az új SharePoint-felügyeleti központ.</span><span class="sxs-lookup"><span data-stu-id="9b533-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="9b533-109">Ellenkező esetben kell használnia a Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9b533-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="9b533-110">Az Office 365 csoporthoz tartozó webhely visszaállítása, állítsa vissza a csoportot az Exchange felügyeleti központban kell.</span><span class="sxs-lookup"><span data-stu-id="9b533-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="9b533-111">Csoportok állíthatók vissza 30 napig, miután törölve van.</span><span class="sxs-lookup"><span data-stu-id="9b533-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

