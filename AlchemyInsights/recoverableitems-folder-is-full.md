---
title: 1336 RecoverableItems mappa megtelt
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720254"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="d21bf-102">A Helyreállítható elemek mappa megtelt</span><span class="sxs-lookup"><span data-stu-id="d21bf-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="d21bf-103">Exchange Online-postaládák esetén a Helyreállítható elemek mappa alapértelmezett tárolási korlátja 30 GB.</span><span class="sxs-lookup"><span data-stu-id="d21bf-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="d21bf-104">A Helyreállítható elemek mappa tárolási korlátja automatikusan 100 GB-ra nő, ha a postaláda peres eljárás miatti tartásba, elektronikus adatfeltárási visszatartásba kerül, vagy adatmegőrzési házirendhez van rendelve.</span><span class="sxs-lookup"><span data-stu-id="d21bf-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="d21bf-105">Amikor a Helyreállítható elemek mappa eléri a tárolási korlátot, a postaláda funkciója a következő módokon változik:</span><span class="sxs-lookup"><span data-stu-id="d21bf-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="d21bf-106">A felhasználó nem törölhet elemeket a postaládából.</span><span class="sxs-lookup"><span data-stu-id="d21bf-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="d21bf-107">A Felügyelt mappasegéd nem tudja törölni az elemeket az adatmegőrzési címke vagy a kezelt mappa beállításai alapján.</span><span class="sxs-lookup"><span data-stu-id="d21bf-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="d21bf-108">Az on-item recovery engedélyezve van vagy várakoztatott postaládák esetében az írásra másolási oldal védelmi folyamata nem tudja karbantartani a felhasználó által szerkesztett elemek verzióit.</span><span class="sxs-lookup"><span data-stu-id="d21bf-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="d21bf-109">Azon postaládák esetében, amelyeknél engedélyezve van a postaláda naplózása, a Helyreállítható elemek mappa Naplózás almappájába nem lehet postaláda-naplóbejegyzéseket menteni.</span><span class="sxs-lookup"><span data-stu-id="d21bf-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="d21bf-110">A nem várakoztatott postaládák esetén a `Search-Mailbox -SearchDumpsterOnly -DeleteContent` rendszergazdák az Exchange Online PowerShell parancsával törölhetik a Helyreállítható elemek mappában lévő elemeket.</span><span class="sxs-lookup"><span data-stu-id="d21bf-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="d21bf-111">További tudnivalókat a következő témakörökben talál:</span><span class="sxs-lookup"><span data-stu-id="d21bf-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="d21bf-112">Üzenetek keresése és törlése</span><span class="sxs-lookup"><span data-stu-id="d21bf-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="d21bf-113">Keresés-postaláda</span><span class="sxs-lookup"><span data-stu-id="d21bf-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="d21bf-114">A várakoztatott postaládák esetében a rendszergazdáknak el kell távolítaniuk a visszatartást, mielőtt törölhetik az elemeket a Helyreállítható elemek mappából.</span><span class="sxs-lookup"><span data-stu-id="d21bf-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="d21bf-115">További információt az [Elemek törlése a felhőalapú postaládák visszatartott helyreállítható elemek mappájában című témakörben talál.](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)</span><span class="sxs-lookup"><span data-stu-id="d21bf-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="d21bf-116">A Helyreállítható elemek mappa megteltsíthetőj, a rendszergazdák növelhetik a visszatartott postaládák Helyreállítható elemek mappájának tárolási korlátját, és beállíthatnak egy postaláda-adatmegőrzési házirendet, amely a Helyreállítható elemek mappából a felhasználó archív postaládájába helyezi át az elemeket.</span><span class="sxs-lookup"><span data-stu-id="d21bf-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="d21bf-117">Lásd: [A visszatartott postaládák helyreállítható elemek kvótájának növelése.](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)</span><span class="sxs-lookup"><span data-stu-id="d21bf-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
