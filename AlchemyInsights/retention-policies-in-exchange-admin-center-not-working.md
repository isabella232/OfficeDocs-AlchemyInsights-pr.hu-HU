---
title: Nem működik az Exchange Felügyeleti központ adatmegőrzési házirendjei
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742435"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Adatmegőrzési házirendek az Exchange Felügyeleti központban

 **Probléma:** Az Exchange Felügyeleti központban az újonnan létrehozott vagy frissített adatmegőrzési házirendek nem vonatkoznak a postaládákra, vagy az elemek nem kerülnek át az archív postaládába, és nem törlődnek. 
  
 **Kiváltó okok:**
  
- Ennek az lehet az oka, hogy a **Felügyelt mappasegéd** nem dolgozta fel a felhasználó postaládáját. A Felügyelt mappasegéd hétnaponta egyszer próbálja meg feldolgozni a felhőalapú szervezet összes postaládáját. Ha módosítja az adatmegőrzési címkét, vagy más adatmegőrzési szabályt alkalmaz egy postaládára, megvárhatja, amíg a Felügyelt mappasegéd feldolgozza a postaládát, vagy a Start-ManagedFolderAssistant parancsmag futtatásával elindíthatja a Felügyelt mappasegédet egy adott postaláda feldolgozásához. A parancsmag futtatása adatmegőrzési házirend vagy adatmegőrzési címke beállításainak teszteléséhez vagy hibaelhárításához hasznos. További információt [a Felügyelt mappasegéd futtatása](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)című területen talál.
    
  - **Megoldás:** A következő parancs futtatásával indítsa el a felügyelt mappasegédet egy adott postaládához:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Ez akkor is előfordulhat, ha a **RetentionHold** **engedélyezve** van a postaládán. Ha a postaláda egy retentionholdra került, a postaláda adatmegőrzési szabálya ez idő alatt nem lesz feldolgozva. További informaton a RetentionHold beállítás lásd: [Postaláda megőrzése hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Megoldás:**
    
  - Ellenőrizze az RetentionHold beállítás állapotát az [EXO powershell adott postaládáján:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Futtassa a következő parancsot az RetentionHold **letiltásához** egy adott postaládán:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Most futtassa újra a Felügyelt mappasegédet:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Megjegyzés:** Ha egy postaláda 10 MB-nál kisebb, a Felügyelt mappasegéd nem dolgozza fel automatikusan a postaládát.
 
Az Exchange Felügyeleti központban található adatmegőrzési házirendekről az:
- [Adatmegőrzési címkék és adatmegőrzési házirendek](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Adatmegőrzési szabály alkalmazása postaládákra](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Adatmegőrzési címkék hozzáadása vagy eltávolítása](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [A postaládára helyezett várakoztatás típusának azonosítása](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
