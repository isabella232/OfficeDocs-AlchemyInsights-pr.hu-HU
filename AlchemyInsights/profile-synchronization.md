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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>A profilom szinkronizálása a SharePoint felhasználóiprofil-alkalmazással módosul?

A SharePoint Online szolgáltatás az Active Directory importálás időzítőfeladatának (AD import) segítségével importálja a felhasználókat és a csoportokat a felhasználóiprofil-alkalmazásba. 
  
1. Az AD import szinkronizálja a SharePoint Online Címtártárolóból a felhasználóiprofil-alkalmazásba történő módosításokat. Ezek a változtatások kötegekben kerülnek feldolgozásra.
    
2. Az időzítőfeladat addig fut, amíg a változások szinkronizálása meg nem fejeződik.
    
> [!NOTE]
> A feladat futtatásához igénybe vesz idő a folyamat változásainak számától függ. Számos változtatás hosszabb ideig tart. A szolgáltatásszintű szerződés (SLA) megállapítja, hogy a SharePoint Online címtárban lévő felhasználó módosítását 24 órán belül a felhasználóiprofil-alkalmazás fogja tükröződni. 
  
[További információ a felhasználói profil szinkronizálásához a SharePoint Online szolgáltatásban](https://go.microsoft.com/fwlink/?linkid=875671)
  

