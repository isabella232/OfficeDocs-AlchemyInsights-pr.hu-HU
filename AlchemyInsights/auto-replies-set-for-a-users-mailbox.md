---
title: Automatikus válasz beállítása egy postaládához
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
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788884"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="6a0c4-102">Automatikus válasz beállítása egy felhasználó postaládájához</span><span class="sxs-lookup"><span data-stu-id="6a0c4-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="6a0c4-103">**1. módszer**</span><span class="sxs-lookup"><span data-stu-id="6a0c4-103">**Method 1**</span></span>

1. <span data-ttu-id="6a0c4-104">Jelentkezzen be a Microsoft 365 portálon.</span><span class="sxs-lookup"><span data-stu-id="6a0c4-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="6a0c4-105">Ugorjon a **Felhasználók > Aktív felhasználók** (vagy a **Csoportok > Megosztott postaládák** lehetőségre, ha megosztott postaládára szeretné beállítani).</span><span class="sxs-lookup"><span data-stu-id="6a0c4-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="6a0c4-106">Jelöljön ki egy Microsoft Exchange-postaládával rendelkező felhasználót.</span><span class="sxs-lookup"><span data-stu-id="6a0c4-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="6a0c4-107">A jobb oldali legördülő menüben válassza a **Levelek beállításai > Automatikus válaszok** lehetőséget (ha megosztott postaládája van, egyszerűen kattintson az **Automatikus válaszokra** a legördülő menüben).</span><span class="sxs-lookup"><span data-stu-id="6a0c4-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="6a0c4-108">**2. módszer**</span><span class="sxs-lookup"><span data-stu-id="6a0c4-108">**Method 2**</span></span>

1. <span data-ttu-id="6a0c4-109">Jelentkezzen be a Microsoft 365 felügyeleti portálján rendszergazdai hitelesítő adatokkal.</span><span class="sxs-lookup"><span data-stu-id="6a0c4-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="6a0c4-110">Bontsa ki a **Felügyeleti központot**, és kattintson az **Exchange** elemre.</span><span class="sxs-lookup"><span data-stu-id="6a0c4-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="6a0c4-111">Kattintson a jobb felső sarokban lévő képre, majd kattintson a **Másik felhasználó** lehetőségre, és válassza ki a módosítani kívánt felhasználói postaládát.</span><span class="sxs-lookup"><span data-stu-id="6a0c4-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="6a0c4-112">A bal oldalon válassza a **Beállítások** lehetőséget, kattintson az **E-mailek rendszerezése**, majd az**Automatikus válaszok** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="6a0c4-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="6a0c4-113">**3. módszer**</span><span class="sxs-lookup"><span data-stu-id="6a0c4-113">**Method 3**</span></span>

<span data-ttu-id="6a0c4-114">Az Exchange Online PowerShell-ben futtassa a következő cmdlet parancsot:</span><span class="sxs-lookup"><span data-stu-id="6a0c4-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="6a0c4-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="6a0c4-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="6a0c4-116">További információt a cmdlet parancsról a [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="6a0c4-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
