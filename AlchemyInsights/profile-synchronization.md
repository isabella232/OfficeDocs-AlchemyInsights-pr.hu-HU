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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923646"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Mikor szinkronizálódnak a profilváltozások a felhasználói SharePoint alkalmazással?

SharePoint Az Online az Active Directory importálási időzítőfeladatával importálja a felhasználókat és a csoportokat a Felhasználói profil alkalmazásba. 
  
1. AD-importálási szolgáltatás szinkronizálja a módosításokat a SharePoint Online Címtár-áruházból a felhasználóiprofil-alkalmazásba. Ezek a módosítások kötegekként vannak feldolgozva.
    
2. Az időzítőfeladat addig fut, amíg a módosításokat nem szinkronizálja.
    
> [!NOTE]
> A folyamat változásainak számától függ, hogy a feladat hány ideig tart. A nagyszámú módosítás hosszabb időt vesz igénybe. A szolgáltatásiszint-szerződés (SLA) kimondja, hogy a SharePoint Online Címtárban egy felhasználóra vonatkozó módosítás 24 órán belül megjelenik a Felhasználói profil alkalmazásban. 
  
[További információ a felhasználói profil szinkronizálásról a SharePoint Online-ban](https://go.microsoft.com/fwlink/?linkid=875671)
  

