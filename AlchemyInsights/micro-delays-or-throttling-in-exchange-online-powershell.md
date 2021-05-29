---
title: Mikrokésés és -szabályozás az Exchange Online PowerShellben
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
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702128"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="df74a-102">Mikrokésés és -szabályozás az Exchange Online PowerShellben</span><span class="sxs-lookup"><span data-stu-id="df74a-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="df74a-103">Amikor parancsfájlokat és parancsmagokat futtat az Exchange Online-ban, "mikrokésés alkalmazása" figyelmeztetések vagy késések léphetnek fel.</span><span class="sxs-lookup"><span data-stu-id="df74a-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="df74a-104">A probléma megoldásához íme néhány javaslat:</span><span class="sxs-lookup"><span data-stu-id="df74a-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="df74a-105">Kérjük, hogy a diagnosztika futtatásával pihentetve pihentetje bérlői PowerShell-szabályozási szabályzatát.</span><span class="sxs-lookup"><span data-stu-id="df74a-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="df74a-106">Ez a megoldás a legtöbb esetben megoldja a problémát.</span><span class="sxs-lookup"><span data-stu-id="df74a-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="df74a-107">Ha a probléma továbbra sem oldódik meg, használja a [Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)modult, amely REST API-n alapuló parancsmagokat tartalmaz, és jelentősen hatékonyabb.</span><span class="sxs-lookup"><span data-stu-id="df74a-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="df74a-108">Ez nagyszerű megoldás lehet a gyakran használt beszerzési parancsmagok esetén.</span><span class="sxs-lookup"><span data-stu-id="df74a-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="df74a-109">Ha olyan parancsmagokat kell használnia, amelyekre a [v2](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)modul nem vonatkozik, olvassa el a PowerShell-parancsmagok futtatása nagyszámú felhasználó esetén a Office 365-ban . Ez a cikk a PowerShell szabályozási korlátainak az Exchange Online-ban való használatát tárgyalja.</span><span class="sxs-lookup"><span data-stu-id="df74a-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
