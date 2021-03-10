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
ms.openlocfilehash: 14d2c9b1fe6764f5cd3a5a968586a19a03b62694
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641520"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="ba9db-102">Törölt postaláda visszaállítása</span><span class="sxs-lookup"><span data-stu-id="ba9db-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="ba9db-103">Ha egy felhasználó elveszíti az Exchange Online-licencet, postaládája 30 napig megmarad, és egyszerűen újra hozzárendelve helyreállítható a felhasználóhoz.</span><span class="sxs-lookup"><span data-stu-id="ba9db-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
1. <span data-ttu-id="ba9db-104">A Microsoft 365 Felügyeleti központban  válassza a Felhasználók aktív felhasználók \> **lapot.**</span><span class="sxs-lookup"><span data-stu-id="ba9db-104">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="ba9db-105">Jelölje ki a kérdéses felhasználót.</span><span class="sxs-lookup"><span data-stu-id="ba9db-105">Select the user in question.</span></span>

2. <span data-ttu-id="ba9db-106">A **Licencek és alkalmazások** lapon rendelje hozzá az Exchange Online-licencet, és válassza a **Módosítások mentése lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="ba9db-106">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="ba9db-107">Ha egy megosztott postaládát vagy egy törölt felhasználót próbál helyreállítani, az 30 napig is helyreállítható.</span><span class="sxs-lookup"><span data-stu-id="ba9db-107">If you are trying to recover a shared mailbox or a user that was deleted, it is also recoverable for 30 days.</span></span> <span data-ttu-id="ba9db-108">Ezeket a Felhasználók törölt **felhasználók** csoportban találja; a megosztott postaládákhoz nincs szükség \> licencre.</span><span class="sxs-lookup"><span data-stu-id="ba9db-108">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="ba9db-109">Lásd: [Felhasználó visszaállítása.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="ba9db-109">Please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="ba9db-110">A felhasználók postaládájából az e-mailek helyreállítását a rendszergazdák az új [Exchange Felügyeleti központba használhatja.](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353)</span><span class="sxs-lookup"><span data-stu-id="ba9db-110">Recovery of email from user's mailbox can be done by admins by going to the [new Exchange Admin Center](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353).</span></span>

<span data-ttu-id="ba9db-111">Végül, ha inaktív postaládát próbál helyreállítani, [kövesse az itt található utasításokat.](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox)</span><span class="sxs-lookup"><span data-stu-id="ba9db-111">Finally, if you are trying to recover an Inactive mailbox, [follow the instructions here](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox).</span></span>
  
