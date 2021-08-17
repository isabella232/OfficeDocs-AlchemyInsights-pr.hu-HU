---
title: Profilszinkronizálás
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320711"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Mikor szinkronizálódnak a profiljaim a felhasználói SharePoint alkalmazással?

SharePoint Az Online az Active Directory importálási időzítőfeladatával importálja a felhasználókat és a csoportokat a Felhasználói profil alkalmazásba. 
  
1. AD Import szolgáltatás szinkronizálja a módosításokat a SharePoint Online Címtár-áruházból a felhasználóiprofil-alkalmazásba. Ezek a módosítások kötegekként vannak feldolgozva.
    
2. Az időzítőfeladat addig fut, amíg a módosításokat nem szinkronizálja.
    
**Megjegyzés:** A folyamat változásainak számától függ, hogy a feladat hány ideig tart. A nagyszámú módosítás hosszabb időt vesz igénybe. A szolgáltatásiszint-szerződés (SLA) kimondja, hogy a SharePoint Online Címtárban egy felhasználóra vonatkozó módosítás 24 órán belül megjelenik a Felhasználói profil alkalmazásban. 
  
[További információ a felhasználói profil szinkronizálásról a SharePoint Online-ban](https://go.microsoft.com/fwlink/?linkid=875671)
  

