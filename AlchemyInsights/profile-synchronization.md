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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371986"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Ha nincs saját profil módosítás szinkronizálja a SharePoint felhasználóiprofil-alkalmazás?

A SharePoint Online használja az Active Directory importálás időzítőfeladat (AD importálása) felhasználók és csoportok importálása a felhasználóiprofil-alkalmazás. 
  
1. AD behozatali szinkronizálja a módosításokat a SharePoint Online Directory tárolóból a felhasználóiprofil-alkalmazás. Ezek a módosítások a kötegek feldolgozása.
    
2. Az időzítőfeladat addig fut, amíg a módosítások szinkronizálása megtörténik.
    
> [!NOTE]
> A feladat futtatásához szükséges idő függ a feldolgozásához módosítások számát. Nagy mennyiségű módosítást hosszabb időt vesz igénybe. A szolgáltatás szint megállapodás (SLA) kijelenti, hogy módosítja a felhasználó a SharePoint Online könyvtárban megjelennek a felhasználóiprofil-alkalmazás 24 órán belül. 
  
[További információ a SharePoint Online felhasználóiprofil-szinkronizálás](https://go.microsoft.com/fwlink/?linkid=875671)
  

