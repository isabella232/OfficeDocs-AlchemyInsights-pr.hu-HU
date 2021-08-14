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
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868536"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrokésés és -szabályozás az Exchange Online PowerShellben

Amikor parancsfájlokat és parancsmagokat futtat az Exchange Online-ban, "mikrokésés alkalmazása" figyelmeztetések vagy késések léphetnek fel. A probléma megoldásához íme néhány javaslat:

- Kérjük, hogy a diagnosztika futtatásával pihentetve pihentetje bérlői PowerShell-szabályozási szabályzatát. Ez a megoldás a legtöbb esetben megoldja a problémát.
- Ha a probléma továbbra sem oldódik meg, használja a [Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)modult, amely a REST API-n alapuló, jelentősen hatékonyabb parancsmagokat tartalmaz. Ez nagyszerű megoldás lehet a gyakran használt beszerzési parancsmagok esetén.
- Ha olyan parancsmagokat kell használnia, amelyekre a [v2](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)modul nem vonatkozik, olvassa el a PowerShell-parancsmagok futtatása nagyszámú felhasználó számára a Office 365-ban . Ez a cikk a PowerShell szabályozási korlátainak az Exchange Online-ban való használatát tárgyalja.
