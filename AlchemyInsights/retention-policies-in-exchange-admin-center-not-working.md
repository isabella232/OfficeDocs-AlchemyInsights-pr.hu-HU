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
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="3266f-102">Adatmegőrzési házirendek az Exchange felügyeleti központban</span><span class="sxs-lookup"><span data-stu-id="3266f-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="3266f-103">Ha azt szeretné, hogy az alábbi beállítások automatikus ellenőrzését végezze el, válassza a vissza < gombot a lap tetején, és írja be annak a felhasználónak az e-mail-címét, aki problémákat tapasztal az adatmegőrzési szabályokkal kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="3266f-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="3266f-104">**Probléma:** Az Exchange felügyeleti központban újonnan létrehozott vagy frissített adatmegőrzési házirendek nem vonatkoznak postaládákra vagy elemekre, nem az archív postaládába kerülnek, vagy törlődnek.</span><span class="sxs-lookup"><span data-stu-id="3266f-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="3266f-105">**Kiváltó okok:**</span><span class="sxs-lookup"><span data-stu-id="3266f-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="3266f-106">Ennek oka az lehet, hogy a **felügyelt mappa segéd** nem dolgozza fel a felhasználó postaládáját.</span><span class="sxs-lookup"><span data-stu-id="3266f-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="3266f-107">A felügyelt mappa segéd hét naponta egyszer megkísérli feldolgozni a felhőalapú szervezet minden postaládáját.</span><span class="sxs-lookup"><span data-stu-id="3266f-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="3266f-108">Ha módosítja egy adatmegőrzési címkét, vagy eltérő adatmegőrzési házirendet alkalmaz egy postaládára, megvárhatja, amíg a felügyelt mappa támogatása feldolgozza a postaládát, vagy a Start-ManagedFolderAssistant parancsmag futtatásával elindíthatja a felügyelt mappa segédjét egy adott postaláda feldolgozásához.</span><span class="sxs-lookup"><span data-stu-id="3266f-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="3266f-109">Ez a parancsmag akkor hasznos, ha adatmegőrzési házirendet vagy adatmegőrzési címke beállításait teszteli vagy hibaelhárítás céljából használja.</span><span class="sxs-lookup"><span data-stu-id="3266f-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="3266f-110">További információért olvassa el [a felügyelt mappa segéd futtatása](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)című témakört.</span><span class="sxs-lookup"><span data-stu-id="3266f-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="3266f-111">**Megoldás:** Az alábbi parancsot futtatva indítsa el a felügyelt mappa segédjét egy adott postaládához:</span><span class="sxs-lookup"><span data-stu-id="3266f-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="3266f-112">Ez akkor is előfordulhat, ha a **RetentionHold** **engedélyezve** van a postaládában.</span><span class="sxs-lookup"><span data-stu-id="3266f-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="3266f-113">Ha a postaláda egy RetentionHold van elhelyezve, a postaláda adatmegőrzési házirendjét a program nem dolgozza fel az adott idő alatt.</span><span class="sxs-lookup"><span data-stu-id="3266f-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="3266f-114">További információk a RetentionHold beállításáról a postaláda- [adatmegőrzési mentesség](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)című témakörben olvashat.</span><span class="sxs-lookup"><span data-stu-id="3266f-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="3266f-115">**Megoldás**</span><span class="sxs-lookup"><span data-stu-id="3266f-115">**Solution:**</span></span>
    
  - <span data-ttu-id="3266f-116">Ellenőrizze az [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)-kiszolgálón az adott postaládában lévő RetentionHold beállítás állapotát:</span><span class="sxs-lookup"><span data-stu-id="3266f-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="3266f-117">A következő parancs futtatásával **letilthatja** a RetentionHold egy adott postaládában:</span><span class="sxs-lookup"><span data-stu-id="3266f-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="3266f-118">Ezután futtassa újra a felügyelt mappa Segédet:</span><span class="sxs-lookup"><span data-stu-id="3266f-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="3266f-119">**Megjegyzés:** Ha egy postaláda 10 MB-nál kisebb, akkor a felügyelt mappa Segéd nem dolgozza fel automatikusan a postaládát.</span><span class="sxs-lookup"><span data-stu-id="3266f-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="3266f-120">Az Exchange felügyeleti központban az adatmegőrzési házirendekről további információt a következő témakörökben talál:</span><span class="sxs-lookup"><span data-stu-id="3266f-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="3266f-121">Adatmegőrzési címkék és adatmegőrzési házirendek</span><span class="sxs-lookup"><span data-stu-id="3266f-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="3266f-122">Adatmegőrzési szabály alkalmazása postaládákra</span><span class="sxs-lookup"><span data-stu-id="3266f-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="3266f-123">Adatmegőrzési Címkék hozzáadása és eltávolítása</span><span class="sxs-lookup"><span data-stu-id="3266f-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="3266f-124">Egy postaládában elhelyezett mentesség típusának megállapítása</span><span class="sxs-lookup"><span data-stu-id="3266f-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
