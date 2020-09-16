---
title: Nem működött az adatmegőrzési házirendek az Exchange felügyeleti központban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740512"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Adatmegőrzési házirendek az Exchange felügyeleti központban

Ha azt szeretné, hogy az alábbi beállítások automatikus ellenőrzését végezze el, válassza a vissza < gombot a lap tetején, és írja be annak a felhasználónak az e-mail-címét, aki problémákat tapasztal az adatmegőrzési szabályokkal kapcsolatban.

 **Probléma:** Az Exchange felügyeleti központban újonnan létrehozott vagy frissített adatmegőrzési házirendek nem vonatkoznak postaládákra vagy elemekre, nem az archív postaládába kerülnek, vagy törlődnek. 
  
 **Kiváltó okok:**
  
- Ennek oka az lehet, hogy a **felügyelt mappa segéd** nem dolgozza fel a felhasználó postaládáját. A felügyelt mappa segéd hét naponta egyszer megkísérli feldolgozni a felhőalapú szervezet minden postaládáját. Ha módosítja egy adatmegőrzési címkét, vagy eltérő adatmegőrzési házirendet alkalmaz egy postaládára, megvárhatja, amíg a felügyelt mappa támogatása feldolgozza a postaládát, vagy a Start-ManagedFolderAssistant parancsmag futtatásával elindíthatja a felügyelt mappa segédjét egy adott postaláda feldolgozásához. Ez a parancsmag akkor hasznos, ha adatmegőrzési házirendet vagy adatmegőrzési címke beállításait teszteli vagy hibaelhárítás céljából használja. További információért olvassa el [a felügyelt mappa segéd futtatása](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)című témakört.
    
  - **Megoldás:** Az alábbi parancsot futtatva indítsa el a felügyelt mappa segédjét egy adott postaládához:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Ez akkor is előfordulhat, ha a **RetentionHold** **engedélyezve** van a postaládában. Ha a postaláda egy RetentionHold van elhelyezve, a postaláda adatmegőrzési házirendjét a program nem dolgozza fel az adott idő alatt. További információk a RetentionHold beállításáról a postaláda- [adatmegőrzési mentesség](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)című témakörben olvashat.
    
    **Megoldás**
    
  - Ellenőrizze az [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)-kiszolgálón az adott postaládában lévő RetentionHold beállítás állapotát:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - A következő parancs futtatásával **letilthatja** a RetentionHold egy adott postaládában:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Ezután futtassa újra a felügyelt mappa Segédet:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Megjegyzés:** Ha egy postaláda 10 MB-nál kisebb, akkor a felügyelt mappa Segéd nem dolgozza fel automatikusan a postaládát.
 
Az Exchange felügyeleti központban az adatmegőrzési házirendekről további információt a következő témakörökben talál:
- [Adatmegőrzési címkék és adatmegőrzési házirendek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Adatmegőrzési szabály alkalmazása postaládákra](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Adatmegőrzési Címkék hozzáadása és eltávolítása](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Egy postaládában elhelyezett mentesség típusának megállapítása](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
