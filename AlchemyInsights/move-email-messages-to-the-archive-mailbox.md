---
title: E-mailek áthelyezése az archív postaládába
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822164"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="d7553-102">E-mailek áthelyezése az archív postaládába</span><span class="sxs-lookup"><span data-stu-id="d7553-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="d7553-103">Ellenőrizze, hogy az **archív postaláda** engedélyezve van-e.</span><span class="sxs-lookup"><span data-stu-id="d7553-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="d7553-104">Ha nem, akkor az ebben a [cikkben](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) leírt lépésekkel engedélyezheti az archív postaládát.</span><span class="sxs-lookup"><span data-stu-id="d7553-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="d7553-105">Ha automatikusan szeretné archiválni az üzeneteket az archív postaládába, az **Áthelyezés az archiválandó** műveletre beállított adatmegőrzési címkét a **teljes postafiók (alapértelmezett) címke automatikus alkalmazására**kell állítani.</span><span class="sxs-lookup"><span data-stu-id="d7553-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="d7553-106">Használja a lépéseket ide, hogy megteremtse a tag: [Archívum default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="d7553-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="d7553-107">Ezután adja hozzá az **archív** címkét az adatmegőrzési szabályhoz.</span><span class="sxs-lookup"><span data-stu-id="d7553-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="d7553-108">Az Exchange felügyeleti központban válassza az **adatmegőrzési szabályok** > az **Áthelyezés az archív címkéhez** parancsot a > **Mentés**házirendbe.</span><span class="sxs-lookup"><span data-stu-id="d7553-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="d7553-109">[Rendelje hozzá az adatmegőrzési szabályt](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) az adott felhasználó postaládájához.</span><span class="sxs-lookup"><span data-stu-id="d7553-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="d7553-110">Ugyanez a házirend vonatkozik az **elsődleges** és az **archív** postaládára is.</span><span class="sxs-lookup"><span data-stu-id="d7553-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="d7553-111">Szükség lehet a kezelt mappák segédjének (MFA) futtatására, és az új beállításoknak a felhasználó postaládájára történő alkalmazására.</span><span class="sxs-lookup"><span data-stu-id="d7553-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="d7553-112">Futtassa a következő parancsot, miközben [csatlakozik az EXO PowerShell-hoz](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) a kezelt mappa segéd indításához egy adott postafiókhoz:</span><span class="sxs-lookup"><span data-stu-id="d7553-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="d7553-113">Start-ManagedFolderAssistant-identitás<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="d7553-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="d7553-114">Az archiválási házirendek beállításával kapcsolatos további tudnivalókért tanulmányozza a [postaládák archiválási és törlési házirendjének beállítása](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)című témakört.</span><span class="sxs-lookup"><span data-stu-id="d7553-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  