---
title: Külső e-mailek továbbításának azonosítása postaládákban a naplókban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508954"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="cf20f-102">Annak azonosítása, hogy mikor van konfigurálva a külső e-mailek továbbítása postaládákon</span><span class="sxs-lookup"><span data-stu-id="cf20f-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="cf20f-103">Ha egy Microsoft 365-felhasználó külső e-mail továbbítást konfigurál egy postaládán, a rendszer a **set-mailbox** parancsmag részeként naplózza a tevékenységet.</span><span class="sxs-lookup"><span data-stu-id="cf20f-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="cf20f-104">A tevékenységet a Biztonsági & megfelelőségi központban, a naplózási keresés sel láthatja.</span><span class="sxs-lookup"><span data-stu-id="cf20f-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="cf20f-105">Jelentkezzen be a [Microsoft 365 Biztonsági & megfelelőségi központjába.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="cf20f-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="cf20f-106">Nyissa meg a **Keresési**  >  **napló keresési naplójának keresési** lapját.</span><span class="sxs-lookup"><span data-stu-id="cf20f-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="cf20f-107">Válassza ki a dátumtartományt a **Kezdési dátum** és a **Záró dátum** mezőben.</span><span class="sxs-lookup"><span data-stu-id="cf20f-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="cf20f-108">Nem kell megadnia felhasználónevet.</span><span class="sxs-lookup"><span data-stu-id="cf20f-108">You don't need to specify a username.</span></span> <span data-ttu-id="cf20f-109">Ellenőrizze, hogy a **Tevékenységek** mező az **összes tevékenység eredményeinek megjelenítése**beállításra van-e állítva.</span><span class="sxs-lookup"><span data-stu-id="cf20f-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="cf20f-110">Kattintson a **Keresés gombra.**</span><span class="sxs-lookup"><span data-stu-id="cf20f-110">Click **Search**.</span></span>

<span data-ttu-id="cf20f-111">Az eredmények között kattintson az **Eredmények szűrése** gombra, és írja be a **Set-Mailbox (Postaláda** beállítása) mezőbe jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="cf20f-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="cf20f-112">Jelöljön ki egy naplózási rekordot az eredmények között.</span><span class="sxs-lookup"><span data-stu-id="cf20f-112">Select an audit record in the results.</span></span> <span data-ttu-id="cf20f-113">A **Részletek** úszó panelen kattintson a **További információ gombra.**</span><span class="sxs-lookup"><span data-stu-id="cf20f-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="cf20f-114">Meg kell néznie az egyes naplózási rekordok részleteit annak megállapításához, hogy a tevékenység kapcsolódik-e az e-mailek továbbításához.</span><span class="sxs-lookup"><span data-stu-id="cf20f-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="cf20f-115">**ObjectId**: A módosított postaláda aliasértéke.</span><span class="sxs-lookup"><span data-stu-id="cf20f-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="cf20f-116">**Paraméterek**: _A ForwardingSmtpAddress_ a cél e-mail címet jelzi.</span><span class="sxs-lookup"><span data-stu-id="cf20f-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="cf20f-117">**UserId**: Az a felhasználó, aki az **ObjectId** mezőben beállította az e-mailek továbbítását a postaládán.</span><span class="sxs-lookup"><span data-stu-id="cf20f-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="cf20f-118">További információt a [Postaláda e-mail-továbbítási beállításának meghatározása](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="cf20f-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
