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
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29920090"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="f69a0-102">Ha nincs saját profil módosítás szinkronizálja a SharePoint felhasználóiprofil-alkalmazás?</span><span class="sxs-lookup"><span data-stu-id="f69a0-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="f69a0-103">A SharePoint Online használja az Active Directory importálás időzítőfeladat (AD importálása) felhasználók és csoportok importálása a felhasználóiprofil-alkalmazás.</span><span class="sxs-lookup"><span data-stu-id="f69a0-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="f69a0-p101">AD behozatali szinkronizálja a módosításokat a SharePoint Online Directory tárolóból a felhasználóiprofil-alkalmazás. Ezek a módosítások a kötegek feldolgozása.</span><span class="sxs-lookup"><span data-stu-id="f69a0-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="f69a0-106">Az időzítőfeladat addig fut, amíg a módosítások szinkronizálása megtörténik.</span><span class="sxs-lookup"><span data-stu-id="f69a0-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="f69a0-p102">A feladat futtatásához szükséges idő függ a feldolgozásához módosítások számát. Nagy mennyiségű módosítást hosszabb időt vesz igénybe. A szolgáltatás szint megállapodás (SLA) kijelenti, hogy módosítja a felhasználó a SharePoint Online könyvtárban megjelennek a felhasználóiprofil-alkalmazás 24 órán belül.</span><span class="sxs-lookup"><span data-stu-id="f69a0-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="f69a0-110">További információ a SharePoint Online felhasználóiprofil-szinkronizálás</span><span class="sxs-lookup"><span data-stu-id="f69a0-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

