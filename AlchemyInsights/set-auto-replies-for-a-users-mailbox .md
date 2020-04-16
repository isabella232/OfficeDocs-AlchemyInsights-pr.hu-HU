---
title: Automatikus válasz beállítása a felhasználó postaládájához
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506520"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="e5815-102">Automatikus válasz beállítása a felhasználó postaládájához</span><span class="sxs-lookup"><span data-stu-id="e5815-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="e5815-103">**1. módszer**</span><span class="sxs-lookup"><span data-stu-id="e5815-103">**Method 1**</span></span>

1. <span data-ttu-id="e5815-104">Bejelentkezés az Office 365-portálra.</span><span class="sxs-lookup"><span data-stu-id="e5815-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="e5815-105">Ugorjon a **Felhasználók > Aktív felhasználók** (vagy a **Csoportok > Megosztott postaládák** lehetőségre, ha megosztott postaládára szeretné beállítani).</span><span class="sxs-lookup"><span data-stu-id="e5815-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="e5815-106">Jelöljön ki egy Microsoft Exchange-postaládával rendelkező felhasználót.</span><span class="sxs-lookup"><span data-stu-id="e5815-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="e5815-107">A jobb oldali legördülő menüben válassza a **Levelek beállításai > Automatikus válaszok** lehetőséget (ha megosztott postaládája van, egyszerűen kattintson az **Automatikus válaszokra** a legördülő menüben).</span><span class="sxs-lookup"><span data-stu-id="e5815-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="e5815-108">**2. módszer**</span><span class="sxs-lookup"><span data-stu-id="e5815-108">**Method 2**</span></span>

1. <span data-ttu-id="e5815-109">Jelentkezzen be az Office 365 felügyeleti portálján rendszergazdai hitelesítő adatokkal.</span><span class="sxs-lookup"><span data-stu-id="e5815-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="e5815-110">Bontsa ki a **Felügyeleti központot**, és kattintson az **Exchange** elemre.</span><span class="sxs-lookup"><span data-stu-id="e5815-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="e5815-111">Kattintson a jobb felső sarokban lévő képre, majd kattintson a **Másik felhasználó** lehetőségre, és válassza ki a módosítani kívánt felhasználói postaládát.</span><span class="sxs-lookup"><span data-stu-id="e5815-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="e5815-112">A bal oldalon válassza a **Beállítások** lehetőséget, kattintson az **E-mailek rendszerezése**, majd az**Automatikus válaszok** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="e5815-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="e5815-113">**3. módszer**</span><span class="sxs-lookup"><span data-stu-id="e5815-113">**Method 3**</span></span>

<span data-ttu-id="e5815-114">Az Exchange Online PowerShell-ben futtassa a következő cmdlet parancsot:</span><span class="sxs-lookup"><span data-stu-id="e5815-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="e5815-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="e5815-115">PowerShellCopy</span></span>

    Set-MailboxAutoReplyConfiguration

<span data-ttu-id="e5815-116">További információt a cmdlet parancsról a [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="e5815-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
