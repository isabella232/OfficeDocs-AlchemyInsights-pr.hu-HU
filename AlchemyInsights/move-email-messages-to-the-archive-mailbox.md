---
title: E-mailek áthelyezése az archív postaláda
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941713"
---
<span data-ttu-id="aa29a-p101">A problémák az archív postaládába elemek archiválását. Ellenőrizze, hogy a hajtott végre a következő lépéseket:</span><span class="sxs-lookup"><span data-stu-id="aa29a-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="aa29a-p102">Győződjön meg arról, hogy a **postaláda archiválása** engedélyezve van. Ha nem, [Ez a cikk](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) lépések segítségével engedélyezze az archív postaláda.</span><span class="sxs-lookup"><span data-stu-id="aa29a-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="aa29a-106">Az Exchange felügyeleti központ **Adatmegőrzési címkék** **Való kezelés**alatt válassza ki, az **Archív Ugrás** műveletet a kívánt **Megőrzési kor**tartalmazó **adatmegőrzési címke** létrehozása.</span><span class="sxs-lookup"><span data-stu-id="aa29a-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="aa29a-107">Az Exchange felügyeleti központ **Adatmegőrzési szabályok**kiválasztása, **Adatmegőrzési szabály** létrehozása és az **archívum áthelyezése** adatmegőrzési címke hozzáadása házirendhez.</span><span class="sxs-lookup"><span data-stu-id="aa29a-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="aa29a-p103">[A megőrzési házirendet](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) az adott felhasználó postaládájához. Ugyanaz a házirend az **elsődleges** és az **Archív** postaláda vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="aa29a-p103">[Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="aa29a-p104">A felhasználó postafiókja elemek áthelyezése az archív postaláda archiválási házirend most már látnia kell. A kezelt mappa Segéd (MFA) és az új beállítások alkalmazása a felhasználó postaládájában, hogy szükség lehet. Futtassa a következő parancsot közben [csatlakoztatva EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) indítása a kezelt Mappakezelő egy adott postaláda:</span><span class="sxs-lookup"><span data-stu-id="aa29a-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="aa29a-113">Archiválási házirend beállításával kapcsolatos további információra van szükségünk, lásd: [postafiókok az archív és törlési házirend beállítása](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="aa29a-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

