---
title: E-mail-üzenetek áthelyezése az archív postaládába
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799782"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="ca1b3-102">E-mailek áthelyezése az archív postaládába</span><span class="sxs-lookup"><span data-stu-id="ca1b3-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="ca1b3-103">Ha azt szeretné, hogy az alábbi beállítások automatikus ellenőrzését végezze el, válassza a vissza < gombot a lap tetején, és írja be annak a felhasználónak az e-mail-címét, aki problémákat tapasztal az e-mailek archív postaládájába való áthelyezésével kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="ca1b3-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="ca1b3-104">Ellenőrizze, hogy engedélyezve van-e egy **archív postaláda** .</span><span class="sxs-lookup"><span data-stu-id="ca1b3-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="ca1b3-105">Ha nem, akkor a [jelen cikkben](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) található lépéseket követve engedélyezze az archív postaládát.</span><span class="sxs-lookup"><span data-stu-id="ca1b3-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="ca1b3-106">Ha automatikusan szeretné archiválni az üzeneteket az archív postaládába, az **Áthelyezés az archiválási** eljárásra beállításnál a **teljes postaláda (alapértelmezett) címkére kell alkalmazni**az adatmegőrzési címkét.</span><span class="sxs-lookup"><span data-stu-id="ca1b3-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="ca1b3-107">Az alábbi lépésekkel hozhatja létre a címkét: [Archívum alapértelmezett címke](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="ca1b3-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="ca1b3-108">Ezután adja hozzá az **archív** címkét az adatmegőrzési házirendhez.</span><span class="sxs-lookup"><span data-stu-id="ca1b3-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="ca1b3-109">Az Exchange felügyeleti központban válassza az **adatmegőrzési házirendek** > az **Áthelyezés az archívumba címkét** a házirend > **Mentés**elemre.</span><span class="sxs-lookup"><span data-stu-id="ca1b3-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="ca1b3-110">Most [rendelje az adatmegőrzési házirendet](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) az adott felhasználó postaládájához.</span><span class="sxs-lookup"><span data-stu-id="ca1b3-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="ca1b3-111">Ugyanezt a házirendet alkalmazza mind az **elsődleges** , mind az **archív** postaládára.</span><span class="sxs-lookup"><span data-stu-id="ca1b3-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="ca1b3-112">Előfordulhat, hogy a felügyelt mappa Segédének (MFA) kell kikényszeríteni, hogy fusson, és az új beállításokat alkalmazza a felhasználó postaládájába.</span><span class="sxs-lookup"><span data-stu-id="ca1b3-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="ca1b3-113">Futtassa az alábbi parancsot, miközben az [EXO powershellhez csatlakozik](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , és egy adott postaládához szeretné elindítani a felügyelt mappa Segédet:</span><span class="sxs-lookup"><span data-stu-id="ca1b3-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="ca1b3-114">Start – ManagedFolderAssistant – identitás <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="ca1b3-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="ca1b3-115">Az archiválási házirend beállításáról további információt a [postaládák archiválási és törlési házirendjének beállítása](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="ca1b3-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  