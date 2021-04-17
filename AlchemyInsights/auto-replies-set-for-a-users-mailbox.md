---
title: Automatikus válasz beállítása egy postaládához
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820936"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="bbe37-102">Automatikus válasz beállítása egy felhasználó postaládájához</span><span class="sxs-lookup"><span data-stu-id="bbe37-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="bbe37-103">**1. módszer**</span><span class="sxs-lookup"><span data-stu-id="bbe37-103">**Method 1**</span></span>

1. <span data-ttu-id="bbe37-104">Jelentkezzen be a Microsoft 365 portálon.</span><span class="sxs-lookup"><span data-stu-id="bbe37-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="bbe37-105">Ugorjon a **Felhasználók > Aktív felhasználók** (vagy a **Csoportok > Megosztott postaládák** lehetőségre, ha megosztott postaládára szeretné beállítani).</span><span class="sxs-lookup"><span data-stu-id="bbe37-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="bbe37-106">Jelöljön ki egy Microsoft Exchange-postaládával rendelkező felhasználót.</span><span class="sxs-lookup"><span data-stu-id="bbe37-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="bbe37-107">A jobb oldali legördülő menüben válassza a **Levelek beállításai > Automatikus válaszok** lehetőséget (ha megosztott postaládája van, egyszerűen kattintson az **Automatikus válaszokra** a legördülő menüben).</span><span class="sxs-lookup"><span data-stu-id="bbe37-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="bbe37-108">**2. módszer**</span><span class="sxs-lookup"><span data-stu-id="bbe37-108">**Method 2**</span></span>

1. <span data-ttu-id="bbe37-109">Jelentkezzen be a Microsoft 365 felügyeleti portálján rendszergazdai hitelesítő adatokkal.</span><span class="sxs-lookup"><span data-stu-id="bbe37-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="bbe37-110">Bontsa ki a **Felügyeleti központot**, és kattintson az **Exchange** elemre.</span><span class="sxs-lookup"><span data-stu-id="bbe37-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="bbe37-111">Kattintson a jobb felső sarokban lévő képre, majd kattintson a **Másik felhasználó** lehetőségre, és válassza ki a módosítani kívánt felhasználói postaládát.</span><span class="sxs-lookup"><span data-stu-id="bbe37-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="bbe37-112">A bal oldalon válassza a **Beállítások** lehetőséget, kattintson az **E-mailek rendszerezése**, majd az **Automatikus válaszok** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="bbe37-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="bbe37-113">**3. módszer**</span><span class="sxs-lookup"><span data-stu-id="bbe37-113">**Method 3**</span></span>

<span data-ttu-id="bbe37-114">Az Exchange Online PowerShell-ben futtassa a következő cmdlet parancsot:</span><span class="sxs-lookup"><span data-stu-id="bbe37-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="bbe37-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="bbe37-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="bbe37-116">További információt a cmdlet parancsról a [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="bbe37-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
