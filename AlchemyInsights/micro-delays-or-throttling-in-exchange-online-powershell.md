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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrokésés és -szabályozás az Exchange Online PowerShellben

Amikor parancsfájlokat és parancsmagokat futtat az Exchange Online-ban, "mikrokésés alkalmazása" figyelmeztetések vagy késések léphetnek fel. A probléma megoldásához íme néhány javaslat:

- Kérjük, hogy a diagnosztika futtatásával pihentetve pihentetje bérlői PowerShell-szabályozási szabályzatát. Ez a megoldás a legtöbb esetben megoldja a problémát.
- Ha a probléma továbbra sem oldódik meg, használja a [Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)modult, amely REST API-n alapuló parancsmagokat tartalmaz, és jelentősen hatékonyabb. Ez nagyszerű megoldás lehet a gyakran használt beszerzési parancsmagok esetén.
- Ha olyan parancsmagokat kell használnia, amelyekre a [v2](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)modul nem vonatkozik, olvassa el a PowerShell-parancsmagok futtatása nagyszámú felhasználó esetén a Office 365-ban . Ez a cikk a PowerShell szabályozási korlátainak az Exchange Online-ban való használatát tárgyalja.
