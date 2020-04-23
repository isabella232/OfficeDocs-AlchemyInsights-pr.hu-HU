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
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="9d9c5-102">Adatmegőrzési házirendek az Exchange Felügyeleti központban</span><span class="sxs-lookup"><span data-stu-id="9d9c5-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="9d9c5-103">**Probléma:** Az Exchange Felügyeleti központban az újonnan létrehozott vagy frissített adatmegőrzési házirendek nem vonatkoznak a postaládákra, vagy az elemek nem kerülnek át az archív postaládába, és nem törlődnek.</span><span class="sxs-lookup"><span data-stu-id="9d9c5-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="9d9c5-104">**Kiváltó okok:**</span><span class="sxs-lookup"><span data-stu-id="9d9c5-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="9d9c5-105">Ennek az lehet az oka, hogy a **Felügyelt mappasegéd** nem dolgozta fel a felhasználó postaládáját.</span><span class="sxs-lookup"><span data-stu-id="9d9c5-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="9d9c5-106">A Felügyelt mappasegéd hétnaponta egyszer próbálja meg feldolgozni a felhőalapú szervezet összes postaládáját.</span><span class="sxs-lookup"><span data-stu-id="9d9c5-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="9d9c5-107">Ha módosítja az adatmegőrzési címkét, vagy más adatmegőrzési szabályt alkalmaz egy postaládára, megvárhatja, amíg a Felügyelt mappasegéd feldolgozza a postaládát, vagy a Start-ManagedFolderAssistant parancsmag futtatásával elindíthatja a Felügyelt mappasegédet egy adott postaláda feldolgozásához.</span><span class="sxs-lookup"><span data-stu-id="9d9c5-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="9d9c5-108">A parancsmag futtatása adatmegőrzési házirend vagy adatmegőrzési címke beállításainak teszteléséhez vagy hibaelhárításához hasznos.</span><span class="sxs-lookup"><span data-stu-id="9d9c5-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="9d9c5-109">További információt [a Felügyelt mappasegéd futtatása](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)című területen talál.</span><span class="sxs-lookup"><span data-stu-id="9d9c5-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="9d9c5-110">**Megoldás:** A következő parancs futtatásával indítsa el a felügyelt mappasegédet egy adott postaládához:</span><span class="sxs-lookup"><span data-stu-id="9d9c5-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="9d9c5-111">Ez akkor is előfordulhat, ha a **RetentionHold** **engedélyezve** van a postaládán.</span><span class="sxs-lookup"><span data-stu-id="9d9c5-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="9d9c5-112">Ha a postaláda egy retentionholdra került, a postaláda adatmegőrzési szabálya ez idő alatt nem lesz feldolgozva.</span><span class="sxs-lookup"><span data-stu-id="9d9c5-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="9d9c5-113">További informaton a RetentionHold beállítás lásd: [Postaláda megőrzése hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="9d9c5-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="9d9c5-114">**Megoldás:**</span><span class="sxs-lookup"><span data-stu-id="9d9c5-114">**Solution:**</span></span>
    
  - <span data-ttu-id="9d9c5-115">Ellenőrizze az RetentionHold beállítás állapotát az [EXO powershell adott postaládáján:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="9d9c5-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="9d9c5-116">Futtassa a következő parancsot az RetentionHold **letiltásához** egy adott postaládán:</span><span class="sxs-lookup"><span data-stu-id="9d9c5-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="9d9c5-117">Most futtassa újra a Felügyelt mappasegédet:</span><span class="sxs-lookup"><span data-stu-id="9d9c5-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="9d9c5-118">**Megjegyzés:** Ha egy postaláda 10 MB-nál kisebb, a Felügyelt mappasegéd nem dolgozza fel automatikusan a postaládát.</span><span class="sxs-lookup"><span data-stu-id="9d9c5-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="9d9c5-119">Az Exchange Felügyeleti központban található adatmegőrzési házirendekről az:</span><span class="sxs-lookup"><span data-stu-id="9d9c5-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="9d9c5-120">Adatmegőrzési címkék és adatmegőrzési házirendek</span><span class="sxs-lookup"><span data-stu-id="9d9c5-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="9d9c5-121">Adatmegőrzési szabály alkalmazása postaládákra</span><span class="sxs-lookup"><span data-stu-id="9d9c5-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="9d9c5-122">Adatmegőrzési címkék hozzáadása vagy eltávolítása</span><span class="sxs-lookup"><span data-stu-id="9d9c5-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="9d9c5-123">A postaládára helyezett várakoztatás típusának azonosítása</span><span class="sxs-lookup"><span data-stu-id="9d9c5-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
