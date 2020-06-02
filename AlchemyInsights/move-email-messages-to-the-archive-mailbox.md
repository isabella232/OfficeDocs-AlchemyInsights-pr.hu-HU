---
title: E-mailek áthelyezése az Archív postaládába
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511042"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="2b911-102">E-mailek áthelyezése az archív postaládába</span><span class="sxs-lookup"><span data-stu-id="2b911-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="2b911-103">Ellenőrizze, hogy engedélyezve **van-e az archív postaláda.**</span><span class="sxs-lookup"><span data-stu-id="2b911-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="2b911-104">Ha nem, a [cikkben](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) ismertetett lépésekkel engedélyezze az archív postaládát.</span><span class="sxs-lookup"><span data-stu-id="2b911-104">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="2b911-105">Ha az üzeneteket automatikusan archiválni szeretné az archív postaládába, **be** kell állítania, hogy az automatikusan alkalmazza a **teljes postaláda -ra (alapértelmezett) címkét.**</span><span class="sxs-lookup"><span data-stu-id="2b911-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="2b911-106">Az itt leírt lépésekkel hozhatja létre a címkét: [Archiválás i. címke](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="2b911-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="2b911-107">Ezután adja hozzá az **Archív** címkét az adatmegőrzési házirendhez.</span><span class="sxs-lookup"><span data-stu-id="2b911-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="2b911-108">Az Exchange Felügyeleti központban válassza az **Adatmegőrzési házirendek** lehetőséget, > adja hozzá az **Áthelyezés az archívumba címkét** a Mentés > **házirendhez.**</span><span class="sxs-lookup"><span data-stu-id="2b911-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="2b911-109">Most [rendelje hozzá az adatmegőrzési szabályt](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) az adott felhasználó postaládájához.</span><span class="sxs-lookup"><span data-stu-id="2b911-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="2b911-110">Ugyanez a házirend lesz alkalmazva mind az **Elsődleges,** mind az **Archív** postaládára.</span><span class="sxs-lookup"><span data-stu-id="2b911-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="2b911-111">Szükség lehet arra, hogy a felügyelt mappasegédet (MFA) a felhasználó postaládájára kényszerítse és alkalmazza az új beállításokra.</span><span class="sxs-lookup"><span data-stu-id="2b911-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="2b911-112">Futtassa a következő parancsot, miközben [az EXO PowerShellhez csatlakozik](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) egy adott postaláda felügyelt mappasegédének elindításához:</span><span class="sxs-lookup"><span data-stu-id="2b911-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="2b911-113">Start-ManagedFolderAssistant -Identitás<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="2b911-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="2b911-114">Az archiválási házirend beállításáról a [postaládák archiválási és törlési házirendjének beállítása](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)című témakörben talál további információt.</span><span class="sxs-lookup"><span data-stu-id="2b911-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  