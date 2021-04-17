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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830035"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrokésés és -szabályozás az Exchange Online PowerShellben

Amikor parancsfájlokat és parancsmagokat futtat az Exchange Online-ban, "mikrokésés alkalmazása" figyelmeztetések vagy késések léphetnek fel. Ezzel kapcsolatban íme két javaslat:

- Jobb megoldás lenne az [Exchange Online v2 PowerShell-modul](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) használata, amely a REST API-alapú parancsmagokat is tartalmazza, és lényegesen jobb teljesítményt nyújt. Ez nagyszerű megoldás lehet a gyakran használt beszerzési parancsmagok esetén.
- Ha a v2 modulban nem szereplő parancsmagokat kell használnia, olvassa el a [PowerShell-parancsmagok használata nagy számú felhasználó esetén az Office 365-ben](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#) című témakört, amelyből megtudhatja, hogy miként tájékozódhat az Exchange Online-ban várható PowerShell-szabályozási korlátozásokról.
