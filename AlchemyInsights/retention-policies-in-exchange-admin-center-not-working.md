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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473805"
---
 <span data-ttu-id="b44fd-102">**Hiba:** Az újonnan létrehozott, vagy az Exchange felügyeleti központban frissített adatmegőrzési szabályok nem alkalmazzák a postafiókokat vagy elemek nem kerülnek az archív postaládába áthelyezték vagy törölték.</span><span class="sxs-lookup"><span data-stu-id="b44fd-102">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="b44fd-103">**Alapvető okok:**</span><span class="sxs-lookup"><span data-stu-id="b44fd-103">**Root Causes:**</span></span>
  
- <span data-ttu-id="b44fd-p101">Ez azért lehet, mert a **Kezelt Mappakezelő** nem dolgozta fel a felhasználó postafiókját. A kezelt Mappakezelő próbálja feldolgozni a felhőalapú szervezet hét naponta minden postaláda. Ha módosítja egy adatmegőrzési címkét vagy különböző adatmegőrzési szabály alkalmazása egy postaládához, megvárhatja, mindaddig, amíg a kezelt mappa segítő dolgozza fel a postaláda, vagy a kezelt Mappakezelő feldolgozni egy adott el a Start-ManagedFolderAssistant parancsmag futtatása a postafiókot. Ez a parancsmag fut akkor hasznos, tesztelésére és hibaelhárítására adatmegőrzési vagy adatmegőrzési címke beállításai. További információért látogassa meg [futtatni a kezelt Mappakezelő](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="b44fd-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="b44fd-109">**Megoldás:** Elindítani a kezelt Mappakezelő adott postaládához a következő parancsot futtassa:</span><span class="sxs-lookup"><span data-stu-id="b44fd-109">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="b44fd-p102">Ez is lehet jelentkezhet, ha **RetentionHold** volt **engedélyezett** a postaládához. Ha a postaláda került a RetentionHold, az a postaláda adatmegőrzési nem lehet feldolgozni ez idő alatt. Vonatkozó további információk a RetentionHold beállítást lásd: [Postaláda adatmegőrzési tartsa](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="b44fd-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="b44fd-113">Megoldás</span><span class="sxs-lookup"><span data-stu-id="b44fd-113">**Solution:**</span></span>
    
  - <span data-ttu-id="b44fd-114">A RetentionHold beállítást az adott postafiókhoz [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)állapotának ellenőrzése:</span><span class="sxs-lookup"><span data-stu-id="b44fd-114">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="b44fd-115">Egy adott postaláda **letiltása** RetentionHold a következő parancsot futtassa:</span><span class="sxs-lookup"><span data-stu-id="b44fd-115">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="b44fd-116">Most futtassa újra a kezelt mappa segéd:</span><span class="sxs-lookup"><span data-stu-id="b44fd-116">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="b44fd-117">**Megjegyzés:** Ha a postafiók 10 MB-nál kisebb, a kezelt Mappakezelő nem dolgozza fel automatikusan a postafiókot.</span><span class="sxs-lookup"><span data-stu-id="b44fd-117">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

