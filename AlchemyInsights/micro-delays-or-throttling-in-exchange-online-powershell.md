---
title: Mikrokésés és -szabályozás az Exchange Online PowerShellben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947911"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrokésés és -szabályozás az Exchange Online PowerShellben

Amikor parancsfájlokat és parancsmagokat futtat az Exchange Online-ban, "mikrokésés alkalmazása" figyelmeztetések vagy késések léphetnek fel. Ezzel kapcsolatban íme két javaslat:

- Jobb megoldás lenne az [Exchange Online v2 PowerShell-modul](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) használata, amely a REST API-alapú parancsmagokat is tartalmazza, és lényegesen jobb teljesítményt nyújt. Ez nagyszerű megoldás lehet a gyakran használt beszerzési parancsmagok esetén.
- Ha a v2 modulban nem szereplő parancsmagokat kell használnia, olvassa el a [PowerShell-parancsmagok használata nagy számú felhasználó esetén az Office 365-ben](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#) című témakört, amelyből megtudhatja, hogy miként tájékozódhat az Exchange Online-ban várható PowerShell-szabályozási korlátozásokról.
