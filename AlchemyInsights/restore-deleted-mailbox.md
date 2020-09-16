---
title: Törölt postaláda visszaállítása
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "360"
- "3500005"
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 899eb7e171d125c509871c219f99dfd1106b858a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728073"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="aa091-102">Törölt postaláda visszaállítása</span><span class="sxs-lookup"><span data-stu-id="aa091-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="aa091-103">Ha egy felhasználó elveszíti az Exchange Online-licencét, a postaládáját a rendszer 30 napig megőrzi, és visszaállíthatja úgy, hogy a licencet egyszerűen hozzárendeli a felhasználóhoz.</span><span class="sxs-lookup"><span data-stu-id="aa091-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="aa091-104">*Ez csak 30 napon belül fog működni.*</span><span class="sxs-lookup"><span data-stu-id="aa091-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="aa091-105">A Microsoft 365 felügyeleti központban nyissa meg a **felhasználók** \> **aktív felhasználók** lapot.</span><span class="sxs-lookup"><span data-stu-id="aa091-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="aa091-106">Jelölje ki a kérdéses felhasználót.</span><span class="sxs-lookup"><span data-stu-id="aa091-106">Select the user in question.</span></span>

2. <span data-ttu-id="aa091-107">A **licencek és alkalmazások** lapon rendelje hozzá az Exchange Online-licencet, és válassza a **módosítások mentése**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="aa091-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="aa091-108">Ha megpróbál helyreállítani egy megosztott postaládát, az is 30 napig állítható helyre.</span><span class="sxs-lookup"><span data-stu-id="aa091-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="aa091-109">Ezek a **felhasználók** által \> **törölt felhasználók**csoportban találhatók; a megosztott postaládákhoz nincs szükség licencre.</span><span class="sxs-lookup"><span data-stu-id="aa091-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="aa091-110">Ha úgy látja, hogy vissza kell állítania egy törölt felhasználót, olvassa el [a felhasználó helyreállítása](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)című témakört.</span><span class="sxs-lookup"><span data-stu-id="aa091-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
  