---
title: Profil szinkronizálása
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768115"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="d5929-102">Mikor szinkronizálódik a profilom a SharePoint felhasználói profil alkalmazással?</span><span class="sxs-lookup"><span data-stu-id="d5929-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="d5929-103">A SharePoint Online az Active Directory importálási időzítőfeladatával (AD importálás) importálja a felhasználókat és csoportokat a felhasználói profil alkalmazásba.</span><span class="sxs-lookup"><span data-stu-id="d5929-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="d5929-104">Az AD importálás szinkronizálja a SharePoint Online címtártárból a felhasználói profil alkalmazásba történő módosításokat.</span><span class="sxs-lookup"><span data-stu-id="d5929-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="d5929-105">Ezeket a módosításokat kötegekben dolgozzuk fel.</span><span class="sxs-lookup"><span data-stu-id="d5929-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="d5929-106">Az időzítőfeladat a módosítások szinkronizálásáig fut.</span><span class="sxs-lookup"><span data-stu-id="d5929-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="d5929-107">A feladat futtatásához szükséges idő a feldolgozási módosítások számától függ.</span><span class="sxs-lookup"><span data-stu-id="d5929-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="d5929-108">Számos módosítás hosszabb időt vesz igénybe.</span><span class="sxs-lookup"><span data-stu-id="d5929-108">A large number of changes takes longer.</span></span> <span data-ttu-id="d5929-109">A szolgáltatásiszint-szerződés (SLA) kimondja, hogy a SharePoint Online-címtárban lévő felhasználó módosítása 24 órán belül megjelenik a felhasználói profil alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="d5929-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="d5929-110">További információ a felhasználói profilok SharePoint Online-ban való szinkronizálásáról</span><span class="sxs-lookup"><span data-stu-id="d5929-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

