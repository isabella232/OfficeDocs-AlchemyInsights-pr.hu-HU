---
title: Archív postaláda engedélyezése
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811707"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="62a91-102">Archív postaláda engedélyezése</span><span class="sxs-lookup"><span data-stu-id="62a91-102">Enable an archive mailbox</span></span>

<span data-ttu-id="62a91-103">Ha szeretné, hogy a rendszer automatikusan ellenőrizze az archiválási postaláda konfigurálását, jelölje be a vissza gombot < a lap tetején, majd adja meg a fiók e-mail-címét.</span><span class="sxs-lookup"><span data-stu-id="62a91-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="62a91-104">A Microsoft 365-ban archivált postaládák (más néven *online archívumok* vagy *helyi archívumok*) további e-mail-tárterületet adhatnak a felhasználóknak.</span><span class="sxs-lookup"><span data-stu-id="62a91-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="62a91-105">A felhasználók az archív postaládába áthelyezhetik vagy másolhatják az elemeket, a rendszergazdák pedig létrehozhatnak egy archiválási házirendet, amely automatikusan áthelyezi az elemeket az archív postaládákba.</span><span class="sxs-lookup"><span data-stu-id="62a91-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="62a91-106">Az alábbi módon hozhat létre archív postaládát:</span><span class="sxs-lookup"><span data-stu-id="62a91-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="62a91-107">Nyissa meg a [https://protection.office.com](https://protection.office.com) lapot.</span><span class="sxs-lookup"><span data-stu-id="62a91-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="62a91-108">Bejelentkezés a Microsoft 365-be a rendszergazdai fiókjával.</span><span class="sxs-lookup"><span data-stu-id="62a91-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="62a91-109">A biztonsági megfelelőségi központ bal oldali ablaktáblájában &amp; válassza az **adatkezelési** \> **Archívum**elemet.</span><span class="sxs-lookup"><span data-stu-id="62a91-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="62a91-110">Jelölje ki azt a felhasználót, akinek az archív postaládáját engedélyezni szeretné.</span><span class="sxs-lookup"><span data-stu-id="62a91-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="62a91-111">A jobb oldali ablaktáblában kattintson az **Engedélyezés** elemre, majd a figyelmeztető üzenetben az **Igen** gombra kattintva engedélyezze az archív postaládát.</span><span class="sxs-lookup"><span data-stu-id="62a91-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="62a91-112">Az archiválási postaládák tömeges engedélyezéséhez több felhasználó kijelölésével (a **SHIFT** vagy a **CTRL** billentyű lenyomásával), majd a Részletek ablaktáblában az **Engedélyezés** elemre kattinthat.</span><span class="sxs-lookup"><span data-stu-id="62a91-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="62a91-113">Megosztott postaládák</span><span class="sxs-lookup"><span data-stu-id="62a91-113">Shared mailboxes</span></span>

<span data-ttu-id="62a91-114">Ha engedélyezni szeretné az archiválást egy megosztott postaládához, az Exchange Online-csomag 2 licence vagy egy Exchange Online-csomag (1) licence szükséges az Exchange Online archiválási licenccel.</span><span class="sxs-lookup"><span data-stu-id="62a91-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="62a91-115">A megosztott postaláda archiválásának engedélyezése:</span><span class="sxs-lookup"><span data-stu-id="62a91-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="62a91-116">Nyissa meg az [Exchange felügyeleti központot](https://outlook.office365.com/ecp) , és használja a rendszergazdai fiókját.</span><span class="sxs-lookup"><span data-stu-id="62a91-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="62a91-117">Válassza a **megosztott címzettek**lehetőséget  >  **Shared**.</span><span class="sxs-lookup"><span data-stu-id="62a91-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="62a91-118">Jelölje ki a megosztott postaládát.</span><span class="sxs-lookup"><span data-stu-id="62a91-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="62a91-119">A jobb oldali ablaktáblán, a **helyi Archívum**csoportban kattintson az **Engedélyezés**, majd az **Igen** gombra az archív postaláda engedélyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="62a91-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="62a91-120">További információ:</span><span class="sxs-lookup"><span data-stu-id="62a91-120">For more information, see:</span></span>
  
- [<span data-ttu-id="62a91-121">Archív postaládák engedélyezése</span><span class="sxs-lookup"><span data-stu-id="62a91-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="62a91-122">Archiválási és törlési házirend beállítása</span><span class="sxs-lookup"><span data-stu-id="62a91-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
