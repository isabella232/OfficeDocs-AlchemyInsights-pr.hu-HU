---
title: E-mailek áthelyezése az archív postaláda
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28294217"
---
A problémák az archív postaládába elemek archiválását. Ellenőrizze, hogy a hajtott végre a következő lépéseket:
  
1. Győződjön meg arról, hogy a **postaláda archiválása** engedélyezve van. Ha nem, [Ez a cikk](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) lépések segítségével engedélyezze az archív postaláda. 
    
2. Az Exchange felügyeleti központ **Adatmegőrzési címkék** **Való kezelés**alatt válassza ki, az **Archív Ugrás** műveletet a kívánt **Megőrzési kor**tartalmazó **adatmegőrzési címke** létrehozása.
    
3. Az Exchange felügyeleti központ **Adatmegőrzési szabályok**kiválasztása, **Adatmegőrzési szabály** létrehozása és az **archívum áthelyezése** adatmegőrzési címke hozzáadása házirendhez. 
    
4. [A megőrzési házirendet](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) az adott felhasználó postaládájához. Ugyanaz a házirend az **elsődleges** és az **Archív** postaláda vonatkozik. 
    
A felhasználó postafiókja elemek áthelyezése az archív postaláda archiválási házirend most már látnia kell. A kezelt mappa Segéd (MFA) és az új beállítások alkalmazása a felhasználó postaládájában, hogy szükség lehet. Futtassa a következő parancsot közben [csatlakoztatva EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) indítása a kezelt Mappakezelő egy adott postaláda: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Archiválási házirend beállításával kapcsolatos további információra van szükségünk, lásd: [postafiókok az archív és törlési házirend beállítása](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

