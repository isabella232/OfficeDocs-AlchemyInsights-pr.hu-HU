---
title: a 1336 RecoverableItems mappája megtelt
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741269"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="07b10-102">A helyreállítható elemek mappa megtelt</span><span class="sxs-lookup"><span data-stu-id="07b10-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="07b10-103">Az Exchange Online-postaládák esetében a helyreállítható elemek mappa alapértelmezett tárterülete 30 GB.</span><span class="sxs-lookup"><span data-stu-id="07b10-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="07b10-104">A helyreállítható elemek mappa tárterülete automatikusan 100 GB-ra növekszik, ha a postaláda jogellenes tartásra, eDiscovery tartása vagy adatmegőrzési házirendhez van rendelve.</span><span class="sxs-lookup"><span data-stu-id="07b10-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="07b10-105">Ha a helyreállítható elemek mappa eléri a tárterületet, a postaláda működését az alábbi módokon érinti:</span><span class="sxs-lookup"><span data-stu-id="07b10-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="07b10-106">A felhasználó nem tud elemeket törölni a postaládából.</span><span class="sxs-lookup"><span data-stu-id="07b10-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="07b10-107">A felügyelt mappa Segéd nem tudja törölni az elemeket adatmegőrzési címke vagy a felügyelt mappa beállításai alapján.</span><span class="sxs-lookup"><span data-stu-id="07b10-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="07b10-108">Az egyelemes helyreállítást engedélyező vagy felfüggesztett postaládák esetén a copy-on-Write lap védelmi folyamata nem tudja megőrizni a felhasználó által szerkesztett elemek verziószámát.</span><span class="sxs-lookup"><span data-stu-id="07b10-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="07b10-109">Ha a postaláda-naplózás engedélyezve van, a postaláda-naplózási bejegyzéseket nem lehet menteni a helyreállítható elemek mappa naplózási almappájában.</span><span class="sxs-lookup"><span data-stu-id="07b10-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="07b10-110">A nem tartott postaládák esetében a rendszergazdák az `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Exchange Online PowerShellben a parancs segítségével törölhetik az elemeket a helyreállítható elemek mappában.</span><span class="sxs-lookup"><span data-stu-id="07b10-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="07b10-111">További tudnivalókat a következő témakörökben talál:</span><span class="sxs-lookup"><span data-stu-id="07b10-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="07b10-112">Üzenetek keresése és törlése</span><span class="sxs-lookup"><span data-stu-id="07b10-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="07b10-113">Keresés a postaládában</span><span class="sxs-lookup"><span data-stu-id="07b10-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="07b10-114">A levezetett postaládák esetében a rendszergazdáknak el kell távolítaniuk a mentességet, mielőtt a helyreállítható elemek mappából törölt elemek.</span><span class="sxs-lookup"><span data-stu-id="07b10-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="07b10-115">További tudnivalókat az [elemek törlése a felhőalapú postaládák visszanyerhető elemek mappájából lenyomva](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="07b10-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="07b10-116">Ha meg szeretné akadályozni, hogy a helyreállítható elemek mappa teljes mértékben megmaradjon, a rendszergazdák növelhetik a helyreállítható elemek mappa tárolási korlátját, és beállíthatja a postaláda-adatmegőrzési házirendet, amely áthelyezi az elemeket a helyreállítható elemek mappából a felhasználó archív postaládájába.</span><span class="sxs-lookup"><span data-stu-id="07b10-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="07b10-117">Lásd: [a helyreállítható elemek visszanyerhető kvótájának növelése a letartott postaládákban](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="07b10-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
