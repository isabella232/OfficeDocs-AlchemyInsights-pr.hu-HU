---
title: Profil-szinkronizálás
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801771"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="c5609-102">Mikor változik meg a profilom szinkronizálása a SharePoint felhasználói profil alkalmazással?</span><span class="sxs-lookup"><span data-stu-id="c5609-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="c5609-103">A SharePoint Online az Active Directory-importálási időzítőfeladat (AD importálás) segítségével importálja a felhasználókat és csoportokat a felhasználóiprofil-alkalmazásba.</span><span class="sxs-lookup"><span data-stu-id="c5609-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="c5609-104">Az AD import szinkronizálja a SharePoint Online-címtárban lévő módosításokat a felhasználóiprofil-alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="c5609-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="c5609-105">Ezek a módosítások kötegekben kerülnek feldolgozásra.</span><span class="sxs-lookup"><span data-stu-id="c5609-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="c5609-106">Az időzítő csak a módosítások szinkronizálásakor fut.</span><span class="sxs-lookup"><span data-stu-id="c5609-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="c5609-107">A futtatandó feladat elvégzésének időpontja a folyamat változásainak számától függ.</span><span class="sxs-lookup"><span data-stu-id="c5609-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="c5609-108">A módosítások nagy száma hosszabb időt vesz igénybe.</span><span class="sxs-lookup"><span data-stu-id="c5609-108">A large number of changes takes longer.</span></span> <span data-ttu-id="c5609-109">A Service Level Agreement (SLA) azt jelzi, hogy a SharePoint Online-címtárban a felhasználó a felhasználói profil alkalmazásban 24 óra múlva fog megjelenni.</span><span class="sxs-lookup"><span data-stu-id="c5609-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="c5609-110">További információ a felhasználói profilok szinkronizálásáról a SharePoint Online-ban</span><span class="sxs-lookup"><span data-stu-id="c5609-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

