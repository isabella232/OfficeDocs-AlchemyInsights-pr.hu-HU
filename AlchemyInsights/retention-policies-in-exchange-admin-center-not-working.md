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
ms.openlocfilehash: d0af4c933f262fe1ec4c2a6ff16d5f6195398b0d
ms.sourcegitcommit: e98443a049108e0dc83d63895af66944bdb1f108
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/16/2019
ms.locfileid: "36444810"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="fe33a-102">Az Exchange felügyeleti központ adatmegőrzési szabályok</span><span class="sxs-lookup"><span data-stu-id="fe33a-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="fe33a-103">**Hiba:** Az újonnan létrehozott, vagy az Exchange felügyeleti központban frissített adatmegőrzési szabályok nem alkalmazzák a postafiókokat vagy elemek nem kerülnek az archív postaládába áthelyezték vagy törölték.</span><span class="sxs-lookup"><span data-stu-id="fe33a-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="fe33a-104">**Alapvető okok:**</span><span class="sxs-lookup"><span data-stu-id="fe33a-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="fe33a-105">Ez azért lehet, mert a **Kezelt Mappakezelő** nem dolgozta fel a felhasználó postafiókját.</span><span class="sxs-lookup"><span data-stu-id="fe33a-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="fe33a-106">A kezelt Mappakezelő próbálja feldolgozni a felhőalapú szervezet hét naponta minden postaláda.</span><span class="sxs-lookup"><span data-stu-id="fe33a-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="fe33a-107">Ha módosítja egy adatmegőrzési címkét vagy különböző adatmegőrzési szabály alkalmazása egy postaládához, megvárhatja, mindaddig, amíg a kezelt mappa segítő dolgozza fel a postaláda, vagy a kezelt Mappakezelő feldolgozni egy adott el a Start-ManagedFolderAssistant parancsmag futtatása a postafiókot.</span><span class="sxs-lookup"><span data-stu-id="fe33a-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="fe33a-108">Ez a parancsmag fut akkor hasznos, tesztelésére és hibaelhárítására adatmegőrzési vagy adatmegőrzési címke beállításai.</span><span class="sxs-lookup"><span data-stu-id="fe33a-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="fe33a-109">További információért látogassa meg [futtatni a kezelt Mappakezelő](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="fe33a-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="fe33a-110">**Megoldás:** Elindítani a kezelt Mappakezelő adott postaládához a következő parancsot futtassa:</span><span class="sxs-lookup"><span data-stu-id="fe33a-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="fe33a-111">Ez is lehet jelentkezhet, ha **RetentionHold** volt **engedélyezett** a postaládához.</span><span class="sxs-lookup"><span data-stu-id="fe33a-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="fe33a-112">Ha a postaláda került a RetentionHold, az a postaláda adatmegőrzési nem lehet feldolgozni ez idő alatt.</span><span class="sxs-lookup"><span data-stu-id="fe33a-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="fe33a-113">Vonatkozó további információk a RetentionHold beállítást lásd: [Postaláda adatmegőrzési tartsa](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="fe33a-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="fe33a-114">**Megoldás:**</span><span class="sxs-lookup"><span data-stu-id="fe33a-114">**Solution:**</span></span>
    
  - <span data-ttu-id="fe33a-115">A RetentionHold beállítást az adott postafiókhoz [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)állapotának ellenőrzése:</span><span class="sxs-lookup"><span data-stu-id="fe33a-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="fe33a-116">Egy adott postaláda **letiltása** RetentionHold a következő parancsot futtassa:</span><span class="sxs-lookup"><span data-stu-id="fe33a-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="fe33a-117">Most futtassa újra a kezelt mappa segéd:</span><span class="sxs-lookup"><span data-stu-id="fe33a-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="fe33a-118">**Megjegyzés:** Ha a postafiók 10 MB-nál kisebb, a kezelt Mappakezelő nem dolgozza fel automatikusan a postafiókot.</span><span class="sxs-lookup"><span data-stu-id="fe33a-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="fe33a-119">Adatmegőrzési szabályok az Exchange felügyeleti központban található további információ az alábbi témakörökben található:</span><span class="sxs-lookup"><span data-stu-id="fe33a-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="fe33a-120">Adatmegőrzési címkéket és adatmegőrzési szabályok</span><span class="sxs-lookup"><span data-stu-id="fe33a-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="fe33a-121">Postafiókok adatmegőrzési szabály alkalmazása</span><span class="sxs-lookup"><span data-stu-id="fe33a-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="fe33a-122">És adatmegőrzési címkék törlése</span><span class="sxs-lookup"><span data-stu-id="fe33a-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="fe33a-123">Tartás típusának azonosítása fektetni postafiók</span><span class="sxs-lookup"><span data-stu-id="fe33a-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/en-us/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
