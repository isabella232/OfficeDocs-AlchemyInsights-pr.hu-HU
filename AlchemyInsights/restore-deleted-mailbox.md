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
ms.openlocfilehash: 18e56305b60469422a154ffa1b097c238baaae16
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764658"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="51f1a-102">Törölt postaláda visszaállítása</span><span class="sxs-lookup"><span data-stu-id="51f1a-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="51f1a-103">Ha egy felhasználó elveszíti az Exchange Online-licencet, postaládája 30 napig megmarad, és a licenc nek a felhasználóhoz való egyszerű hozzárendelésével helyrehozható.</span><span class="sxs-lookup"><span data-stu-id="51f1a-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="51f1a-104">*Ez csak 30 napon belül fog működni.*</span><span class="sxs-lookup"><span data-stu-id="51f1a-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="51f1a-105">A Microsoft 365 Felügyeleti központban nyissa meg a **Felhasználók** \> **aktív felhasználók** lapot.</span><span class="sxs-lookup"><span data-stu-id="51f1a-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="51f1a-106">Válassza ki a kérdéses felhasználót.</span><span class="sxs-lookup"><span data-stu-id="51f1a-106">Select the user in question.</span></span>

2. <span data-ttu-id="51f1a-107">A **Licencek és alkalmazások** lapon rendelje hozzá az Exchange Online-licencet, és válassza a **Módosítások mentése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="51f1a-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="51f1a-108">Ha megosztott postaládát próbál helyreállítani, az 30 napig is helyreállítható.</span><span class="sxs-lookup"><span data-stu-id="51f1a-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="51f1a-109">Ezeket a **Törölt felhasználók csoportban** \> **Deleted users**találja meg; a megosztott postaládákhoz nincs szükség licencre.</span><span class="sxs-lookup"><span data-stu-id="51f1a-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="51f1a-110">Ha észreveszi, hogy vissza kell állítania egy törölt felhasználót, olvassa el [a Felhasználó visszaállítása ..](https://docs.microsoft.com/office365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="51f1a-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  