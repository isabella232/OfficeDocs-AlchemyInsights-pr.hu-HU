---
title: Törölt elemek helyreállítása parancsmaggal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 86744d92a44096991079d1da3bdf4e95e58c55b7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493171"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="d7bc9-102">Törölt elemek helyreállítása parancsmaggal</span><span class="sxs-lookup"><span data-stu-id="d7bc9-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="d7bc9-103">A [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) parancsmag segítségével megtekintheti a postaládákban lévő törölt elemeket.</span><span class="sxs-lookup"><span data-stu-id="d7bc9-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="d7bc9-104">Miután megtalálta a törölt elemeket, a [Visszaállítás-helyreállítható elemek](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) parancsmagsegítségével visszaállíthatja azokat.</span><span class="sxs-lookup"><span data-stu-id="d7bc9-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="d7bc9-105">A teljes részleteket a [Get-RecoverableItems .](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="d7bc9-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="d7bc9-106">A parancsmag futtatásához hozzá kell rendelnie a postaláda importálása exportálási szerepkört.</span><span class="sxs-lookup"><span data-stu-id="d7bc9-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="d7bc9-107">További információt a [Get-RecoverableItems című témakörben](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) talál.</span><span class="sxs-lookup"><span data-stu-id="d7bc9-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
