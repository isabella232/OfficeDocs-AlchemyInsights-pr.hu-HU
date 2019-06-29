---
title: E-mailek áthelyezése az archív postaláda
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
ms.openlocfilehash: a29fb799b68f5c187ca1d44aeaf94e6cd8760b0e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35379499"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="d2b9c-102">E-mail áthelyezése az archív postaláda</span><span class="sxs-lookup"><span data-stu-id="d2b9c-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="d2b9c-103">Győződjön meg arról, hogy a **postaláda archiválása** engedélyezve van.</span><span class="sxs-lookup"><span data-stu-id="d2b9c-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="d2b9c-104">Ha nem, az archív postaláda engedélyezése [Ebben](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) a cikkben leírtakat.</span><span class="sxs-lookup"><span data-stu-id="d2b9c-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="d2b9c-105">Archiválása az archív postaláda üzeneteket automatikusan, az **Ugrás archiválása** művelettel adatmegőrzési címke **automatikusan**alkalmazandó teljes postafiók (alapértelmezés) címkével kell állítani.</span><span class="sxs-lookup"><span data-stu-id="d2b9c-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="d2b9c-106">Kövesse a lépéseket Itt a címke létrehozása: [Archív alapértelmezett címkét](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span><span class="sxs-lookup"><span data-stu-id="d2b9c-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>

3. <span data-ttu-id="d2b9c-107">Ezután adja hozzá az **Archív** címke az adatmegőrzési szabály.</span><span class="sxs-lookup"><span data-stu-id="d2b9c-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="d2b9c-108">Válassza ki az Exchange felügyeleti központ **Adatmegőrzési** > hozzá a **címke archívum áthelyezése** a házirend > **menteni**.</span><span class="sxs-lookup"><span data-stu-id="d2b9c-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="d2b9c-109">Most [a megőrzési házirendet](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) az adott felhasználó postaládájához.</span><span class="sxs-lookup"><span data-stu-id="d2b9c-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="d2b9c-110">Ugyanaz a házirend az **elsődleges** és az **Archív** postaláda vonatkozik.</span><span class="sxs-lookup"><span data-stu-id="d2b9c-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="d2b9c-111">A kezelt mappa Segéd (MFA) és az új beállítások alkalmazása a felhasználó postaládájában, hogy szükség lehet.</span><span class="sxs-lookup"><span data-stu-id="d2b9c-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="d2b9c-112">Futtassa a következő parancsot közben [csatlakoztatva EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) indítása a kezelt Mappakezelő egy adott postaláda:</span><span class="sxs-lookup"><span data-stu-id="d2b9c-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="d2b9c-113">Start-ManagedFolderAssistant-azonosító<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="d2b9c-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="d2b9c-114">Archiválási házirend beállításával kapcsolatos további tudnivalókért lásd [az archív és törlési házirend postafiókok beállítása](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="d2b9c-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  