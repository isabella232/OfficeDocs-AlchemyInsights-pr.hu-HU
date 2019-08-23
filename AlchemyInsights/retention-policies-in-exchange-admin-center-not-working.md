---
title: Adatmegőrzési szabályok Exchange felügyeleti központ nem működik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551345"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Az Exchange felügyeleti központ adatmegőrzési szabályok

 **Hiba:** Az újonnan létrehozott, vagy az Exchange felügyeleti központban frissített adatmegőrzési szabályok nem alkalmazzák a postafiókokat vagy elemek nem kerülnek az archív postaládába áthelyezték vagy törölték. 
  
 **Alapvető okok:**
  
- Ez azért lehet, mert a **Kezelt Mappakezelő** nem dolgozta fel a felhasználó postafiókját. A kezelt Mappakezelő próbálja feldolgozni a felhőalapú szervezet hét naponta minden postaláda. Ha módosítja egy adatmegőrzési címkét vagy különböző adatmegőrzési szabály alkalmazása egy postaládához, megvárhatja, mindaddig, amíg a kezelt mappa segítő dolgozza fel a postaláda, vagy a kezelt Mappakezelő feldolgozni egy adott el a Start-ManagedFolderAssistant parancsmag futtatása a postafiókot. Ez a parancsmag fut akkor hasznos, tesztelésére és hibaelhárítására adatmegőrzési vagy adatmegőrzési címke beállításai. További információért látogassa meg [futtatni a kezelt Mappakezelő](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Megoldás:** Elindítani a kezelt Mappakezelő adott postaládához a következő parancsot futtassa:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Ez is lehet jelentkezhet, ha **RetentionHold** volt **engedélyezett** a postaládához. Ha a postaláda került a RetentionHold, az a postaláda adatmegőrzési nem lehet feldolgozni ez idő alatt. Vonatkozó további információk a RetentionHold beállítást lásd: [Postaláda adatmegőrzési tartsa](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Megoldás:**
    
  - A RetentionHold beállítást az adott postafiókhoz [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)állapotának ellenőrzése:
    
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
 
Adatmegőrzési szabályok az Exchange felügyeleti központban található további információ az alábbi témakörökben található:
- [Adatmegőrzési címkéket és adatmegőrzési szabályok](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Postafiókok adatmegőrzési szabály alkalmazása](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [És adatmegőrzési címkék törlése](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Tartás típusának azonosítása fektetni postafiók](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
