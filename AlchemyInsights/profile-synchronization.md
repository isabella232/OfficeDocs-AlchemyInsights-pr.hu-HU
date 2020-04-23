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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Mikor szinkronizálódik a profilom a SharePoint felhasználói profil alkalmazással?

A SharePoint Online az Active Directory importálási időzítőfeladatával (AD importálás) importálja a felhasználókat és csoportokat a felhasználói profil alkalmazásba. 
  
1. Az AD importálás szinkronizálja a SharePoint Online címtártárból a felhasználói profil alkalmazásba történő módosításokat. Ezeket a módosításokat kötegekben dolgozzuk fel.
    
2. Az időzítőfeladat a módosítások szinkronizálásáig fut.
    
> [!NOTE]
> A feladat futtatásához szükséges idő a feldolgozási módosítások számától függ. Számos módosítás hosszabb időt vesz igénybe. A szolgáltatásiszint-szerződés (SLA) kimondja, hogy a SharePoint Online-címtárban lévő felhasználó módosítása 24 órán belül megjelenik a felhasználói profil alkalmazásban. 
  
[További információ a felhasználói profilok SharePoint Online-ban való szinkronizálásáról](https://go.microsoft.com/fwlink/?linkid=875671)
  

