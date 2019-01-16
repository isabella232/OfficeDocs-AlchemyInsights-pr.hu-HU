---
title: Adatmegőrzési szabályok Exchange felügyeleti központ nem működik
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293146"
---
 **Hiba:** Az újonnan létrehozott, vagy az Exchange felügyeleti központban frissített adatmegőrzési szabályok nem alkalmazzák a postafiókokat vagy elemek nem kerülnek az archív postaládába áthelyezték vagy törölték. 
  
 **Alapvető okok:**
  
- Ez azért lehet, mert a **Kezelt Mappakezelő** nem dolgozta fel a felhasználó postafiókját. A kezelt Mappakezelő próbálja feldolgozni a felhőalapú szervezet hét naponta minden postaláda. Ha módosítja egy adatmegőrzési címkét vagy különböző adatmegőrzési szabály alkalmazása egy postaládához, megvárhatja, mindaddig, amíg a kezelt mappa segítő dolgozza fel a postaláda, vagy a kezelt Mappakezelő feldolgozni egy adott el a Start-ManagedFolderAssistant parancsmag futtatása a postafiókot. Ez a parancsmag fut akkor hasznos, tesztelésére és hibaelhárítására adatmegőrzési vagy adatmegőrzési címke beállításai. További információért látogassa meg [futtatni a kezelt Mappakezelő](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Megoldás:** Elindítani a kezelt Mappakezelő adott postaládához a következő parancsot futtassa: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Ez is lehet jelentkezhet, ha **RetentionHold** volt **engedélyezett** a postaládához. Ha a postaláda került a RetentionHold, az a postaláda adatmegőrzési nem lehet feldolgozni ez idő alatt. Vonatkozó további információk a RetentionHold beállítást lásd: [Postaláda adatmegőrzési tartsa](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Megoldás:**
    
  - A RetentionHold beállítást az adott postafiókhoz [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)állapotának ellenőrzése:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Egy adott postaláda **letiltása** RetentionHold a következő parancsot futtassa: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Most futtassa újra a kezelt mappa segéd:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Megjegyzés:** Ha a postafiók 10 MB-nál kisebb, a kezelt Mappakezelő nem dolgozza fel automatikusan a postafiókot. 
  

