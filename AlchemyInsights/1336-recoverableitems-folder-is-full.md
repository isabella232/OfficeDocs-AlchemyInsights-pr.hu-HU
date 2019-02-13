---
title: 1336 RecoverableItems mappa megtelt
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: dbf4930c34e4175a14b77fab4eafc953bb37cc02
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29909290"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="326bc-102">A helyreállítható elemek mappa megtelt.</span><span class="sxs-lookup"><span data-stu-id="326bc-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="326bc-p101">A helyreállítható elemek mappa alapértelmezett tárolási korlátját az Office 365 rendszerben az Exchange Online postafiókok 30 GB. A helyreállítható elemek mappa tárolási korlátját automatikusan nő a 100 GB-os, amikor a postaláda helyezett per tartsa lenyomva tartás elektronikus adatok feltárása, vagy az Office 365 adatmegőrzési házirend hozzá van rendelve.</span><span class="sxs-lookup"><span data-stu-id="326bc-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="326bc-105">Ha a helyreállítható elemek mappa eléri a tárolási korlát, postafiók funkció hatással van a következő módon:</span><span class="sxs-lookup"><span data-stu-id="326bc-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="326bc-106">A felhasználó az elemek nem törölhetők a postaládából.</span><span class="sxs-lookup"><span data-stu-id="326bc-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="326bc-107">A kezelt Mappakezelő nem törölhető elemek adatmegőrzési címke vagy kezelt mappa beállításai alapján.</span><span class="sxs-lookup"><span data-stu-id="326bc-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="326bc-108">A postafiókokhoz, vagy egyetlen elem helyreállítása engedélyezve van a Másolás írás közbeni lap védelem folyamatának a felhasználó által szerkeszthető elemek verziói nem tudja kezelni.</span><span class="sxs-lookup"><span data-stu-id="326bc-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="326bc-109">-Postafiókok, amelyek rendelkeznek a postaláda-naplózás engedélyezve van postafiók napló bejegyzések a helyreállítható elemek mappában lévő eseményeket almappájába menti.</span><span class="sxs-lookup"><span data-stu-id="326bc-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="326bc-p102">Nem mentesített postafiókok, rendszergazdák használhatják a `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Exchange Online PowerShell a helyreállítható elemek mappa elemeinek törlése parancsot. További információt a következő témakörökben talál:</span><span class="sxs-lookup"><span data-stu-id="326bc-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="326bc-112">Keresse meg és törölje a szükségtelen üzeneteket</span><span class="sxs-lookup"><span data-stu-id="326bc-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="326bc-113">Keresés-postafiók</span><span class="sxs-lookup"><span data-stu-id="326bc-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="326bc-p103">Visszatartott postafiókok rendszergazdák kell távolítsa el a mentesség, mielőtt azok a helyreállítható elemek mappából törölt elemek is. További tudnivalók: [törli az elemeket a helyreállítható elemek mappájában lévő felhőalapú postaládákba tartsa](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="326bc-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="326bc-p104">A helyreállítható elemek mappa teljes ne megelőzése érdekében rendszergazdák növelheti a helyreállítható elemek mappa postaládára tartsa, és állítsa be, hogy az elemek a helyreállítható elemek mappába helyez át a felhasználó archív postaláda adatmegőrzési tárolási korlátját a postafiókot. Lásd [a helyreállítható elemek tartsa postaládára vonatkozó kvóta növelése](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="326bc-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

