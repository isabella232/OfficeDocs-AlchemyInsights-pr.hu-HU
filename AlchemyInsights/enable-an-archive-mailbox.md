---
title: Archív postaláda engedélyezése
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 5f5fea1e442b489bc81d9f6c4213e302c80f4ea7
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788668"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="47355-102">Archív postaláda engedélyezése</span><span class="sxs-lookup"><span data-stu-id="47355-102">Enable an archive mailbox</span></span>

<span data-ttu-id="47355-103">A Microsoft 365 archiválási postaládái (más néven *online archívumok* vagy *helyszíni archívumok) további e-mail*tárhelyet biztosítanak a felhasználóknak.</span><span class="sxs-lookup"><span data-stu-id="47355-103">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="47355-104">A felhasználók áthelyezhetik vagy átmásolhatják az elemeket az archív postaládájukba, a rendszergazdák pedig létrehozhatnak egy archiválási házirendet, amely automatikusan áthelyezi az elemeket a postaládák archív rendszerébe.</span><span class="sxs-lookup"><span data-stu-id="47355-104">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="47355-105">Az archív postaládák at a következőképpen hozhat létre:</span><span class="sxs-lookup"><span data-stu-id="47355-105">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="47355-106">Nyissa meg a [https://protection.office.com](https://protection.office.com) lapot.</span><span class="sxs-lookup"><span data-stu-id="47355-106">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="47355-107">Jelentkezzen be a Microsoft 365-be rendszergazdai fiókjával.</span><span class="sxs-lookup"><span data-stu-id="47355-107">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="47355-108">A Biztonsági &amp; megfelelőségi központ bal oldali ablaktáblájában válassza az **Információirányítási** \> **Archívum lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="47355-108">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="47355-109">Jelölje ki azt a felhasználót, akinek engedélyezni szeretné az archív postaládáját.</span><span class="sxs-lookup"><span data-stu-id="47355-109">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="47355-110">A jobb oldali jobb oldali ablaktáblában kattintson az **Engedélyezés** gombra, majd a figyelmeztető üzenetben az **Igen** gombra az archív postaláda engedélyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="47355-110">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="47355-111">Az archív postaládák tömeges engedélyezéséhez több felhasználót is kijelöl (a **Shift** vagy a **Ctrl** billentyűvel), majd a részletek ablaktáblán az **Engedélyezés** gombra kattint.</span><span class="sxs-lookup"><span data-stu-id="47355-111">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="47355-112">Megosztott postaládák</span><span class="sxs-lookup"><span data-stu-id="47355-112">Shared mailboxes</span></span>

<span data-ttu-id="47355-113">Egy megosztott postaláda archiválásának engedélyezéséhez Exchange Online Plan 2 licencre vagy Exchange Online Plan 1 licencre van szükség Exchange Online archiválási licenccel.</span><span class="sxs-lookup"><span data-stu-id="47355-113">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="47355-114">Megosztott postaláda archiválásának engedélyezése:</span><span class="sxs-lookup"><span data-stu-id="47355-114">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="47355-115">Nyissa meg az [Exchange Felügyeleti központot,](https://outlook.office365.com/ecp) és jelentkezzen be a rendszergazdai fiókjával.</span><span class="sxs-lookup"><span data-stu-id="47355-115">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="47355-116">Nyissa meg a Megosztott címzettek > **(Címzettek) (Címzettek) (** **Címzettek**) ( Ugrás</span><span class="sxs-lookup"><span data-stu-id="47355-116">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="47355-117">Jelölje ki a megosztott postaládát.</span><span class="sxs-lookup"><span data-stu-id="47355-117">Select the shared mailbox.</span></span>

4. <span data-ttu-id="47355-118">A jobb oldali, jobb oldali **ablaktáblában**kattintson az **Engedélyezés**gombra, majd az **Igen** gombra az archív postaláda engedélyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="47355-118">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="47355-119">További információ:</span><span class="sxs-lookup"><span data-stu-id="47355-119">For more information, see:</span></span>
  
- [<span data-ttu-id="47355-120">Archív postaládák engedélyezése</span><span class="sxs-lookup"><span data-stu-id="47355-120">Enable archive mailboxes</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)

- [<span data-ttu-id="47355-121">Archiválási és törlési házirend beállítása</span><span class="sxs-lookup"><span data-stu-id="47355-121">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
