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
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 56c2bea5e205358d0ef29fa937e36a88ffc46a1e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761584"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="53390-102">Az Exchange felügyeleti központ adatmegőrzési szabályok</span><span class="sxs-lookup"><span data-stu-id="53390-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="53390-103">**Hiba:** Az újonnan létrehozott, vagy az Exchange felügyeleti központban frissített adatmegőrzési szabályok nem alkalmazzák a postafiókokat vagy elemek nem kerülnek az archív postaládába áthelyezték vagy törölték.</span><span class="sxs-lookup"><span data-stu-id="53390-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="53390-104">**Alapvető okok:**</span><span class="sxs-lookup"><span data-stu-id="53390-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="53390-105">Ez azért lehet, mert a **Kezelt Mappakezelő** nem dolgozta fel a felhasználó postafiókját.</span><span class="sxs-lookup"><span data-stu-id="53390-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="53390-106">A kezelt Mappakezelő próbálja feldolgozni a felhőalapú szervezet hét naponta minden postaláda.</span><span class="sxs-lookup"><span data-stu-id="53390-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="53390-107">Ha módosítja egy adatmegőrzési címkét vagy különböző adatmegőrzési szabály alkalmazása egy postaládához, megvárhatja, mindaddig, amíg a kezelt mappa segítő dolgozza fel a postaláda, vagy a kezelt Mappakezelő feldolgozni egy adott el a Start-ManagedFolderAssistant parancsmag futtatása a postafiókot.</span><span class="sxs-lookup"><span data-stu-id="53390-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="53390-108">Ez a parancsmag fut akkor hasznos, tesztelésére és hibaelhárítására adatmegőrzési vagy adatmegőrzési címke beállításai.</span><span class="sxs-lookup"><span data-stu-id="53390-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="53390-109">További információért látogassa meg [futtatni a kezelt Mappakezelő](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="53390-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="53390-110">**Megoldás:** Elindítani a kezelt Mappakezelő adott postaládához a következő parancsot futtassa:</span><span class="sxs-lookup"><span data-stu-id="53390-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="53390-111">Ez is lehet jelentkezhet, ha **RetentionHold** volt **engedélyezett** a postaládához.</span><span class="sxs-lookup"><span data-stu-id="53390-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="53390-112">Ha a postaláda került a RetentionHold, az a postaláda adatmegőrzési nem lehet feldolgozni ez idő alatt.</span><span class="sxs-lookup"><span data-stu-id="53390-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="53390-113">Vonatkozó további információk a RetentionHold beállítást lásd: [Postaláda adatmegőrzési tartsa](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="53390-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="53390-114">**Megoldás:**</span><span class="sxs-lookup"><span data-stu-id="53390-114">**Solution:**</span></span>
    
  - <span data-ttu-id="53390-115">A RetentionHold beállítást az adott postafiókhoz [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)állapotának ellenőrzése:</span><span class="sxs-lookup"><span data-stu-id="53390-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="53390-116">Egy adott postaláda **letiltása** RetentionHold a következő parancsot futtassa:</span><span class="sxs-lookup"><span data-stu-id="53390-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="53390-117">Most futtassa újra a kezelt mappa segéd:</span><span class="sxs-lookup"><span data-stu-id="53390-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="53390-118">**Megjegyzés:** Ha a postafiók 10 MB-nál kisebb, a kezelt Mappakezelő nem dolgozza fel automatikusan a postafiókot.</span><span class="sxs-lookup"><span data-stu-id="53390-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

