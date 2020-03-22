---
title: Nem lehet hozzáférni a nyilvános mappákhoz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891751"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Az Outlook nem tud nyilvános mappákhoz csatlakozni

Ha a nyilvános mappák hoz való hozzáférés egyes felhasználók nál nem működik, próbálkozzon az alábbiakkal:

Csatlakozzon az EXO PowerShell alkalmazáshoz, és konfigurálja úgy a problémás felhasználói fiók DefaultPublicFolderMailbox paraméterét, hogy az megfeleljen egy működő felhasználói fiók paraméterének.

Példa:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<érték az előző parancsból>

Várjon legalább egy órát, amíg a módosítás érvénybe lép.

Ha a probléma továbbra is fennáll, kövesse [az alábbi eljárást](https://aka.ms/pfcte) a nyilvános mappákhoz való hozzáféréssel kapcsolatos problémák megoldásához az Outlook programban.