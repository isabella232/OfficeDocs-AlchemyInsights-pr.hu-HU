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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554335"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Ha nincs saját profil módosítás szinkronizálja a SharePoint felhasználóiprofil-alkalmazás?

A SharePoint Online használja az Active Directory importálás időzítőfeladat (AD importálása) felhasználók és csoportok importálása a felhasználóiprofil-alkalmazás. 
  
1. AD behozatali szinkronizálja a módosításokat a SharePoint Online Directory tárolóból a felhasználóiprofil-alkalmazás. Ezek a módosítások a kötegek feldolgozása.
    
2. Az időzítőfeladat addig fut, amíg a módosítások szinkronizálása megtörténik.
    
> [!NOTE]
> A feladat futtatásához szükséges idő függ a feldolgozásához módosítások számát. Nagy mennyiségű módosítást hosszabb időt vesz igénybe. A szolgáltatás szint megállapodás (SLA) kijelenti, hogy módosítja a felhasználó a SharePoint Online könyvtárban megjelennek a felhasználóiprofil-alkalmazás 24 órán belül. 
  
[További információ a SharePoint Online felhasználóiprofil-szinkronizálás](https://go.microsoft.com/fwlink/?linkid=875671)
  

