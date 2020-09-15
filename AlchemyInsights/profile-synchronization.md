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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Mikor változik meg a profilom szinkronizálása a SharePoint felhasználói profil alkalmazással?

A SharePoint Online az Active Directory-importálási időzítőfeladat (AD importálás) segítségével importálja a felhasználókat és csoportokat a felhasználóiprofil-alkalmazásba. 
  
1. Az AD import szinkronizálja a SharePoint Online-címtárban lévő módosításokat a felhasználóiprofil-alkalmazásban. Ezek a módosítások kötegekben kerülnek feldolgozásra.
    
2. Az időzítő csak a módosítások szinkronizálásakor fut.
    
> [!NOTE]
> A futtatandó feladat elvégzésének időpontja a folyamat változásainak számától függ. A módosítások nagy száma hosszabb időt vesz igénybe. A Service Level Agreement (SLA) azt jelzi, hogy a SharePoint Online-címtárban a felhasználó a felhasználói profil alkalmazásban 24 óra múlva fog megjelenni. 
  
[További információ a felhasználói profilok szinkronizálásáról a SharePoint Online-ban](https://go.microsoft.com/fwlink/?linkid=875671)
  

