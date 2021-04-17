---
title: Törölt elemek helyreállítása parancsmaggal
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
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835813"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="f67a7-102">Törölt elemek helyreállítása parancsmaggal</span><span class="sxs-lookup"><span data-stu-id="f67a7-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="f67a7-103">A postaládák törölt elemeinek megtekintéséhez használja a [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) parancsmagot.</span><span class="sxs-lookup"><span data-stu-id="f67a7-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="f67a7-104">Miután megtalálta a törölt elemeket, a visszaállításukhoz használja a [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) parancsmagot.</span><span class="sxs-lookup"><span data-stu-id="f67a7-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="f67a7-105">Részletes információkat a [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)lapon találhat.</span><span class="sxs-lookup"><span data-stu-id="f67a7-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="f67a7-106">A parancsmag futtatásához postaláda-importálási és -exportálási szerepkörrel kell rendelnie.</span><span class="sxs-lookup"><span data-stu-id="f67a7-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="f67a7-107">További információt [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) lapon találhat.</span><span class="sxs-lookup"><span data-stu-id="f67a7-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
