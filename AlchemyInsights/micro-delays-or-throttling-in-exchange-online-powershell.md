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
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314702"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrokésés és -szabályozás az Exchange Online PowerShellben

Amikor parancsfájlokat és parancsmagokat futtat az Exchange Online-ban, "mikrokésés alkalmazása" figyelmeztetések vagy késések léphetnek fel. A probléma megoldásához íme néhány javaslat:

- Kérjük, hogy a diagnosztika futtatásával pihentetve pihentetje bérlői PowerShell-szabályozási szabályzatát. Ez a megoldás a legtöbb esetben megoldja a problémát.
- Ha a probléma továbbra sem oldódik meg, használja a [Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)modult, amely a REST API-n alapuló parancsmagokat tartalmazza, és jelentősen hatékonyabb. Ez nagyszerű megoldás lehet a gyakran használt beszerzési parancsmagok esetén.
- Ha olyan parancsmagokat kell használnia, amelyekre a [v2](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)modul nem vonatkozik, olvassa el a PowerShell-parancsmagok futtatása nagyszámú felhasználó számára a Office 365-ban . Ez a cikk a PowerShell szabályozási korlátainak használatát tárgyalja Exchange Online.
