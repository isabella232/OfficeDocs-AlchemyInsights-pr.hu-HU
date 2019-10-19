---
title: Törölt webhely visszaállítása
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
ms.openlocfilehash: 9e4e9ade058c60ecd7a6ce1b2a40c4996ac5676f
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36552471"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="930f2-102">Törölt webhely visszaállítása</span><span class="sxs-lookup"><span data-stu-id="930f2-102">Restore a deleted site</span></span>

<span data-ttu-id="930f2-103">Amikor egy admin töröl egy webhelyet, akkor az a webhelycsoport lomtárába kerül, ahol a 93 nappal azelőtt tartják, hogy végleg törölve lett.</span><span class="sxs-lookup"><span data-stu-id="930f2-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="930f2-104">A webhely visszaállításához:</span><span class="sxs-lookup"><span data-stu-id="930f2-104">To restore the site:</span></span>
  
1. <span data-ttu-id="930f2-105">Az új SharePoint felügyeleti központban kattintson a **Lomtár** gombra a menüszalagon.</span><span class="sxs-lookup"><span data-stu-id="930f2-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="930f2-106">Jelölje be a jelölőnégyzetet a visszaállítani kívánt webhelycsoport mellett.</span><span class="sxs-lookup"><span data-stu-id="930f2-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="930f2-107">Kattintson a **törölt elemek visszaállítása**gombra.</span><span class="sxs-lookup"><span data-stu-id="930f2-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="930f2-108">A törölt kommunikációs hely visszaállításához használhatja az új SharePoint felügyeleti központot.</span><span class="sxs-lookup"><span data-stu-id="930f2-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="930f2-109">Ellenkező esetben a Microsoft PowerShellt kell használnia.</span><span class="sxs-lookup"><span data-stu-id="930f2-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="930f2-110">Az Office 365-csoportokhoz tartozó webhelyek visszaállításához vissza kell állítania a csoportot az Exchange felügyeleti központjában.</span><span class="sxs-lookup"><span data-stu-id="930f2-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="930f2-111">A csoportok a törlés után 30 nappal visszaállíthatók.</span><span class="sxs-lookup"><span data-stu-id="930f2-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

