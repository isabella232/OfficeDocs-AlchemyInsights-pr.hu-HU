---
title: Profilszinkronizálás
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554335"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="41979-102">A profilom szinkronizálása a SharePoint felhasználóiprofil-alkalmazással módosul?</span><span class="sxs-lookup"><span data-stu-id="41979-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="41979-103">A SharePoint Online szolgáltatás az Active Directory importálás időzítőfeladatának (AD import) segítségével importálja a felhasználókat és a csoportokat a felhasználóiprofil-alkalmazásba.</span><span class="sxs-lookup"><span data-stu-id="41979-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="41979-104">Az AD import szinkronizálja a SharePoint Online Címtártárolóból a felhasználóiprofil-alkalmazásba történő módosításokat.</span><span class="sxs-lookup"><span data-stu-id="41979-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="41979-105">Ezek a változtatások kötegekben kerülnek feldolgozásra.</span><span class="sxs-lookup"><span data-stu-id="41979-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="41979-106">Az időzítőfeladat addig fut, amíg a változások szinkronizálása meg nem fejeződik.</span><span class="sxs-lookup"><span data-stu-id="41979-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="41979-107">A feladat futtatásához igénybe vesz idő a folyamat változásainak számától függ.</span><span class="sxs-lookup"><span data-stu-id="41979-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="41979-108">Számos változtatás hosszabb ideig tart.</span><span class="sxs-lookup"><span data-stu-id="41979-108">A large number of changes takes longer.</span></span> <span data-ttu-id="41979-109">A szolgáltatásszintű szerződés (SLA) megállapítja, hogy a SharePoint Online címtárban lévő felhasználó módosítását 24 órán belül a felhasználóiprofil-alkalmazás fogja tükröződni.</span><span class="sxs-lookup"><span data-stu-id="41979-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="41979-110">További információ a felhasználói profil szinkronizálásához a SharePoint Online szolgáltatásban</span><span class="sxs-lookup"><span data-stu-id="41979-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

